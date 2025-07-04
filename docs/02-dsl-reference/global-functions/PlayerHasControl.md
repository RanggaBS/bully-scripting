---
description: Checks whether the player currently has control over the active ped.
sidebar_class_name: hidden
---

# PlayerHasControl

> **_This function was added in DSL 2_**

## Description

Checks whether the player currently has control over the active ped. When a script calls [`PlayerSetControl`](/docs/game-reference/global-functions/PlayerSetControl), it either enables or disables player input instruction for the ped. This function allows you to verify whether player control is currently enabled.

```lua
function PlayerHasControl() --[[ ... ]] end
```

## Parameters

None.

## Return Values

`control`: _`boolean`_

## Example

```lua
if IsKeyBeingPressed('T') then
  PlayerSetControl(0)
elseif IsKeyBeingPressed('Y') then
  PlayerSetControl(1)
end

if PlayerHasControl() then
  DrawTextInline('controlling..', 0, 1)
end
```

