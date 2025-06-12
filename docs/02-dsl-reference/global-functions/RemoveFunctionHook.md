---
description: Remove a function hook.
sidebar_class_name: hidden
---

# RemoveFunctionHook

> **_This function was added in DSL 6_**

## Description

Remove a hook registered with [`HookFunction`](HookFunction). Keep in mind that hooks are automatically removed when your script dies, so you do not need to call this manually.

```lua
function RemoveFunctionHook(hook) --[[ ... ]] end
```

## Parameters

- `hook`: _`userdata`_ - The handle to the hook you want to remove. This is the value returned by [`HookFunction`](HookFunction).

## Return Values

None.

## Example

```lua
-- highlight-next-line
local hook = HookFunction('GetPlayerName', function(args, results, isReplacement)
  print('GetPlayerName called with args:', args)
  if isReplacement then
    print('This was a replacement function.')
  else
    print('This was the original function.')
  end
end)
-- Later, you can remove the hook if needed
RemoveFunctionHook(hook)
```

## See Also

- DSL
  - [`HookFunction`](HookFunction)
