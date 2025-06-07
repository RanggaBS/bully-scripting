---
title: BASYNC - Global API
sidebar_label: Global API
description: Basync's global API provides a more intuitive way to interact with the game world, similar to client scripting.
---

# [BASYNC](.) - Global API

## Summary

Normally, you'd use the [net table](/docs/dsl-reference/basic-concepts/global-variables#net) to access [basync functions](functions) and then use methods to interact with basync objects. This is still useful when you need more direct control over things, but it is often easier to use basync's **global api**. Many global functions are made by basync (and its [modules](modules)) that try to mock the game's normal functions.

Keep in mind that even though the point of these functions is to make server scripting more like client scripting, not everything will work exactly the same. There are some limitations, some changes, and some entirely new functions. So make sure to read the description for whatever function you're using.

For example, see these two approaches to spawning a ped on a server script. To most people, the 2nd approach is more intuitive.

```lua
-- approach #1: using normal basync functions
ped = net.basync.create_ped(75)
ped:set_position(270, -110, 7)
```

```lua
-- approach #2: using basync's global api
ped = PedCreateXYZ(75, 270, -110, 7)
```

## Built-in

These functions are defined in `sv_api.lua`, and are always available when basync is running.

| Function                                   | Description                                                                                    |
| ------------------------------------------ | ---------------------------------------------------------------------------------------------- |
| AllPeds()                                  | Returns an iterator to use with for loops (`for ped in AllPeds() do --[[stuff]] end`).         |
| AllVehicles()                              | Returns an iterator to use with for loops (`for vehicle in AllVehicles() do --[[stuff]] end`). |
| ChapterGet()                               | Returns the current chapter.                                                                   |
| ChapterSet(chapter)                        | Set the current chapter (zero-based).                                                          |
| ClockGet()                                 | Returns the current hour and minute.                                                           |
| ClockGetTickRate()                         | Returns how many game seconds pass per real second.                                            |
| ClockSet(hour, minute)                     | Set the current hour and minute.                                                               |
| ClockSetTickRate(rate)                     | Set how many game seconds pass per real second.                                                |
| PedCreateXYZ(model, x, y, z, h)            | Create (and return) a ped with a custom position and heading.                                  |
| PedDelete(ped)                             | Delete a ped.                                                                                  |
| PedFaceHeading(ped, h)                     | Set a ped's heading in degrees.                                                                |
| PedFindInAreaXYZ(x1, y1, z1, range)        | Returns a boolean saying if any peds were found, and all found peds.                           |
| PedGetArea(ped)                            | Returns a ped's area code (not guaranteed to be a valid area).                                 |
| PedGetHeading(ped)                         | Returns a ped's heading in radians.                                                            |
| PedGetModelId(ped)                         | Returns a ped's model id (number).                                                             |
| PedGetName(ped)                            | Returns a ped's name (the name used by basync, not their localized name tag).                  |
| PedGetPosXYZ(ped)                          | Returns a ped's position (in 3 values).                                                        |
| PedInRectangle(ped, lx, ly, hx, hy)        | Returns true if a ped is within the rectangle.                                                 |
| PedIsInAnyVehicle(ped)                     | Returns true if a ped is in any vehicle.                                                       |
| PedIsInAreaXYZ(ped, x1, y1, z1, range)     | Returns true if a ped is in the area.                                                          |
| PedIsInVehicle(ped, veh)                   | Returns true if a ped is in a specific vehicle.                                                |
| PedIsModel(ped, model)                     | Returns true if a ped is a specific model (number).                                            |
| PedIsPlayer(ped)                           | Returns true if a ped is a player (has nothing to do with model).                              |
| PedIsValid(ped)                            | Returns true if a ped is valid (most other functions fail if invalid).                         |
| PedPutOnBike(ped, veh)                     | Warp a ped into a vehicle (exact same as PedWarpIntoCar).                                      |
| PedSetArea(ped, area)                      | Set a ped's area code (they will only show up in this area).                                   |
| PedSetName(ped, name)                      | Set a ped's name (the name is just for scripts, and is not used by the game).                  |
| PedSetPosXYZ(ped, x, y, z)                 | Set a ped's position.                                                                          |
| PedSwapModel(ped, name)                    | Set a ped's model (using a number or string).                                                  |
| PedWarpIntoCar(ped, veh, seat)             | Warp a ped into a vehicle (don't worry if it's a car or bike).                                 |
| PedWarpOutOfCar()                          | Warp a ped out of any vehicle they're in (if in one).                                          |
| VehicleCreateXYZ(model, x, y, z, h)        | Create (and return) a vehicle with a custom position and heading.                              |
| VehicleDelete(veh)                         | Delete a vehicle                                                                               |
| VehicleFaceHeading(veh, h)                 | Set a vehicle's heading in degrees.                                                            |
| VehicleFindInAreaXYZ(x1, y1, z1, range)    | Returns a table of vehicles in the area _if_ there are any.                                    |
| VehicleGetArea(veh)                        | Returns a vehicle's area code (not guranteed to be a valid area).                              |
| VehicleGetHeading(veh)                     | Returns a vehicle's heading in radians.                                                        |
| VehicleGetModelId(veh)                     | Returns a vehicle's model id (number).                                                         |
| VehicleGetName(veh)                        | Returns a vehicle's name (the name used by basync).                                            |
| VehicleGetPosXYZ(veh)                      | Returns a vehicle's position (in 3 values).                                                    |
| VehicleIsInAreaXYZ(veh, x1, y1, z1, range) | Returns true if a vehicle is in the area                                                       |
| VehicleIsModel(ped, model)                 | Returns true if a vehicle is a specific model (number).                                        |
| VehicleIsValid(veh)                        | Returns true if a vehicle is valid (most other functions fail if invalid).                     |
| VehicleSetArea(veh, area)                  | Set a vehicle's area (it will only show up in this area).                                      |
| VehicleSetName(veh, name)                  | Set a vehicle's name (the name is just for scripts, and is not used by the game).              |
| VehicleSetPosXYZ(veh, x, y, z)             | Set a vehicle's position.                                                                      |
| WeatherGet()                               | Returns the current weather type.                                                              |
| WeatherSet(weather)                        | Set the current weather type (can be any integer, even if a corrupt weather type).             |
