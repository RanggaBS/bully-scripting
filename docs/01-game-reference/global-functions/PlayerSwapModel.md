---
description: ...
sidebar_class_name: hidden
---

# PlayerSwapModel

## Description

Just like [`PedSwapModel`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/PedSwapModel), but does not require the ped argument, as it defaults to the player.

```lua
function PlayerSwapModel(model) --[[ ... ]] end
```

## Parameters

- `model`: _`string`_ - Ped model name to swap to.

## Return Values

...

## Example

Swap to Algie.

```lua
PlayerSwapModel("NDH1a_Algernon")
```