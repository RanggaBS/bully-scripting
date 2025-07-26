---
description: Starts a new thread using the specified function or an anonymous function.
sidebar_class_name: hidden
---

# CreateThread

> **_This function was added in DSL 1_**

## Description

:::info
This function replaces the existing [`CreateThread`](/docs/game-reference/global-functions/CreateThread).
:::

If DSL is not running or [`UseBaseGameScriptFunctions`](UseBaseGameScriptFunctions) was called with _`true`_, the original function is used. Otherwise a [**`GAME`**](/docs/dsl-reference/basic-concepts/scripts#thread-types) thread is created and added to the current script. These threads run directly after the base game's.

When creating a DSL script, `func` can be a string to refer to a function in the current script's environment. In this case, the name of the thread is also preserved to be shown in console messages or returned with [`GetThreadName`](./GetThreadName).

Any extra arguments (`...`) are passed to the thread function when the thread starts.

```lua
function CreateThread(func, ...) --[[ ... ]] end
```

## Parameters

- `func` - _`function|string`_ - The function to run in the thread. If a string is provided, it refers to a function in the current script's environment.
- `...`: _`any`_ - (Optional) Additional arguments to pass to the thread function when it starts. These can be any Lua values, such as numbers, strings, tables, etc.

## Return Values

- `thread` - _`thread`_ - The thread that was created. This can be used to control the thread, such as pausing or stopping it.

## Example

Do something on a delay by quickly creating a thread with an anonymous function.

```lua
function main()
  while not SystemIsReady() do
    Wait(0)
  end
  while true do
    local ped = PedGetTargetPed(gPlayer)
    if PedIsValid(ped) and IsButtonBeingPressed(7, 0) then
      -- player insulted a ped, let's apply emotional damage after a second delay
      CreateThread(function()
        Wait(1000)
        if PedIsValid(ped) then -- make sure they're still valid after waiting
          PedApplyDamage(ped, 1000)
        end
      end)
    end
  end
end
```

## See Also

- DSL
  - [`UseBaseGameScriptFunctions`](./UseBaseGameScriptFunctions)
  - [`GetThreadName`](./GetThreadName)
- Game's Native
  - [`CreateThread`](/docs/game-reference/global-functions/CreateThread)
