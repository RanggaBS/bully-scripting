---
description: Copies an existing timecycle object.
sidebar_class_name: hidden
---

# CopyTimecycle

_**This function was added in DSL 10**_

## Description

Creates a new timecycle object by copying all fields and values from an existing one. This function is useful when you need an isolated copy of a timecycle object that won't be affected by changes in other scripts, or when you want to create a backup of a specific timecycle for later use.

```lua
function CopyTimecycle(timecycle) --[[ ... ]] end
```

## Parameters

- `timecycle`: _`userdata`_ - A timecycle object.

## Return Values

- `a copy of timecycle`: _`userdata`_ - A timecycle object.

## Example

Script 1:
```lua
local Hour = ClockGet()
local TC = CopyTimecycle(GetTimecycle(Hour, SeasonGet(), WeatherGet()))
while true do
  ClockSet(Hour)
  
  DrawTextInline('~xy~- SCRIPT 1 -\nFogst: '..TC.Fogst, 0.25, 0.5, 0, 2)
  Wait(0)
end
```

Script 2:
```lua
local Hour = ClockGet()
while true do
  ClockSet(Hour)
  local TC = GetTimecycle(Hour, SeasonGet(), WeatherGet())
  if TC.Fogst ~= -400 then
    TC.Fogst = -400
  end

  DrawTextInline('~xy~- SCRIPT 2 -\nFogst: '..TC.Fogst, 0.75, 0.5, 0, 2)
  Wait(0)
end
```
