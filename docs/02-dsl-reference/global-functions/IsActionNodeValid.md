---
description: This function was added in DSL 4.
sidebar_class_name: hidden
---

# IsActionNodeValid

## Description

Checks whether an action node is valid. A valid action node should be applicable to peds, vehicles, and objects. However, in some cases, this function may return `false` even if the action node exists in the system and is applicable to those entities.

:::warning
This function does not support validation for:
- `ExecuteNodes/(node)/(node)/(node) and so on..`
:::

```lua
function IsActionNodeValid(actionNode) --[[ ... ]] end
```

## Parameters

`actionNode`: _`string`_ - Action node.

## Return Values

`valid`: _`boolean`_

## Example

```lua
local ActionNode = '/Global/Player/Attacks/Strikes/LightAttacks/Left1/Right2/Left3/Release/Unblockable/JackieKick'
local CanKick = IsActionNodeValid(ActionNode)

if CanKick and IsKeyBeingPressed('V') then
  ForceActionNode(gPlayer, ActionNode, 'Player.act')
end
```
