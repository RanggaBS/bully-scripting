---
description: Disables the troublemeter.
sidebar_class_name: hidden
---

# DisablePunishmentSystem

## Description

Disables the punishment system, preventing the player from accumulating punishment or wanted points.
Note that this does not reset current punishment points (use [**PlayerSetPunishmentPoints**](https://bully-scripting.vercel.app/docs/game-reference/global-functions/PlayerSetPunishmentPoints) for that), nor does it stop prefects or cops from spawning (use [**PedSetUniqueModelStatus**](https://bully-scripting.vercel.app/docs/game-reference/global-functions/PedSetUniqueModelStatus) to control that).

```lua
function DisablePunishmentSystem(state) --[[ ... ]] end
```

## Parameters

- `state`: _`boolean`_ - Pass true to disable the punishment system, false to enable it.

## Return Values

None.

## Example

None.

