---
description: Sets the font to use for subsequent text drawing operations.
sidebar_class_name: hidden
---

# SetTextFont

## Description

Sets the font to be used for text drawing. Can accept either a font object created with `CreateFont` or a string representing a system font name. When using a string, the font is automatically created and cached internally on a per-script basis.

```lua
function SetTextFont(font) --[[ ... ]] end
```

## Parameters

- `font`: _`string`_ - A font object returned by `CreateFont` or a string with the system font name

## Return Values

- `font`: - Returns the font object that will be used for text drawing.

## Example

```lua
-- Using a font object
local customFont = CreateFont('path/to/font.ttf')
-- highlight-next-line
SetTextFont(customFont)

-- Draw text with the selected font
SetTextPosition(0.5, 0.5)
SetTextScale(1.0)
DrawText("This text uses the selected font")
```

```lua
-- Using a string (automatically creates and caches the font)
-- highlight-next-line
SetTextFont("Arial")

-- Draw text with the selected font
SetTextPosition(0.5, 0.5)
SetTextScale(1.0)
DrawText("This text uses the selected font")
```

## See Also

- DSL
  - [`CreateFont`](./CreateFont)
  - [`SetTextPosition`](./SetTextPosition)
  - [`SetTextScale`](./SetTextScale)