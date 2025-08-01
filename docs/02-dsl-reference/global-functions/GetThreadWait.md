---
description: Returns the time until a thread will be allowed to update again.
sidebar_class_name: hidden
---

# GetThreadWait

> **_This function was added in DSL 1_**

## Description

Returns the time until `thread` or the current thread will be allowed to update again. If a coroutine you created calls [`Wait`](Wait), this function can be used with the current thread to get what time was passed.

```lua
function GetThreadWait(thread) --[[ ... ]] end
```

## Parameters

- `thread?`: _`thread|nil`_ - (Optional) The thread to check the wait time for.

## Return Values

- `milliseconds`: _`number`_ - The time in milliseconds until the thread will be allowed to update again.

## Example

```lua
local thread = CreateThread(function()
  Wait(1000)
  print('This thread will not update for another', GetThreadWait(thread), 'milliseconds')
end)
print(GetThreadWait(thread))

-- Output:
--> 0
--> This thread will not update for another 1000 milliseconds
```

## See Also

- DSL
  - [`CreateThread`](./CreateThread)
  - [`Wait`](./Wait)
