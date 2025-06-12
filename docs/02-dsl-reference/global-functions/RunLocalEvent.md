---
description: Run a local event with the given type and arguments.
sidebar_class_name: hidden
---

# RunLocalEvent

> **_This function was added in DSL 4_**

## Description

Activate an event of `type`, passing any `arguments` you want.

:::tip
Keep in mind that tables in Lua are passed by reference, so a decent strategy for allowing other scripts to respond to your event is by passing some sort of table.
:::

The `result` is `false` unless at least one of the callbacks return true. This can be used as a way of letting certain events be cancelled, or for any other arbitrary use.

```lua
function RunLocalEvent(type, ...) --[[ ... ]] end
```

## Parameters

- `type`: _`string`_ - The type of the event to run. This is usually a string that identifies the event.
- `...`: _`any`_ - Any number of arguments to pass to the event. These can be any Lua values, including tables, numbers, strings, etc.

## Return Values

- `result`: _`boolean`_ - Returns `true` if at least one of the callbacks for the event returned `true`, otherwise returns `false`.

## Example

```lua
RegisterLocalEventHandler('MyMod:MyEvent', function(arg1, arg2)
  print('MyMod:MyEvent was triggered with arguments:', arg1, arg2)
  return true -- Indicate that the event was handled
end)
-- highlight-next-line
RunLocalEvent('MyMod:MyEvent', 'Hello', 42)
```

## See Also

- DSL
  - [`RegisterLocalEventHandler`](./RegisterLocalEventHandler)
