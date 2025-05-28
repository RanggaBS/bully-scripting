---
description: Makes the camera smoothly rotate to look at a specified position.
sidebar_class_name: hidden
---

# CameraLookAtXYZ

## Description

Rotates the camera smoothly to look at the given XYZ coordinates.
Unlike the direct snap in [**CameraSetXYZ**](https://bully-scripting.vercel.app/docs/game-reference/global-functions/CameraSetXYZ), this function animates the rotation toward the target position.

```lua
function CameraLookAtXYZ(x, y, z) --[[ ... ]] end
```

## Parameters

- `x`: _`number`_ - X coordinate to look at.
- `y`: _`number`_ - Y coordinate to look at.
- `z`: _`number`_ - Z coordinate to look at.

## Return Values

None.

## Example

None.

