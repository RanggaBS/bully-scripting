---
description: Call a function from a native script.
sidebar_class_name: hidden
---

# CallFunctionFromScript

> **_This function was added in DSL 1_**

## Description

Call a function from a native script. The way this is done is by spoofing the game into thinking a certain game script is running, while also temporarily telling DSL that none of its scripts are.

In most cases, this is just as good as actually calling a function from the script in question. The most notable example of that not being the case is with [`ButtonHistorySetCallbackFailed`](/docs/game-reference/global-functions/ButtonHistorySetCallbackFailed) and its related functions. If you want a simpler way to make this apply to your entire script for a certain function, consider using [`UseProxyScriptForFunction`](./UseProxyScriptForFunction).

_`script`_ should be the name of a native script that is currently running, or a DSL script object. Passing `nil` instead of any other value will spoof the game into thinking there is no scripts at all. Otherwise, your options will usually consist of `main.lua`, `STimeCycle.lua`, the current area script, and the current mission / errand.

:::warning
If you use this to create something (such as a blip for instance), make sure to delete that something by the time your script ends or it could permanently take up resources.

If using `nil` for a script, do not create or destroy native game scripts (by using something like [`LaunchScript`](/docs/game-reference/global-functions/LaunchScript)). It will result in undefined behavior.
:::

```lua
function CallFunctionFromScript(script, function, ...) --[[ ... ]] end
```

## Parameters

- `script?`: _`string|nil`_ - The name of the script to call the function from.
- `function`: _`fun`_ - The function to call.
- `...`: _`any`_ - The arguments to pass to the function.

## Return Values

- `...`: _`any`_ - The return values of the function.

## Versions

- **DSL 5** - A DSL script object can be passed for _`script`_ to call the function from that script.

## Example

```lua
local result = CallFunctionFromScript('main.lua', function(arg1, arg2)
  print('This is called from main.lua!')
  print(arg1, arg2)
  return 'Done!'
end, 'hello', 'world')
print(result) --> 'Done!'
```
