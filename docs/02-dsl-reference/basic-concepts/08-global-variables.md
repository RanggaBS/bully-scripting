---
sidebar_position: 8
title: Global Variables
pagination_label: Global Variables
sidebar_label: Global Variables
description: Global variables are variables that are always available in DSL scripts. They can be used to check for the presence of DSL, or to access shared tables from script collections.
---

# Global Variables

## `gDerpyScriptLoader`

Set to the current [version of DSL](about-dsl#version-history).

You can use this value to conditionally support certain features of DSL, or to check for the presence of DSL when making a script that should work anywhere.

This value _does_ actually refer to the full version number. This means if you're running a version like **7.1**, this value will actually be **7.1** and _not_ just **7**.

```lua
if gDerpyScriptLoader then
  DrawTextInline("You can make use of DSL functions!", 3, 1)
else
  TextPrintString("Support running this script without DSL.", 3, 1)
end
```

## `dsl`

:::info

- **(DSL7)** - This feature was introduced in version 7.
  :::

The `dsl` table can be used to get shared tables from script collections that used [`GetScriptSharedTable`](/docs/dsl-reference/global-functions/GetScriptSharedTable). A shared table can be retrieved by indexing `dsl` using the desired script collection's name (case-insensitive). If the collection does not exist, is shutting down, or isn't sharing its table then you will get `nil`. You should not set values in `dsl`.

If you are making network scripts, it is suggested you use the [`net`](#net) table instead since the `dsl` table does not differentiate between local and network scripts. This would mean that a table from a local script could override the one you may expect from a network script.

Usually you should only use `dsl` instead of `net` if you are not making network scripts.

## `net`

:::info

- **(DSL8)** - This feature was introduced in version 8.
  :::

The `net` table behaves very similarly to the `dsl` table, but it gets tables from [`GetScriptNetworkTable`](/docs/dsl-reference/global-functions/GetScriptNetworkTable) instead. Only network scripts (client scripts from a server or main scripts on a server) can make these tables, so it helps ensure that network scripts have their own "namespace" independent from local scripts.

When making client network scripts, it is suggested you use `net` instead of `dsl`. Although server scripts can't have naming conflicts like the client can, using `net` will still make your code more consistent.

Sometimes it may seem more tempting to just make a global function or put a value in `shared`, but using a shared table from net is often the better choice for a few reasons.

- It naturally creates a namespace for each mod (since you must do `net.modname`), so shared function names will never conflict with other mods.
- The presence of a network table can be tested for by checking if `net.modname` is `nil`, allowing simple conditional usage of shared functions from other mods.
- Tables from `net` are only accessible while the collection is running, which ensures shared functions can only be called when the mod they came from is running.
- It is DSL's standard way of sharing functions between multiple script collections, so using it will make your mod more consistent with other scripts and official DSL scripts.

### `chat/sv_chat.lua`

```lua
api = GetScriptNetworkTable()

api.notify = function(text)
  -- some code that sends some notification message to all players
end
```

### `test.lua`

```lua
function main()
  if net.chat then
    net.chat.notify("a chat notification from an entirely different mod")
  end
end
```
