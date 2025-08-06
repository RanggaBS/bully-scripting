---
description: Gets the time elapsed since the last frame in seconds, useful for frame rate independent movement and animations.
sidebar_class_name: hidden
---

# GetFrameTime

> **_This function was added in DSL 1_**

## Description

Returns the amount of time that has passed since the last frame in seconds - delta time.

Gets the time elapsed since the last frame in seconds, useful for frame rate independent movement and animations.

```lua
function GetFrameTime() --[[ ... ]] end
```

## Parameters

None.

## Return Values

- `frameTime`: _`number`_ - The amount of time that has passed since the last frame in seconds.

## Example

Use frame time to move forward at 3 meters per second when a button is pressed, regardless of frame rate.

```lua
function main()
  while not SystemIsReady() do
    Wait(0)
  end
  while true do
    if IsButtonPressed(3, 0) then
      local h, x, y, z = PedGetHeading(gPlayer), PlayerGetPosXYZ()

      -- multiply the distance that we move by the frame time, so we only move
      -- that many units per second
      -- highlight-next-line
      local distance = 3 * GetFrameTime()

      local newX = x - distance * math.sin(h)
      local newY = y + distance * math.cos(h)
      PlayerSetPosSimple(newX, newY, z)
    end
    Wait(0)
  end
end
```

## See Also

- Game's Native
  - [`IsButtonPressed`](/docs/game-reference/global-functions/IsButtonPressed)
  - [`PedGetHeading`](/docs/game-reference/global-functions/PedGetHeading)
  - [`PlayerGetPosXYZ`](/docs/game-reference/global-functions/PlayerGetPosXYZ)
  - [`PlayerSetPosSimple`](/docs/game-reference/global-functions/PlayerSetPosSimple)
  - [`SystemIsReady`](/docs/game-reference/global-functions/SystemIsReady)
