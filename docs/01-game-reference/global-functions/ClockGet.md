---
description: Gets the current time.
sidebar_class_name: hidden
---

# ClockGet

## Description

...

```lua
function ClockGet() --[[ ... ]] end
```

## Parameters

None.

## Return Values

- `hour`: _`number`_ - Current in-game hour.
- `minute`: _`number`_ - Current in-game minute.

## Example

Constantly print the current in-game time.

```lua
local ClockH, ClockM

	while true do
		ClockH, ClockM = ClockGet()
		TextPrintString("It is currently "..ClockH..":"..ClockM, 0, 1)
		Wait(0)
	end
```

