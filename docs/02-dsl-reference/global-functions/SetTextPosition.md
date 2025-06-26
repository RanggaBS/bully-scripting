---
description: Sets the position for the text.
sidebar_class_name: hidden
---

# SetTextPosition

## Description

Set the normalized coordinates for the text draw. The coordinate system uses values from 0.0 to 1.0, where (0.0, 0.0) is the top left of the display and (1.0, 1.0) is the bottom right. The exact meaning of these coordinates depends on the text alignment settings.

```lua
function SetTextPosition(x, y) --[[ ... ]] end
```

## Parameters

- `x`: _`number`_ - The X coordinate for text positioning (0.0 to 1.0)
- `y`: _`number`_ - The Y coordinate for text positioning (0.0 to 1.0)

## Return Values

None.

## Example

```lua
-- Basic text positioning
-- highlight-next-line
SetTextPosition(0.5, 0.1) -- Center horizontally, near top
SetTextHeight(0.05)
SetTextAlign("center")
SetTextColor(255, 255, 255, 255)
DrawText("Title Text")
```

```lua
-- Position text in different screen areas
local positions = {
    {x = 0.1, y = 0.1, text = "Top Left"},
    {x = 0.9, y = 0.1, text = "Top Right"},
    {x = 0.1, y = 0.9, text = "Bottom Left"},
    {x = 0.9, y = 0.9, text = "Bottom Right"},
    {x = 0.5, y = 0.5, text = "Center"}
}

SetTextHeight(0.03)
for _, pos in ipairs(positions) do
-- highlight-next-line
    SetTextPosition(pos.x, pos.y)
    SetTextAlign("center")
    SetTextColor(255, 255, 0, 255)
    DrawText(pos.text)
end
```

```lua
-- Grid layout using calculated positions
local gridCols = 3
local gridRows = 2
local startX = 0.2
local startY = 0.3
local gridWidth = 0.6
local gridHeight = 0.4

for row = 1, gridRows do
    for col = 1, gridCols do
        local x = startX + (col - 1) * (gridWidth / (gridCols - 1))
        local y = startY + (row - 1) * (gridHeight / (gridRows - 1))
        -- highlight-next-line
        SetTextPosition(x, y)
        SetTextAlign("center")
        SetTextHeight(0.025)
        SetTextColor(255, 255, 255, 255)
        DrawText("Item %d-%d", row, col)
    end
end
```

```lua
-- Moving text animation
local time = 0
while true do
    time = time + GetFrameTime()
    
    -- Sine wave movement
    local x = 0.5 + 0.3 * math.sin(time)
    local y = 0.8
    -- highlight-next-line
    SetTextPosition(x, y)
    SetTextAlign("center")
    SetTextHeight(0.03)
    SetTextColor(100, 255, 255, 255)
    DrawText("Moving Text")
    
    Wait(0)
end
```

## See Also

- DSL
  - [`SetTextHeight`](./SetTextHeight)
  - [`SetTextAlign`](./SetTextAlign)
  - [`SetTextShadow`](./SetTextShadow)
  - [`SetTextColor`](./SetTextColor)