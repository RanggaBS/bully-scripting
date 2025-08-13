---
description: Serialize a table into a string.
sidebar_class_name: hidden
---

# PackTable

> **_This function was added in DSL 4_**

## Description

Serialize the table into a single string that can be unpacked using [`UnpackTable`](./UnpackTable). This is a lower level version of the [`PackData`](./PackData) function.

Only the following values are allowed to be serialized: _`boolean`_, _`number`_, _`string`_, _`table`_, and _`light userdata`_. Do not use any tables that refer back to themselves.

```lua
function PackTable(tbl) --[[ ... ]] end
```

## Parameters

- `tbl`: _`table`_ - The table to serialize. It can contain nested tables, but circular references are not allowed.

## Return Values

- `serializedTable`: _`string`_ - The serialized string representation of the table.

## Versions

- **DSL 7** - _`light userdata`_ is supported, which lets you serialize hashes returned by [`ObjectNameToHashID`](./ObjectNameToHashID).

## Example

```lua
local myTable = {
  name = 'Example',
  value = 42,
  nested = { key = 'value' },
  flag = true,
}
local serialized = PackTable(myTable)
print('Serialized Table: ' .. serialized)
```
