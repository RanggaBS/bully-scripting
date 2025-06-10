---
description: Print output to the console.
sidebar_class_name: hidden
---

# print

> **_This function was added in DSL 1_**

## Description

This function is an alias to [`PrintOutput`](PrintOutput) that replaces the originally useless [`print`](/docs/game-reference/global-functions/print) function.

```lua
function print(...) --[[ ... ]] end
```

## Parameters

- `...`: _`any`_ - The values to be printed. Each value will be converted to a string using `tostring`.

## Return Values

None.

## Example

```lua
print('Hello, world!', 42, true, function() end, {})
```

## See Also

- Game's Native
  - [`print`](/docs/game-reference/global-functions/print)
- DSL
  - [`PrintOutput`](PrintOutput)
