---
description: Fades the camera (screen) in or out over a specified duration.
sidebar_class_name: hidden
---

# CameraFade

## Description

Fades the screen to black or back to the game view.
If the screen remains faded out for a while, a loading screen may appear.

```lua
function CameraFade(duration, state) --[[ ... ]] end
```

## Parameters

- `duration`: _`integer`_ - How long the fade should take, in milliseconds.
- `state`: _`integer`_ - Use 0 to fade out (to black), or 1 to fade in (show the game).

## Return Values

None.

## Example

None.

