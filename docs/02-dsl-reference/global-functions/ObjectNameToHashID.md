---
description: Returns light userdata representing the hashed string.
sidebar_class_name: hidden
---

# ObjectNameToHashID

> **_This function was added in DSL 8_**

## Description

This function is not defined on the client, so the normal [`ObjectNameToHashID`](/docs/game-reference/global-functions/ObjectNameToHashID) will be used instead.

On the server, this function **returns light userdata representing the hashed string** to copy the client behavior.

```lua
function ObjectNameToHashID(name) --[[ ... ]] end
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

  local hash = ObjectNameToHashID('example_object')
  print('Hash ID for "example_object": ' .. tostring(hash))
end
```
