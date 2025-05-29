---
description: Create a projectile (like an egg or spud).
sidebar_class_name: hidden
---

# CreateProjectile

## Description

Creates a projectile (such as an egg or spud) at the specified position and direction. The direction values also determine the speed of the projectile. For example, (1, 0, 0) would be straight right on the X axis.

```lua
function CreateProjectile(projectileId, posx, posy, posz, dirx, diry, dirz, damage) --[[ ... ]] end
```

## Parameters

- `projectileId`: _`integer `_ - The weapon ID of the projectile to spawn.
- `posx`: _`number`_ - X coordinate where the projectile will appear.
- `posy`: _`number`_ - Y coordinate where the projectile will appear.
- `posz`: _`number`_ - Z coordinate where the projectile will appear.
- `dirx`: _`number`_ - X component of the direction/speed vector.
- `diry`: _`number`_ - Y component of the direction/speed vector.
- `dirz`: _`number`_ - Z component of the direction/speed vector.
- `damage`: _`number`_ - Amount of health to reduce from peds on impact.

## Return Values

- `handle`: _`integer`_ - A handle to the created projectile.

## Example

```lua
local X, Y, Z = PedGetOffsetInWorldCoords(gPlayer, 1, 0, 1) -- get front-mid coords of the player
local H = PedGetHeading(gPlayer) -- heading
CreateProjectile(322, X, Y, Z, -math.sin(H) / 5, math.cos(H) / 5, 0, 9999)
```

## See Also

- Game's Native
  - [`CreateProjectile`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/DestroyProjectile)