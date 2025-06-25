---
description: Spawns any registered non-ped object at the specified position.
sidebar_class_name: hidden
---

# CreatePersistentEntity

## Description

Creates and spawns a persistent non-ped object (such as machines, props, or interactable objects) in the world.

```lua
function CreatePersistentEntity(modelname, x, y, z, rotation, area) --[[ ... ]] end
```

## Parameters

- `modelname`: _`string`_ - The object’s modelname (e.g. "DPI_Fraffy").
- `x`: _`integer`_ - X coordinate for the spawn position.
- `y`: _`integer`_ - Y coordinate for the spawn position.
- `z`: _`integer`_ - Z coordinate for the spawn position.
- `rotation`: _`integer`_ - Rotation angle for the object.
- `area`: _`integer`_ - The area code in which to spawn the object.

## Return Values

- `objectID`: _`integer`_ - The object ID.
- `objectPool`: _`integer`_ - The object pool index.

## Example

```lua
-- Spawn a Beam Soda machine (plus its interactable entity) in front of the Boys' Dorm.
Soda1, Soda2 = CreatePersistentEntity("DPI_Fraffy", 270, -114, 6.15, 180, 0)
pxSoda1, pxSoda2 = CreatePersistentEntity("pxFraffy", 270, -114, 6.15, 180, 0)
```

## See Also

- Game's Native
  - [`DeletePersistentEntity`](./DeletePersistentEntity)