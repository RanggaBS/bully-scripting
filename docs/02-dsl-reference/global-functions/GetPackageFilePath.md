---
description: Get the path of a file located in DSL's packages folder.
sidebar_class_name: hidden
---

# GetPackageFilePath

> **_This function was added in DSL 3_**

## Description

Get the path of a file located in DSL's `packages` folder.

The `filename` is optional just like in [`GetScriptFilePath`](GetScriptFilePath). If not specified, it will return the path to the `packages` folder itself. <!-- This is useful for loading DLL files or other resources that are part of your DSL package. -->

This is what you should be using to get your DLL file if you have a package script using `loadlib`.

```lua
function GetPackageFilePath(filename) --[[ ... ]] end
```

## Parameters

- `filename`: _`string?`_ - (Optional) The name of the file to get the path for.

## Return Values

- `fullPath`: _`string`_ - The full path to the file in the `packages` folder. If `filename` is not specified, it returns the path to the `packages` folder itself.

## Example

```lua
local fullPath = GetPackageFilePath('mydll.dll')
print('The full path to the DLL is: ' .. fullPath)
```

## See Also

- DSL
  - [`GetScriptFilePath`](GetScriptFilePath)
