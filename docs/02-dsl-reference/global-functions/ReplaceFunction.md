---
description: Replace a base game C function with a given replacement function.
sidebar_class_name: hidden
---

# ReplaceFunction

> **_This function was added in DSL 6_**

## Description

Replace a base game C function with a given `name` with a `replacement` function.

If no replacement is given (or `nil`), then any existing replacement will be removed. The replacement function is passed the original function and all the arguments that the function was called with. An `exclusive` replacement should only be used when absolutely needed by your mod, as it will cause subsequent attempts to replace the function to fail.

Function replacements are tied to the current script, and will be automatically removed when the script is terminated.

Function replacements do not interfere with hooks, both can exist at the same time.

```lua
function ReplaceFunction(name, replacement, exclusive) --[[ ... ]] end
```

## Parameters

- `name`: _`string`_ - The name of the function to replace.
- `replacement?`: _`fun(originalFunc: function, ...: any): unknown`_ - (Optional) A function that will be called with the original function and all the arguments passed to the replaced function. If `nil`, any existing replacement will be removed.
- `exclusive`: _`boolean?`_ - (Optional) If `true`, this replacement will prevent any other replacements from being made to the same function. Defaults to `false`.

## Return Values

- `successful`: _`boolean`_ - `true` if the replacement was successful, `false` if the function does not exist or if an exclusive replacement was already made by another script.

## Versions

- **DSL5** - This function was introduced, but was not working properly.
- **DSL6** - This function now works as intended.

## Example

<!-- ```lua
ReplaceFunction('GetPlayerName', function(original, playerId)
  print('GetPlayerName called with playerId:', playerId)
  return original(playerId) .. ' (modified)'
end)
``` -->

Make all created peds random.

```lua
ReplaceFunction("PedCreatePoint", function(original, model, point, index)
  return original(4, point, index)
end)
```

## See Also

- DSL
  - [`HookFunction`](HookFunction)
  - [`RemoveFunctionHook`](RemoveFunctionHook)
