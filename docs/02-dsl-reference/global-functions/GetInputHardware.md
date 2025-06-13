---
description: Returns what hardware a certain input is bound to.
sidebar_class_name: hidden
---

# GetInputHardware

> **_This function was added in DSL 5_**

## Description

Returns what hardware a certain input is bound to. The possible values for `type` are as follows.

- **button**: `value` is a button from an xbox controller [0-15]
- **analog**: `value` is an analog stick from an xbox controller [16-23]
- **special**: `value` is the skateboard button from an xbox controller (24)
- **keyboard**: `value` is a DirectInput Keyboard Scan Code [0,255]
- **mouse_button**: `value` is a DirectInput Mouse button index [0,3]
- **mouse_movement**: `value` represents DirectInput mouse movement [0,5]

```lua
function GetInputHardware(button_or_stick, controller) --[[ ... ]] end
```

## Parameters

- `button_or_stick`: _`integer`_ - The button or stick ID to get the hardware for. <!-- See the [Button Codes](../button-codes) and [Stick Codes](../stick-codes) pages for a list of button and stick IDs. -->
- `controller`: _`0|1|2|3`_ - The controller to get the hardware for. <!-- `0` is the keyboard, `1` is the first controller, `2` is the second controller, and `3` is the third controller. -->

## Return Values

- `type`: _`string`_ - The type of hardware the input is bound to. Possible values are `button`, `analog`, `special`, `keyboard`, `mouse_button`, or `mouse_movement`.
- `value`: _`number`_ - The value associated with the input. The meaning of this value depends on the `type` returned.

## Example

```lua
local type, value = GetInputHardware(0, 1) -- Get the hardware for button 0 on controller 1 (Left arrow keyboard key, d-pad left)
if type == 'button' then
  print('Button 0 on controller 1 is bound to hardware value:', value)
elseif type == 'analog' then
  print('Analog stick 0 on controller 1 is bound to hardware value:', value)
elseif type == 'special' then
  print('Special button on controller 1 is bound to hardware value:', value)
elseif type == 'keyboard' then
  print('Keyboard input on controller 1 is bound to hardware value:', value)
elseif type == 'mouse_button' then
  print('Mouse button on controller 1 is bound to hardware value:', value)
elseif type == 'mouse_movement' then
  print('Mouse movement on controller 1 is bound to hardware value:', value)
else
  print('Unknown input type:', type)
end
```
