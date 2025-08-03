---
description: Sets a ped's model index without actually changing the ped's model.
sidebar_class_name: hidden
---

# PedSpoofModel

> **_This function was added in DSL 5_**

## Description

Sets a ped's model index without actually changing the ped's model.

Set a ped's model index. This doesn't _actually_ change the ped's model, which is why it is referred to as "spoofing" here. This is a good way to get around certain hard coded behaviors of some models, such as dogs not being able to have a wanted level.

```lua
function PedSpoofModel(ped, model) --[[ ... ]] end
```

## Parameters

- `ped`: _`integer`_ - The ped to spoof the model for.
- `model`: _`integer`_ - The model ID to spoof the ped with.

## Return Values

None.

## Example

Spoof a ped's model to a random model ID between 2 and 258 (inclusive). This is useful for testing or creating random behaviors without changing the actual model of the ped.

```lua
local target = PedGetTargetPed(gPlayer)
if PedIsValid(target) and IsKeyBeingPressed('P') then
  local randomId = math.random(2, 258)
  PedSpoofModel(target, randomId)
end
```

## See Also

- [Peds Models](/docs/game-reference/object-models/peds-models)
- Game's Native
  - [`PedGetTargetPed`](/docs/game-reference/global-functions/PedGetTargetPed)
  - [`PedIsValid`](/docs/game-reference/global-functions/PedIsValid)
- DSL
  - [`IsKeyBeingPressed`](/docs/dsl-reference/global-functions/IsKeyBeingPressed)
