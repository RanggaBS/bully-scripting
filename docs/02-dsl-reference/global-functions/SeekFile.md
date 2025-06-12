---
description: Seek a file like ANSI C.
sidebar_class_name: hidden
---

# SeekFile

> **_This function was added in DSL 4_**

## Description

Only allowed on non-zipped files, seeks a file like ANSI C.

```lua
function SeekFile(file, offset, whence) --[[ ... ]] end
```

## Parameters

- `file`: _`userdata`_ - The file handle to seek. This should be the same handle returned by [`OpenFile`](./OpenFile).
- `offset`: _`number`_ - The number of bytes to move the file pointer.
- `whence`: _`string`_ - The position from which to seek.
<!-- (not sure... AI suggestion) - Can be one of:
  - `'set'`: Seek from the beginning of the file.
  - `'cur'`: Seek from the current position in the file.
  - `'end'`: Seek from the end of the file. -->

## Return Values

None.

## Example

```lua
-- Todo...
```

## See Also

- DSL
  - [`OpenFile`](./OpenFile)
