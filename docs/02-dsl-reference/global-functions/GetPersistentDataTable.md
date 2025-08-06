---
description: Returns a persistent data table for the current collection.
sidebar_class_name: hidden
---

# GetPersistentDataTable

> **_This function was added in DSL 4_**

## Description

Returns a _persistent data table_ for the current collection.

This table is preserved after [DSL is reset](/docs/dsl-reference/basic-concepts/collections#startup), and is tied to the name of the current collection.

```lua
function GetPersistentDataTable() --[[ ... ]] end
```

## Parameters

None.

## Return Values

- `persistentDataTable`: _`table`_ - A table that can be used to store persistent data for the current collection. This table is automatically saved and loaded by DSL.

## Example

```lua
function main()
  local persistentData = GetPersistentDataTable()
  persistentData.someValue = 42
end
```
