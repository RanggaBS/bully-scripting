---
description: This function was added in DSL 10.
sidebar_class_name: hidden
---

# VehicleGetPassenger

## Description

Retrieves a passenger (ped) handle based on the seat index in/on the vehicle.
`0`: Driver's seat
`1`: Front passenger seat
`2`: Rear-left seat
`3`: Rear-right seat

```lua
function VehicleGetPassenger(vehicle, seatIndex) --[[ ... ]] end
```

## Parameters

`vehicle`: _`number`_ - Handle of a created vehicle.
`seatIndex`: _`number`_ - Seat index.

## Return Values

`passenger`: _`number`_ - Handle of a passenger (ped).

## Example

```lua
if PlayerIsInAnyVehicle() and PedMePlaying(gPlayer, 'Driver') then
  local Vehicle = VehicleFromDriver(gPlayer) -- gets vehicle's handle

  -- find a passenger
  local Passenger
  for Seat = 1, 3 do
    Passenger = VehicleGetPassenger(Vehicle, Seat)
    if Passenger ~= -1 then break end
  end

  -- see the passenger's name
  if Passenger == -1 then
    DrawTextInline('you have no passenger :(', 0, 1)
  else
    local Name = string.sub(PedGetName(Passenger), 3)
    DrawTextInline('say hi to '..Name, 0, 1)
  end
end
```

