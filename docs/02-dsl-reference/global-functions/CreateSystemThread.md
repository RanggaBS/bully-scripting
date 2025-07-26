---
description: Create a system thread using the specified function or an anonymous function.
sidebar_class_name: hidden
---

# CreateSystemThread

> **_This function was added in DSL 1_**

## Description

Create a [**`SYSTEM`**](/docs/dsl-reference/basic-concepts/scripts#thread-types) thread, using the same general rules as [CreateThread](CreateThread).

These threads run while the game is paused or out of focus, before most parts of the game are updated each frame.

Any extra arguments (`...`) are passed to the thread function when the thread starts.

```lua
function CreateSystemThread(func, ...) --[[ ... ]] end
```

## Parameters

- `func`: _`function|string`_ - The function to run in the thread. If a string is provided, it refers to a function in the current script's environment.
- `...`: _`any`_ - (Optional) Additional arguments that will be passed to the thread function when it starts.

## Return Values

- `thread`: _`thread`_ - The thread object representing the newly created system thread.

## Example

```lua
local thread = CreateSystemThread(function(arg1, arg2)
  print('Thread started with arguments:', arg1, arg2)
  -- Perform background tasks here
end, 'Hello', 'World')
```

## See Also

- DSL
  - [`CreateThread`](./CreateThread)
