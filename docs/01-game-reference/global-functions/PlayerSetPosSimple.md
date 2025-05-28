---
description: Set the player's position without extra behaviors.
sidebar_class_name: hidden
---

# PlayerSetPosSimple

## Description

Will not behave correctly if the position is not loaded, so only use this for moving a short distance.
Unlike PlayerSetPosXYZ and PedSetPosXYZ, this will not affect anything other than the player's position.

```lua
function PlayerSetPosSimple(x, y, z) --[[ ... ]] end
```

## Parameters

- `x`: _`number`_ - The X coordinate of the position where the player will be moved.
- `y`: _`number`_ - The Y coordinate of the position where the player will be moved.
- `z`: _`number`_ - The Z coordinate of the position where the player will be moved.

## Return Values

None.

## Example

Move the player forward.

```lua
local x, y, z = PlayerGetPosXYZ()
local heading = PedGetHeading(gPlayer)
local distance = 3

PlayerSetPosSimple(x - distance * math.sin(heading), y + distance * math.cos(heading), z)
```

