---
description: Checks if the typing was aborted.
sidebar_class_name: hidden
---

# WasTypingAborted

> **_This function was added in DSL 1_**

## Description

Returns if the reason [`IsTypingActive`](IsTypingActive) returned `false` was because the typing was aborted.

Typing can be aborted by pressing the enter key, or by using [`StopTyping`](StopTyping).

```lua
function WasTypingAborted() --[[ ... ]] end
```

## Parameters

None.

## Return Values

- `aborted`: _`boolean`_ - `true` if the typing was aborted, `false` otherwise.

## Example

```lua
if WasTypingAborted() then
  print('Typing was aborted.')
else
  print('Typing completed successfully.')
end
```

## See Also

- DSL
  - [`IsTypingActive`](IsTypingActive)
  - [`StopTyping`](StopTyping)
