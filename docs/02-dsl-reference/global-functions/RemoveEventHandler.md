---
description: Remove an event handler created with `RegisterLocalEventHandler`.
sidebar_class_name: hidden
---

# RemoveEventHandler

## Description

Remove an event handler created with [`RegisterLocalEventHandler`](RegisterLocalEventHandler).

```lua
function RemoveEventHandler(eventHandler) --[[ ... ]] end
```

## Parameters

- `eventHandler`: _`userdata`_ - The event handler to remove. This is the return value of [`RegisterLocalEventHandler`](RegisterLocalEventHandler).

## Return Values

None.

## Example

```lua
function main()
  local eventHandler = RegisterLocalEventHandler("example:notifyPlayerDeath", function(name)
    TextPrintString(name.." has died!", 3, 2)
  end)

  -- Do something...

  -- Remove the event handler when no longer needed
  -- highlight-next-line
  RemoveEventHandler(eventHandler)
end
```

## See Also

- DSL
  - [`RegisterLocalEventHandler`](RegisterLocalEventHandler)
  - [`RegisterNetworkEventHandler`](RegisterNetworkEventHandler)
