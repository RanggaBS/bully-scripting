---
description: Restores previously saved text formatting settings.
sidebar_class_name: hidden
---

# SetTextFormatting

## Description

Restores text formatting settings from a text format table previously saved with `GetTextFormatting()` or `PopTextFormatting()`. This allows you to save a formatting state, make temporary changes, and then restore the original formatting configuration.

```lua
function SetTextFormatting(formatting) --[[ ... ]] end
```

## Parameters

- `formatting`: _`table`_ - A text format table returned by `GetTextFormatting()` or `PopTextFormatting()`

## Return Values

None.

## Example

```lua
-- Save current formatting state
SetTextPosition(0.5, 0.3)
SetTextScale(1.0)
SetTextColor(255, 255, 255, 255)
SetTextAlign("center", "top")

local originalFormat = GetTextFormatting()

-- Make temporary changes
SetTextScale(1.5)
SetTextColor(255, 0, 0, 255)
SetTextBold()
DrawText("ALERT MESSAGE")

-- Restore original formatting
-- highlight-next-line
SetTextFormatting(originalFormat)
SetTextPosition(0.5, 0.5)
DrawText("Back to normal formatting")
```

```lua
-- Function to switch between text styles
local textStyles = {
    header = nil,
    body = nil,
    caption = nil
}

local function initializeTextStyles()
    -- Header style
    SetTextScale(1.3)
    SetTextColor(200, 200, 255, 255)
    SetTextBold()
    SetTextAlign("center", "top")
    textStyles.header = PopTextFormatting()
    
    -- Body style
    SetTextScale(0.8)
    SetTextColor(255, 255, 255, 255)
    SetTextAlign("left", "top")
    textStyles.body = PopTextFormatting()
    
    -- Caption style
    SetTextScale(0.7)
    SetTextColor(200, 200, 200, 255)
    SetTextItalic()
    SetTextAlign("center", "bottom")
    textStyles.caption = PopTextFormatting()
end

local function applyTextStyle(styleName)
    if textStyles[styleName] then
        -- highlight-next-line
        SetTextFormatting(textStyles[styleName])
        return true
    end
    return false
end

-- Initialize styles
initializeTextStyles()

-- Use the styles
applyTextStyle("header")
SetTextPosition(0.5, 0.1)
DrawText("Chapter 1: Introduction")

applyTextStyle("body")
SetTextPosition(0.1, 0.2)
SetTextWrapping(0.8)
DrawText("Lorem ipsum dolor sit amet, consectetur adipiscing elit.")

applyTextStyle("caption")
SetTextPosition(0.5, 0.9)
DrawText("Figure 1.1: Sample diagram")
```

## See Also

- DSL
  - [`GetTextFormatting`](./GetTextFormatting)
  - [`PopTextFormatting`](./PopTextFormatting)