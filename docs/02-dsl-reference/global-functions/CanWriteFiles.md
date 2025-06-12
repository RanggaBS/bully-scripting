---
description: Check if files can be written.
sidebar_class_name: hidden
---

# CanWriteFiles

## Description

Check if files can be written.

If this returns `false`, then any functions that open files for writing or write files will fail. As of now, file writing is only disabled once a server is connected to so that client scripts sent by servers cannot write files.

```lua
function CanWriteFiles() --[[ ... ]] end
```

## Parameters

None.

## Return Values

- `allowed`: _`boolean`_ - `true` if files can be written, `false` otherwise.

## Example

```lua
if CanWriteFiles() then
  print('Files can be written')
else
  print('Files cannot be written')
end
```

## See Also

- DSL
  - [`OpenFile`](OpenFile)
  - [`WriteFile`](WriteFile)
  - [`ReadFile`](ReadFile)
  - [`CloseFile`](CloseFile)
  - [`FlushFile`](FlushFile)
  - [`LoadTable`](LoadTable)
  - [`SaveTable`](SaveTable)
  - [`PackTable`](PackTable)
  - [`UnpackTable`](UnpackTable)
