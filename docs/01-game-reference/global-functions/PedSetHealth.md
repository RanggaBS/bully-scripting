---
description: Sets a ped's health.
sidebar_class_name: hidden
---

# PedSetHealth

## Description

Will raise max health if set higher than their current max health.

```lua
function PedSetHealth(id, health) --[[ ... ]] end
```

## Parameters

- `id`: _`integer`_ - The ped's model ID.
- `health`: _`number`_ - The ped's health value.

## Return Values

None.

## Example

Heal a ped (assumed to already exist) by 100 health points without affecting their max health.

```lua
local health = PedGetHealth(ped) + 100

if health > PedGetMaxHealth(ped) then
	health = PedSetMaxHealth(ped)
end
PedSetHealth(ped, health)
```

