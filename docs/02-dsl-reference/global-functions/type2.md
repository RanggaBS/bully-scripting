---
description: This function was added in DSL 10.
sidebar_class_name: hidden
---

# type2

## Description

Similar to the built-in `type` function, but `type2` is designed to identify DSL-specific userdata types. Userdata returned from C can represent a wide range of values such as pointers, C data types, textures, scripts, time cycles, and many more type of values. This function can recognize those DSL specific userdata. If the value is not a DSL userdata, the default type function is used.

```lua
function type2(value) --[[ ... ]] end
```

## Parameters

`value`: _`nil, number, string, function, CFunction, userdata, or table`_

## Return Values

`valueType`: _`string`_

## Example

```lua
local Userdata = CreateTexture('box.png')
local Type = type2(Userdata) --> texture
```

