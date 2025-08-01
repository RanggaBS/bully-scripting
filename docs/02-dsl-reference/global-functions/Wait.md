---
description: Wait for a specified amount of time.
sidebar_class_name: hidden
---

# Wait

> **_This function was added in DSL 1_**

## Description

Wait for a specified amount of time.

This function replaces the existing [`Wait`](/docs/game-reference/global-functions/Wait). If DSL is not running or [`UseBaseGameScriptFunctions`](UseBaseGameScriptFunctions) was called with `true`, the original function is used. Otherwise the current thread will yield and next time it will be allowed to update is set to `milliseconds` from now.

```lua
function Wait(milliseconds) --[[ ... ]] end
```

## Parameters

- `milliseconds`: _`number`_ - The time to wait in milliseconds.

## Return Values

None.

## Example

Almost every script will need to make use of Wait.

```lua
function main()
  -- wait until the system is ready before doing anything else
  while not SystemIsReady() do
    Wait(0)
  end

  -- main loop that is always running for as long as the script is alive
  while true do
    TextPrintString('you can script things that run every frame here', 0, 2)
    Wait(0)
  end
end
```
