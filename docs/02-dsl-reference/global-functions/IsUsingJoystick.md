---
description: Returns if the controller is an xbox controller.
sidebar_class_name: hidden
---

# IsUsingJoystick

> **_This function was added in DSL 5_**

## Description

Returns if the controller is an xbox controller (otherwise it a keyboard).

```lua
function IsUsingJoystick(controllerId) --[[ ... ]] end
```

## Parameters

- `controllerId`: _`0|1|2|3`_ - The controller to check. <!-- `0` is the keyboard, `1` is the first controller, `2` is the second controller, and `3` is the third controller. -->

## Return Values

- `isUsingJoystick`: _`boolean`_ - `true` if the controller is an xbox controller, `false` if it is a keyboard.

## Example

```lua
if IsUsingJoystick(0) then
  print('Player 1 is using an xbox controller.')
else
  print('Player 1 is using a keyboard.')
end
```
