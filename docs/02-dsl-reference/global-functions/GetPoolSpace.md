---
description: Returns the amount of space left in a pool (the size minus the usage).
sidebar_class_name: hidden
---

# GetPoolSpace

> **_This function was added in DSL 6_**

## Description

Returns the amount of space left in a pool (the size minus the usage).

Pool names are the same as the ones used with [`GetPoolSize`](GetPoolSize).

```lua
function GetPoolSpace(pool) --[[ ... ]] end
```

## Parameters

- `pool`: _`string`_ - The name of the pool to get the size of. This is case-sensitive and must match the pool name exactly. See the [list of available pools](GetPoolSize#pools-for-the-pool-argument).

## Return Values

- `space`: _`integer`_ - The amount of space available in the specified pool.

## Example

```lua
local poolSpace = GetPoolSpace('PED')
print(poolSpace)
```
