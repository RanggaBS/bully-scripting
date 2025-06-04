---
description: ...
sidebar_class_name: hidden
---

# ForceStartMissionIndex

## Description

The unorthodox method to start missions or minigames. Arguably, this is the low-level function of [ForceStartMission](/docs/01-game-reference/global-functions/ForceStartMission) and [StartMission](/docs/01-game-reference/global-functions/StartMission) in Lua.

See: [`Mission Index`](/docs/01-game-reference/scripting-enumeration/mission-index)

```lua
function ForceStartMissionIndex(missionIndex) --[[ ... ]] end
```

## Parameters

`missionIndex`: _`number`_ - index of a mission.

## Return Values

None.

## Example

Skips Math 1 - 4 and proceeds directly to Math 5.
```lua
if IsButtonBeingPressed(3, 0) then
  ForceStartMissionIndex(188)
end
```
