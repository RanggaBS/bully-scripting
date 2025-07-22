---
description: Resets all timecycles to their original default state.
sidebar_class_name: hidden
---

# RestoreTimecycles

_**This function was added in DSL 10**_

## Description

Resets all timecycles to their original default state, as defined at the beginning of the game session.

```lua
function RestoreTimecycles() --[[ ... ]] end
```

## Parameters

None.

## Return Values

None.

## Example

```lua
while true do
  if IsKeyBeingPressed('T') then
    SetAllTimecycles(CopyTimecycle(GetTimecycle(2, 0, 4)))
  elseif IsKeyBeingPressed('Y') then
    RestoreTimecycles()
  end

  DrawTextInline('[T] Apply | [Y] Restore', 0, 2)
  Wait(0)
end

```

