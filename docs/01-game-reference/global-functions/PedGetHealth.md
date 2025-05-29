---
description: Gets a ped's health.
sidebar_class_name: hidden
---

# PedGetHealth

## Description


```lua
function PedGetHealth(id) --[[ ... ]] end
```

## Parameters

- `id`: _`integer`_ - The ped's model ID.

## Return Values

- `Health`: _`integer`_ - The ped's health value.

## Example

Print how much health the target ped has.

```lua
local ped = PedGetTargetPed(gPlayer)

if PedIsValid(ped) then
	TextPrintString(PedGetName(ped)..": "..PedGetHealth(ped).." hp", 3, 2)
end
```

## See Also

- Game's Native
  - [`PedGetTargetPed`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/PedGetTargetPed)
  - [`PedIsValid`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/PedIsValid)
  - [`PedSetHealth`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/PedSetHealth)