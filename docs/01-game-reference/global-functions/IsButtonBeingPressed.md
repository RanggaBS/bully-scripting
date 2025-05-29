---
description: Check if a button was JUST pressed this exact frame.
sidebar_class_name: hidden
---

# IsButtonBeingPressed

## Description

Use this if you want things to only happen once per button press.
Check [`here`](https://bully-scripting.vercel.app/docs/game-reference/scripting-enumeration/controls) for more info about the button ID and the controller ID.

```lua
function IsButtonBeingPressed(button, controller) --[[ ... ]] end
```

## Parameters

- `button`: _`integer`_ - The button ID to check.
- `controller`: _`integer`_ - The controller index.

## Return Values

- `state`: _`boolean`_ - Returns true if the button was just pressed this frame, false otherwise.

## Example

Creates Russell ped in front of the player and sets his HP to 30.

```lua
if IsButtonBeingPressed(0, 0) then
	local x, y, z = PedGetOffsetInWorldCoords(gPlayer, 0, 1, 0)
	local Russell = PedCreateXYZ(75, x, y, z)
	PedSetHealth(Russell, 30)
end
```

## See Also

- Game's Native
  - [`IsButtonBeingReleased`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/IsButtonBeingReleased)
  - [`IsButtonPressed`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/IsButtonPressed)

