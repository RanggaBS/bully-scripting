---
description: Returns all peds within a specified 3D area.
sidebar_class_name: hidden
---

# PedFindInAreaXYZ

## Description

Return all the peds in an area. Use a big number (like 9999999) to get all peds in the world.
Since this function can return many results, it is smart to wrap the call in a table (like { PedFindInAreaXYZ(0,0,0,9999999)}).
If you do that, the table will be full of peds (except the first result, it is not a ped).

```lua
function PedFindInAreaXYZ(x, y, z, range) --[[ ... ]] end
```

## Parameters

- `x`: _`number`_ - X coordinate of the center point.
- `y`: _`number`_ - Y coordinate of the center point.
- `z`: _`number`_ - Z coordinate of the center point.
- `range`: _`number`_ - Radius around the point to search for peds.

## Return Values

Multiple values: The first return value is an unknown number, followed by zero or more ped handles.

## Example

None.

