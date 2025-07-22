---
description: ...
sidebar_class_name: hidden
---

# GetTimecycle

_**This function was added in DSL 10**_

## Description

Returns a timecycle object corresponding to the specified hour, season, and weather conditions. A distinct timecycle exists for each combination of hour (0–23), season (0–3), and weather type (0–5). To easily retrieve the current season, you may use the [`SeasonGet`](/docs/dsl-reference/global-functions/SeasonGet) function in conjunction with this function.


The returned object is a reference to the actual timecycle data. Therefore, any modifications made to this object will take an immediate effect to the game. If you intend to configure a timecycle without applying the changes instantly, you can copy the timecycle using the [`CopyTimecycle`](/docs/dsl-reference/global-functions/CopyTimecycle) function or create a new one using the [`CreateTimecycle`](/docs/dsl-reference/global-functions/CreateTimecycle) function.


Some fields within the timecycle structure are color values, represented as `tc_color` objects. These can be modified either by assigning a table containing RGB values (e.g., `tc.Amb_World = {255, 255, 255}`) or by indexing the color object directly (e.g., `tc.Amb_World.r = 255`).


Timecycle Fields:
| Name            | Description               |
|-----------------|---------------------------|
| Amb_Props       | `tc_color`                |
| Amb_World       | `tc_color`                |
| Amb_Peds        | `tc_color`                |
| SunRGB          | `tc_color`                |
| Back            | `tc_color`                |
| BackInt         | `float`                   |
| NightFactor     | `float`                   |
| lowcloudsRGB    | `tc_color` [0.0, 1.0]     |
| TopCloudRGB     | `tc_color`                |
| BottomCloudRGB  | `tc_color`                |
| GlowThresh      | `integer`                 |
| GlowStrength    | `integer`                 |
| SKYTOP          | `tc_color`                |
| Skybot          | `tc_color`                |
| SunRGBcore      | `tc_color`                |
| SunRGBcorona    | `tc_color`                |
| SunRGBsz        | `float`                   |
| Sprsz           | `float`                   |
| Sprbrght        | `float`                   |
| Shdw            | `integer`                 |
| Lightshd        | `float`                   |
| Poleshd         | `float`                   |
| Farclip         | `integer`                 |
| Fogst           | `integer`                 |
| Unknown1        | `integer`                 |
| Unknown2        | `integer`                 |
| CloudSpeed      | `float`                   |
| CloudTopRGB     | `tc_color`                |
| CloudBotRGB     | `tc_color`                |
| ColFilterMode   | `integer`                 |
| ColFilterRGBA   | `tc_color` with alpha     |
| AmbLRange       | `float`                   |
| AmbHRange       | `float`                   |
| SunLRange       | `float`                   |
| SunHRange       | `float`                   |
| BackLRange      | `float`                   |
| BackHRange      | `float`                   |
| NearFarRatio    | `integer`                 |


```lua
function GetTimecycle(hour, season, weather) --[[ ... ]] end
```

## Parameters

`hour`: _`number`_ - An integer value ranging from 0 to 23.
`season`: _`number`_ - An integer value ranging from 0 to 3.
`weather`: _`number`_ - An integer value ranging from 0 to 5.

## Return Values

`timecycle`: _`userdata`_ - A timecycle userdata.

## Example

Instantly changes the current cloud speed:
```lua
local TC = GetTimecycle(ClockGet(), SeasonGet(), WeatherGet())
TC.CloudSpeed = 1.2
```

Turns the game into eternal night:
```lua
-- Arg/Param 1: 2 --> means 2 AM
-- Arg/Param 2: 0 --> means Summer
-- Arg/Param 3: 4 --> means Normal
local TC = CopyTimecycle(GetTimecycle(2, 0, 4))

-- Apply the same timecycle to all hours, seasons, and weather conditions (exterior only)
for Hour = 0, 23 do
  for Season = 0, 3 do
    for Weather = 0, 5 do
      SetTimecycle(Hour, Season, Weather, TC)
    end
  end
end
```
