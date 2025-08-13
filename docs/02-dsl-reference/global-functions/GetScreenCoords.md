---
description: Convert world coordinates to screen coordinates.
sidebar_class_name: hidden
---

# GetScreenCoords

> **_This function was added in DSL 10_**

## Description

Convert world coordinates to screen coordinates.

This function retrieves the screen coordinates of a point in the game world, given its world coordinates (x, y, z). It is useful for converting 3D positions into 2D screen positions for rendering or UI purposes.

If the position is not on screen, it returns `nil` for the screen coordinates.

```lua
function GetScreenCoords(x, y, z) --[[ ... ]] end
```

## Parameters

- `x`: _`number`_ - The x-coordinate in the game world.
- `y`: _`number`_ - The y-coordinate in the game world.
- `z`: _`number`_ - The z-coordinate in the game world.

## Return Values

- `screenX`: _`number?`_ - The x-coordinate on the screen, or `nil` if the point is not visible. Range 0 to 1.
- `screenY`: _`number?`_ - The y-coordinate on the screen, or `nil` if the point is not visible. Range 0 to 1.

## Example

```lua
-- In front of the boys' dorm
local screenX, screenY = GetScreenCoords(270, -113, 7)

if screenX and screenY then
  print('Screen coordinates:', screenX, screenY)
else
  print('Point is not visible on screen.')
end
```
