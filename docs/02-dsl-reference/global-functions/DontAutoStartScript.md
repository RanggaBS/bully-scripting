---
description: Stop execution of your script and shut it down if it was started automatically.
sidebar_class_name: hidden
---

# DontAutoStartScript

> **_This function was added in DSL 1_**

## Description

Stop execution of your script and shut it down if it was started automatically.

This is a _header_ function, meaning it is meant to go on the top of your main script as an alternative to using [config.txt](/docs/dsl-reference/basic-concepts/collections#config).

Calling this function will instantly stop execution of your script and shut it down if it was [started automatically](/docs/dsl-reference/basic-concepts/collections#startup). If a main script of a collection is shutdown as a result of calling this function, the entire collection will also be shutdown.

:::warning
It is worth noting that a script being loaded as a _dependency_ to an automatically started script or collection will _not_ be stopped by this function.
:::

```lua
function DontAutoStartScript() --[[ ... ]] end
```

## Parameters

None.

## Return Values

None.

## Example

Give the player money, but only if the script was started manually.

```lua
DontAutoStartScript()
PlayerAddMoney(10000)
```
