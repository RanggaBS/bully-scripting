---
description: Starts a new thread using the specified function name.
sidebar_class_name: hidden
---

# CreateThread

## Description

Creates a new thread using the specified function name as the entry point. The original [**CreateThread**](https://bully-scripting.vercel.app/docs/game-reference/global-functions/CreateThread) can only take a string, while DSL's version supports both a string and a function directly. The original can't be passed an arbitrary number of arguments, but DSL's can. 
The normal one is limited to the game's maximum thread count, DSL's has no arbitrary limitation. There's also the fact that a DSL thread it different internally, and that it's stored in the DSL script object rather than the game script object of course.
If a DSL script is not running however, the original version is used.

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
    -- DSL CreateThread arguments
    MyThread = CreateThread("ThreadWithArgs", "Hello", 42, true)
    
end

function ThreadWithArgs(message, number, flag)
    while true do
        print("Args: " .. message .. ", " .. number .. ", " .. tostring(flag))
        Wait(1000)
    end
end
```

## See Also

- Game's Native
  - [`CreateThread`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/CreateThread)