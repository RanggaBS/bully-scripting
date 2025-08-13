---
description: Get the raw save data table.
sidebar_class_name: hidden
---

# GetRawSaveDataTable

> **_This function was added in DSL 1_**

## Description

Return the raw save data table.

You should usually be using [`GetSaveDataTable`](./GetSaveDataTable) instead.

```lua
function GetRawSaveDataTable() --[[ ... ]] end
```

## Parameters

None.

## Return Values

- `rawSaveData`: _`table`_ - The raw save data table.

## Versions

- **DSL 4** - Save data is now more reliable, and accurately reports when it is not ready.

## Example

```lua
local rawSaveData = GetRawSaveDataTable()
print('Raw Save Data: ', rawSaveData)
```
