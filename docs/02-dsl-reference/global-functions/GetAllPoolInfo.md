---
description: Returns a table containing more tables with info about each individual pool.
sidebar_class_name: hidden
---

# GetAllPoolInfo

> **_This function was added in DSL 6_**

## Description

Returns a table containing more tables with info about each individual pool.

Each table in the returned table contain 4 fields: `name`, `size`, `limit`, and `count`.

It is worth noting that the names of pools in the table do not directly match the names expected by [`GetPoolSize`](GetPoolSize).

```lua
function GetAllPoolInfo(pool) --[[ ... ]] end
```

## Parameters

- `pool?`: _`string|nil`_ - The name of the pool to get the size of. This is case-sensitive and must match the pool name exactly. See the [list of available pools](GetPoolSize#pools-for-the-pool-argument). If not provided, it will return info for all pools.

## Return Values

- `info`: _`table[]`_ - A table containing info about the specified pool or all pools if no pool is specified. Each table in the returned table contains the following fields:
  - `name`: _`string`_ - The name of the pool.
  - `count`: _`integer`_ - The number of elements currently used in the pool.
  - `limit`: _`integer`_ - The current limit of the pool (usually equal to size).
  - `size`: _`integer`_ - The maximum number of elements allowed in the pool.

## Example

Print all pool info.

```lua
for index, pool in pairs(GetAllPoolInfo()) do
  for key, value in pairs(pool) do
    print(key .. ': ' .. value)
  end
  print('---', index)
end
```
