---
description: Adds an outline effect around text.
sidebar_class_name: hidden
---

# SetTextOutline

## Description

Adds an outline effect around text. The outline appears as a border around the text characters, which can significantly improve text readability over busy or similar-colored backgrounds.

```lua
function SetTextOutline(red, green, blue) --[[ ... ]] end
```

## Parameters

- `red`: _`number`_ - (Optional) The red color component for the outline (0-255). Defaults to black if not specified
- `green`: _`number`_ - (Optional) The green color component for the outline (0-255). Defaults to black if not specified
- `blue`: _`number`_ - (Optional) The blue color component for the outline (0-255). Defaults to black if not specified

## Return Values

None.

## Example

```lua
-- Add a black outline (default)
-- highlight-next-line
SetTextOutline()
SetTextPosition(0.5, 0.3)
SetTextScale(1.5)
SetTextColor(255, 255, 255, 255)
DrawText("White text with black outline")

-- Add a white outline for dark text
-- highlight-next-line
SetTextOutline(255, 255, 255) -- White outline
SetTextPosition(0.5, 0.5)
SetTextColor(0, 0, 0, 255) -- Black text
DrawText("Black text with white outline")

-- Colored outline
-- highlight-next-line
SetTextOutline(255, 0, 255) -- Magenta outline
SetTextPosition(0.5, 0.7)
SetTextColor(0, 255, 0, 255) -- Green text
DrawText("Green text with magenta outline")
```

## See Also

- DSL
  - [`SetTextPosition`](./SetTextPosition)
  - [`SetTextColor`](./SetTextColor)
  - [`SetTextScale`](./SetTextScale)
