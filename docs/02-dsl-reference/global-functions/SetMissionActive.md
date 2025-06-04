---
description: ...
sidebar_class_name: hidden
---

# SetMissionActive

## Description

Simulates an active mission state without fully initiating it. This function tricks the game into treating a mission as currently active. However, it does not trigger mission cutscenes, camera transitions, or objectives. Its primary effects include disabling the save book, preventing mission/minigame start triggers, and suppressing class-related activities.

:::info
- Although this function accepts any mission index, including many that are unplayable, it is safe to use in the sense that it will not cause softlocks or crashes on its own.
- That said, SetMissionActive is a powerful tool, especially for implementing custom missions without replacing existing scripts. However, it must be used responsibly. Since it can be called from any script without built-in safeguards, it has a high potential for conflicts between mods.
:::

```lua
function SetMissionActive(missionIndex) --[[ ... ]] end
```

## Parameters

`missionIndex`: _`number`_

See: [`Mission Index`](/docs/game-reference/scripting-enumeration/mission-index)

## Return Values

None.

## Example

Simulates a mission.
```lua
if not IsMissionActiveSpecific('1_04') then
  SetMissionActive(12)
end
```

Stops the simulation.
```lua
SetMissionActive(-1)
```
