---
description: Returns the normalized width and height of what a text draw would be without actually drawing it.
sidebar_class_name: hidden
---

# MeasureText

## Description

Returns the normalized width and height of what the text draw would be. The returned value is the same as what `DrawText` returns, so this is a good way to measure text draws before drawing. This function uses the current text formatting settings.

```lua
function MeasureText(text) --[[ ... ]] end
```

## Parameters

- `text`: _`string`_ - The text to measure

## Return Values

- `width`: _`number`_ - The normalized width the text would occupy
- `height`: _`number`_ - The normalized height the text would occupy

## Example

```lua
-- Create a text box with background
local message = "This is an important message!"
SetTextHeight(0.03)
-- highlight-next-line
local textWidth, textHeight = MeasureText(message)

-- Add padding
local padding = 0.02
local boxX = 0.5 - (textWidth + padding)/2
local boxY = 0.3 - (textHeight + padding)/2

-- Draw background rectangle
DrawRectangle(boxX, boxY, textWidth + padding, textHeight + padding, 0, 0, 0, 128)

-- Draw text centered in box
SetTextPosition(0.5, 0.3)
SetTextAlign("center", "center")
SetTextColor(255, 255, 255, 255)
DrawText(message)
```

## See Also

- DSL
  - [`MeasureTextInline`](./MeasureTextInline)
