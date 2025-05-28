---
description: Sets the player's health.
sidebar_class_name: hidden
---

# PlayerSetHealth

## Description

Health can go as high as you want, but it is only meant to go to double the max health (that extra health being from the kissing bonus).
Unlike [**PedSetHealth**](https://bully-scripting.vercel.app/docs/game-reference/global-functions/PedSetHealth), this function will not change the player's max health if health is set higher. By default, the player's max health is 200.

```lua
function PlayerSetHealth(health) --[[ ... ]] end
```

## Parameters

- `health`: _`number`_ - The player's health value.

## Return Values

None.

## Example

Restore full player health.

```lua
PlayerSetHealth(PedGetMaxHealth(gPlayer))
```