---
description: Returns the string being typed.
sidebar_class_name: hidden
---

# GetTypingString

> **_This function was added in DSL 1_**

## Description

Returns the string being typed (see [`StartTyping`](StartTyping)).

:::warning
Do not call this function if you have not started typing.
:::

```lua
function GetTypingString() --[[ ... ]] end
```

## Parameters

None.

## Return Values

- `text`: _`string`_ - The string being typed.

## Example

```lua
local text = GetTypingString()
print(text)
```

## See Also

- DSL
  - [`StartTyping`](StartTyping)
  - [`IsTypingActive`](IsTypingActive)
