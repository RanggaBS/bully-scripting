---
description: Terminate a thread or the current thread.
sidebar_class_name: hidden
---

# TerminateThread

> **_This function was added in DSL 1_**

## Description

Terminate a thread or the current thread.

This function replaces the existing [`TerminateThread`](/docs/game-reference/global-functions/TerminateThread). If DSL is not running _or_ [`UseBaseGameScriptFunctions`](UseBaseGameScriptFunctions) was called with `true`, the original function is used. Otherwise it will shutdown `thread` or the current thread.

```lua
function TerminateThread(thread) --[[ ... ]] end
```

## Parameters

- `thread?`: _`thread|nil`_ - (Optional) The thread to terminate. If not provided, the current thread is terminated.

## Return Values

None.

## Example

Create a thread that will terminate itself after 1 second

```lua
local thread = CreateThread(function()
  Wait(1000)
  TerminateThread() -- Terminate the current thread
end)
```

## See Also

- DSL
  - [`CreateThread`](./CreateThread)
  - [`TerminateCurrentThread`](./TerminateCurrentThread)
