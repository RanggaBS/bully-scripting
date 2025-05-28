---
description: Gives or removes ammo for a specified weapon to the player.
sidebar_class_name: hidden
---

# GiveAmmoToPlayer

## Description

Note that giving a weapon like the spudgun will not give spuds, but instead give spudguns (instead, use the potato weapon).

```lua
function GiveAmmoToPlayer(weapon, ammo, show) --[[ ... ]] end
```

## Parameters

- `weapon`: _`integer`_ - The ID of the weapon to modify ammo for.
- `ammo`: _`integer`_ - The amount of ammo to give (can be negative to remove ammo).
- `show`: _`boolean`_ - If false, the on-screen ammo update prompt will not be shown.

## Return Values

None.

## Example

None.

