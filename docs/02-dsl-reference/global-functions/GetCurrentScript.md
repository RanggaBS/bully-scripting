---
description: Returns the current `script`.
sidebar_class_name: hidden
---

# GetCurrentScript

> **_This function was added in DSL 8_**

## Description

Returns the current `script`.

```lua
function GetCurrentScript() --[[ ... ]] end
```

## Parameters

None.

## Return Values

- `script`: _`userdata|script`_ - The script object. `userdata` if checked with `type(script)`, `script` if checked with `type2(script)`.

## Example

```lua
local script = GetCurrentScript()
print(script, GetScriptCollection(script))
```

## See Also

- DSL
  - [GetScriptCollection](GetScriptCollection)
