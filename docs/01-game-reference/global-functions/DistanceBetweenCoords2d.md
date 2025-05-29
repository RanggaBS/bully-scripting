---
description: Calculates the 2D distance between two points.
sidebar_class_name: hidden
---

# DistanceBetweenCoords2d

## Description

Returns the 2D distance between two coordinate points. Only the X and Y values are considered.

```lua
function DistanceBetweenCoords2d(x1, y1, x2, y2) --[[ ... ]] end
```

## Parameters

- `x1`: _`number`_ - X coordinate of the first point.
- `y1`: _`number`_ - Y coordinate of the first point.
- `x2`: _`number`_ - X coordinate of the second point.
- `y2`: _`number`_ - Y coordinate of the second point.

## Return Values

- `dist`: _`number`_ - The distance between the two points.

## Example

```lua
function main()
    print("Creating character and monitoring distance...")
    
    -- Get position 1 meter in front of the player
    local char_x, char_y, char_z = PedGetOffsetInWorldCoords(gPlayer, 0, 1, 0)
    
    -- Create a character at that position (model ID 75)
    local character = PedCreateXYZ(75, char_x, char_y, char_z)
    
    print("Character created at position: (" .. char_x .. ", " .. char_y .. ", " .. char_z .. ")")
    
    -- Continuous distance monitoring loop
    while true do
        -- Get player's current position
        local player_x, player_y, player_z = PedGetPosXYZ(gPlayer)
        
        -- Get character's current position
        local char_x, char_y, char_z = PedGetPosXYZ(character)
        
        -- Calculate 2D distance between player and character
        local distance = DistanceBetweenCoords2d(player_x, player_y, char_x, char_y)
        
        print("Distance between player and character: " .. string.format("%.2f", distance) .. " meters")
        
        -- Example distance checks
        if distance < 2.0 then
            print("Character is very close to player")
        elseif distance < 5.0 then
            print("Character is nearby")
        else
            print("Character is far from player")
        end
       
        Wait(1000)
    end
end
```

## See Also

- Game's Native
  - [`DistanceBetweenCoords3d`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/DistanceBetweenCoords3d)
