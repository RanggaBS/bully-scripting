---
description: Print output to the console as warning text.
sidebar_class_name: hidden
---

# PrintWarning

> **_This function was added in DSL 1_**

## Description

Convert all arguments to strings using `tostring` and print them in the console as warning text.

```lua
function PrintWarning(...) --[[ ... ]] end
```

## Parameters

- `...`: _`any`_ - The values to be printed. Each value will be converted to a string using `tostring`.

## Return Values

None.

## Example

```lua
PrintWarning('This is a warning message!', 42, true, function() end, {})
```
