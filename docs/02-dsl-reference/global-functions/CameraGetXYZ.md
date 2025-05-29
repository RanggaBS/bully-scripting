---
description: Returns the current camera position and its look-at coordinates.
sidebar_class_name: hidden
---

# CameraGetXYZ

## Description

Returns the current position of the camera and the coordinates it is looking at.
Useful for debugging or placing static cameras with [**CameraSetXYZ**](https://bully-scripting.vercel.app/docs/game-reference/global-functions/CameraSetXYZ).

```lua
function CameraGetXYZ() --[[ ... ]] end
```

## Parameters

None.

## Return Values

- `posx`: _`number`_ - The camera's X position.
- `posy`: _`number`_ - The camera's Y position.
- `posz`: _`number`_ - The camera's Z position.
- `lookx`: _`number`_ - The X coordinate the camera is looking at.
- `looky`: _`number`_ - The Y coordinate the camera is looking at.
- `lookz`: _`number`_ - The Z coordinate the camera is looking at.

## Example

```lua
local posx, posy, posz, lookx, looky, lookz = CameraGetXYZ()
print(string.format("Position: X=%.2f, Y=%.2f, Z=%.2f", posx, posy, posz))
print(string.format("Looking at: X=%.2f, Y=%.2f, Z=%.2f", lookx, looky, lookz))
```

