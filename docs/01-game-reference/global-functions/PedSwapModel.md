---
description: ...
sidebar_class_name: hidden
---

# PedSwapModel

## Description

Unlike what the name implies, this swaps a ped to another ped's entire stats, not just their model.

```lua
function PedSwapModel(ped, model) --[[ ... ]] end
```

## Parameters

- `ped`: _`integer`_ - The ped to swap the model of.
- `model`: _`string`_ - Ped model name to swap to.

## Return Values

...

## Example

Spawn Constantinos by the boys' dorm and swap him to Algie.

```lua
const = PedCreateXYZ(70, 270, -113, 7)
PedSwapModel(const, "NDH1a_Algernon")
```

## See Also

- Game's Native
  - [`PlayerSwapModel`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/PlayerSwapModel)