---
description: Returns how long the server has been running in milliseconds.
sidebar_class_name: hidden
---

# GetTimer

> **_This function was added in DSL 5_**

## Description

This function is not defined on the client, so the normal [`GetTimer`](/docs/game-reference/global-functions/GetTimer) will be used instead.

On the server, this function **returns how long the server has been running in milliseconds** to copy the client behavior.

```lua
function GetTimer() --[[ ... ]] end
```

## Parameters

None.

## Return Values

- `milliseconds`: _`number`_ - The number of milliseconds since the server started.

## Example

```lua
function main()
  while not SystemIsReady() do
    Wait(0)
  end

  print('Server has been running for ' .. GetTimer() .. ' milliseconds.')
end
```
