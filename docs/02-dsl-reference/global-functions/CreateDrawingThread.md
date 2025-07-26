---
description: Create a drawing thread using the specified function or an anonymous function.
sidebar_class_name: hidden
---

# CreateDrawingThread

> **_This function was added in DSL 1_**

## Description

Create a [**`DRAWING`**](/docs/dsl-reference/basic-concepts/scripts#thread-types) thread, using the same general rules as [`CreateThread`](CreateThread).

These threads run directly before the game presents its back buffer, meaning anything you draw will be on top of everything the game drew.

This is useful for drawing custom UI elements, overlays, or any other graphical elements that need to be rendered on top of the game.

Any extra arguments (`...`) are passed to the thread function when the thread starts.

```lua
function CreateDrawingThread(func, ...) --[[ ... ]] end
```

## Parameters

- `func`: _`function|string`_ - The function to run in the drawing thread. If a string is provided, it refers to a function in the current script's environment.
- `...`: _`any`_ - (Optional) Additional arguments that will be passed to the thread function when it starts.

## Return Values

- `thread`: _`thread`_ - The thread object representing the newly created drawing thread. This can be used to control the thread, such as pausing or stopping it.

## Example

```lua
local thread = CreateDrawingThread(function()
  while true do
    -- Drawing operations go here
    Wait(0) -- Yield to prevent blocking the main thread
  end
end)
```

## See Also

- DSL
  - [`CreateThread`](./CreateThread)
