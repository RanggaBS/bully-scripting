---
description: Set the player's position and current area.
sidebar_class_name: hidden
---

# PlayerSetPosXYZArea

## Description

Unless [**AreaDisableCameraControlForTransition**](https://bully-scripting.vercel.app/docs/game-reference/global-functions/AreaDisableCameraControlForTransition) was called, switching to a new area will cause the camera to fade out then in.
This is the backing function for [**AreaTransitionXYZ**](https://bully-scripting.vercel.app/docs/game-reference/global-functions/AreaTransitionXYZ) and will return immediately rather than waiting for the area to load, you can use [**AreaIsLoading**](https://bully-scripting.vercel.app/docs/game-reference/global-functions/AreaIsLoading) to monitor the loading process.

```lua
function PlayerSetPosXYZArea(x, y, z, id) --[[ ... ]] end
```

## Parameters

- `x`: _`number`_ - The X coordinate of the location where the player will be moved.
- `y`: _`number`_ - The Y coordinate of the location where the player will be moved.
- `z`: _`number`_ - The Z coordinate of the location where the player will be moved.
- `id`: _`number`_ - The area ID to which the player will be moved.

## Return Values

None.

## Example

Move the player in front of the boy's dorm.

```lua
PlayerSetPosXYZArea(270, -110, 6, 0)
while AreaIsLoading() do
	Wait(0)
end
TextPrintString("Warped to boy's dorm!", 3, 1)
```

