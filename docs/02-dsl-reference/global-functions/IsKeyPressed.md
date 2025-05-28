---
description: Returns if a key is currently pressed.
sidebar_class_name: hidden
---

# IsKeyPressed

## Description

Checks if a key is currently being pressed. You can provide a virtual key code or a string representation of the key. Also returns whether this is a new key press, using the same logic as [**IsKeyBeingPressed**](https://bully-scripting.vercel.app/docs/dsl-reference/global-functions/IsKeyBeingPressed).

```lua
function IsKeyPressed(vk) --[[ ... ]] end
```

## Parameters

- `vk`: _`integer/string`_ - A virtual key code as an integer, OR a string. You can find key codes [**here**](https://learn.microsoft.com/en-us/windows/win32/inputdev/virtual-key-codes).

You can use any constant VK_* value (e.g. "VK_SPACE"), or a single character string like "W" or "1".

## Return Values

- `state`: _`boolean`_ - true if the key is currently being held down.
- `state`: _`boolean`_ - true if this is a new key press (same as [**IsKeyBeingPressed**](https://bully-scripting.vercel.app/docs/dsl-reference/global-functions/IsKeyBeingPressed)).

## Example

None.

