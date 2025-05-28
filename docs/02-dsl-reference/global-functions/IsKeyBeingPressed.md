---
description: Returns if a key was pressed, but only once per time the key is pressed.
sidebar_class_name: hidden
---

# IsKeyBeingPressed

## Description

Returns whether a key was pressed, but only triggers once per individual key press. This prevents repeated triggering while the key is held down.

```lua
function IsKeyBeingPressed(vk) --[[ ... ]] end
```

## Parameters

- `vk`: _`integer/string`_ - A virtual key code or string, following the same rules described by [**IsKeyPressed**](https://bully-scripting.vercel.app/docs/dsl-reference/global-functions/IsKeyPressed).

## Return Values

- `state`: _`boolean`_ - Returns **true** if the key was pressed.

Will not return true again until the key is released and pressed again.

## Example

None.

