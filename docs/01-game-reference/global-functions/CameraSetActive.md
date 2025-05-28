---
description: Sets the active camera mode.
sidebar_class_name: hidden
---

# CameraSetActive

## Description

Sets the active camera to the specified camera ID.
The ID values correspond to those returned by [**CameraGetActive**](https://bully-scripting.vercel.app/docs/game-reference/global-functions/CameraGetActive).
Note: This will have no effect if camera changes are disabled using [**CameraAllowChange**](https://bully-scripting.vercel.app/docs/game-reference/global-functions/CameraAllowChange).

```lua
function CameraSetActive(cameraId) --[[ ... ]] end
```

## Parameters

- `cameraId`: _`integer`_ - The desired camera ID to activate.

## Return Values

None.

## Example

None.

