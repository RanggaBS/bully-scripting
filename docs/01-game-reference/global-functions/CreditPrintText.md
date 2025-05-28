---
description: Prints credit text on the screen until [**CreditReset**](https://bully-scripting.vercel.app/docs/game-reference/global-functions/CreditReset) is called.
sidebar_class_name: hidden
---

# CreditPrintText

## Description

Displays credit text at specified screen coordinates.
Before using this function, call [**CreditLoadDB**](https://bully-scripting.vercel.app/docs/game-reference/global-functions/CreditLoadDB) once and [**CreditSetup**](https://bully-scripting.vercel.app/docs/game-reference/global-functions/CreditSetup) as needed.

```lua
function CreditPrintText(x, y, unk, text) --[[ ... ]] end
```

## Parameters

- `x`: _`integer`_ - X screen coordinate (0 to 640, regardless of resolution).
- `y`: _`integer`_ - Y screen coordinate (0 to 480).
- `unk`: _`boolean`_ - Unknown, use false.
- `text`: _`string`_ - The text entry to be printed.

## Return Values

None.

## Example

None.

