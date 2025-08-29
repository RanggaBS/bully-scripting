---
# description: Documentation for Bully Lua scripting POINTLIST system — anchor points, spawn markers, and teleport destinations used throughout the world.
description: Point is a data structure representing locations, spawn positions, and anchors in the game world.
---

# Point

Points (accessed via the global `POINTLIST`) are **named spatial anchors** in the game world.  
They represent things such as:

- **Spawn locations** (e.g., where a mission NPC or vehicle appears).
- **Teleport targets** (used in [`AreaTransitionPoint`](/docs/game-reference/global-functions/AreaTransitionPoint)).
- **Restart positions** (for respawning after arrest, knockout, or cutscenes).
- **Environmental anchors** (such as where leaves spawn, or shop items appear).

Unlike [`TRIGGER`](./trigger), which defines **areas/volumes**, `POINTLIST` entries define **single or multiple coordinates** that serve as specific positions.

---

## Why You Can't Iterate POINTLIST with `pairs()`

Just like [`TRIGGER`](./trigger), the `POINTLIST` object **cannot be iterated with `pairs()`**.

1. **Engine-managed container**  
   The list is stored internally by the game engine. Lua only receives integer handles when `.dat` files are loaded.

2. **Non-stable IDs**  
   Each entry in `POINTLIST` is just an engine-assigned handle. IDs change between play sessions and are not guaranteed to be stable.

Instead of iterating, you must **directly reference the desired point by name** (e.g., `POINTLIST._PLAYER_START`).

::::note[Note on Key Access]

Keys in `POINTLIST` and [`TRIGGER`](./trigger) are **case-insensitive**.

For example, the following will all work and return the same value:

```lua
DATLoad("Chapt1Trans.DAT", 2)
print(POINTLIST._PLAYER_START)
print(POINTLIST._player_start)
print(POINTLIST._PlAyEr_StArT)
```

:::tip

However, best practice is to always use UPPERCASE keys to match the game's
internal style and avoid confusion.

:::

::::

## Example Usage

Some internal Lua code shows how `POINTLIST` entries are used:

```lua
-- Teleport the player to a point in the world
AreaTransitionPoint(0, POINTLIST._BUS_POLICEDROPPLAYER, 1, true)

-- Spawn a vehicle at a defined point
shared.veh1 = VehicleCreatePoint(295, POINTLIST._BUS_POLICEDROP, 1)

-- Set restart positions
SetDefaultArrestPoint(POINTLIST._RESTART_B_PS, 0)
SetDefaultArrestRestartCameraPos(POINTLIST._RESTART_B_PS_CAM)

AddArrestRestartPoint(POINTLIST._KO_SCHOOL_INFIRMOUT, 0, 8, 19, POINTLIST._ARREST_RESTART_1, 2)
AddArrestRestartPoint(POINTLIST._KO_SCHOOL_INFIRMOUT, 0, 19, 8, POINTLIST._BOYSDORM_BEDWAKEUP, 14)

-- Interior restart points
AddInteriorArrestRestartPoint(2, POINTLIST._ARREST_RESTART_1, 2, 8, 19)
AddInteriorArrestRestartPoint(2, POINTLIST._BOYSDORM_BEDWAKEUP, 14, 19, 8)

-- Get coordinates from a point
local schoolx, schooly, schoolz = GetPointList(POINTLIST._PLAYER_START)

-- Special effect anchors
EffectAddLeavesInArea(POINTLIST._LEAVESRICHAREA, 0)

-- Shop system referencing a point
ShopAddItem(0, 502, POINTLIST._STORE_DT_GENERAL_ITEM3, 100, 0, callbackFunction, 1)

-- Spawn an NPC at a point
Players[1].Player = PedCreatePoint(130, POINTLIST._CM_GARYSTAND, 1) -- 130: Gary Smith model ID
```

Minimal example:

```lua
-- Move player instantly to dorm restart point
AreaTransitionPoint(0, POINTLIST._BOYSDORM_BEDWAKEUP, 1, true)
```

## Points Dump

For the full list of points (including how many positions each contains), see the [Points Dump](./points-dump) page.

## Notes & Best Practices

- Always load the correct `.dat` file with [DATLoad](/docs/game-reference/global-functions/DATLoad) before referencing a point. Otherwise, the value will stay `-1`.
- Some points contain multiple sub-coordinates (like an array). Use [`GetPointList`](/docs/game-reference/global-functions/GetPointList) to retrieve them, and use [`GetPointListSize`](/docs/game-reference/global-functions/GetPointListSize) to get the number of sub-coordinates.
- Point handles are not stable; always reference by constant name.
- Use points to avoid hardcoding coordinates in scripts — it keeps your mod compatible with mission logic.
