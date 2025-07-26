---
description: Shutdown `script`, or the current script if not given.
sidebar_class_name: hidden
---

# TerminateScript

> **_This function was added in DSL 1_**

## Description

Shutdown `script`, or the current script if not given.

```lua
function TerminateScript(script) --[[ ... ]] end
```

## Parameters

- `script?`: _`userdata|script|nil`_ - (Optional) The script object.

## Return Values

None.

## Example

```lua
TerminateScript()

-- Same as above
TerminateScript(GetCurrentScript())
```

## See Also

- DSL
  - [GetCurrentScript](GetCurrentScript)
  - [TerminateCurrentScript](TerminateCurrentScript)
