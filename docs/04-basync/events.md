---
title: BASYNC - Events
sidebar_label: Events
description: This file contains the documentation for the events provided by the basync module.
---

# [BASYNC](.) - Events

## Usage

All of these are **local events**, meaning you should use [RegisterLocalEventHandler](/docs/dsl-reference/global-functions/RegisterLocalEventHandler) to register handlers for them.

## general (server)

| Event                     | Description                                                           |
| ------------------------- | --------------------------------------------------------------------- |
| basync:initPlayer(player) | a player has been initialized for basync (after their ped is spawned) |

## general (client)

| Event                 | Description                                                                |
| --------------------- | -------------------------------------------------------------------------- |
| basync:updateServer() | activated at the same rate as the server's refresh rate (by default 30 hz) |

## peds (server)

| Event                             | Description                                                                                   |
| --------------------------------- | --------------------------------------------------------------------------------------------- |
| basync:spawnedPlayer(player, ped) | a player ped was spawned (only happens once during initialization)                            |
| basync:enterVehicle(ped, vehicle) | a ped is entering a vehicle because a player's game said to (cancelled by returning true)     |
| basync:exitVehicle(ped)           | a ped is exiting a vehicle because a player's game said to (cancelled by returning true)      |
| basync:updatePed(ped)             | a ped was updated by a player (so you can check for any bad changes and possibly revert them) |
| basync:createdPed(ped)            | a new ped was created                                                                         |
| basync:deletePed(ped)             | a ped is being deleted by a player (but this can be cancelled by returning true)              |
| basync:deletedPed(ped)            | a ped was deleted (either by a player or the server)                                          |

## peds (server, advanced)

| Event               | Description                                                                                                 |
| ------------------- | ----------------------------------------------------------------------------------------------------------- |
| basync:initPed(ped) | a ped object was created (but is not yet valid) and it's time to initialize its state                       |
| basync:setPed(k, v) | a field is being changed by a player (ped.server\[k\] = v, return true to allow it or the player is kicked) |

## peds (client)

| Event                       | Description                                                                                     |
| --------------------------- | ----------------------------------------------------------------------------------------------- |
| basync:assignPed(ped, real) | a ped was assigned a real ped (which could be invalid if they are currently despawned)          |
| basync:hidePed(real)        | a real ped (not a basync ped object) is going to be "hidden" unless cancelled by returning true |
| basync:createdPed(ped)      | a new ped was created                                                                           |
| basync:deletePed(ped)       | a ped is being deleted (this cannot be cancelled)                                               |

## peds (client, advanced)

| Event                     | Description                                 |
| ------------------------- | ------------------------------------------- |
| basync:getPed(ped, state) | a ped is getting data to send to the server |
| basync:setPed(ped)        | a ped is being updated                      |

## vehicles (server)

| Event                          | Description                                                                                       |
| ------------------------------ | ------------------------------------------------------------------------------------------------- |
| basync:updateVehicle(vehicle)  | a vehicle was updated by a player (so you can check for any bad changes and possibly revert them) |
| basync:createdVehicle(vehicle) | a new vehicle was created                                                                         |
| basync:deleteVehicle(vehicle)  | a vehicle is being deleted by a player (but this can be cancelled by returning true)              |
| basync:deletedVehicle(vehicle) | a vehicle was deleted (either by a player or the server)                                          |

## vehicles (server, advanced)

| Event                       | Description                                                                                                     |
| --------------------------- | --------------------------------------------------------------------------------------------------------------- |
| basync:initVehicle(vehicle) | a vehicle object was created (but is not yet valid) and it's time to initialize its state                       |
| basync:setVehicle(k, v)     | a field is being changed by a player (vehicle.server\[k\] = v, return true to allow it or the player is kicked) |

## vehicles (client)

| Event                               | Description                                                                                             |
| ----------------------------------- | ------------------------------------------------------------------------------------------------------- |
| basync:assignVehicle(vehicle, real) | a vehicle was assigned a real vehicle (which could be invalid if they are currently despawned)          |
| basync:hideVehicle(real)            | a real vehicle (not a basync vehicle object) is going to be "hidden" unless cancelled by returning true |
| basync:createdVehicle(vehicle)      | a new vehicle was created                                                                               |
| basync:deleteVehicle(vehicle)       | a vehicle is being deleted (this cannot be cancelled)                                                   |

## vehicles (client, advanced)

| Event                             | Description                                     |
| --------------------------------- | ----------------------------------------------- |
| basync:getVehicle(vehicle, state) | a vehicle is getting data to send to the server |
| basync:setVehicle(vehicle)        | a vehicle is being updated                      |
