---
description: Unregister a `command` from the current script. Nothing will happen if the command is not registered with the script, and no error will be raised.
sidebar_class_name: hidden
---

# ClearCommand

> **_This function was added in DSL 1_**

## Description

Unregister a `command` from the current script. Nothing will happen if the command is not registered with the script, and no error will be raised.

```lua
function ClearCommand(command) --[[ ... ]] end
```

## Parameters

- `command`: _`string`_ - The name of the command to unregister. This should be the same name used when registering the command with `RegisterCommand`.

## Return Values

None.

## Example

```lua
ClearCommand("my_custom_command")
```

## See Also

- DSL
  - [`DoesCommandExist`](./DoesCommandExist) - To check if a command is registered before attempting to clear it.
  - [`SetCommand`](./SetCommand) - To register a command that can be executed in the script.
