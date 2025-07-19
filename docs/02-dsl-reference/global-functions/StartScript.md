---
description: Start a *DSL* script and add it to the current collection.
sidebar_class_name: hidden
---

# StartScript

> **_This function was added in DSL 1_**

## Description

Start a DSL script and add it to the current collection.

:::info
This differs from [`LoadScript`](LoadScript) as _starting_ a script means it gets its own _script object_, environment, and [flow threads](/docs/dsl-reference/basic-concepts/scripts#script-flow).
:::

`name` is given as a relative path.

You can optionally supply your own `environment` instead of letting the default one be generated.

The `script` may not be returned if the script is terminated before this function returns.

```lua
function StartScript(name, environment) --[[ ... ]] end
```

## Parameters

- `name`: _`string`_ - The name of the script to start.
- `environment`: _`table`_ - Optional. The environment to use for the script. If not provided, a new environment will be created.

## Return Values

- `script`: _`userdata|script|nil`_ - The script object that was started. This will be `nil` if the script was terminated before this function returned. `userdata` if checked with `type(script)`, `script` if checked with `type2(script)`.

## Versions

- **DSL4** - Passing a custom `environment` no longer stops a script from creating normal script [flow threads](/docs/dsl-reference/basic-concepts/scripts#script-flow).

## Example

Run two scripts in the same collection by using `StartScript`.

### `main.lua`

```lua
-- highlight-next-line
StartScript("secondary.lua")

function main()
  while not SystemIsReady() do
    Wait(0)
  end
  while true do
    TextPrintString("hello from main.lua", 0, 1)
    Wait(0)
  end
end
```

### `secondary.lua`

```lua
function main()
  while not SystemIsReady() do
    Wait(0)
  end
  while true do
    TextPrintString("hello from secondary.lua", 0, 2)
    Wait(0)
  end
end
```

## See Also

- DSL
  - [LoadScript](LoadScript)
