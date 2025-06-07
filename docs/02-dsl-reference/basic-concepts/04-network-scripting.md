---
sidebar_position: 4
title: Network Scripting
pagination_label: Network Scripting
sidebar_label: Network Scripting
description: Network scripting in DSL allows you to create client scripts that run on players' machines when they connect to a server. This guide covers how to define client scripts, handle network events, and manage player objects.
---

# Network Scripting

Read about the basics of the server version in the [about](about-dsl#derpy-script-server) section, and download the latest server version in the [download](/docs/miscellaneous/downloads/dsl) section.

## Client Scripts

Client scripts can be defined using `client_script` in the `config.txt` of a server script collection. If the collection is running, these scripts are sent to players when they join and also sent when the collection is restarted. Additional files the script may need (such as images or manually loaded scripts) can be sent using `client_file`.

When a player connects to a server, they stop all of their local script collections (unless they're marked with `allow_on_server` for the sake of allowing mods like the window mod). Then all active server script collections are started using the sent client scripts and files. Server script collections can only be controlled by the server, although players can still use `/list` to see them.

The full `config.txt` from each server script collection is sent to players, so be sure not to include any sensitive data (such as IP addresses) in it. If you need to store something sensitive (such as a scripted whitelist), make a seperate config file for the server to use and make sure not to mark it as a client script or file.

## Network Events

A network event handler can be created using [RegisterNetworkEventHandler](/docs/dsl-reference/global-functions/RegisterNetworkEventHandler) to run some code when a network event is triggered using [SendNetworkEvent](/docs/dsl-reference/global-functions/SendNetworkEvent).

By default no network events exist, and you can make your own events by just sending one as there is no "creation" of events. Although events can be named whatever you like, it is advised you prefix your event to make sure it is unique and to make it easy to tell what script it may have come from. For example instead of `"playerKilled"`, you are urged to use something like `"mod_name:playerKilled"`.

Network events can only be activated by the other side of the connection. This means client network events can only be activated by the server, and server network events can only be activated by a client. A server should not trust the events sent by clients, as a hacker or network error could affect the event sent and its arguments. The only thing servers can count on with network events is that the first argument is a valid connected player.

## Local Server Events

A local event handler can be created using [RegisterLocalEventHandler](/docs/dsl-reference/global-functions/RegisterLocalEventHandler).

You may need to make these on the server to respond to player related events. Player events (such as `PlayerDropped`) are considered local because they come from the server itself, which means you can always trust them and their arguments unlike network events.

## Server Player Objects

In Lua scripts, players are represented using a numeric ID. Player IDs start at zero, and a negative player ID is considered invalid. When some player joins the server after another has left, it is possible for them to re-use an old player ID. This means it is **very important** that you remove any references to a player during local `PlayerDropped` events to prevent unexpected behavior.

Players can be said to have 3 states: `invalid`, `valid`, and `connected`. All connected players are valid. You can always count on a `PlayerDropped` event to tell you when a player that was once valid is no longer valid, except during a `PlayerListing` event where the player is only considered valid for the duration of that event.

You can always do some basic things with a player as long as they're valid (such as kick them or get their name), but you can only send data to players that are connected. A player returned by `AllPlayers` is always connected, unless the optional argument for it is `true` which means it can return players that are only valid as well. You can also use `IsPlayerValid` to check if a player is connected or valid.

You can use the following local server events to know when a player changes state.

- `PlayerConnecting`: an invalid player has become valid.
- `PlayerConnected`: a valid player has connected (and wasn't connected before).
- `PlayerDropped`: a player is now invalid (and may or may not have been valid before the event).
- `PlayerListing`: a player is valid _only for the duration of this event_ (and no drop event will follow this event).
