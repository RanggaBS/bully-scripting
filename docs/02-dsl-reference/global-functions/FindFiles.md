---
description: Searches for files matching the given name.
sidebar_class_name: hidden
---

# FindFiles

_**This function was added in DSL 10**_

## Description

Searches for files matching the given name, which may include wildcard characters such as `*` or `?`. This function returns an iterator, intended for use in a for loop. Each iteration yields a table representing a found file, with two fields: "name" and "directory".

```lua
function FindFiles(name) --[[ ... ]] end
```

## Parameters

`name`: _`string`_ - Specifies the search pattern. This can be a directory path, a file name, or a wildcard (*, ?).

## Return Values

`iterator`: _`function`_

## Example

Gets all folders and files in the relative path:
```lua
for Found in FindFiles('*') do --> * is one of wildcard character
  print(Found.name) --> see the results on the DSL console
end
```

Gets all Lua files in the relative path:
```lua
for Found in FindFiles('*.lua') do
  if not Found.directory then
    print(Found.name)
  end
end
```
