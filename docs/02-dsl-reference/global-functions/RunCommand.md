---
description: Process a command line string as if it was typed into the console.
sidebar_class_name: hidden
---

# RunCommand

> **_This function was added in DSL 4_**

## Description

Process a command line string as if it was typed into the console.

```lua
function RunCommand(commandLine) --[[ ... ]] end
```

## Parameters

- `commandLine`: _`string`_ - The command line string to process. <!-- .It can include multiple commands separated by semicolons (`;`). Each command will be processed in the order they appear in the string. (AI suggestion) -->

## Return Values

- `ran`: _`boolean`_ - `true` if the command was successfully processed, `false` if it was not recognized or could not be executed.

:::info
**DSL5** - An error is no longer raised if the command does not exist or an error occurs during parsing, and `ran` will indicate success or failure instead.
:::

## Example

```lua
RunCommand('greet John') -- Assuming 'greet' is a command that has been set up to greet the user.
RunCommand('restart MyMod')
```

## See Also

- DSL
  - [`ClearCommand`](ClearCommand)
  - [`DoesCommandExist`](DoesCommandExist)
  - [`SetCommand`](SetCommand)
