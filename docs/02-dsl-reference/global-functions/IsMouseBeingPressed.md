---
description: Check if a mouse button was just pressed.
sidebar_class_name: hidden
---

# IsMouseBeingPressed

> **_This function was added in DSL 5_**

## Description

Check if a mouse button was just pressed this frame.

Mouse buttons are in the range of `[0,3]` for a total of 4 buttons.

- _`0`_: Left mouse button
- _`1`_: Right mouse button
- _`2`_: Middle mouse button (scroll wheel)
- _`3`_: Extra mouse button (if available)

```lua
function IsMouseBeingPressed(button) --[[ ... ]] end
```

## Parameters

- `button`: _`0|1|2|3`_ - The mouse button to check.

## Return Values

- `justPressed`: _`boolean`_ - _`true`_ if the specified mouse button was just pressed, otherwise _`false`_.

## Example

```lua
function main()
  while true do
    if IsMouseBeingPressed(0) then
      DrawTextInline('Left mouse button was just pressed.', 0.5, 1) -- 500ms/0.5sec
    end
    Wait(0)
  end
end
```

## See Also

- DSL
  - [`IsMousePressed`](./IsMousePressed)
  - [`IsMouseBeingReleased`](./IsMouseBeingReleased)
