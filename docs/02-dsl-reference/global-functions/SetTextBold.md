---
description: Enables bold formatting for subsequent text drawing operations.
sidebar_class_name: hidden
---

# SetTextBold

## Description

Enables bold text formatting for subsequent text drawing operations.

*Introduced in DSL 2.*

```lua
function SetTextBold() --[[ ... ]] end
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

-- Enable bold formatting
-- highlight-next-line
SetTextBold()
SetTextPosition(0.5, 0.4)
DrawText("This is bold text")   
```

## See Also

- DSL
  - [`SetTextPosition`](./SetTextPosition)
  - [`SetTextItalic`](./SetTextItalic)
  - [`SetTextShadow`](./SetTextShadow)