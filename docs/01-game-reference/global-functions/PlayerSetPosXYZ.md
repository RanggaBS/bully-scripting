---
description: Sets the player's position.
sidebar_class_name: hidden
---

# PlayerSetPosXYZ

## Description

This will not change the player's area, if that is something you need consider using PlayerSetPosXYZArea or AreaTransitionXYZ.
Like any other function that sets the player's position (with the exception of PlayerSetPosSimple) this will despawn most ambient peds and move allies / hostiles along with you.

```lua
function PlayerSetPosXYZ(x, y, z) --[[ ... ]] end
```

## Parameters

- `x`: _`number`_ - The X coordinate of the position where the player will be moved.
- `y`: _`number`_ - The Y coordinate of the position where the player will be moved.
- `z`: _`number`_ - The Z coordinate of the position where the player will be moved.

## Return Values

None.

## Example

Warp the player in front of the boy's dorm.

```lua
PlayerSetPosXYZ(270, -110, 6)
```

