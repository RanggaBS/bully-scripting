---
description: Check if a DSL script is currently running.
sidebar_class_name: hidden
---

# IsDslScriptRunning

> **_This function was added in DSL 4_**

## Description

Check if a DSL script is currently running so that you can conditionally make use of features that cannot be used by scripts in `Scripts.img`.

```lua
function IsDslScriptRunning() --[[ ... ]] end
```

## Parameters

None.

## Return Values

- `isRunning`: _`boolean`_ - Returns `true` if a DSL script is currently running, otherwise `false`.

## Example

```lua
function main()
  if IsDslScriptRunning() then
    print('A DSL script is currently running.')
  else
    print('No DSL script is running.')
  end
end
```
