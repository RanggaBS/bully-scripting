---
description: Registers a new network event handler.
sidebar_class_name: hidden
---

# RegisterNetworkEventHandler

> **_This function was added in DSL 5_**

## Description

Registers a new network event handler. The `callback` function is called when the event is activated. The returned `eventHandler` object is registered with the current script, meaning it will be removed when the script dies. If there is no current DSL script to register with, it will exist until removed manually with [`RemoveEventHandler`](RemoveEventHandler).

An `eventType` is just a string. Unlike [`RegisterLocalEventHandler`](RegisterLocalEventHandler), there are no built-in events. Network events can only be activated by the [`SendNetworkEvent`](SendNetworkEvent) function being called on the other side of the connection.

Since the event is sent over a network connection, you should **not** trust the arguments given to your callback. Make sure to type check them if you do not want your script misbehaving.

On the server, the first argument given to your callback function is the `playerId` for the player that sent the event. You can always trust this is a valid player id.

```lua
function RegisterNetworkEventHandler(eventType, callback) --[[ ... ]] end
```

## Parameters

- `eventType`: _`string`_ - The name of the event to register. This can be any string, but should be unique to avoid conflicts with other scripts.
- `callback`: _`fun(playerId: integer, ...: any): any`_ - The function to call when the event is triggered. The first argument is the `playerId` of the player that sent the event, and the rest are the arguments sent with the event.

## Return Values

- `eventHandler`: _`userdata`_ - An object representing the event handler.

## Example

Tell all players in the server when a player dies.

### Client script

```lua
function main()
  while not SystemIsReady() do
    Wait(0)
  end
  while true do
    if PedIsDead(gPlayer) then
      SendNetworkEvent("example:playerDied") -- putting "yourModName:" in front of events helps prevent naming conflicts with other scripts
      repeat
        Wait(0)
      until not PedIsDead(gPlayer) -- wait until we're not dead so that the server isn't just spammed with events every frame we're dead
    end
    Wait(0)
  end
end
RegisterNetworkEventHandler("example:notifyPlayerDeath",function(name)
  TextPrintString(name.." has died!",3,2)
end)
```

### Server script

```lua
RegisterNetworkEventHandler("example:playerDied",function(player) -- on the server, a valid player is always the first argument
  SendNetworkEvent(-1,"example:notifyPlayerDeath",GetPlayerName(player)) -- using -1 as the first argument means this event is sent to ALL players
end)
```

## See Also

- DSL
  - [`RegisterLocalEventHandler`](RegisterLocalEventHandler)
  - [`RemoveEventHandler`](RemoveEventHandler)
  - [`SendNetworkEvent`](SendNetworkEvent)
