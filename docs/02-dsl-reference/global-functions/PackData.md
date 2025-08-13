---
description: Serialize values into a single string.
sidebar_class_name: hidden
---

# PackData

> **_This function was added in DSL 1_**

## Description

Serialize all of the values given into a single string that can be unpacked using [`UnpackData`](./UnpackData).

If you only want to pack a single table, consider using [`PackTable`](./PackTable).

Only the following values are allowed to be serialized: _`boolean`_, _`number`_, _`string`_, _`table`_, and _`light userdata`_. Do not use any tables that refer back to themselves.

```lua
function PackData(...) --[[ ... ]] end
```

## Parameters

- `...`: _`boolean|number|string|table|light userdata`_ - The values to serialize. You can pass any number of values, and they can be of any of the allowed types.

## Return Values

- `serializedData`: _`string`_ - The serialized string containing all the packed values.

## Versions

- **DSL 7** - _`light userdata`_ is supported, which lets you serialize hashes returned by [`ObjectNameToHashID`](./ObjectNameToHashID).

## Example

```lua
local packedData = PackData(true, 123, 'Hello', { key = 'value' }, lightUserData)
print('Packed Data: ' .. packedData)
```
