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

```lua
function main()
    -- all your code goes here
    MyThread = CreateThread("ActionThread")
    -- any leftover code goes here
end

function ActionThread()
    -- this is the thread that will run in the background
    while true do
        -- do something here, like checking a condition or performing an action
        print("ActionThread is running...")
        Wait(0)  -- waiting 0 seconds so that your game won't run out of memory
    end
end
```

## See Also

- DSL
  - [`CreateThread`](https://bully-scripting.vercel.app/docs/dsl-reference/global-functions/CreateThread)

