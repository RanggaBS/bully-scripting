---
description: Abort typing.
sidebar_class_name: hidden
---

# StopTyping

> **_This function was added in DSL 1_**

## Description

Abort typing (see [`StartTyping`](StartTyping)).

```lua
function StopTyping() --[[ ... ]] end
```

## Parameters

None.

## Return Values

None.

## Example

```lua
if IsTypingActive() then
  StopTyping()
  print('Typing was aborted.')
else
  print('No typing was active.')
end
```

## See Also

- DSL
  - [`StartTyping`](StartTyping)
