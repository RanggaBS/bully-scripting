---
description: Get the script's environment.
sidebar_class_name: hidden
---

# GetScriptEnvironment

> **_This function was added in DSL 1_**

## Description

Returns the environment assigned to `script` or the current script.

```lua
function GetScriptEnvironment(script) --[[ ... ]] end
```

## Parameters

- `script?`: _`userdata|script|nil`_ - (Optional) The script object. `userdata` if checked with `type(script)`, `script` if checked with `type2(script)`.

## Return Values

- `environment`: _`table`_ - The environment assigned to the script.

## Example

```lua
local someLocal = 7
someGlobal = 7

for key, value in pairs(GetScriptEnvironment()) do
  print(key, value)
end

--[[ Output:
exports        table: XXXXXXXX
ImportScript:  function: XXXXXXXX
someGlobal     7
]]
```
