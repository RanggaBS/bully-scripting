---
description: Returns the value of GetTickCount, primarily intended for use with math.randomseed to improve the random number generator.
sidebar_class_name: hidden
---

# GetSystemTimer

> **_This function was added in DSL 4_**

## Description

Returns the value of [`GetTickCount`](https://learn.microsoft.com/en-us/windows/win32/api/sysinfoapi/nf-sysinfoapi-gettickcount), primarily intended for use with `math.randomseed` to improve the random number generator.

Retrieves the number of milliseconds that have elapsed since the system was started, up to 49.7 days.

```lua
function GetSystemTimer() --[[ ... ]] end
```

## Parameters

None.

## Return Values

The return value is the number of milliseconds that have elapsed since the system was started.

- `tickCount`: _`number`_ - The value of `GetTickCount`, which is the number of milliseconds since the system started.

## Example

```lua
function main()
  -- Seed the random number generator with the current system timer
  math.randomseed(GetSystemTimer())

  -- Generate a random number between 1 and 100
  local randomNumber = math.random(1, 100)

  print('Random Number: ' .. randomNumber)
end
```
