---
description: Print output to the console as special text.
sidebar_class_name: hidden
---

# PrintSpecial

> **_This function was added in DSL 5_**

## Description

Convert all arguments to strings using `tostring` and print them in the console as special text.

```lua
function PrintSpecial(...) --[[ ... ]] end
```

## Parameters

- `...`: _`any`_ - The values to be printed. Each value will be converted to a string using `tostring`.

## Return Values

None.

## Example

```lua
PrintSpecial('This is a special message!', 42, true, function() end, {})
```
