---
description: Creates a function in the calling environment that will use `CallFunctionFromScript` to call the function given.
sidebar_class_name: hidden
---

# UseProxyScriptForFunction

> **_This function was added in DSL 4_**

## Description

Creates a function in the calling environment that will use [`CallFunctionFromScript`](./CallFunctionFromScript) to call the function given. _`function`_ is presumed to be in the global environment.

For some functions, this can give you a way to make use of things that don't work in DSL. The most notable example is [`BlipAddXYZ`](/docs/game-reference/global-functions/BlipAddXYZ) not letting you create ground blips.

```lua
function UseProxyScriptForFunction(script, functionName) --[[ ... ]] end
```

## Parameters

- `script`: _`string|nil`_ - The name of the script to use as a proxy. If `nil`, it will spoof the game into thinking there are no scripts running.
- `functionName`: _`string`_ - The name of the function to create in the calling environment.

## Return Values

None.

## Example

Add a ground blip in front of the boy's dorm.

```lua
UseProxyScriptForFunction('main.lua', 'BlipAddXYZ')
UseProxyScriptForFunction('main.lua', 'BlipRemove')

gCreatedBlip = -1

function main()
  while not SystemIsReady() do
    Wait(0)
  end

  -- since we setup a proxy script for this function, the blip is actually going
  -- to be created by main.lua
  gCreatedBlip = BlipAddXYZ(270, -110, 6, 25, 1, 1)
end

function MissionCleanup()
  -- it is very important we delete the blip ourselves since it doesn't belong
  -- to our script, meaning it won't be cleaned up naturally
  if gCreatedBlip ~= -1 then
    BlipRemove(gCreatedBlip)
  end
end
```
