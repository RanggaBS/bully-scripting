---
description: Open a file given a relative path.
sidebar_class_name: hidden
---

# OpenFile

> **_This function was added in DSL 4_**

## Description

Open a file given a [relative path](/docs/dsl-reference/basic-concepts/relative-paths). `mode` should be `'r'` for reading, `'w'` for writing, or `'a'` for updating.

Files are always opened in binary, and the size of the file is returned in `bytes`.

Zipped scripts (see [`IsScriptZipped`](IsScriptZipped)) can only open files for reading.

```lua
function OpenFile(name, mode) --[[ ... ]] end
```

## Parameters

- `name`: _`string`_ - The relative path to the file to open. This can be a path to a file in the script's package or in the script's directory.
- `mode`: _`'a'|'r'|'w'`_ - The mode to open the file in.

## Return Values

- `file`: _`userdata`_ - The file handle, which can be used with other file functions like [`ReadFile`](ReadFile) or [`WriteFile`](WriteFile).
- `bytes`: _`number`_ - The size of the file in bytes, or `0` if the file does not exist or could not be opened.

## Versions

- **DSL6** - The `'a'` mode was added.

## Example

```lua
local file, bytes = OpenFile('data.txt', 'r')
if file then
  print('File opened successfully, size:', bytes)
else
  print('Failed to open file')
end
```

## See Also

- DSL
  - [`IsScriptZipped`](IsScriptZipped)
