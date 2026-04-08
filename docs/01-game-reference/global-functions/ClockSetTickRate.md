---
description: Controls the speed at which the game clock advances, allowing you to speed up or slow down the passage of time in the game.
sidebar_class_name: hidden
---
# ClockSetTickRate
## Description
Controls the rate at which the in-game clock advances. This function allows you to speed up or slow down the passage of time in Bully: Scholarship Edition.

**Important:** This function exhibits non-linear behavior with discrete speed tiers rather than direct multipliers. The relationship between parameters and actual time speed is complex and may not behave as intuitively expected.
```lua
function ClockSetTickRate(speedParam, requiredParam) --[[ ... ]] end
```

## Parameters
* `speedParam`: `number` - Speed control parameter (higher values generally = faster time)
  - Must be greater than `requiredParam` for reliable behavior
  - If equal to or less than `requiredParam`, clock may freeze or behave unpredictably
  - See "Tested Speed Values" below for reliable configurations
  
* `requiredParam`: `number` - Required parameter with unknown exact purpose
  - Game scripts consistently use `30` as the standard value
  - Acts as a threshold: `speedParam` should significantly exceed this value
  - Setting `speedParam = requiredParam` typically freezes the clock

## Return Values
None.

## Tested Speed Values
Based on systematic testing, these configurations produce reliable results:

| Configuration | Observed Behavior | Notes |
|--------------|-------------------|-------|
| `(60, 30)` | Inconsistent/Frozen | Despite appearing in game scripts, unreliable in testing |
| `(120, 30)` | ~12 game min/real sec | Slower than expected |
| `(300, 30)` | ~36 game min/real sec | Moderate speed |
| `(600, 30)` | ~42 game min/real sec | Fast time progression |
| `(1000, 30)` | ~48 game min/real sec | Very fast time progression |

**Note:** The engine uses discrete speed tiers, not linear scaling. Values between tiers may produce identical speeds.

## Examples

### Basic Usage
```lua
-- Fast time progression (recommended for testing)
function main()
    Wait(1000)  -- Let game initialize
    ClockSetTickRate(600, 30)
    print("Time set to fast mode")
    
    while true do
        Wait(0)
    end
end
```

### Dynamic Time Control
```lua
-- Speed up time during specific hours
function main()
    while true do
        local hour = ClockGet()
        
        if hour >= 23 or hour < 6 then
            -- Fast-forward through night
            ClockSetTickRate(1000, 30)
        else
            -- Normal speed during day
            ClockSetTickRate(300, 30)
        end
        
        Wait(1000)
    end
end
```

### Game Script Example
```lua
-- Example from decompiled game scripts (3_B.lua)
function F_LoadTime()
    ClockSet(8, 0)
    WeatherSet(0)
    WeatherRelease()
    ClockSetTickRate(60, 30)
end
```

### Alternative Single-Parameter Variant
```lua
-- Found in STimeCycle.lua (behavior untested)
ClockSetTickRate(0.006)
```

## Important Notes

### Critical Warnings
- **First parameter must be significantly larger than second parameter** - Equal or close values cause freezing
- **Non-linear behavior** - Speed increases are not proportional to parameter values
- **Context-dependent** - Function may behave differently during missions vs. free roam
- **Testing environment matters** - Results documented from custom mod scripts, not in-mission behavior

### Unknowns & Limitations
- Exact purpose of second parameter remains undocumented
- Formula for speed tier calculation is unknown
- Single-parameter variant (0.006) found in game scripts but behavior untested
- Why game's standard (60, 30) appears frozen in testing but works in game scripts

### Testing Methodology
Results obtained through systematic testing:
1. Set clock to 6:00 AM with `ClockSet(6, 0)`
2. Call `ClockSetTickRate(param1, param2)`
3. Wait exactly 10 real seconds with `Wait(10000)`
4. Measure hours passed with `ClockGet()`

### Recommendations
- **For modding:** Use tested values (300, 600, 1000) with second parameter = 30
- **For safety:** Always keep first parameter significantly larger than 30
- **For debugging:** Use `ClockGet()` and `Wait()` to measure actual time passage
- **Don't assume linear scaling** - Test your specific use case

## Related Functions
- [`ClockGet()`](ClockGet) - Get current game time
- [`ClockSet()`](ClockSet) - Set game time to specific hour/minute
- [`Wait()`](Wait) - Pause script execution

## Test Environment
- **Game:** Bully: Scholarship Edition (Steam)
- **Tool:** Derpy's Script Loader v11.1
- **Context:** Custom mod scripts (non-mission)
- **Date:** Systematic testing conducted December 2024
