---
description: Get the script's name.
sidebar_class_name: hidden
---

# GetScriptName

> **_This function was added in DSL 4_**

## Description

Returns the name of `script` or the current script.

```lua
function GetScriptName(script) --[[ ... ]] end
```

## Parameters

- `script?`: _`userdata|script|nil`_ - (Optional) The script object. `userdata` if checked with `type(script)`, `script` if checked with `type2(script)`.

## Return Values

- `collection`: _`string`_ - The name of the script's collection.

## Example

```lua
print(GetScriptName())
```
