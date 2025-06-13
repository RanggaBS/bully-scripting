---
description: Check if any keyboard key is currently pressed.
sidebar_class_name: hidden
---

# GetAnyKeyPressed

> **_This function was added in DSL 1_**

## Description

Returns any `keyId` that would satisfy [`IsKeyPressed`](IsKeyPressed).

```lua
function GetAnyKeyPressed() --[[ ... ]] end
```

## Parameters

None.

## Return Values

- `keyId`: _`integer?`_ - The ID of the key that is currently pressed. ` nil` if no key is pressed. <!-- See the [Key Codes](../key-codes) page for a list of key IDs. Returns  `0` if no key is pressed. -->

## Versions

- **DSL4** - DirectInput keyboard scan codes are now used, but virtual key code names will still be converted for legacy support.
- **DSL5** - Keys are also reported as pressed when they are being pressed, and no longer when they are being released.

## Example

```lua
function main()
  while true do
    -- highlight-next-line
    local key = GetAnyKeyPressed()
    if key then
      DrawTextInline('Key ID ' .. tostring(key) .. ' is currently pressed!', 0, 1)
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
