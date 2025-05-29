---
description: Check if a button was JUST released this frame.
sidebar_class_name: hidden
---

# IsButtonBeingReleased

## Description

Use this to trigger actions only once per button release, rather than while it is up.
Check [`here`](https://bully-scripting.vercel.app/docs/game-reference/scripting-enumeration/controls) for more info about the button ID and the controller ID.

```lua
function IsButtonBeingReleased(button, controller) --[[ ... ]] end
```

## Parameters

- `button`: _`integer`_ - The button ID to check.
- `controller`: _`integer`_ - The controller index.

## Return Values

- `state`: _`boolean`_ - Returns true if the button was just released this frame, false otherwise.

## Example

```lua
function main()
    print("Hold down Space Bar to spawn a character...")
    
    while true do
        if IsButtonBeingReleased("8", 0) then
            SpawnCharacterInFrontOfPlayer()
        end
        Wait(0)
    end
end

function SpawnCharacterInFrontOfPlayer()
    -- Get position 1 unit in front of the player
    local x, y, z = PedGetOffsetInWorldCoords(gPlayer, 0, 1, 0)
    
    -- Create a new character at that position
    local character = PedCreateXYZ(75, x, y, z)
    
    -- Set the character's health to 30
    PedSetHealth(character, 30)
end
```

## See Also

- Game's Native
  - [`IsButtonBeingPressed`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/IsButtonBeingPressed)
  - [`IsButtonPressed`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/IsButtonPressed)