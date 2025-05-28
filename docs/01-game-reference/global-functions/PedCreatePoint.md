---
description: Create a character at a pre-defined point, as opposed to a custom position like PedCreateXYZ. 
sidebar_class_name: hidden
---

# PedCreatePoint

## Description

The ped will be tied to the current script so that it is cleaned up when the script terminates, and will of course be returned for you to script with.

Remember you can only use information from .DAT files that are loaded.

```lua
function PedCreatePoint(id, plist, pnumber) --[[ ... ]] end
```

## Parameters

- `id`: _`integer`_ - Ped model ID
- `plist`: _`number`_ - Point list
- `pnumber`: _`number`_ - Point number

## Return Values

- `ped`: _`integer`_ - The ID of the created ped (Not the model ID).

## Example

Create Tad and Parker in the boxing gym.

```lua
DATLoad("2_03.DAT", 2) -- Load the .DAT with the point we need

local tad = PedCreateXYZ(31, POINTLIST._2_03_PlayerStart, 1)
local parker = PedCreateXYZ(40, POINTLIST._2_03_PlayerStart, 2)
```