---
description: Check if a hash is equal to a number represented by a string.
sidebar_class_name: hidden
---

# IsHash

> **_This function was added in DSL 9_**

## Description

Check if a hash (returned by functions like [`ObjectNameToHashID`](./ObjectNameToHashID)) is equal to a number represented by a string. The string is specified in hexadecimal.

```lua
function IsHash(hash: userdata, check: string): boolean equal --[[ ... ]] end
```

## Parameters

- `hash`: _`userdata`_ - The hash to check.
- `check`: _`string`_ - The hexadecimal string to compare against.

## Return Values

- `equal`: _`boolean`_ - Returns `true` if the hash is equal to the number represented by the string, otherwise `false`.

## Example

Check if Jimmy is wearing the Bullworth vest by checking the hash of the clothing item:

```lua
if IsHash(ClothingGetPlayer(1), '65A6B72C') then
  TextPrintString('Wearing Bullworth vest.', 0, 1)
end
```

.

```lua
function main()
  while not SystemIsReady() do
    Wait(0)
  end

  local hash = ObjectNameToHashID('example_object')
  local isEqual = IsHash(hash, '0x12345678')

  if isEqual then
    print('The hash matches the specified number.')
  else
    print('The hash does not match the specified number.')
  end
end
```
