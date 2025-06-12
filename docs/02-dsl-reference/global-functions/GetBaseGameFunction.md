---
description: Get the original version of a C function registered by Rockstar.
sidebar_class_name: hidden
---

# GetBaseGameFunction

> **_This function was added in DSL 5_**

## Description

Get the original version of a C function registered by Rockstar.

```lua
function GetBaseGameFunction(name) --[[ ... ]] end
```

## Parameters

- `name`: _`string`_ -- The name of the function to retrieve. This should be the name as it appears in the C code, not the Lua wrapper.

## Return Values

- `func`: _`function?`_ -- The original C function if it exists, or `nil` if the function is not found.

## Example

```lua
local originalFunction = GetBaseGameFunction('SomeCFunction')
if originalFunction then
  print('Original C function found:', originalFunction)
else
  print('Original C function not found.')
end
```
