---
description: Sets timecycle object to a specific time, season, and weather condition.
sidebar_class_name: hidden
---

# SetTimecycle

_**This function was added in DSL 10**_

## Description

Sets the given timecycle object for a specific hour, season, and weather condition. Unlike the [`SetExtraTimecycle`](/docs/dsl-reference/global-functions/SetExtraTimecycle) function, this function applies the timecycle only to exterior environments, and does not affect interior scenes.

:::info
A timecycle object (_**userdata**_) can be obtained from the following functions:
- [`GetTimecycle`](/docs/dsl-reference/global-functions/GetTimecycle)
- [`GetExtraTimecycle`](/docs/dsl-reference/global-functions/GetExtraTimecycle)
- [`CopyTimecycle`](/docs/dsl-reference/global-functions/CopyTimecycle)
- [`CreateTimecycle`](/docs/dsl-reference/global-functions/CreateTimecycle)
:::


```lua
function SetTimecycle(hour, season, weather, timecycle) --[[ ... ]] end
```

## Parameters

- `hour`: _`number`_ - An integer value ranging from 0 to 23.
- `season`: _`number`_ - An integer value ranging from 0 to 3.
- `weather`: _`number`_ - An integer value ranging from 0 to 5.
- `timecycle`: _`userdata`_ - A timecycle object.

## Return Values

None.

## Example

Applies the current timecycle for the next timecycle.
```lua
local Hour = ClockGet()
local Season = SeasonGet()
local Weather = WeatherGet()

local TC = CopyTimecycle(GetTimecycle(Hour, Season, Weather))
SetTimecycle(Hour + 1, Season, Weather, TC)
```

