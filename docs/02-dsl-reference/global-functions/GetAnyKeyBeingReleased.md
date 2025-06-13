---
description: Check if any keyboard key was just released.
sidebar_class_name: hidden
---

# GetAnyKeyBeingReleased

> **_This function was added in DSL 1_**

## Description

Returns any `keyId` that would satisfy [`IsKeyBeingReleased`](IsKeyBeingReleased).

```lua
function GetAnyKeyBeingReleased() --[[ ... ]] end
```

## Parameters

None.

## Return Values

- `keyId`: _`integer`_ - The ID of the key that was just released. `nil` if no key was released. <!-- See the [Key Codes](../key-codes) page for a list of key IDs. Returns `0` if no key was released. -->

## Example

```lua
function main()
  while true do
    -- highlight-next-line
    local key = GetAnyKeyBeingReleased()
    if key then
      DrawTextInline('Key ID ' .. tostring(key) .. ' was just released!', 0, 1)
    end
    Wait(0)
  end
end
```

## See Also

- DSL
  - [`IsKeyBeingPressed`](./IsKeyBeingPressed) - Check if a key was just pressed.
  - [`IsKeyBeingReleased`](./IsKeyBeingReleased) - Check if a key was just released.
  - [`IsKeyPressed`](./IsKeyPressed) - Check if a key is currently pressed.
