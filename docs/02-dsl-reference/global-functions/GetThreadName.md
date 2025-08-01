---
description: Get the name of a thread.
sidebar_class_name: hidden
---

# GetThreadName

> **_This function was added in DSL 4_**

## Description

Return the name of `thread` or of the current thread. It is possible this function will not return anything if the thread was not created with a name.

```lua
function GetThreadName(thread) --[[ ... ]] end
```

## Parameters

- `thread?`: _`thread|nil`_ - (Optional) The thread to get the name of. If not provided, the current thread is used.

## Return Values

- `name`: _`string|nil`_ - The name of the thread, or `nil` if the thread was not created with a name.

## Example

```lua
function MyThreadFunction()
  print('This is my thread function')
  print('Thread name:', GetThreadName(thread))
end

thread = CreateThread('MyThreadFunction')
```

## See Also

- DSL
  - [`CreateThread`](./CreateThread)
