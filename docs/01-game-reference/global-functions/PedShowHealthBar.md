---
description: Displays a specific type of HealthBar for a specific ped.
sidebar_class_name: hidden
---

# PedShowHealthBar

## Description

The first boolean determines the **HealthBar Type**, where false is the ground HealthBar, while true is whatever's determined by the second boolean.
The second boolean determines **HealthBar Style**, where false is the ally HealthBar, while true is the boss HealthBar.

```lua
function PedShowHealthBar(id, type, name, style) --[[ ... ]] end
```

## Parameters

- `id`: _`integer`_ - Ped ID.
- `type`: _`boolean`_ - HealthBar Type.
- `name`: _`string`_ - Ped name.
- `style`: _`boolean`_ - HealthBar Style.

## Return Values

None.

## Example

None.

