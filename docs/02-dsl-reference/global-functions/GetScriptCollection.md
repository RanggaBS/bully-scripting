---
description: Get script collection's name.
sidebar_class_name: hidden
---

# GetScriptCollection

> **_This function was added in DSL 4_**

## Description

Returns the name of `script`'s collection, or of the current collection.

```lua
function GetScriptCollection(script) --[[ ... ]] end
```

## Parameters

- `script?`: _`userdata|script|nil`_ - (Optional) The script object. `userdata` if checked with `type(script)`, `script` if checked with `type2(script)`.

## Return Values

- `collection`: _`string`_ - The name of the script's collection.

## Example

```lua
print(GetScriptCollection())
```

## See Also

- DSL
  - [GetCurrentScript](GetCurrentScript)
