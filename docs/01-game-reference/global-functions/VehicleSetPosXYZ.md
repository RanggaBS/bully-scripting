---
description: Sets the position of a vehicle in the world.
sidebar_class_name: hidden
---

# VehicleSetPosXYZ

## Description

Sets the position of a vehicle in the world.
In addition to the X, Y, and Z position, this function allows manipulation of the vehicle’s internal matrix via three extra parameters (a, b, and c), which can distort or rotate the vehicle.
The final boolean argument toggles which set of values (position vs. matrix) is applied. (?)

```lua
function VehicleSetPosXYZ(car, x, y, z, a, b, c, set) --[[ ... ]] end
```

## Parameters

- `car`: _`handle`_ - A handle to the vehicle.
- `x`: _`number`_ - The new X coordinate for the vehicle.
- `y`: _`number`_ - The new Y coordinate for the vehicle.
- `z`: _`number`_ - The new Z coordinate for the vehicle.
- `a`: _`number`_ - A matrix component that affects orientation/distortion. (optional)
- `b`: _`number`_ - A matrix component that affects orientation/distortion.	(optional)
- `c`: _`number`_ - A matrix component that affects orientation/distortion. (optional)
- `set`: _`boolean`_ - Applies matrix values only, ignores position values when false. (optional)

## Return Values

None.

## Example

```lua
function main()
    -- Get player's current position
    local x, y, z = PedGetPosXYZ(gPlayer)
    
    -- Create a vehicle next to the player
    local car = VehicleCreateXYZ(295, x, y + 3, z) -- 295 = Police Car
    
    print("Vehicle created!")
    
    -- Basic positioning (normal use)
    VehicleSetPosXYZ(car, x, y + 10, z, 0, 0, 0, true)
    Wait(2000)
    
    -- Matrix manipulation example - these create visual distortions
    VehicleSetPosXYZ(car, x, y + 10, z, 1, 1, 333, false)
    Wait(5000)
    
    -- Reset to normal
    VehicleSetPosXYZ(car, x, y + 10, z, 0, 0, 0, true)
end
```

## See Also

- Game's Native
  - [`VehicleCreateXYZ`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/VehicleCreateXYZ)
  - [`VehicleDelete`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/VehicleDelete)
  - [`VehicleSetColor`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/VehicleSetColor)
  