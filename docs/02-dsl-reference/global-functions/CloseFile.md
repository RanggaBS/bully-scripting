---
description: Close a file.
sidebar_class_name: hidden
---

# CloseFile

> **_This function was added in DSL 4_**

## Description

Close a file.

Although you should close a file as soon as you are done with it, don't worry too much about closing it in the case that your script shuts down earlier than expected. It will automatically be collected at that time, as long as there aren't references to it anywhere else.

```lua
function CloseFile(file) --[[ ... ]] end
```

## Parameters

- `file`: _`userdata`_ - The file handle to close. This should be the same handle returned by [`OpenFile`](OpenFile). If the file is already closed, this function does nothing.

## Return Values

None.

## Example

```lua
local file, bytes = OpenFile('data.txt', 'r')
if file then
  -- Do something with the file
  -- highlight-next-line
  CloseFile(file)  -- Close the file when done
else
  print('Failed to open file')
end
```

## See Also

- DSL
  - [`OpenFile`](OpenFile)
