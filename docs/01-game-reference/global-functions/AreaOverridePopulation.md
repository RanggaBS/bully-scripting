---
description: Override the current's area population.
sidebar_class_name: hidden
---

# AreaOverridePopulation

## Description

It works just like "PedPop.dat" in the game's Config folder.

```lua
function AreaOverridePopulation() --[[ ... ]] end
```

## Parameters

- `number` - Total
- `number` - Prefects
- `number` - Nerds
- `number` - Jocks
- `number` - Dropouts
- `number` - Greasers
- `number` - Preppies
- `number` - Students
- `number` - Cops
- `number` - Teachers
- `number` - Townpeople
- `number` - Shopkeep
- `number` - Bully

## Return Values

None.

## Example

Set a population total of 4 peds: 1 Prefect, 1 Preppy, 2 Students and 1 Greaser.

```lua
AreaOverridePopulation(4, 1, 0, 0, 0, 1, 1, 2, 0, 0, 0, 0, 0)
```