---
description: Check if a keyboard key was just pressed this frame.
sidebar_class_name: hidden
---

# IsKeyBeingPressed

> **_This function was added in DSL 1_**

## Description

Check if a key was just pressed, meaning it is pressed this frame but was not on the previous one.

`key` and `controller` are interpreted the same way as they are by [`IsKeyPressed`](IsKeyPressed).

```lua
function IsKeyBeingPressed(key, controller) --[[ ... ]] end
```

## Parameters

- `key`: _`string`_ - The name of the key to check.
- `controller?`: _`0|1|2|3`_ - (Optional) The controller to check the key on. Defaults to `0`, which is the keyboard.

## Return Values

- `justPressed`: _`boolean`_ - Returns _`true`_ if the key was just pressed, otherwise _`false`_.

## Versions

- **DSL4** - DirectInput keyboard scan codes are now used, but virtual key code names will still be converted for legacy support.
- **DSL6** - The optional `controller` argument was added.

## Example

Check if the 'W' key was just pressed and print a message.

```lua
function main()
  local key = 'W'
  while true do
    -- highlight-next-line
    if IsKeyBeingPressed(key) then
      DrawTextInline(key .. ' key was just pressed!', 0, 1)
    end
    Wait(0)
  end
end
```

## See Also

- DSL
  - [`IsKeyBeingReleased`](./IsKeyBeingReleased) - Check if a key was just released.
  - [`IsKeyPressed`](./IsKeyPressed) - Check if a key is being held down.
  - [`IsKeyValid`](./IsKeyValid) - Check if a key is valid.
