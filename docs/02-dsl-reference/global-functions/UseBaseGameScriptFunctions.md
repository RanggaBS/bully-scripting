---
description: Use base game script functions.
sidebar_class_name: hidden
---

# UseBaseGameScriptFunctions

> **_This function was added in DSL 1_**

## Description

Use base game script functions.

If you ever need one of the replaced base script manager functions to run when it normally wouldn't, you can use this function. Usually this will just result in issues, but it is provided for the sake of giving scripters the option to use the original functions.

```lua
function UseBaseGameScriptFunctions(useBaseFunctions) --[[ ... ]] end
```

## Parameters

- `useBaseFunctions`: _`boolean`_ - Whether to use the base game script functions or not.

## Return Values

None.

## Example

```lua
UseBaseGameScriptFunctions(true) -- Use the base game script functions

function main()
  -- This will now use the base game script function
  Wait(1000) -- Wait for 1 second using the base game function
end
```

## See Also

- DSL
  - [`Wait`](./Wait)
