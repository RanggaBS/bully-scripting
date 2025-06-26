---
description: Sets text clipping boundaries to limit text display area.
sidebar_class_name: hidden
---

# SetTextClipping

## Description

Sets the clipping boundaries for text drawing, limiting how large the text can be before it gets cut off. For example if you use 0.5 for the width and draw at 0 x, anything past the center of the screen will be cut off. This is useful for constraining text to specific areas of the screen or creating text boxes with defined boundaries. Text clipping and word wrapping are not compatible - using one will disable the other. Not specifying an argument means that direction will not be clipped.

*Introduced in DSL 2.*

```lua
function SetTextClipping(width, height) --[[ ... ]] end
```

## Parameters


- `width`: _`number`_ - (Optional) The maximum normalized width for text display (0.0 to 1.0). Use `nil` to disable width clipping
- `height`: _`number`_ - (Optional) The maximum normalized height for text display (0.0 to 1.0). Use `nil` to disable height clipping

## Return Values

None.

## Example

```lua
-- Clip text to left half of screen
SetTextClipping(0.5, nil) -- Width limited to 50%, height unlimited
SetTextPosition(0.5, 0.3)
SetTextScale(1.0)
DrawText("The birds of the air, and the fish of the sea, the things that pass through the paths of the sea.")
```

```lua
-- Create a chat box area
local function drawChatMessage(message, x, y)
    -- highlight-next-line
    SetTextClipping(0.4, 0.15) -- Chat box area
    SetTextPosition(x, y)
    SetTextScale(0.7)
    SetTextAlign("left", "top")
    SetTextColor(255, 255, 255, 255)
    DrawText(message)
end

-- Usage
drawChatMessage("Player1: This is a long chat message that will be clipped to fit in the chat area.", 0.05, 0.7)
drawChatMessage("Player2: This is even a longer chat message that will be clipped to fit in the chat area down to the last character.", 0.05, 0.75)
```

```lua
-- Create a status display area
-- highlight-next-line
SetTextClipping(0.25, 0.1) -- Status area in corner
SetTextPosition(0.75, 0.05)
SetTextScale(0.6)
SetTextAlign("left", "top")
SetTextColor(200, 255, 200, 255)
DrawText("Health: 100\nAmmo: 50\nScore: 1250\nTime: 05:42")
```

## See Also

- DSL
  - [`SetTextPosition`](./SetTextPosition)
  - [`SetTextScale`](./SetTextScale)
  - [`SetTextAlign`](./SetTextAlign)
  - [`SetTextColor`](./SetTextColor)