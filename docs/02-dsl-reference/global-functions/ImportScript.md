---
description: Import a script from Scripts.img into the current script's environment.
sidebar_class_name: hidden
---

# ImportScript

> **_This function was added in DSL 4_**

## Description

Loads a script from `Scripts.img` into the current script's environment.

This function emulates the `ImportScript` normally available to base game scripts.

This function is a special case, because the original version is actually hidden by `util.lur`. The version typically available to base game scripts is actually provided by `util.lur` that is made specifically for each script.

In an effort to mimic this behavior, DSL does not register this function as a global function. Instead, it is put into each script's environment just like `util.lur` would normally do.

```lua
function ImportScript(name) --[[ ... ]] end
```

## Parameters

- `name`: _`string`_ - The name of the script to import. This should be the name of a script file in `Scripts.img`, with the `.lua` extension.

## Return Values

None.

## Example

```lua
ImportScript('util.lua')
ImportScript('chap2/Boxing_util.lua')

ImportScript('Library/LibTable.lua')
ImportScript('Library/LibPed.lua')

ImportScript('Library\\LibTable.lua')
ImportScript('Library\\LibPed.lua')
ImportScript('Library\\LibPropNew.lua')
```
