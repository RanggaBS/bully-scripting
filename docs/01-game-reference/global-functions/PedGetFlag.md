---
description: ...
sidebar_class_name: hidden
---

# PedGetFlag

## Description

Returns the current state of a given flag of ped.

```lua
function PedGetFlag(ped, flag) --[[ ... ]] end
```

## Parameters

- `ped`: _`integer`_ - The ped to get the flag state of.
- `flag`: _`integer`_ - The flag to get the state of.

## Return Values

- `flag`: _`boolean`_ - The state of the flag.

## Example

Check if the locked-on ped is strafing.

```lua
while true do
    Wait(0)
    local targ = PedGetTargetPed(gPlayer)
    if PedIsValid(targ) then
        if PedGetFlag(PedGetTargetPed(gPlayer), 11, true) then
            TextPrintString("Target Ped is strafing.", 0, 1)
        else
            TextPrintString("Target Ped is not strafing.", 0, 1)
        end
    else
        TextPrintString("No Target Ped detected.", 0, 1)
    end
end
```

