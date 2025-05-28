---
description: Checks if a ped has line of sight to an object or ped.
sidebar_class_name: hidden
---

# PedCanSeeObject

## Description

...

```lua
function PedCanSeeObject(ped, object, visionType) --[[ ... ]] end
```

## Parameters

- `ped`: _`integer`_ - The ped performing the vision check.
- `object`: _`integer`_ - The object or ped to be checked for visibility.
- `visionType`: _`integer`_ - The type of vision check. 2 is most commonly used, but this has something to do with how sight is checked.

## Return Values

- `state`: _`boolean`_ - Returns true if the ped can see the object, otherwise false.

## Example

None.

