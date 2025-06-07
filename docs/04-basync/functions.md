---
title: BASYNC - Functions
sidebar_label: Functions
description: The documentation for the functions provided by the basync module.
---

# [BASYNC](.) - Functions

## Summary

These are the main functions used to interact with basync, though you may find it easier to use the [global api](api) a lot of the time.

The [net table](/docs/dsl-reference/basic-concepts/global-variables#net) is used to access these functions, naturally requiring basync to be running for them to be used.

## peds (server)

| Function                           | Description                                                                                                                                                                                 |
| ---------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| net.basync.create_ped(model)       | Create and return a new ped object.                                                                                                                                                         |
| net.basync.is_ped_valid(ped)       | Returns if the value is a valid ped object.                                                                                                                                                 |
| net.basync.get_player_ped(player)  | Return a player's ped object, or **nil** if they don't have a valid one.                                                                                                                    |
| net.basync.get_ped_from_player(id) | Return a valid ped object if one exists with this network ID.                                                                                                                               |
| net.basync.all_player_peds()       | Return an iterator that returns each a player and ped object for each valid player ped.<br/>For example: `for player, ped in net.basync.all_player_peds() do --\[\[ do something \]\] end`. |
| net.basync.all_peds()              | Return an iterator that returns each valid ped object.<br/>For example: `for ped in net.basync.all_peds() do --\[\[ do something \]\] end`.                                                 |

## peds (client)

| Function                                | Description                                                                                                                                                                         |
| --------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| net.basync.get_player_ped()             | Return the local player's ped object, or **nil** if they don't have a valid one.                                                                                                    |
| net.basync.get_ped_by_ped(ped)          | Return a ped object for the ped handle (a "real" ped) if a valid one exists.                                                                                                        |
| net.basync.get_ped_from_server(id, pre) | Return a valid ped object if one exists with this network ID.<br/>If the ped has not received its first state update, the function will not return anything unless pre is **true**. |
| net.basync.all_peds()                   | Return an iterator that returns each valid ped object.                                                                                                                              |

## vehicles (server)

| Function                                       | Description                                                                                                                                         |
| ---------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| net.basync.create_vehicle(model)               | Create and return a new vehicle object.                                                                                                             |
| net.basync.is_vehicle_valid(veh)               | Returns if the value is a valid vehicle object.                                                                                                     |
| net.basync.get_vehicle_from_player(player, id) | Return a valid vehicle object if one exists with this network ID.                                                                                   |
| net.basync.all_vehicles()                      | Return an iterator that returns each valid vehicle object.<br/>For example: `for veh in net.basync.all_vehicles() do --\[\[ do something \]\] end.` |

## vehicles (client)

| Function                               | Description                                                                                                                                                                                 |
| -------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| net.basync.get_vehicle_by_vehicle(veh) | Return a vehicle object for the vehicle handle (a "real" vehicle) if a valid one exists.                                                                                                    |
| net.basync.get_vehicle_from_server(id) | Return a valid vehicle object if one exists with this network ID.<br/>If the vehicle has not received its first state update, the function will not return anything unless pre is **true**. |
| net.basync.all_vehicles()              | Return an iterator that returns each valid vehicle object.                                                                                                                                  |

## world (server)

| Function                          | Description                                                                      |
| --------------------------------- | -------------------------------------------------------------------------------- |
| net.basync.get_chapter()          | Return the current chapter.                                                      |
| net.basync.get_weather()          | Return the current weather type.                                                 |
| net.basync.get_time()             | Return the current hour and minute.                                              |
| net.basync.get_time_rate()        | Return how many real milliseconds are in a game minute (or 0 if time is frozen). |
| net.basync.set_chapter(chapter)   | Set the current chapter.                                                         |
| net.basync.set_weather(weather)   | Set the current weather type.                                                    |
| net.basync.set_time(hour, minute) | Set the current hour and minute.                                                 |
| net.basync.set_time_rate(ms)      | Set how many real milliseconds are in a game minute (or 0 to freeze time).       |

## world (client)

| Function                    | Description                                                                                                                                                                  |
| --------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| net.basync.get_chapter()    | Return the current chapter.                                                                                                                                                  |
| net.basync.get_weather()    | Return the current weather type.                                                                                                                                             |
| net.basync.get_time()       | Return the current hour and minute.                                                                                                                                          |
| net.basync.get_time_rate()  | Return how many real milliseconds are in a game minute (or 0 if time is frozen).                                                                                             |
| net.basync.is_world_ready() | Return if the client has got at least one message from the server about world sync. If the world is not ready, it means all other client world functions will just return 0. |
