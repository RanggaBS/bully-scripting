---
description: Save a table to a file.
sidebar_class_name: hidden
---

# SaveTable

> **_This function was added in DSL 4_**

## Description

Save a table to a file given a [relative path](/docs/dsl-reference/basic-concepts/relative-paths).

The same restrictions apply here as with [`PackTable`](PackTable).

```lua
function SaveTable(name, table) --[[ ... ]] end
```

## Parameters

- `name`: _`string`_ - The name of the file to save the table to. This should be a relative path, such as `data/my_table.lua`. The file will be created if it does not exist, or overwritten if it does.
- `table`: _`table`_ - The table to save. This can be any Lua table, including nested tables. The table will be serialized to a Lua script that can be loaded later using [`LoadTable`](LoadTable).

## Return Values

None.

## Example

```lua
local myTable = {
  name = 'Example',
  values = {1, 2, 3},
  nested = {key = 'value'}
}

SaveTable('data/my_table.lua', myTable)
```

## See Also

- DSL
  - [`LoadTable`](LoadTable)
  - [`PackTable`](PackTable)
  - [`UnpackTable`](UnpackTable)
