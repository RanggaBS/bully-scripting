---
description: Configures the text appearance for credit printing.
sidebar_class_name: hidden
---

# CreditSetup

## Description

Sets the color, transparency, scale, and justification of text printed by [**CreditPrintText**](https://bully-scripting.vercel.app/docs/game-reference/global-functions/CreditPrintText).
This function should be called before printing credit text.

```lua
function CreditSetup(red, green, blue, alpha, scale, justify) --[[ ... ]] end
```

## Parameters

- `red`: _`integer`_ - Red color value [0–255].
- `green`: _`integer`_ - Green color value [0–255].
- `blue`: _`integer`_ - Blue color value [0–255].
- `alpha`: _`integer`_ - Transparency (opacity) [0–255], where 255 is fully visible.
- `scale`: _`number`_ - Text scale, with 1.0 as a standard size.
- `justify`: _`integer`_ - Text justification: 0 = left, 1 = right, 2 = centered.

## Return Values

None.

## Example

None.

