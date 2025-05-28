---
description: Returns the ID of the currently active camera mode.
sidebar_class_name: hidden
---

# CameraGetActive

## Description

Returns which camera mode is currently active. Possible return values:

1: Normal camera

2: First person

3: Black screen

4: Script camera (started by [**CameraSetXYZ**](https://bully-scripting.vercel.app/docs/game-reference/global-functions/CameraSetXYZ))

5-8: Invalid or useless modes

9: Similar to normal camera but positioned lower

10: Static camera (remains fixed where set)

11: Nothing

12: Causes crash

13: Shoulder view

14: Top down view

```lua
function CameraGetActive() --[[ ... ]] end
```

## Parameters

None.

## Return Values

- `camera`: _`integer`_ - The currently active camera ID.

## Example

None.

