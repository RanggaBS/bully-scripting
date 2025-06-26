---
description: Sets the color and alpha transparency for text drawing.
sidebar_class_name: hidden
---

# SetTextColor

## Description

Use the specified color and alpha value for text drawing. The color values should be in the range of 0 to 255. This function is also defined as `SetTextColour` for those who prefer British spelling.

```lua
function SetTextColor(red, green, blue, alpha) --[[ ... ]] end
```

## Parameters

- `red`: _`number`_ - The red color component (0 to 255)
- `blue`: _`number`_ - The green color component (0 to 255)
- `blue`: _`number`_ - The blue color component (0 to 255)
- `alpha`: _`number`_ - The alpha transparency (0 = transparent, 255 = opaque)

## Return Values

None.

## Example

```lua
-- Basic color examples
local colors = {
    {255, 255, 255, 255, "White"},
    {255, 0, 0, 255, "Red"},
    {0, 255, 0, 255, "Green"},
    {0, 0, 255, 255, "Blue"},
    {255, 255, 0, 255, "Yellow"},
    {255, 0, 255, 255, "Magenta"},
    {0, 255, 255, 255, "Cyan"},
    {128, 128, 128, 255, "Gray"}
}

local y = 0.1
for _, color in ipairs(colors) do
    SetTextPosition(0.1, y)
    SetTextHeight(0.03)
    SetTextAlign("left", "top")
    -- highlight-next-line
    SetTextColor(color[1], color[2], color[3], color[4])
    DrawText(color[5])
    y = y + 0.04
end

-- Transparency effects
local alphaValues = {255, 200, 150, 100, 50}
local x = 0.5
for i, alpha in ipairs(alphaValues) do
    SetTextPosition(x, 0.3)
    SetTextHeight(0.03)
    SetTextAlign("center")
    -- highlight-next-line
    SetTextColor(255, 255, 255, alpha)
    DrawText("Alpha: %d", alpha)
    x = x + 0.1
end
```

```lua
-- UI color coding
CreateDrawingThread(function()
    while true do
        -- Health status with color coding
        local health = 75 -- Example health value
        local healthColor = {255, 255, 255, 255} -- Default white
        
        if health > 75 then
            healthColor = {0, 255, 0, 255} -- Green for good health
        elseif health > 50 then
            healthColor = {255, 255, 0, 255} -- Yellow for medium health
        elseif health > 25 then
            healthColor = {255, 128, 0, 255} -- Orange for low health
        else
            healthColor = {255, 0, 0, 255} -- Red for critical health
        end
        
        SetTextPosition(0.05, 0.05)
        SetTextHeight(0.03)
        SetTextAlign("left", "top")
        -- highlight-next-line
        SetTextColor(healthColor[1], healthColor[2], healthColor[3], healthColor[4])
        DrawText("Health: %d%%", health)
        
        Wait(0)
    end
end)
```

```lua
-- Gradient text effect
local function drawGradientText(text, x, y, startR, startG, startB, endR, endG, endB)
    SetTextHeight(0.04)
    local textWidth, textHeight = MeasureText(text)
    
    local steps = string.len(text)
    for i = 1, steps do
        local char = string.sub(text, i, i)
        local progress = (i - 1) / (steps - 1)
        
        -- Interpolate colors
        local r = startR + (endR - startR) * progress
        local g = startG + (endG - startG) * progress
        local b = startB + (endB - startB) * progress
        
        local charWidth = MeasureText(char)
        local charX = x + (i - 1) * (textWidth / steps)
        
        SetTextPosition(charX, y)
        SetTextAlign("left", "top")
        -- highlight-next-line
        SetTextColor(r, g, b, 255)
        DrawText(char)
    end
end

-- Example gradient text
drawGradientText("GRADIENT EFFECT", 0.3, 0.7, 255, 0, 0, 0, 0, 255) -- Red to blue
```

```lua
-- System message colors
local function showSystemMessage(message, messageType)
    local colors = {
        info = {100, 200, 255, 255},    -- Light blue
        warning = {255, 200, 0, 255},   -- Orange
        error = {255, 100, 100, 255},   -- Light red
        success = {100, 255, 100, 255}  -- Light green
    }
    
    local color = colors[messageType] or colors.info
    
    SetTextPosition(0.5, 0.1)
    SetTextAlign("center")
    SetTextHeight(0.03)
    -- highlight-next-line
    SetTextColor(color[1], color[2], color[3], color[4])
    DrawText(message)
end

-- Example system messages
showSystemMessage("Game saved successfully", "success")
```

## See Also

- DSL
  - [`SetTextColour`](./SetTextColour)
  - [`SetTextPosition`](./SetTextPosition)
  - [`SetTextAlign`](./SetTextAlign)
  - [`SetTextHeight`](./SetTextHeight)