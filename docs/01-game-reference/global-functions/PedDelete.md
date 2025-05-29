---
description: Deletes a specified ped from the game world.
sidebar_class_name: hidden
---

# PedDelete

## Description

Deletes the given ped from the game.

:::warning or danger
Passing an invalid value (such as nil, a table, etc...) will crash the game.
Always ensure the ped exists and is valid before calling this function.
:::

```lua
function PedDelete(ped) --[[ ... ]] end
```

## Parameters

- `ped`: _`integer`_ - The ped to delete.

## Return Values

None.

## Example

Deletes Russell ped by pressing button.
```lua
local x, y, z = PedGetOffsetInWorldCoords(gPlayer, 0, 1, 0)
local Russell = PedCreateXYZ(75, x, y, z)
if IsButtonBeingPressed(3, 0) then
    PedDelete(Russell)
end
```

## See Also

- Game's Native
  - [`IsButtonBeingPressed`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/IsButtonBeingPressed)
  - [`PedCreateXYZ`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/PedCreateXYZ)
  - [`PedGetOffsetInWorldCoords`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/PedGetOffsetInWorldCoords)

