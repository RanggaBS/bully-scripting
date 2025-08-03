---
description: Return the number of elements currently used in a pool.
sidebar_class_name: hidden
---

# GetPoolUsage

> **_This function was added in DSL 6_**

## Description

Return the number of elements currently used in a pool.

Pool names are the same as the ones used with [`GetPoolSize`](GetPoolSize).

```lua
function GetPoolUsage(pool) --[[ ... ]] end
```

## Parameters

- `pool`: _`string`_ - The name of the pool to get the size of. This is case-sensitive and must match the pool name exactly. See the [list of available pools](GetPoolSize#pools-for-the-pool-argument).

## Return Values

- `usage`: _`integer`_ - The number of elements currently used in the specified pool.

## Example

```lua
local poolUsage = GetPoolUsage('PED')
print(poolUsage)
```
