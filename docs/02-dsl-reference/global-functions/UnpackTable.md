---
description: Unpacks a table previously packed using `PackTable`.
sidebar_class_name: hidden
---

# UnpackTable

> **_This function was added in DSL 4_**

## Description

Unpacks a table previously packed using [`PackTable`](./PackTable).

```lua
function UnpackTable(serializedTable) --[[ ... ]] end
```

## Parameters

- `serializedTable`: _`string`_ - The serialized string containing the packed table.

## Return Values

- _`table`_ - The unpacked table.

## Versions

- **DSL 7** - _`light userdata`_ is supported, which lets you serialize hashes returned by [`ObjectNameToHashID`](./ObjectNameToHashID).

## Example

```lua
local serialized = PackTable({
  name = 'Example',
  value = 42,
  nested = { key = 'value' },
  flag = true,
})
local unpacked = UnpackTable(serialized)
print('Unpacked Table Name: ' .. unpacked.name)
print('Unpacked Table Value: ' .. unpacked.value)
```
