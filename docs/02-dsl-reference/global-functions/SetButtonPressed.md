---
description: Set a button as pressed.
sidebar_class_name: hidden
---

# SetButtonPressed

> **_This function was added in DSL 5_**

## Description

Set a button as pressed.

This function is intended to be called during a `ControllerUpdating` event. Calling it at any other time may produce unexpected results. This is often a good way of disabling a specific button on a specific controller.

```lua
function SetButtonPressed(button, controller, pressed) --[[ ... ]] end
```

## Parameters

- `button`: _`integer`_ - The button ID to set as pressed. <!-- See the [Button Codes](../button-codes) page for a list of button IDs. -->
- `controller`: _`0|1|2|3`_ - The controller to set the button on. <!-- `0` is the keyboard, `1` is the first controller, `2` is the second controller, and `3` is the third controller. -->
- `pressed`: _`boolean`_ - Whether to set the button as pressed or not. If `true`, the button will be considered pressed, if `false`, it will be considered not pressed.

## Return Values

None.

## Example

Disable the sprint button for all controllers.

```lua
RegisterLocalEventHandler('ControllerUpdating', function(controller)
  SetButtonPressed(7, controller, false)
end)
```

## See Also

- Game's Native
  - [`IsButtonBeingPressed`](/docs/game-reference/global-functions/IsButtonBeingPressed)
  - [`IsButtonBeingReleased`](/docs/game-reference/global-functions/IsButtonBeingReleased)
  - [`IsButtonPressed`](/docs/game-reference/global-functions/IsButtonPressed)
