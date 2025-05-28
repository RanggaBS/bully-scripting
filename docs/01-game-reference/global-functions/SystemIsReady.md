---
description: Checks if the game is ready for most forms of scripting.
sidebar_class_name: hidden
---

# SystemIsReady

## Description

This is very important in any script that runs as soon as the game starts, and you should wait until it returns true before doing most things. In a few cases, you may find it necessary to wait an additional second after the system is ready.

```lua
function SystemIsReady() --[[ ... ]] end
```

## Parameters

None.

## Return Values

- `state`: _`boolean` - System ready state.

## Example

Wait for the system to be ready before any other code.

```lua
while not SystemIsReady() do
	Wait(0)
end
-- actual stuff you want to do here
```

Move the player outside when it is safe to do so.

```lua
if not SystemIsReady() then -- check if we need to wait for the system at all (won't be the case if the script started late)
	repeat
		Wait(0)
	until SystemIsReady() and AreaIsLoading()
	Wait(1000) -- an extra second for safety
end
while AreaIsLoading() do -- in case the area started switching during the wait, or was already switching without the wait
	Wait(0)
end
PlayerSetPosXYZArea(270, -110, 6, 0)
```

