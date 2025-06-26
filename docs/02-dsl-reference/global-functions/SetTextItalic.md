---
description: Enables italic formatting for subsequent text drawing operations.
sidebar_class_name: hidden
---

# SetTextItalic

## Description

Enables italic text formatting for subsequent text drawing operations.

*Introduced in DSL 2.*

```lua
function SetTextItalic() --[[ ... ]] end
```

## Parameters

None.

## Return Values

None.

## Example

```lua
-- Draw normal text
SetTextPosition(0.5, 0.3)
SetTextScale(1.0)
DrawText("This is normal text")

-- Enable italic formatting
-- highlight-next-line
SetTextItalic()
SetTextPosition(0.5, 0.4)
DrawText("This is italic text")

-- Combine italic with other formatting
-- highlight-next-line
SetTextItalic()
SetTextScale(1.2)
SetTextColor(0, 0, 255, 255)
SetTextPosition(0.5, 0.7)
DrawText("Large blue italic text")
```

## See Also

- DSL
  - [`SetTextPosition`](./SetTextPosition)
  - [`SetTextBold`](./SetTextBold)
  - [`SetTextShadow`](./SetTextShadow)
  - [`SetTextColor`](./SetTextColor)
