---
description: Finds a random spawn position for a ped.
sidebar_class_name: hidden
---

# PedFindRandomSpawnPosition

## Description

Find a random spawn position for a ped.
If ped production is stopped (using [**StopPedProduction**](https://bully-scripting.vercel.app/docs/game-reference/global-functions/StopPedProduction)), this will never return a position.

```lua
function PedFindRandomSpawnPosition(pedId) --[[ ... ]] end
```

## Parameters

- `pedId`: _`integer`_ - The ID of the ped to find a spawn position for. **(optional)**

## Return Values

- `x`: _`number`_ - X coordinate of the spawn position, or 9999 if no valid position found.
- `y`: _`number`_ - Y coordinate of the spawn position.
- `z`: _`number`_ - Z coordinate of the spawn position.

## Example

None.

