---
description: Spawns a vehicle at the specified position.
sidebar_class_name: hidden
---

# VehicleCreateXYZ

## Description

Creates a vehicle at a specific 3D position in the world using the provided vehicle ID.
Check [`here`](https://bully-scripting.vercel.app/docs/game-reference/object-models/cars-models) for more info about the vehicle ID and such.

```lua
function VehicleCreateXYZ(vehicleid, x, y, z) --[[ ... ]] end
```

## Parameters

- `vehicleid`: _`integer`_ - The ID of the vehicle to spawn.
- `x`: _`number`_ - The X coordinate where the vehicle will appear.
- `y`: _`number`_ - The Y coordinate where the vehicle will appear.
- `z`: _`number`_ - The Z coordinate where the vehicle will appear.

## Return Values

None.

## Example

```lua
-- Get player's current position
local x, y, z = PedGetPosXYZ(gPlayer)

-- Create a vehicle next to the player
local car = VehicleCreateXYZ(295, x, y + 3, z) -- 295 = Police Car

print("Vehicle created!")
```

## See Also

- Game's Native
  - [`VehicleDelete`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/VehicleDelete)
  - [`VehicleSetPosXYZ`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/VehicleSetPosXYZ)
  - [`VehicleSetColor`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/VehicleSetColor)

