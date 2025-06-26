---
description: Adds a drop shadow effect to text.
sidebar_class_name: hidden
---

# SetTextShadow

## Description

Adds a drop shadow effect to text. The shadow appears as a slightly offset duplicate of the text, creating a depth effect that can improve text readability over complex backgrounds.

```lua
function SetTextShadow(red, green, blue) --[[ ... ]] end
```

## Parameters

- `red`: _`number`_ - (Optional) The red color component for the shadow (0-255). Defaults to black if not specified.
- `green`: _`number`_ - (Optional) The green color component for the shadow (0-255). Defaults to black if not specified.
- `blue`: _`number`_ - (Optional) The blue color component for the shadow (0-255). Defaults to black if not specified.

## Return Values

None.

## Example

```lua
-- Add a black drop shadow (default)
-- highlight-next-line
SetTextShadow()
SetTextPosition(0.5, 0.3)
SetTextScale(1.5)
SetTextColor(255, 255, 255, 255)
DrawText("White text with black shadow")

-- Add a colored shadow
-- highlight-next-line
SetTextShadow(255, 0, 0) -- Red shadow
SetTextPosition(0.5, 0.5)
SetTextColor(255, 255, 255, 255)
DrawText("White text with red shadow")
```

## See Also

- DSL
  - [`SetTextPosition`](./SetTextPosition)
  - [`SetTextItalic`](./SetTextItalic)
  - [`SetTextColor`](./SetTextColor)