---
description: Ensure that a specific collection is running before executing the script.
sidebar_class_name: hidden
---

# RequireDependency

> **_This function was added in DSL 4_**

## Description

Ensure that a specific collection is running before executing the script.

This is a _header_ function, meaning it is meant to go on the top of your main script as an alternative to using [config.txt](/docs/dsl-reference/basic-concepts/collections#config).

This function makes sure that _Collection_ is running, and if it is not then it should be started. If it does not exist or it fails to start, then this script will be shutdown, execution will instantly stop, and the console will inform the user that they are missing a needed dependency. If a main script of a collection is shutdown as a result of calling this function, the entire collection will also be shutdown.

:::info
A difference between setting a dependency in the config and requiring it using this function, is that requiring it in the config ensures it was running **before** starting the dependent collection at all.
:::

```lua
function RequireDependency(collection) --[[ ... ]] end
```

## Parameters

- `collection`: _`string`_ - The name of the collection that this script depends on. This should be the name of the collection as defined in its `config.txt` file.

## Return Values

None.

## Example

Require all animations to be loaded for this script to run.

Remember `loadanim.lua` is released as part of DSL, so this won't require extra effort from the user. It will just ensure that it is running if they have opted to not have their scripts automatically start.

```lua
RequireDependency('loadanim.lua')
```
