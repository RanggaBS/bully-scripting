---
description: Flush writing operations.
sidebar_class_name: hidden
---

# FlushFile

> **_This function was added in DSL 4_**

## Description

Flush writing operations.

```lua
function FlushFile(file) --[[ ... ]] end
```

## Parameters

- `file`: _`userdata`_ - The file handle to flush. This should be the same handle returned by [`OpenFile`](OpenFile). If the file is not open for writing, this function does nothing.

## Return Values

None.

## Example

```lua
local file, bytes = OpenFile('data.txt', 'w')
if file then
  WriteFile(file, 'Hello, world!')
  -- highlight-next-line
  FlushFile(file)  -- Ensure all data is written to the file
  CloseFile(file)
else
  print('Failed to open file')
end
```

## See Also

- DSL
  - [`CloseFile`](CloseFile)
  - [`OpenFile`](OpenFile)
  - [`WriteFile`](WriteFile)
