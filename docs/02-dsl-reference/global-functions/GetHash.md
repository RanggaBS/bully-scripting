---
description: Returns light userdata representing the hashed string, but is case-sensitive.
sidebar_class_name: hidden
---

# GetHash

> **_This function was added in DSL 9_**

## Description

Works just like [`ObjectNameToHashID`](./ObjectNameToHashID), but it is case-sensitive.

```lua
function GetHash(name) --[[ ... ]] end
```

## Parameters

- `name`: _`string`_ - The name of the object to hash.

## Return Values

- `hash`: _`userdata`_ - Light userdata representing the hashed string.

## Example

```lua
function main()
  while not SystemIsReady() do
    Wait(0)
  end

  local hash = GetHash('example_object')
  print('Hash ID for "example_object": ' .. tostring(hash))
end
```
