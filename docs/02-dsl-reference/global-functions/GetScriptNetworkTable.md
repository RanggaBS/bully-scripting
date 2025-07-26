---
description: Returns a table that is available to all scripts in the current collection.
sidebar_class_name: hidden
---

# GetScriptNetworkTable

> **_This function was added in DSL 8_**

## Description

Returns a table that is available to all scripts in the current collection.

The table is only actually created the first time this function is called.

The table will be accessible from anywhere using [`net`](/docs/dsl-reference/basic-concepts/global-variables#net).

This function will fail if it is not called by a network script (client scripts from a server or main scripts on a server).

```lua
function GetScriptNetworkTable(shareMode) --[[ ... ]] end
```

## Parameters

- `shareMode?`: _`boolean|nil`_ - (Optional) If `true`, the shared table cannot be accessed through dsl. If no value is given, the share mode will not be changed.

## Return Values

- `tbl`: _`table`_ - The shared table.

## Versions

- **DSL7** - A mostly useless argument was removed, and the optional `shareMode` argument was added.

## Example

```lua
print(GetScriptNetworkTable())
```
