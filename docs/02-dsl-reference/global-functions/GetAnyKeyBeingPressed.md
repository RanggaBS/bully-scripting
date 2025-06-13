---
description: Check if any keyboard key was just pressed.
sidebar_class_name: hidden
---

# GetAnyKeyBeingPressed

> **_This function was added in DSL 1_**

## Description

Returns any `keyId` that would satisfy [`IsKeyBeingPressed`](IsKeyBeingPressed).

```lua
function GetAnyKeyBeingPressed() --[[ ... ]] end
```

## Parameters

None.

## Return Values

- `keyId`: _`integer`_ - The ID of the key that was just pressed. `nil` if no key was pressed. <!-- See the [Key Codes](../key-codes) page for a list of key IDs. Returns `0` if no key was pressed. -->

## Example

```lua
function main()
  while true do
    -- highlight-next-line
    local key = GetAnyKeyBeingPressed()
    if key then
      DrawTextInline('Key ID ' .. tostring(key) .. ' was just pressed!', 0, 1)
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
