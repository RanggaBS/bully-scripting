---
description: Discards the current text formatting, resetting all text formatting settings to their default values.
sidebar_class_name: hidden
---

# DiscardText

## Description

Discards the current text formatting, resetting all text formatting settings to their default values. This function should be called when you have configured text formatting but decide not to call `DrawText`, ensuring that subsequent text drawing operations are not affected by the previous formatting settings.

```lua
function DiscardText() --[[ ... ]] end
```

## Parameters

None.

## Return Values

None.

## Example

```lua
-- Set up some text formatting
SetTextPosition(0.5, 0.5)
SetTextScale(5.0)
SetTextColor(0, 255, 0, 255)
SetTextBold()

-- Discard the formatting
DiscardText()

-- The next DrawText will be using default formatting
SetTextPosition(0.5, 0.25)
DrawText("This text uses default formatting")
```

## See Also

- DSL
  - [`DrawText`](./DrawText)
  - [`SetTextPosition`](./SetTextPosition)