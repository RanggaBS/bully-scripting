---
description: Returns direct mouse input.
sidebar_class_name: hidden
---

# GetMouseInput

> **_This function was added in DSL 1_**

## Description

Returns the direct mouse movement input as relative changes (deltas) in the X and Y axes since the last input poll.

These values indicate how much the mouse has moved, not its absolute screen position.

The magnitude of these values depends on the speed of the mouse movement.

```lua
function GetMouseInput() --[[ ... ]] end
```

## Parameters

None.

## Return Values

Two numbers representing the mouse movement:

- `deltaX`: _`number`_ - The relative horizontal movement (delta X) of the mouse. Positive values typically indicate movement to the right, while negative values indicate movement to the left. The value can range, for example, from approximately -300 to 300, depending on how quickly the mouse is moved.
- `deltaY`: _`number`_ - The relative vertical movement (delta Y) of the mouse. Positive values typically indicate movement downwards, while negative values indicate movement upwards. The value can range, for example, from approximately -300 to 300, depending on how quickly the mouse is moved.

## Versions

- **DSL4** - This function now works properly, without the need for running on a specific thread.

## Example

Polling the mouse input in a loop and displaying the movement deltas:

```lua
function main()
  while true do
    local mouseDeltaX, mouseDeltaY = GetMouseInput()

    -- Check if the mouse has moved
    if mouseDeltaX ~= 0 or mouseDeltaY ~= 0 then
      DrawTextInline('Mouse moved by: X = ' .. mouseDeltaX .. ', Y = ' .. mouseDeltaY, 0, 1)
    end

    Wait(0)
  end
end
```
