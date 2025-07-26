---
description: Create an advanced thread using the specified type and function.
sidebar_class_name: hidden
---

# CreateAdvancedThread

> **_This function was added in DSL 4_**

## Description

Create [any type](/docs/dsl-reference/basic-concepts/scripts#thread-types) of thread, using the same general rules as [`CreateThread`](CreateThread).

Some threads can only be created using this function.

These threads run at different points in the game's execution, depending on the type specified. This allows for more control over when and how the thread operates within the game's lifecycle.

Any extra arguments (`...`) are passed to the thread function when the thread starts.

```lua
function CreateAdvancedThread(type, func, ...) --[[ ... ]] end
```

## Parameters

- `type`: _`string`_ - The type of thread to create. This determines the thread's behavior and capabilities.
- `func`: _`function|string`_ - The function to run in the thread. If a string is provided, it refers to a function in the current script's environment.
- `...`: _`any`_ - (Optional) Additional arguments that will be passed to the thread function when it starts.

## Return Values

- `thread`: _`thread`_ - The thread object representing the newly created advanced thread. This can be used to control the thread, such as pausing or stopping it.

## Example

```lua
local thread = CreateAdvancedThread('POST_WORLD', function()
  while true do
    -- Perform operations that need to run after the world is updated
    Wait(0) -- Yield to prevent blocking the main thread
  end
end)
```

## See Also

- DSL
  - [`CreateThread`](./CreateThread)
