---
description: Starts a new thread using the specified function name.
sidebar_class_name: hidden
---

# CreateThread

## Description

Creates a new thread using the specified function name as the entry point. The function name must be passed as a string (e.g. "T_Thread", not T_Thread). The named function must exist in the script's environment.

```lua
function CreateThread(funcName) --[[ ... ]] end
```

## Parameters

- `funcName`: _`string`_ - The name of the function to run in the new thread.

## Return Values

None.

## Example

None.

