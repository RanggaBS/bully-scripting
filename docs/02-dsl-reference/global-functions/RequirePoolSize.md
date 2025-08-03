---
description: Makes sure a pool is at least a certain size.
sidebar_class_name: hidden
---

# RequirePoolSize

> **_This function was added in DSL 6_**

## Description

Makes sure a pool is at least a certain size.

This is a _header_ function, meaning it is meant to go on the top of your main script as an alternative to using [`config.txt`](/docs/dsl-reference/basic-concepts/collections#config).

This function makes sure that a _`pool`_ is at least a certain _`size`_. Pool names are the same as the ones used with [`GetPoolSize`](GetPoolSize).

If the pool is not big enough, then this script will be shutdown, execution will instantly stop, and the console will inform the user that they need a larger pool to continue. If a main script of a collection is shutdown as a result of calling this function, the entire collection will also be shutdown.

```lua
function RequirePoolSize(pool, size) --[[ ... ]] end
```

## Parameters

- `pool`: _`string`_ - The name of the pool to get the size of. This is case-sensitive and must match the pool name exactly. See the [list of available pools](GetPoolSize#pools-for-the-pool-argument).
- `size`: _`integer`_ - The minimum size of the pool.

## Return Values

None.

## Example

```lua
RequirePoolSize("my_pool", 10)

-- ... rest of your script
```
