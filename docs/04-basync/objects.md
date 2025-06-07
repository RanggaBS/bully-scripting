---
title: BASYNC - Objects
sidebar_label: Objects
description: The documentation for the objects provided by the basync module.
---

# [BASYNC](.) - Objects

## Usage

Basync objects are technically just tables, but you usually shouldn't be using any of its fields directly unless you're making a module and **really** know what you're doing. Usually, you should just use the methods described on this page to interact with these objects (or the global api functions).

The `ped:` and `veh:` parts of these method names are just provided for clarity, the way you actually use them depends on how you get or store the object. For example if you have a variable named `my_car`, you could delete it using `my_car:delete()`.

## Ped objects (server)

On the server, a basync ped object is the main way peds are represented. A ped is created for each player that joins, and more can be created using the [`net.basync.create_ped`](/docs/basync/functions#peds-server) function. They have the following methods, as well as the shared ones farther down the page.

| Function                         | Description                                                                                                                                                                                                                          |
| -------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ped:delete()                     | Delete the ped. This instantly makes the ped invalid, so you cannot use it anymore.                                                                                                                                                  |
| ped:is_valid()                   | Returns if the ped is valid. Any other function will fail if the ped isn't valid.                                                                                                                                                    |
| ped:is_player()                  | Returns if the ped is a player ped (you cannot create player peds, they are only made by basync).                                                                                                                                    |
| ped:get_owner()                  | Return the ped's owning player. Could be `-1` which means it has no owner.                                                                                                                                                           |
| ped:lock_owner()                 | Don't allow the ped's owner to switch automatically, meaning it can only be switched by `set_owner`.                                                                                                                                 |
| ped:unlock_owner()               | Allow the ped's owner to switch automatically again (the default behavior).                                                                                                                                                          |
| ped:set_owner(player)            | Set the ped's owner. This could instantly change to another player if the ped's owner isn't locked.<br/>If you try to set the owner to a player that hasn't been initialized by basync yet, `false` is returned (instead of `true`). |
| ped:set_name(name)               | Set the ped's name.                                                                                                                                                                                                                  |
| ped:set_model(model)             | Set the ped's model index.                                                                                                                                                                                                           |
| ped:set_area(area)               | Set the ped's area code. The ped will only show up for players who are also in that area.<br/>When changing a player ped's area, it will force the player to move to that area. Make sure they're in a valid position.               |
| ped:set_position(x, y, z, h)     | Set the ped's position, and optionally set their heading (`0` by default).                                                                                                                                                           |
| ped:warp_into_vehicle(veh, seat) | Set the ped's vehicle. Only use seat `0` unless you enabled passengers in basync's `config.txt`.                                                                                                                                     |
| ped:warp_out_of_car()            | Take the ped out of any vehicle they're in.                                                                                                                                                                                          |

## Ped objects (client)

On the client, a basync ped object represents a ped that exists on the server but may or may not actually be created in-game. Make sure not to confuse basync ped objects with "real" peds (which you get using `ped:get_ped`). They have the following methods, as well as the shared ones.

| Function          | Description                                                                                                                                                                                                                                                                                     |
| ----------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ped:is_valid(pre) | Returns if the ped is valid. Any other function will fail if the ped isn't valid.<br/> If the ped has not received its first state update, the function will return `false` unless pre is `true`.<br/> Remember this does not mean there is a valid ped handle associated with this ped object. |
| ped:is_player()   | Returns if the ped is a player ped (not necessarily the local player's ped).<br/> ped:is_owner()Returns if the ped is owned by the local player.                                                                                                                                                |
| ped:get_ped()     | Return the ped handle associated with this ped. Remember to check if they are valid using `PedIsValid`.                                                                                                                                                                                         |

## Ped objects (shared)

These methods are available on both the server and client.

| Function           | Description                                                                                               |
| ------------------ | --------------------------------------------------------------------------------------------------------- |
| ped:get_id()       | Return the ped's network ID.                                                                              |
| ped:get_name()     | Return the ped's name.                                                                                    |
| ped:get_model()    | Return the ped's model index.                                                                             |
| ped:get_area()     | Return the ped's current area code. It is not guaranteed to be a valid area, but it is at least a number. |
| ped:get_position() | Return the ped's position and heading (4 values).                                                         |
| ped:get_vehicle()  | Return the vehicle object the ped is in if they're in a valid one.                                        |

## Vehicle objects (server)

On the server, a basync vehicle object is the main way vehicles are represented. Vehicles can be created using the [`net.basync.create_vehicle`](/docs/basync/functions#vehicles-server) function. They have the following methods, as well as the shared ones farther down the page.

| Function                     | Description                                                                                                                                                                                                                                   |
| ---------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| veh:delete()                 | Delete the vehicle. This instantly makes the vehicle invalid, so you cannot use it anymore.                                                                                                                                                   |
| veh:is_valid()               | Returns if the vehicle is valid. Any other function will fail if the vehicle isn't valid.                                                                                                                                                     |
| veh:get_owner()              | Return the vehicle's owning player. Could be `-1` which means it has no owner.                                                                                                                                                                |
| veh:get_seat(seat)           | Returns a valid ped if one is in the vehicle's seat. Only use seat `0` unless you enabled passengers.                                                                                                                                         |
| veh:lock_owner()             | Don't allow the vehicle's owner to switch automatically, meaning it can only be switched by `set_owner`.                                                                                                                                      |
| veh:unlock_owner()           | Allow the vehicle's owner to switch automatically again (the default behavior).                                                                                                                                                               |
| veh:set_owner(player)        | Set the vehicle's owner. This could instantly change to another player if the vehicle's owner isn't locked.<br/> If you try to set the owner to a player that hasn't been initialized by basync yet, `false` is returned (instead of `true`). |
| veh:set_name(name)           | Set the vehicle's name.                                                                                                                                                                                                                       |
| veh:set_model(model)         | Set the vehicle's model index.                                                                                                                                                                                                                |
| veh:set_area(area)           | Set the vehicle's area code. The vehicle will only show up for players who are also in that area.                                                                                                                                             |
| veh:set_position(x, y, z, h) | Set the vehicle's position, and optionally set its heading (`0` by default).                                                                                                                                                                  |
| veh:set_seat(seat, ped)      | Set the ped in the vehicle's seat. Only use seat `0` unless you enabled passengers.<br/> If you want to clear the seat, pass `nil` instead of a ped.                                                                                          |

## Vehicle objects (client)

On the client, a basync vehicle object represents a vehicle that exists on the server but may or may not actually be created in-game. Make sure not to confuse basync vehicle objects with "real" vehicles (which you get using `veh:get_vehicle()`). They have the following methods, as well as the shared ones.

| Function          | Description                                                                                                                                                                                                                                                                                                         |
| ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| veh:is_valid(pre) | Returns if the vehicle is valid. Any other function will fail if the vehicle isn't valid.<br/> If the vehicle has not received its first state update, the function will return `false` unless pre is `true`.<br/> Remember this does not mean there is a valid vehicle handle associated with this vehicle object. |
| veh:is_owner()    | Returns if the vehicle is owned by the local player.                                                                                                                                                                                                                                                                |
| veh:get_vehicle() | Return the vehicle handle associated with this vehicle. Remember to check it using `VehicleIsValid`.                                                                                                                                                                                                                |

## Vehicle objects (shared)

These methods are available on both the server and client.

| Function           | Description                                                                                                   |
| ------------------ | ------------------------------------------------------------------------------------------------------------- |
| veh:get_id()       | Return the vehicle's network ID.                                                                              |
| veh:get_name()     | Return the vehicle's name.                                                                                    |
| veh:get_model()    | Return the vehicle's model index.                                                                             |
| veh:get_area()     | Return the vehicle's current area code. It is not guaranteed to be a valid area, but it is at least a number. |
| veh:get_position() | Return the vehicle's position and heading (4 values).                                                         |
| veh:get_vehicle()  | Return the vehicle object the vehicle is in if they're in a valid one.                                        |
