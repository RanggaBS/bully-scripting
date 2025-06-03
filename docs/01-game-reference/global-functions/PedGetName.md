---
description: ...
sidebar_class_name: hidden
---

# PedGetName

## Description

Returns the name of a given ped as listed in default.idb.

```lua
function PedGetName(ped) --[[ ... ]] end
```

## Parameters

- `ped`: _`integer`_ - Ped to display the name of.

## Return Values

- `name`: _`string`_ - The name of the ped.

## Example

Prints "N_Jimmy" on the screen.

```lua
TextPrintString(PedGetName(gPlayer), 1, 1)
```

