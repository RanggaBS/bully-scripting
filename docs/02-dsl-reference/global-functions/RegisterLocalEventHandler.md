---
description: Registers a new local event handler.
sidebar_class_name: hidden
---

# RegisterLocalEventHandler

> **_This function was added in DSL 4_**

## Description

Registers a new local event handler. The `callback` function is called when the event is activated. The returned `eventHandler` object is registered with the current script, meaning it will be removed when the script dies. If there is no current DSL script to register with, it will exist until removed manually with [`RemoveEventHandler`](RemoveEventHandler).

An `eventType` is just a string. Although there are a few events built-in and listed below, you are free to define your own for any purpose. Just make sure the name is unique enough that it won't clash with what other developers are likely to use. This is a good way to allow your script's behavior to be influenced by scripts from other developers.

:::tip[Best Practice]

- ❌ `RegisterLocalEventHandler('EventName', function() end)`
- ✅ `RegisterLocalEventHandler('MyMod:EventName', function() end)`
  :::

```lua
function RegisterLocalEventHandler(eventType, callback) --[[ ... ]] end
```

## Parameters

- `eventType`: _`string`_ - The name of the event to register. This can be any string, but should be unique to avoid conflicts with other scripts.
- `callback`: _`fun(...: unknown): boolean?`_ - The function to call when the event is triggered.

## Return Values

- `eventHandler`: _`userdata`_ - An object representing the registered event handler. This can be used to remove the handler later if needed.

## Example

Keep the player up past 2 AM.

```lua
RegisterLocalEventHandler('PlayerSleepCheck', function()
  return true
end)
```

## Events

### Client

| Type                                           | Description                                                                                                                                                             |
| ---------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **DSL6** CameraFaded(ms, fadein)               | The camera is fading in or out. Same arguments as [`CameraFade`](/docs/game-reference/global-functions/CameraFade), but the 2nd value is a boolean instead of a number. |
| **DSL5** ControllersUpdated()                  | All controllers have been updated. This is a good time to call [`SetStickValue`](SetStickValue).                                                                        |
| **DSL5** ControllerUpdating(id)                | A specific controller is being updated. This is a good time to call [`SetButtonPressed`](SetButtonPressed).                                                             |
| **DSL5** GameBeingPaused()                     | The game will pause unless an event handler returns `true`.                                                                                                             |
| **DSL4** NativeScriptLoaded(name, env)         | A base game script has been loaded and run, but not yet updated (meaning its main function hasn't run).                                                                 |
| **DSL5** PedBeingCreated()                     | A ped is about to be created. You can count peds with [`AllPeds`](AllPeds) to determine if you should delete a ped to prevent a crash.                                  |
| **DSL5** PedStatOverriding(ped, stat, value)   | A ped's stat is being changed unless an event handler returns `true`. Beware setting the stat yourself will still activate the event.                                   |
| **DSL7** PedUpdateThrottle(ped)                | A ped is updating their action throttle, which can happen multiple times per frame. This is a good time to call [`PedSetThrottle`](PedSetThrottle).                     |
| **DSL7** PlayerBuilding(is_player,is_cutscene) | A ped's model will rebuild unless an event handler returns `true`. This can prevent replacing ped models with player clothes.                                           |
| **DSL5** PlayerSleepCheck()                    | The game wants to check if the player should fall asleep, but will skip the check if an event handler returns `true`.                                                   |
| **DSL5** SaveGameLoading()                     | A save game is going to be loaded unless an event handler returns `true`.                                                                                               |
| **DSL9** ScriptDestroyed(script)               | A script object has been destroyed.                                                                                                                                     |
| **DSL9** ScriptShutdown(script)                | A script object is being shutdown. This happens before destruction.                                                                                                     |
| **DSL7** ServerConnected()                     | The active server is now fully connected to.                                                                                                                            |
| **DSL7** ServerConnecting(address, hashes)     | A server connection has begun, and can be considered "active" until the `ServerDisconnected` event.                                                                     |
| **DSL7** ServerDisconnected(address)           | A server has been disconnected from. Always comes after a ServerConnecting event (unless the game is quit).                                                             |
| **DSL7** ServerDownloading()                   | The active server is downloading files for the first time.                                                                                                              |
| **DSL7** ServerKicked(reason)                  | The active server issued a kick (and a seperate `ServerDisconnected` event will still follow).                                                                          |
| **DSL7** ServerListing(address, listing)       | A server has provided listing information. The listing table contains `name`, `info`, `mode`, `icon`, `players`, and `max_players`.                                     |
| **DSL5** WindowGoingFullscreen()               | The game will enter exclusive fullscreen mode unless an event handler returns `true`.                                                                                   |
| **DSL5** WindowMinimizing()                    | The game's window will be minimized unless an event handler returns `true`.                                                                                             |
| **DSL5** WindowUpdating(window)                | The game's window can be customly styled if any event handler returns `true`. The window table contains fields describing the window.                                   |

### Server

| Type                                    | Description                                                                                                                                                       |
| --------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **DSL5** PlayerConnected(player)        | A player has fully connected and can be used safely with any networking functions.                                                                                |
| **DSL5** PlayerConnecting(player)       | A player is connecting and can only be used with some functions. Kick them to prevent them from being connected.                                                  |
| **DSL5** PlayerDropped(player)          | A player has been dropped and all references to them should be removed. Will always come after a `PlayerConnecting` event.                                        |
| **DSL5** PlayerListing(player, listing) | A player requested listing information for the server. You can modify the listing table's info and mode. The player is only valid for the duration of this event. |
| **DSL8** ServerShutdown()               | The server is being shutdown. The Lua state closes immediately after this event. This event is only triggered when the server is "gracefully" shutdown.           |

### Shared

| Type                               | Description                                                                                                             |
| ---------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| **DSL5** ScriptPrinted(text, type) | One of the print functions have been called. This is mainly designed to help forward console output into a server chat. |

## See Also

- DSL
  - [`RemoveEventHandler`](RemoveEventHandler)
