---
description: Sets the size of text.
sidebar_class_name: hidden
---

# SetTextHeight

## Description

Set the size of the text. The height is specified as a value from 0.0 to 1.0, where 0.2 means the text will take up 20% of the display's height. This provides consistent text sizing across different screen resolutions.

```lua
function SetTextHeight(height) --[[ ... ]] end
```

## Parameters

- `height`: _`number`_ - The height of the text (0.0 to 1.0)

## Return Values

None.

## Example

```lua
-- HUD elements with appropriate sizes
-- Title text
SetTextPosition(0.5, 0.05)
-- highlight-next-line
SetTextHeight(0.06)
SetTextAlign("center")
SetTextColor(255, 255, 0, 255)
DrawText("GAME TITLE")

-- Subtitle
SetTextPosition(0.5, 0.12)
-- highlight-next-line
SetTextHeight(0.025)
SetTextAlign("center")
SetTextColor(200, 200, 200, 255)
DrawText("Press SPACE to continue")

-- Status text
SetTextPosition(0.05, 0.95)
-- highlight-next-line
SetTextHeight(0.02)
SetTextAlign("left", "bottom")
SetTextColor(255, 255, 255, 255)
DrawText("Version 1.0")
```

```lua
-- Dynamic text scaling for emphasis
local time = 0
while true do
    time = time + GetFrameTime()
    
    -- Pulsing text effect
    local scale = 1.0 + 0.2 * math.sin(time * 3)
    local height = 0.04 * scale
    
    SetTextPosition(0.5, 0.3)
    -- highlight-next-line
    SetTextHeight(height)
    SetTextAlign("center")
    SetTextColor(255, 100, 100, 255)
    DrawText("ALERT!")
    
    Wait(0)
end
```

```lua
-- Text hierarchy with proper sizing
local headings = {
    {text = "Main Heading", height = 0.06, color = {255, 255, 0}},
    {text = "Sub Heading", height = 0.04, color = {200, 200, 200}},
    {text = "Body text content here", height = 0.025, color = {255, 255, 255}},
    {text = "Small details", height = 0.018, color = {150, 150, 150}}
}

local y = 0.2
for _, heading in ipairs(headings) do
    SetTextPosition(0.1, y)
    -- highlight-next-line
    SetTextHeight(heading.height)
    SetTextAlign("left", "top")
    SetTextColor(heading.color[1], heading.color[2], heading.color[3], 255)
    DrawText(heading.text)
    y = y + heading.height + 0.02
end
```

## See Also

- DSL
  - [`SetTextPosition`](./SetTextPosition)
  - [`SetTextAlign`](./SetTextAlign)
  - [`SetTextShadow`](./SetTextShadow)
  - [`SetTextColor`](./SetTextColor)