---
description: Start a *DSL* virtual script and add it to the current collection.
sidebar_class_name: hidden
---

# StartVirtualScript

> **_This function was added in DSL 1_**

## Description

Creating a _virtual script_ is very similar to creating a script with [`StartScript`](StartScript), except that a function is given instead of a file.

This allows you to get the benefits of having another script object, without the need for a dedicated file.

If you do not care about giving it a special `name`, you can just give the `func` as the first argument.

```lua
function StartVirtualScript(name, func) --[[ ... ]] end
```

## Parameters

- `name`: _`string`_ - The name of the script to start. This is optional, and if not provided, the function will be used as the name.
- `func`: _`function`_ - The function to run as the script. This function should not take any parameters and should return nothing.

## Return Values

- `script`: _`userdata|script|nil`_ - The script object that was started. This will be `nil` if the script was terminated before this function returned. `userdata` if checked with `type(script)`, `script` if checked with `type2(script)`.

## Versions

- **DSL4** - The optional `name` argument was added.

## Example

```lua
StartVirtualScript('MyVirtualScript', function()
  print('Hello from a virtual script!')
end)
```

## See Also

- DSL
  - [StartScript](StartScript)
  - [LoadScript](LoadScript)
