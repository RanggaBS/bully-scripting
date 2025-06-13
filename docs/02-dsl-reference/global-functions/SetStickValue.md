---
description: Set a stick's value.
sidebar_class_name: hidden
---

# SetStickValue

> **_This function was added in DSL 5_**

## Description

Set a stick's value.

This function is intended to be called during a `ControllersUpdated` event. Calling it at any other time may produce unexpected results.

```lua
function SetStickValue(stick, controller, value) --[[ ... ]] end
```

## Parameters

- `stick`: _`integer`_ - The stick ID to set the value for. <!-- See the [Stick Codes](../stick-codes) page for a list of stick IDs. -->
- `controller`: _`0|1|2|3`_ - The controller to set the stick on. <!-- `0` is the keyboard, `1` is the first controller, `2` is the second controller, and `3` is the third controller. -->
- `value`: _`number`_ - The value to set the stick to.

## Return Values

None.

## Example

If player one is using keyboard, re-map their camera controls to use direct mouse input.

```lua
RegisterLocalEventHandler('ControllersUpdated', function()
  if not IsUsingJoystick(0) then
    local x, y = GetMouseInput()
    SetStickValue(18, 0, -x * 0.02)
    SetStickValue(19, 0, -y * 0.02)
  end
end)
```
