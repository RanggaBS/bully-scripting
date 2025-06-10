---
description: Print output to the console.
sidebar_class_name: hidden
---

# PrintOutput

> **_This function was added in DSL 1_**

## Description

Convert all arguments to strings using `tostring` and print them in the console as output text.

```lua
function PrintOutput(...) --[[ ... ]] end
```

## Parameters

- `...`: _`any`_ - The values to be printed. Each value will be converted to a string using `tostring`.

## Return Values

None.

## Example

```lua
PrintOutput('Hello, world!', 42, true, function() end, {})
```
