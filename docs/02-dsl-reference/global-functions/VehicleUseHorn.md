---
description: This function was added in DSL 10.
sidebar_class_name: hidden
---

# VehicleUseHorn

## Description

Plays a vehicle horn sound in 3D space, based on the vehicle's position relative to the camera.

```lua
function VehicleUseHorn(vehicle) --[[ ... ]] end
```

## Parameters

`vehicle`: _`number`_ - Handle of a created vehicle.

## Return Values

None.

## Example

```lua
local InCar_or_OnMotorcycle = PedMePlaying(gPlayer, 'Cars') or PedMePlaying(gPlayer, 'Motorcycle')
if PlayerIsInAnyVehicle() and InCar_or_OnMotorcycle and IsButtonBeingPressed(8, 0) then
  local Vehicle = VehicleFromDriver(gPlayer) -- gets vehicle's handle
  VehicleUseHorn(Vehicle)
end
```

