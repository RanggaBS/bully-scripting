---
description: Returns an iterator function that will return each valid ped one at a time.
sidebar_class_name: hidden
---

# AllPeds

> **_This function was added in DSL 5_**

## Description

Returns an iterator function that will return each valid ped one at a time.

```lua
function AllPeds() --[[ ... ]] end
```

## Parameters

None.

## Return Values

- `iterator`: _`fun(): integer ped`_ - An iterator function that returns each valid ped in the game world.

## Example

Iterate through all peds in the game world and print their names:

```lua
for ped in AllPeds() do
  print(PedGetName(ped))
end
--> N_Jimmy
--> N_Trent
--> N_Parker
--> etc...
```

## See Also

- Game's Native
  - [`PedFindInAreaXYZ`](/docs/game-reference/global-functions/PedFindInAreaXYZ)
  - [`PedGetName`](/docs/game-reference/global-functions/PedGetName)
