---
description: Sets timecycle object to all the available timecycles.
sidebar_class_name: hidden
---

# SetAllTimecycles

_**This function was added in DSL 10**_

## Description

Applies the given timecycle object to all available timecycles, making the game's atmosphere look even across all times, seasons, and weather conditions. This function is generally not recommended for typical use, as it can significantly disrupt the visual consistency of both interior and exterior environments. Unless the timecycles are later restored using [`RestoreTimecycles`](/docs/dsl-reference/global-functions/RestoreTimecycles).


If your intention is to modify a specific timecycle, consider using [`SetTimecycle`](/docs/dsl-reference/global-functions/SetTimecycle) or [`SetExtraTimecycle`](/docs/dsl-reference/global-functions/SetExtraTimecycle) instead.

:::info
A timecycle object (_**userdata**_) can be obtained from the following functions:
- [`GetTimecycle`](/docs/dsl-reference/global-functions/GetTimecycle)
- [`GetExtraTimecycle`](/docs/dsl-reference/global-functions/GetExtraTimecycle)
- [`CopyTimecycle`](/docs/dsl-reference/global-functions/CopyTimecycle)
- [`CreateTimecycle`](/docs/dsl-reference/global-functions/CreateTimecycle)
:::


```lua
function SetAllTimecycles(timecycle) --[[ ... ]] end
```

## Parameters

- `timecycle`: _`userdata`_ - A timecycle object.

## Return Values

None.

## Example

```lua
local TC = CopyTimecycle(GetTimecycle(ClockGet(), SeasonGet(), WeatherGet()))
SetAllTimecycles(TC)
```

