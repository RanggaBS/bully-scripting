---
description: Disable camera fading during area switches.
sidebar_class_name: hidden
---

# AreaDisableCameraControlForTransition

## Description

You will need to keep this on until [**AreaIsLoading**](https://bully-scripting.vercel.app/docs/game-reference/global-functions/AreaDisableCameraControlForTransition) returns false for full effect.

```lua
function AreaDisableCameraControlForTransition(state) --[[ ... ]] end
```

## Parameters

- `state`: _`boolean`_ - Disable camera control.

## Return Values

None.

## Example

Fade the screen out and move the player to the front of the boy's dorm, only unfading when the area is fully loaded.

```lua
-- go to the loading screen
CameraFade(1000, 0)
Wait(1000)

-- move the player without letting PlayerSetPosXYZArea affect the camera fade
AreaDisableCameraControlForTransition(true)
PlayerSetPosXYZArea(270, -110, 6, 0)
while AreaIsLoading() do
	Wait(0)
end
AreaDisableCameraControlForTransition(false)

-- wait for all loading to finish
while IsStreamingBusy() do
	Wait(0)
end
Wait(1000) -- wait an extra second for potential pop-in

-- fade the camera back in
CameraFade(1000, 1)
```

## See Also

- Game's Native
  - [`AreaIsLoading`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/AreaIsLoading)