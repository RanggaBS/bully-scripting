---
description: This function is used to retrieve the function environment from native scripts and is typically utilized for hooking or replacing functions in there.
sidebar_class_name: hidden
---

# AddScriptLoaderCallback

> **_This function was added in DSL 1_**

## Description

This function is used to retrieve the function environment from native scripts and is typically utilized for hooking or replacing functions in there.

:::warning
This function has been **deprecated** since DSL version 4 as it has been superseded by the **NativeScriptLoaded** event in [`RegisterLocalEventHandler`](RegisterLocalEventHandler) function. However, it remains accessible for backward compatibility with legacy scripts.
:::

Original documentation from _derpy54320_:

> _Registers a new `NativeScriptLoaded` event handler, meaning `callback` will be called when a base game script is loaded. The script's name and environment is passed to the function so it can apply changes and patches to the script, as well as give it modified versions of normal functions as a way of changing the script's behavior. Keep in mind that the name given is a **full** name, so you may need to print what it says when you expect a script to start in order to get the right name for it._
>
> :::info
> **DSL4** - This function is now just for legacy support, and does the same thing calling [`RegisterLocalEventHandler`](RegisterLocalEventHandler) with `NativeScriptLoaded` would.
> :::

```lua
function AddScriptLoaderCallback(callback) --[[ ... ]] end
```

## Parameters

- `callback`: _`function(name, env)`_

## Return Values

None.

## Example

Automatically pass the geography class

```lua
local Passed = false
AddScriptLoaderCallback(function(Name, Env)
  if Name == 'ClassGeography.lua' or Name == 'secnd/ClassGeography.lua' then
    -- Trigger auto-pass: hook into a function that is called after the minigame has started
    Env.ClassGeographyInvalidOperation = function()
      if not Passed then
        ClassGeographySuccess() -- only called once
        Passed = true
      end
      return ClassGeographyInvalidOperation()
    end

    -- Reset auto-pass: hook into a function that is called after the minigame has ended
    Env.MinigameEnableHUD = function(HUD)
      if not HUD then
        Passed = false
      end
      return MinigameEnableHUD(HUD)
    end
  end
end)
```

Example from derpy54320:

Change store prices to be free and stop the boy's dorm script from despawning little kids.

```lua
function F_ShopAddItem(...)
  arg[5] = 0
  return ShopAddItem(unpack(arg))
end
function F_Nothing()
end
AddScriptLoaderCallback(function(name, env)
  if name == "SStores.lua" then
    -- change SStores.lua's ShopAddItem to be our custom version so we can change prices
    env.ShopAddItem = F_ShopAddItem
  elseif name == "AreaScripts/Bdorm.lua" then
    -- change a function the bdorm script to stop little kids from being despawned
    env.F_KillAllLittleKids = F_Nothing
  end
  print("loaded "..name)
end)
```
