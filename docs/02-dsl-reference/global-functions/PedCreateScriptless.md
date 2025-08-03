---
description: Creates a ped without attaching it to the current script.
sidebar_class_name: hidden
---

# PedCreateScriptless

> **_This function was added in DSL 6_**

## Description

Creates a ped without attaching it to the current script.

Create a ped in a similar way to [`PedCreateXYZ`](/docs/game-reference/global-functions/PedCreateXYZ), but do not attach them to the current script.

Usually this function should not be used unless you have a good reason for it.

```lua
function PedCreateScriptless(model, x, y, z, heading) --[[ ... ]] end
```

## Parameters

- `model`: _`integer`_ - The model ID of the ped to create.
- `x`: _`number`_ - The X coordinate where the ped will be created
- `y`: _`number`_ - The Y coordinate where the ped will be created
- `z`: _`number`_ - The Z coordinate where the ped will be created
- `heading`: _`number`_ - The heading (rotation) of the ped when created, in degrees.

## Return Values

- `ped`: _`integer`_ - The created ped.

## Example

```lua
if IsKeyBeingPressed('L') then
  local randomId = math.random(2, 258)
  local x, y, z = PlayerGetPosXYZ()
  local heading = math.random(0, 360)
  local ped = PedCreateScriptless(randomId, x, y, z, heading)
  -- Do something with the created ped
end
```

## See Also

- Game's Native
  - [`PedCreateXYZ`](/docs/game-reference/global-functions/PedCreateXYZ)
  - [`PedGetPosXYZ`](/docs/game-reference/global-functions/PedGetPosXYZ)
  - [`PlayerGetPosXYZ`](/docs/game-reference/global-functions/PlayerGetPosXYZ)
- DSL
  - [`IsKeyBeingPressed`](/docs/dsl-reference/global-functions/IsKeyBeingPressed)
