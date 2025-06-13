---
description: Check if a keyboard key was just released.
sidebar_class_name: hidden
---

# IsKeyBeingReleased

> **_This function was added in DSL 1_**

## Description

Check if a key was just released, meaning it is not pressed this frame but was on the previous one.

`key` and `controller` are interpreted the same way as they are by [`IsKeyPressed`](IsKeyPressed).

```lua
function IsKeyBeingReleased(key, controller) --[[ ... ]] end
```

## Parameters

- `key`: _`string`_ - The name of the key to check.
- `controller?`: _`0|1|2|3`_ - (Optional) The controller to check the key on. Defaults to `0`, which is the keyboard.

## Return Values

- `justReleased`: _`boolean`_ - Returns _`true`_ if the key was just released, otherwise _`false`_.

## Versions

- **DSL4** - DirectInput keyboard scan codes are now used, but virtual key code names will still be converted for legacy support.
- **DSL6** - The optional `controller` argument was added.

## Example

```lua
function main()
  local key = 'W'
  while true do
    -- highlight-next-line
    if IsKeyBeingReleased(key) then
      DrawTextInline(key .. ' key was just released!', 0, 1)
    end
    Wait(0)
  end
end
```

## See Also

- DSL
  - [`IsKeyBeingPressed`](./IsKeyBeingPressed) - Checks if a key was just pressed.
  - [`IsKeyPressed`](./IsKeyPressed) - Checks if a key is currently pressed.
  - [`IsKeyValid`](./IsKeyValid) - Checks if a key is valid.
