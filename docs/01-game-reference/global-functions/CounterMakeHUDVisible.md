---
description: ...
sidebar_class_name: hidden
---

# CounterMakeHUDVisible

## Description

Turns on the counter at the bottom-right of the screen.
<br/>By default, the max amount is set to 10 unless overriden with [`CounterSetMax`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/CounterSetMax).
<br/>This will override the current state of its visibility, even if previously turned off with [`ToggleHUDComponentVisibility`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/ToggleHUDComponentVisibility).

```lua
function CounterMakeHUDVisible(visibility, maxvisibility) --[[ ... ]] end
```

## Parameters

- `visibility`: _`boolean`_ - Whether to display the counter HUD in general
- `maxvisibility`: _`boolean`_ - Whether to show the maximum value alongside the current count (irrelevant if using [`CounterUseMeter`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/CounterUseMeter))

## Return Values

...

## Example

(Assumes the current max is 10)

```lua
CounterMakeHUDVisible(true, true) -- will display "0/10".
CounterMakeHUDVisible(true, false) -- will display "0".
```

## See Also

- Game's Native
  - [`CounterSetCurrent`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/CounterSetCurrent)
  - [`CounterSetIcon`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/CounterSetIcon)
  - [`CounterSetMax`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/CounterSetMax)
  - [`CounterUseMeter`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/CounterUseMeter)