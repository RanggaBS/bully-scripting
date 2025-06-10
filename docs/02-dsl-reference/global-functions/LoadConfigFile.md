---
description: Load a config file.
sidebar_class_name: hidden
---

# LoadConfigFile

> **_This function was added in DSL 1_**

## Description

Load a [config file](../basic-concepts/config-files) given a [relative path](../basic-concepts/relative-paths).

A valid `config` object is always returned, even if it is missing. It will just behave like an empty config file.

:::tip
You can check if a config is missing using [`IsConfigMissing`](./IsConfigMissing).
:::

```lua
function LoadConfigFile(filename) --[[ ... ]] end
```

## Parameters

- `filename` - _`string`_ - The relative path to the config file to load. If the file does not exist, an empty config object is returned.

## Return Values

- `config`: _`userdata`_ - A config object.

## Example

A simple example of loading a config file and checking if it is missing:

```lua
-- highlight-next-line
local config = LoadConfigFile('my_config.ini')
if IsConfigMissing(config) then
  print('Config file is missing!')
else
  print('Config file loaded successfully!')
end
```

Use a config file to allow the user to customize the behavior of your mod:

```lua
function MissionSetup()
  -- load config with the button for our move
  -- highlight-next-line
  local cfg = LoadConfigFile('fighting_moves.txt')
  gKickButton = GetConfigNumber(cfg, 'kick_button', 8)
end
function main()
  while not SystemIsReady() do
    Wait(0)
  end
  while true do
    local target = PedGetTargetPed(gPlayer)
    if PedIsValid(target) and PedIsInCombat(target) and PedMePlaying(gPlayer, 'Default_KEY', true) then
      -- only allow fighting moves when it is appropriate
      if IsButtonBeingPressed(gKickButton, 0) then
        PedSetActionNode(gPlayer, '/Global/G_Grappler_A/Offense/Short/Strikes/HeavyAttacks/BootKick', 'Act/Anim/G_Grappler_A.act')
      end
    end
    Wait(0)
  end
end
```

## See Also

- DSL
  - [`IsConfigMissing`](./IsConfigMissing)
