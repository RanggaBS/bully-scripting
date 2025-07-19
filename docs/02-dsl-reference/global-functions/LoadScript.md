---
description: Load a *DSL* script into the current script's environment.
sidebar_class_name: hidden
---

# LoadScript

> **_This function was added in DSL 1_**

## Description

Load a **DSL** script into the current script's environment.

:::info
This differs from [`StartScript`](./StartScript) as _loading_ a script means it will load into the current script rather than fully 'starting' a new script.
:::

This can basically be thought of as the DSL version of [`ImportScript`](/docs/game-reference/global-functions/ImportScript) (though you can still use [`ImportScript`](/docs/game-reference/global-functions/ImportScript) to load scripts from `Scripts.img`).

`name` is given as a relative path.

```lua
function LoadScript(name) --[[ ... ]] end
```

## Parameters

- `name`: _`string`_ - The name of the script to load.

## Return Values

None.

## Example

A main script can load a secondary script as a way of splitting large amounts of code into separate files for organization.

The loaded script is loaded into the script that called `LoadScript`, allowing said script to use the functions and variables defined there.

### `main.lua`

```lua
-- highlight-next-line
LoadScript("example.lua")

-- Hello world, from another script! will be printed
F_HelloWorld()

-- nil will be printed, because we cannot access the local variables of the other function
print(some_local)

-- but we do share globals with that script, so we can see 7 printed here
print(some_global)
```

### `example.lua`

```lua
local some_local = 4
some_global = 7
function F_HelloWorld()
  print("Hello world, from another script!")
end
```

## See Also

- DSL
  - [`StartScript`](./StartScript)
- Game's Native
  - [`ImportScript`](./ImportScript)
