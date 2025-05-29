---
description: Check if a button is simply pressed.
sidebar_class_name: hidden
---

# IsButtonPressed

## Description

Returns true when the button is pressed and while it is held.
Check [`here`](https://bully-scripting.vercel.app/docs/game-reference/scripting-enumeration/controls) for more info about the button ID and the controller ID.

```lua
function IsButtonPressed(button, controller) --[[ ... ]] end
```

## Parameters

- `button`: _`integer`_ - The button ID to check.
- `controller`: _`integer`_ - The controller index.

## Return Values

- `state`: _`boolean`_ - Returns true if the button is currently pressed, false otherwise.

## Example

function main()
    print("Press and hold Space Bar to start counting...")
    local counter = 0
    
    while true do
        if IsButtonPressed(8, 0) then
            counter = counter + 1
            print("Count: " .. counter)
            Wait(100)  -- Wait 100ms between counts
        else
            if counter > 0 then
                print("Final count: " .. counter)
                counter = 0  -- Reset counter when button is released
            end
            Wait(0)
        end
    end
end

## See Also

- Game's Native
  - [`IsButtonBeingReleased`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/IsButtonBeingReleased)
  - [`IsButtonBeingPressed`](https://bully-scripting.vercel.app/docs/game-reference/global-functions/IsButtonBeingPressed)