---
description: Set a ped's current throttle value.
sidebar_class_name: hidden
---

# PedSetThrottle

> **_This function was added in DSL 7_**

## Description

Set a ped's current throttle value.

Only has an effect if using during a [`PedUpdateThrottle`](/docs/dsl-reference/global-functions/RegisterLocalEventHandler) event.

```lua
function PedSetThrottle(ped, throttle) --[[ ... ]] end
```

## Parameters

- `ped`: _`integer`_ - The ped to set the throttle value for.
- `throttle`: _`number`_ - The throttle value to set, ranging from 0.0 (no throttle) to 1.5 (full throttle).

## Return Values

None.

## Example

```lua
local target = PedGetTargetPed(gPlayer)
local randomThrottle = math.random() * 1.5
PedSetThrottle(target, randomThrottle)
```

## See Also

- Game's Native
  - [`PedGetTargetPed`](/docs/game-reference/global-functions/PedGetTargetPed)
- DSL
  - [`RegisterLocalEventHandler`](/docs/dsl-reference/global-functions/RegisterLocalEventHandler)
