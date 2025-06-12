---
description: Register a new function hook.
sidebar_class_name: hidden
---

# HookFunction

> **_This function was added in DSL 6_**

## Description

Register a new function hook for a base game C function with a given `functionName`. Your `callback` function will be called with 3 arguments after the function returns.

Callbacks are passed a table of arguments, a table of results, and a boolean indiciating whether or not the function was a replacement.

Registered hooks are tied to the current script, and will be automatically cleaned up when the script is terminated.

```lua
function HookFunction(functionName, callback) --[[ ... ]] end
```

## Parameters

- `functionName`: _`string`_ - The name of the function to hook.
- `callback`: _`fun(args: { [integer]: any, n: integer }, results?: { [integer]: any, n: integer }, isReplacement?: boolean)`_ - A function that will be called with the following parameters:
  - `args`: _`table`_ - A table containing the arguments passed to the hooked function, with an additional key `n` indicating the number of arguments.
  - `results`: _`table`_ - A table containing the results returned by the hooked function, with an additional key `n` indicating the number of results. This may be `nil` if the function does not return any values.
  - `isReplacement?`: _`boolean`_ - A boolean indicating whether the hooked function was replaced by a custom implementation.

## Return Values

- `hook`: _`userdata`_ - A handle to the created hook. This can be used to remove the hook later if needed.

## Versions

- **DSL5** - This function was introduced, but was not working properly.
- **DSL6** - This function now works as intended.

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

Give all created peds a gun:

```lua
HookFunction('PedCreatePoint', function(args, results)
  local ped = results[1]
  if PedIsValid(ped) then -- rare that PedCreatePoint would return an invalid ped, but it can
    PedClearAllWeapons(ped)
    PedSetWeapon(ped, 305, 8)
  end
end)
```

## See Also

- DSL
  - [`RemoveFunctionHook`](./RemoveFunctionHook)
