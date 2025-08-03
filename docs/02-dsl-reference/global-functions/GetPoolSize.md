---
description: Return the maximum number of elements allowed in a pool.
sidebar_class_name: hidden
---

# GetPoolSize

> **_This function was added in DSL 6_**

## Description

Return the maximum number of elements allowed in a pool.

Pool sizes can not normally be changed unless using DSL's [pool options](/docs/dsl-reference/basic-concepts/config-files#hidden-pool-options-dsl-5) or another mod that resizes pools.

```lua
function GetPoolSize(pool) --[[ ... ]] end
```

## Parameters

- `pool`: _`string`_ - The name of the pool to get the size of. This is case-sensitive and must match the pool name exactly.

### Pools (for the _`pool`_ argument)

Please note that some pool names actually refer to multiple parallel pools. For example `PED` actually refers to 9 total pools.

- `PTR_NODE`
- `ENTRY_INFO_NODE`
- `VEHICLE`
- `PED`
- `JOINT_CONSTRAINT`
- `WEAPON`
- `LUA_SCRIPT`
- `DUMMY`
- `PROP_ANIM`
- `BUILDING`
- `TREADABLE`
- `COL_MODEL`
- `STIMULUS`
- `OBJECT`
- `PROJECTILE`
- `CUT_SCENE`
- `UNKNOWN`

## Return Values

- `size`: _`integer`_ - The maximum number of elements allowed in the specified pool.

## Example

```lua
local poolSize = GetPoolSize('PED')
print(poolSize)
```
