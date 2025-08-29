---
# description: Documentation for Bully Lua scripting TRIGGER system — spatial detectors that define areas and events in the world.
description: Trigger is a spatial detector that defines an area in the game world.
---

# Trigger

Triggers are **spatial detectors** used in the game world.  
They typically take the form of a **cuboid** (box) or **sphere** that surrounds a certain part of the map.  
When the player or an NPC walks into or out of this region, a predefined action can occur.

Examples:

- Entering the school gate starts a cutscene.
- Crossing into a mission zone spawns enemies or starts objectives.
- Opening a garage door activates an animation sequence.

Triggers are **not Lua tables**, but engine-managed objects exposed through global constants such as `TRIGGER._AMB_SCHOOL_AREA`.  
To use them, you must first load the corresponding `.dat` file with [`DATLoad`](/docs/game-reference/global-functions/DATLoad). If the required file is not loaded, the value of a trigger constant will remain `-1`.

## Why You Can't Iterate TRIGGER with `pairs()`

Although `TRIGGER` looks like a Lua table, it cannot be iterated with `pairs()` or `ipairs()`. Two main reasons:

1. **Engine-backed structure**  
   The game engine stores triggers in a hidden C-side list. Lua only receives integer handles (IDs).  
   These IDs change between sessions and are not guaranteed to remain stable.

2. **Safety**
   Allowing iteration would expose engine internals directly to Lua. This could cause instability or crashes, so the API deliberately prevents it.

Instead of trying to scan all triggers, you must reference them by name (e.g. `TRIGGER._Garage_SchoolGrounds`).

::::note[Note on Key Access]

Keys in `TRIGGER` and [`POINTLIST`](./points.md) are **case-insensitive**.

For example, the following are equivalent and will all work:

```lua
DATLoad("Chapt1Trans.DAT", 2)
print(TRIGGER._TSCHOOL_FRONTGATE)
print(TRIGGER._tschool_frontgate)
print(TRIGGER._tScHoOl_PaRkInGgAtE)
```

:::tip

However, as a best practice, always use **UPPERCASE keys** to follow the
game's internal code style and avoid confusion.

:::

::::

## Example Usage

Here is a some code snippet from the game's internal code showing how triggers are used:

```lua
-- TRIGGER

if PlayerIsInTrigger(TRIGGER._AMB_SCHOOL_AREA) or AreaGetVisible() == 14 then
  -- ...
end

GarageAdd(TRIGGER._Garage_SchoolGrounds, POINTLIST._Garage_SchoolGrounds)

RegisterTriggerEventHandler(TRIGGER._BA_BMXGARAGE, 1, callbackFunction)

AreaSetDoorLockedToPeds(TRIGGER._BMX_GARAGEDOOR, true)
AreaSetDoorLocked(TRIGGER._BMX_GARAGEDOOR, true)

PAnimSetActionNode(TRIGGER._BA_BMXGARAGE, "/Global/Door/DoorFunctions/Closing/BIKEGAR", "Act/Props/Door.act")

PAnimOpenDoor(TRIGGER._ICOMSHP_BASEMENT)
PAnimDoorStayOpen(TRIGGER._FMDOORN01)
```

Another minimal example:

```lua
-- Check if player enters a defined trigger zone
if PlayerIsInTrigger(TRIGGER._AMB_SCHOOL_AREA) then
  TextPrintString('Inside the school area!', 0, 1)
end
```

## Triggers Dump

For a complete list of all available Trigger, please refer to the [Triggers Dump](./triggers-dump) page.

## Notes & Best Practices

- Always load the corresponding `.dat` file with [`DATLoad`](/docs/game-reference/global-functions/DATLoad) before referencing a trigger. Otherwise, the constant will stay `-1`.
- IDs are **not stable** across sessions; always reference by constant name.
- Do not overlap multiple triggers unless necessary.
