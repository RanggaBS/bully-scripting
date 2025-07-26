---
description: Terminate the current script.
sidebar_class_name: hidden
---

# TerminateCurrentScript

> **_This function was added in DSL 1_**

## Description

This function replaces the existing [`TerminateCurrentScript`](TerminateCurrentScript).

If DSL is not running _or_ [`UseBaseGameScriptFunctions`](UseBaseGameScriptFunctions) was called with `true`, the original function is used. Otherwise the current DSL script is shutdown.

This does not instantly take control away from your script, meaning your code will continue execution until the current thread yields or control is otherwise returned to DSL.

```lua
function TerminateCurrentScript() --[[ ... ]] end
```

## Parameters

None.

## Return Values

None.

## Example

Stop the script when a button is pressed.

```lua
function main()
  while not SystemIsReady() do
    Wait(0)
  end
  while true do
    TextPrintString('running', 0, 2)
    Wait(0)
    if IsButtonBeingPressed(3,0) then
      TerminateCurrentScript()
      print('this will be printed because control is not instantly taken away')
      Wait(0)
      print('this will not be printed because waiting gave control back to DSL')
    end
  end
end
```

## See Also

- Game's Native
  - [TerminateCurrentScript](/docs/game-reference/global-functions/TerminateCurrentScript)
- DSL
  - [TerminateScript](TerminateScript)
