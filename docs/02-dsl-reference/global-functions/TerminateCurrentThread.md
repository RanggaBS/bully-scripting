---
description: Terminate the current thread.
sidebar_class_name: hidden
---

# TerminateCurrentThread

> **_This function was added in DSL 1_**

## Description

Shutdown the current thread. Similar to [`TerminateCurrentScript`](TerminateCurrentScript), control is not instantly taken away. You will have to yield if you want to instantly jump out of thread execution.

```lua
function TerminateCurrentThread() --[[ ... ]] end
```

## Parameters

None.

## Return Values

None.

## Example

```lua
-- Create the thread
local thread = CreateThread(function()
  -- Do some work
  Wait(1000)
  -- Terminate the thread
  TerminateCurrentThread()
end)
```

## See Also

- DSL
  - [`CreateThread`](CreateThread)
  - [`TerminateCurrentScript`](TerminateCurrentScript)
