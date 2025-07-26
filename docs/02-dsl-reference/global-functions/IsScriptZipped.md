---
description: Check if a script is zipped.
sidebar_class_name: hidden
---

# IsScriptZipped

> **_This function was added in DSL 4_**

## Description

Returns if Script's collection or the running collection is a zipped collection.

```lua
function IsScriptZipped(script) --[[ ... ]] end
```

## Parameters

- `script`: _`userdata|script`_ - The script object. `userdata` if checked with `type(script)`, `script` if checked with `type2(script)`.

## Return Values

- `zipped`: _`boolean`_ - If the script's collection or the running collection is a zipped collection.

## Example

```lua
print(IsScriptZipped(GetCurrentScript()))
```

## See Also

- DSL
  - [GetCurrentScript](GetCurrentScript)
