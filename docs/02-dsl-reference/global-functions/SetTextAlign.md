---
description: Sets the horizontal and vertical alignment for text drawing.
sidebar_class_name: hidden
---

# SetTextAlign

## Description

Use alignment strings to control how text is positioned relative to the coordinates set by `SetTextPosition`. The first argument controls horizontal alignment, and the optional second argument controls vertical alignment. Only the first letter of each alignment string is actually used.

```lua
function SetTextAlign(horizontalAlign, verticalAlign) --[[ ... ]] end
```

## Parameters

- `horizontalAlign`: _`string`_ - Horizontal alignment: "left", "right", or "center" (default)
- `verticalAlign`: _`string`_ - (Optional) Vertical alignment: "top" (default), "bottom", or "center"

## Return Values

None.

## Example

```lua
-- HUD elements using proper alignment
-- Top-left health (left-aligned from left edge)
SetTextPosition(0.05, 0.05)
-- highlight-next-line
SetTextAlign("left")
SetTextHeight(0.03)
SetTextColor(255, 100, 100, 255)
DrawText("Health: 100%")

-- Top-center score (center-aligned)
SetTextPosition(0.5, 0.05)
SetTextAlign("center", "top")
SetTextHeight(0.04)
SetTextColor(255, 255, 0, 255)
DrawText("Score: 12,500")

-- Top-right timer (right-aligned from right edge)
SetTextPosition(0.95, 0.05)
SetTextAlign("right", "top")
SetTextHeight(0.03)
SetTextColor(100, 255, 100, 255)
DrawText("Time: 05:23")

-- Bottom-center message (center-aligned from bottom)
SetTextPosition(0.5, 0.9)
SetTextAlign("center", "bottom")
SetTextHeight(0.025)
SetTextColor(255, 255, 255, 255)
DrawText("Press ESC for menu")
```

```lua
-- Table with column alignment
local tableData = {
    {"Name", "Score", "Time"},
    {"Alice", "1500", "02:30"},
    {"Bob", "1200", "03:15"},
    {"Charlie", "900", "04:00"}
}

local colX = {0.2, 0.5, 0.8}
local colAlign = {"left", "center", "right"}
local startY = 0.1
local rowHeight = 0.04

for rowIndex, row in ipairs(tableData) do
    local y = startY + (rowIndex - 1) * rowHeight
    
    for colIndex, cell in ipairs(row) do
        SetTextPosition(colX[colIndex], y)
        SetTextAlign(colAlign[colIndex], "top")
        SetTextHeight(0.025)
        
        if rowIndex == 1 then
            SetTextColor(255, 255, 0, 255) -- Header
        else
            SetTextColor(255, 255, 255, 255) -- Data
        end
        
        DrawText(cell)
    end
end
```

```lua
-- Dialog box with proper text alignment
local function drawDialogBox(title, message, x, y, width, height)
    -- Draw background
    DrawRectangle(x, y, width, height, 0, 0, 0, 200)
    DrawRectangle(x, y, width, 0.002, 255, 255, 255, 255) -- Top border
    
    -- Title (center-aligned at top)
    SetTextPosition(x + width/2, y + 0.02)
    SetTextAlign("center", "top")
    SetTextHeight(0.035)
    SetTextColor(255, 255, 0, 255)
    DrawText(title)
    
    -- Message (left-aligned with margins)
    SetTextPosition(x + 0.02, y + 0.08)
    SetTextAlign("left", "top")
    SetTextHeight(0.025)
    SetTextColor(255, 255, 255, 255)
    SetTextWrapping(width - 0.04) -- Word wrap within box
    DrawText(message)
end

-- Example dialog
drawDialogBox(
    "Important Notice",
    "This is an important message that needs to be displayed to the player. It demonstrates proper text alignment within a dialog box.",
    0.2, 0.3, 0.6, 0.3
)
```

```lua
-- Tooltip with dynamic alignment
local function drawTooltip(text, mouseX, mouseY)
    local padding = 0.02
    
    SetTextHeight(0.02)
    local textWidth, textHeight = MeasureText(text)
    
    local boxWidth = textWidth + padding
    local boxHeight = textHeight + padding
    
    -- Adjust position to keep tooltip on screen
    local x = mouseX
    local y = mouseY - boxHeight - 0.02
    
    -- Right align if too close to right edge
    local align = "left"
    if x + boxWidth > 0.95 then
        x = mouseX - boxWidth
        align = "right"
    end
    
    -- Draw tooltip background
    DrawRectangle(x, y, boxWidth, boxHeight, 50, 50, 50, 240)
    
    -- Draw tooltip text
    SetTextPosition(x + (align == "left" and padding/2 or boxWidth - padding/2), y + padding/2)
    SetTextAlign(align, "top")
    SetTextColor(255, 255, 255, 255)
    DrawText(text)
end

-- Example tooltip usage
drawTooltip("This is a helpful tooltip", 0.7, 0.6)
```

## See Also

- DSL
  - [`SetTextPosition`](./SetTextPosition)
  - [`SetTextHeight`](./SetTextHeight)
  - [`SetTextColor`](./SetTextColor)