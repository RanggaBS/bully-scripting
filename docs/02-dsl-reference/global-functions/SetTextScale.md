---
description: Sets the text size using a scale multiplier based on a predefined normal size.
sidebar_class_name: hidden
---

# SetTextScale

## Description

Sets the size of text using a scale multiplier applied to a predefined "normal" text size. This function provides an alternative to `SetTextHeight` by using a scale factor rather than absolute normalized height.

```lua
function SetTextScale(scale) --[[ ... ]] end
```

## Parameters

- `scale`: _`number`_ - The scale multiplier for text size (1.0 = normal size, 0.5 = half size, 2.0 = double size)

## Return Values

None.

## Example

```lua
-- Set text to normal size
-- highlight-next-line
SetTextScale(1.0)
SetTextPosition(0.5, 0.3)
DrawText("Normal sized text")

-- Set text to half size
-- highlight-next-line
SetTextScale(0.5)
SetTextPosition(0.5, 0.4)
DrawText("Half sized text")

-- Set text to double size
-- highlight-next-line
SetTextScale(2.0)
SetTextPosition(0.5, 0.5)
DrawText("Double sized text")
```

## See Also

- DSL
  - [`SetTextPosition`](./SetTextPosition)
  - [`SetTextItalic`](./SetTextItalic)
  - [`SetTextShadow`](./SetTextShadow)