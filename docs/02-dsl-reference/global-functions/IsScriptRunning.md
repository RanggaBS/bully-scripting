---
description: Check if `script` is running.
sidebar_class_name: hidden
---

# IsScriptRunning

> **_This function was added in DSL 1_**

## Description

Returns if `script` is running, as in not shutdown or shutting down.

```lua
function IsScriptRunning(script) --[[ ... ]] end
```

## Parameters

- `script`: _`userdata|script`_ - The script object. `userdata` if checked with `type(script)`, `script` if checked with `type2(script)`.

## Return Values

- `running`: _`boolean`_ - If `script` is running.

## Example

```lua
print(IsScriptRunning(GetCurrentScript()))
```

## See Also

- DSL
  - [GetCurrentScript](GetCurrentScript)
