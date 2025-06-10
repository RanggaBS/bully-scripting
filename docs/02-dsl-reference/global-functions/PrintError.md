---
description: Print output to the console as error text.
sidebar_class_name: hidden
---

# PrintError

> **_This function was added in DSL 1_**

## Description

Convert all arguments to strings using `tostring` and print them in the console as error text.

```lua
function PrintError(...) --[[ ... ]] end
```

## Parameters

- `...`: _`any`_ - The values to be printed. Each value will be converted to a string using `tostring`.

## Return Values

None.

## Example

```lua
PrintError('This is a error message!', 42, true, function() end, {})
```
