---
description: Gets the current season.
sidebar_class_name: hidden
---

# SeasonGet

_**This function was added in DSL 10**_

## Description

Gets the current season, primarily used by timecycle functions.

```lua
function SeasonGet() --[[ ... ]] end
```

## Parameters

None.

## Return Values

`season`: _`number`_

| Number | Season          |
| ------ | ----------------|
| 0      | Summer          |
| 1      | Autumn          |
| 2      | Winter          |
| 3      | Spring          |


## Example

```lua
local TC = GetTimecycle(ClockGet(), SeasonGet(), WeatherGet())
if type2(TC) == 'timecycle' then
  -- do something
end
```

