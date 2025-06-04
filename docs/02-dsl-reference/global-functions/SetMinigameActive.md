---
description: ...
sidebar_class_name: hidden
---

# SetMinigameActive

## Description

Simulates an active minigame state without fully initiating it. Similar to [`SetMissionActive`](/docs/02-dsl-reference/global-functions/SetMinigameActive), this function tricks the game into treating a minigame as currently active. The primary distinction when using this function is that it removes the corona blips associated with any spawned minigames or class-related activities. This effectively prevents the player from accessing those events while a minigame is marked as active.

:::info
- Although this function accepts any mission index, including many that are unplayable, it is safe to use in the sense that it will not cause softlocks or crashes on its own.
- This function must be used with care because it can be called from any script without built-in safeguards. Therefore, it has a high potential for conflicts between mods.
:::

```lua
function SetMinigameActive(missionIndex) --[[ ... ]] end
```

## Parameters

`missionIndex`: _`number`_

See: [`Mission Index`](/docs/game-reference/scripting-enumeration/mission-index)

## Return Values

None.

## Example

Simulates a minigame.
```lua
if not IsMissionActiveSpecific('C_ART_1') then
  SetMinigameActive(134)
end
```

Stops the simulation.
```lua
SetMinigameActive(-1)
```
