---
description: ...
sidebar_class_name: hidden
---

# MissionGetName

## Description

Converts a mission index to its corresponding name. Note that while this function returns a "name", it actually outputs the internal debug name used during the game's development. As a result, the returned value may not reflect the final or in-game mission name and should not be considered reliable in the current game version.

Example:
Mission index 220 is commonly recognized as "ConSumo" in the released version of the game. However, passing 220 as the argument to this function will return "Train-A-Sumo", its internal development name. This naming mismatch also applies to many mission indices.

See: [`Mission Index`](/docs/01-game-reference/scripting-enumeration/mission-index)

```lua
function MissionGetName(missionIndex) --[[ ... ]] end
```

## Parameters

`missionIndex`: _`number`_ - index of a mission.

## Return Values

`name`: _`string`_ - debug name.

## Example

```lua
local Name = MissionGetName(1)
```
