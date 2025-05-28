---
description: Gets the current in-game time.
sidebar_class_name: hidden
---

# ClockGet

## Description

Returns the current in-game time as hours and minutes.

```lua
function ClockGet() --[[ ... ]] end
```

## Parameters

None.

## Return Values

- `hour`: _`integer`_ - Current in-game hour.
- `minute`: _`integer`_ - Current in-game minute.

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

