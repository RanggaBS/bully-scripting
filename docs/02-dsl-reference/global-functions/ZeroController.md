---
description: Zero all the input memory on a controller.
sidebar_class_name: hidden
---

# ZeroController

> **_This function was added in DSL 6_**

## Description

Zero all the input memory on a controller.

This is a good way to disable all input on an input device, but remember to call it on both controller-related events. If you do not call it during both events, buttons may misbehave and act like they're being repeatedly pressed.

```lua
function ZeroController(controller) --[[ ... ]] end
```

## Parameters

- `controller`: _`0|1|2|3`_ - The controller to zero. <!-- `0` is the keyboard, `1` is the first controller, `2` is the second controller, and `3` is the third controller. -->

## Return Values

None.

## Versions

- **DSL5** - This function was released as `DisableController` but did not work properly.
- **DSL6** - This function now works as intended and was re-named.

## Example

Disable the player's controls fully.

```lua
RegisterLocalEventHandler('ControllerUpdating', function(controller)
  if controller == 0 then
    ZeroController(controller)
  end
end)
RegisterLocalEventHandler('ControllersUpdated', function()
  ZeroController(0)
end)
```
