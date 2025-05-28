---
description: Move the player to a new area, wait for it to load, and optionally opt out of camera fading.
sidebar_class_name: hidden
---

# AreaTransitionXYZ

## Description

This function is defined by SGlFunc.lur and primarily uses PlayerSetPosXYZArea and AreaDisableCameraControlForTransition to do its job.

```lua
function AreaTransitionXYZ(id, x, y, z, state) --[[ ... ]] end
```

## Parameters

- `id`: _`integer`_ - The area ID to which the player will be moved.
- `x`: _`number`_ - The X coordinate of the location where the player will be moved.
- `y`: _`number`_ - The Y coordinate of the location where the player will be moved.
- `z`: _`number`_ - The Z coordinate of the location where the player will be moved.
- `state`: _`boolean`_ - Disable camera control.

## Return Values

None.

## Example

Transition to the front of the boy's dorm without fading the camera out.

```lua
AreaTransitionXYZ(0, 270, -110, 6, true)
```

