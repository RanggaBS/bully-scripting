---
description: Read bytes from a file.
sidebar_class_name: hidden
---

# ReadFile

> **_This function was added in DSL 4_**

## Description

Read `bytes` from `file`.

```lua
function ReadFile(file, bytes) --[[ ... ]] end
```

## Parameters

- `file`: _`userdata`_ - The file handle to read from. This should be the same handle returned by [`OpenFile`](./OpenFile).
- `bytes`: _`number`_ - The number of bytes to read from the file. If the file has fewer bytes than requested, it will return only the available bytes.

## Return Values

- `data`: _`string`_ - The data read from the file. If the end of the file is reached, it returns an empty string.

## Example

```lua
local file, bytes = OpenFile('data.txt', 'r')
if file then
  -- highligh-next-line
  local data = ReadFile(file, 100)  -- Read up to 100 bytes from the file
  if data ~= '' then
    print('Data read from file:', data)
  else
    print('End of file reached or no data read')
  end
  CloseFile(file)
else
  print('Failed to open file')
end
```

## See Also

- DSL
  - [`OpenFile`](./OpenFile)
