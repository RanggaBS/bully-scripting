---
description: Check if custom save data is ready.
sidebar_class_name: hidden
---

# IsSaveDataReady

> **_This function was added in DSL 4_**

## Description

Check if custom save data is ready. If it is not ready, the other save data functions will fail.

```lua
function IsSaveDataReady() --[[ ... ]] end
```

## Parameters

None.

## Return Values

- `ready`: _`boolean`_ - Whether the save data is ready.

## Example

```lua
if IsSaveDataReady() then
  print('Save data is ready!')
else
  print('Save data is not ready yet.')
end
```
