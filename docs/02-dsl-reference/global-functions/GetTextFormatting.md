---
description: Get current text formatting table.
sidebar_class_name: hidden
---

# GetTextFormatting

> **_This function was added in DSL 1_**

## Description

Get a _text formatting table_ representing the current [text formatting](/docs/dsl-reference/basic-concepts/render-functions) options for later re-application with [`SetTextFormatting`](./SetTextFormatting).

This function is usually the less preferable option compared to [`PopTextFormatting`](./PopTextFormatting).

```lua
function GetTextFormatting() --[[ ... ]] end
```

## Parameters

None.

## Return Values

- `formatTable`: _`table`_ - A table containing the current text formatting options.

## Example

```lua
local formatTable = GetTextFormatting()
-- Use the formatTable for later re-application
SetTextFormatting(formatTable)
```

## See Also

- DSL
  - [`PopTextFormatting`](./PopTextFormatting)
  - [`SetTextFormatting`](./SetTextFormatting)
