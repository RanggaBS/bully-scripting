---
description: Write data to a file.
sidebar_class_name: hidden
---

# WriteFile

> **_This function was added in DSL 4_**

## Description

Write `data` to `file`.

```lua
function WriteFile(file, data) --[[ ... ]] end
```

## Parameters

- `file`: _`userdata`_ - The file handle to write to. This should be the same handle returned by [`OpenFile`](./OpenFile).
- `data`: _`string`_ - The data to write to the file. This can be any string, including binary data.

## Return Values

None.

## Example

```lua
local file = OpenFile('output.txt', 'w')
if file then
  -- highligh-next-line
  WriteFile(file, 'Hello, world!')  -- Write data to the file
  CloseFile(file)
else
  print('Failed to open file')
end
```

## See Also

- DSL
  - [`OpenFile`](./OpenFile)
  - [`CloseFile`](./CloseFile)
  - [`FlushFile`](./FlushFile)
  - [`ReadFile`](./ReadFile)
