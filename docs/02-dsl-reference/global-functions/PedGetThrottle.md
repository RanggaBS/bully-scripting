---
description: Get a ped's current throttle value.
sidebar_class_name: hidden
---

# PedGetThrottle

> **_This function was added in DSL 7_**

## Description

Get a ped's current throttle value.

```lua
function PedGetThrottle(ped) --[[ ... ]] end
```

## Parameters

- `ped`: _`integer`_ - The ped to get the throttle value from.

## Return Values

- `throttle`: _`number`_ - The current throttle value of the ped, ranging from 0.0 (no throttle) to 1.5 (full throttle).

## Example

```lua
local target = PedGetTargetPed(gPlayer)
if PedIsValid(target) then
  local name = GetLocalizedText(PedGetName(target))
  local throttle = PedGetThrottle(target)
  DrawTextInline(name .. ': ' .. tostring(throttle), 0.1, 1)
end
```

## See Also

- Game's Native
  - [`PedGetName`](/docs/game-reference/global-functions/PedGetName)
  - [`PedGetTargetPed`](/docs/game-reference/global-functions/PedGetTargetPed)
  - [`PedIsValid`](/docs/game-reference/global-functions/PedIsValid)
- DSL
  - [`DrawTextInline`](/docs/dsl-reference/global-functions/DrawTextInline)
  - [`GetLocalizedText`](/docs/dsl-reference/global-functions/GetLocalizedText)
