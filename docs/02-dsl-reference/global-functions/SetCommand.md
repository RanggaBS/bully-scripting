---
description: Set a command with a callback function in the current DSL script.
sidebar_class_name: hidden
---

# SetCommand

> **_This function was added in DSL 1_**

## Description

Register a `command` with the current script and set the callback function for it. If the command is already registered to the current script, the callback function will be updated to the one given. If the command already exists for any other reason then the command will not be set and a warning will be shown in the console, but it is not an error. If there is no current DSL script to register with, the command will exist until cleared manually with [`ClearCommand`](ClearCommand).

`func` receives the arguments passed from the command line as strings. If a string given in the command line is quoted then it is passed as a single argument, for example `/help arg1 "arg2 arg3"` will only pass two strings to the function, `arg1` and `arg2 arg3`. All non-quoted whitespace is removed. This extra processing can be skipped by requesting a `rawArgument`, meaning only one un-modified string can be passed to the function.

The optional `helpText` is used by the built-in help command by doing something like `/help command`.

```lua
function SetCommand(command, func, rawArgument, helpText) --[[ ... ]] end
```

## Parameters

- `command`: _`string`_ - The name of the command to register. It must be a valid command name, which means it can only contain alphanumeric characters and underscores, and must not start with a number. The command is case-insensitive.
- `func`: _`fun(...: string): nil`_ - The function to call when the command is executed. It receives the arguments passed from the command line as strings.
- `rawArgument`: _`boolean?`_ - If `true`, the command will receive a single string argument that is the raw command line input without any processing. If `false` or not provided, the command will receive processed arguments as separate strings.
- `helpText`: _`string?`_ - An optional help text for the command, which can be used by the built-in help command. If not provided, no help text will be associated with the command.

## Return Values

- `set`: _`boolean`_ - `true` if the command was set successfully, `false` if it already exists for another reason.

## Example

Setting a command that greets the user with a provided name.

Once set, the command can be called from the console or script with `/greet <name>` or `greet <name>`.

```lua
SetCommand('greet', function(name)
  print('Hello, ' .. name .. '!')
end, false, 'Greets the user with the provided name.')

-- Usage: `/greet John` or `greet John`
-- Output: Hello, John!
```

## See Also

- DSL
  - [`ClearCommand`](ClearCommand)
