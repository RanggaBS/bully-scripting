---
description: Load a table from a file.
sidebar_class_name: hidden
---

# LoadTable

> **_This function was added in DSL 4_**

## Description

Load a table from a file created by [`SaveTable`](SaveTable).

```lua
function LoadTable(name) --[[ ... ]] end
```

## Parameters

- `name`: _`string`_ - The name of the file to load the table from. This should be a relative path, such as `data/my_table.lua`. The file must exist and be readable.

## Return Values

- `table`: _`table`_ - The loaded table. If the file does not exist or cannot be read, it returns `nil`.

## Example

```lua
local myTable = LoadTable('data/my_table.lua')
if myTable then
  print('Table loaded successfully:', myTable.name)
else
  print('Failed to load table')
end
```

## See Also

- DSL
  - [`SaveTable`](SaveTable)
  - [`PackTable`](PackTable)
  - [`UnpackTable`](UnpackTable)
