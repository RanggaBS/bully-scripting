---
description: Returns if typing is currently active.
sidebar_class_name: hidden
---

# IsTypingActive

> **_This function was added in DSL 1_**

## Description

Returns if typing is currently active (see [`StartTyping`](StartTyping)).

```lua
function IsTypingActive() --[[ ... ]] end
```

## Parameters

None.

## Return Values

- `active`: _`boolean`_ - `true` if typing is active, `false` otherwise.

## Example

```lua
if IsTypingActive() then
  print('Typing is currently active.')
else
  print('Typing is not active.')
end
```

## See Also

- DSL
  - [`StartTyping`](StartTyping)
