---
description: Unpack values previously packed with `PackData`.
sidebar_class_name: hidden
---

# UnpackData

> **_This function was added in DSL 1_**

## Description

Unpacks values previously packed using [`PackData`](./PackData).

```lua
function UnpackData(serializedData) --[[ ... ]] end
```

## Parameters

- `serializedData`: _`string`_ - The serialized string containing the packed values.

## Return Values

- `...`: _`boolean|number|string|table|light userdata`_ - The unpacked values. The number and types of returned values will match those passed to [`PackData`](./PackData).

## Versions

- **DSL 7** - _`light userdata`_ is supported, which lets you serialize hashes returned by [`ObjectNameToHashID`](./ObjectNameToHashID).

## Example

```lua
local packedData = PackData(true, 123, 'Hello', { key = 'value' }, lightUserData)
local unpackedData = UnpackData(packedData)
print('Unpacked Data: ', unpackedData)
```
