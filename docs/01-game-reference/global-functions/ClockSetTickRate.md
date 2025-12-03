---
description: Controls the speed at which the game clock advances, allowing you to speed up or slow down the passage of time in the game.
sidebar_class_name: hidden
---

# ClockSetTickRate

## Description

Controls the rate at which the in-game clock advances. This function allows you to speed up or slow down the passage of time in Bully: Scholarship Edition. The default game speed is 1 game minute per 1 real second (60 game minutes per real minute).
```lua
function ClockSetTickRate(gameMinutesPerRealMinute, unknown) --[[ ... ]] end
```

## Parameters

* `gameMinutesPerRealMinute`: `number` - The number of game minutes that should pass for each real-world minute. Default is 60.
  - `60` = Normal speed (1 game minute per real second)
  - `120` = 2x speed (2 game minutes per real second)
  - `300` = 5x speed (5 game minutes per real second)
  - `30` = Half speed (0.5 game minutes per real second)

* `unknown`: `number` - Purpose unknown. The game scripts use `30` as the standard value. Further testing needed to determine its effect.

## Return Values

None.

## Example
```lua
-- Speed up time to 5x normal speed (5 game hours pass per real minute)
function main()
    ClockSetTickRate(300, 30)
    
    while true do
        Wait(0)
    end
end
```
```lua
-- Slow down time to half speed
function main()
    ClockSetTickRate(30, 30)
    
    while true do
        Wait(0)
    end
end
```
```lua
-- Example from game's decompiled scripts (normal speed)
function F_LoadTime()
    ClockSet(8, 0)
    WeatherSet(0)
    WeatherRelease()
    ClockSetTickRate(60, 30)  -- Set to normal game speed
end
```

## Notes

- Setting the first parameter to values significantly higher than 60 may cause time to advance too quickly for gameplay.
- Setting it too low (below 10) may cause time to appear frozen or advance extremely slowly.
- The second parameter's purpose is currently undocumented. Standard game scripts consistently use `30`.
- This function can be called at any time during gameplay to dynamically adjust time speed.
