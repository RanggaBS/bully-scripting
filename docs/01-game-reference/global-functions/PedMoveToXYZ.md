---
description: ...
sidebar_class_name: hidden
---

# PedMoveToXYZ

## Description

Makes a ped move to a specified location.

```lua
function PedMoveToXYZ(ped, speed, x, y, z) --[[ ... ]] end
```

## Parameters

- `ped`: _`integer`_ - The ped to move.
- `speed`: _`integer`_ - The speed of the ped to move at from 0-3.
- `x`: _`number`_ - The X coordinate to move to.
- `y`: _`number`_ - The Y coordinate to move to.
- `z`: _`number`_ - The Z coordinate to move to.

## Return Values

...

## Example

Spawn the player, and a Constantinos to manipulate, by the boys' dorm.
```lua
AreaTransitionPoint(0, POINTLIST._SV_BoysDormMain)
const = PedCreateXYZ(70, 268.50, -113.18, 6.24)
local moved
while true do
    if IsButtonBeingPressed(7, 0) then
        if not moved then
            PedMoveToXYZ(const, 1, 273.50, -113.18, 6.24)
            moved = true
        else
            PedDelete(const)
            const = PedCreateXYZ(70, 268.50, -113.18, 6.24)
            PedMoveToXYZ(const, 1, 268.50, -113.18, 6.24)
            moved = false
        end
    end
    TextPrintString("Press ~x~ to make Constantinos jog.\nPress ~x~ again to reset.", 0, 2)
Wait(0)
end
```

