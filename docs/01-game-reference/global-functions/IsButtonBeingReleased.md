---
description: Check if a button was JUST released this frame.
sidebar_class_name: hidden
---

# IsButtonBeingReleased

## Description

Use this to trigger actions only once per button release, rather than while it is up.

```lua
function IsButtonBeingReleased(button, controller) --[[ ... ]] end
```

## Parameters

- `button`: _`integer`_ - The button ID to check.
- `controller`: _`integer`_ - The controller index.

## Return Values

- `state`: _`boolean`_ - Returns true if the button was just released this frame, false otherwise.

## Example

None.

