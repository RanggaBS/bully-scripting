---
description: Returns a table that is available to all scripts in the current collection.
sidebar_class_name: hidden
---

# GetScriptSharedTable

> **_This function was added in DSL 1_**

## Description

Returns a table that is available to all scripts in the current collection.

The table is only actually created the first time this function is called.

By default, the table will be accessible from anywhere using [`dsl`](/docs/dsl-reference/basic-concepts/global-variables#dsl).

If `shareMode` is `true`, the shared table cannot be accessed through _dsl_. If no value is given, the share mode will not be changed.

:::danger
Attempting to change the share mode after the table is created will result in an error.
:::

```lua
function GetScriptSharedTable(shareMode) --[[ ... ]] end
```

## Parameters

- `shareMode?`: _`boolean|nil`_ - (Optional) If `true`, the shared table cannot be accessed through dsl. If no value is given, the share mode will not be changed.

## Return Values

- `tbl`: _`table`_ - The shared table.

## Versions

- **DSL7** - A mostly useless argument was removed, and the optional `shareMode` argument was added.

## Example

Communicate with a second script using a shared table.

### `main.lua`

```lua
gShared = GetScriptSharedTable()
StartScript('secondary.lua')

function main()
  while not SystemIsReady() do
    Wait(0)
  end
  while gShared.some_text do
    TextPrintString(gShared.some_text, 0, 1)
    Wait(0)
  end
end
```

### `secondary.lua`

```lua
gShared = GetScriptSharedTable()
gShared.some_text = 'hello world'

function main()
  Wait(9000)
  gShared.some_text = 'good bye'
  Wait(1000)
  gShared.some_text = nil
end
```
