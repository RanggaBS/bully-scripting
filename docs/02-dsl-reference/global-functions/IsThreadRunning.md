---
description: Check if a thread is running.
sidebar_class_name: hidden
---

# IsThreadRunning

> **_This function was added in DSL 1_**

## Description

Check if a thread is running.

Returns if `thread` is running, as in not shutdown or shutting down.

```lua
function IsThreadRunning(thread) --[[ ... ]] end
```

## Parameters

- `thread`: _`thread`_ - The thread to check if it is running.

## Return Values

- `running`: _`boolean`_ - `true` if the thread is running, `false` otherwise.

## Example

```lua
local thread = CreateThread(function()end)
print(IsThreadRunning(thread)) --> true
Wait(0)
print(IsThreadRunning(thread)) --> false
```

## See Also

- DSL
  - [`CreateThread`](./CreateThread)
