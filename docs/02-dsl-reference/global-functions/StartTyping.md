---
description: Start allowing keyboard input that can be retrieved using `GetTypingString`.
sidebar_class_name: hidden
---

# StartTyping

> **_This function was added in DSL 1_**

## Description

Start allowing keyboard input that can be retrieved using [`GetTypingString`](GetTypingString).

If typing was already active, then this function will return `false`.

```lua
function StartTyping(initial) --[[ ... ]] end
```

## Parameters

- `initial`: _`string?`_ - (Optional) The initial string to set as the starting point for typing. If not provided, it defaults to an empty string.

:::info
**DSL7** - The optional `initial` argument can put some text in the string to begin with.
:::

## Return Values

- `started`: _`boolean`_ - Returns _`true`_ if typing was successfully started, otherwise _`false`_ if typing was already active.

## Example

Start a mission when a button is pressed.

```lua
function main()
  while not SystemIsReady() do
    Wait(0)
  end
  while true do
    -- Arrow down to start typing
    if IsButtonBeingPressed(3, 0) and StartTyping() then
      while IsTypingActive() do
        TextPrintString('Start mission: ' .. GetTypingString(), 0, 1)
        Wait(0)
      end
      if not WasTypingAborted() then
        ForceStartMission(GetTypingString())
      end
    end
    Wait(0)
  end
end
```

## See Also

- DSL
  - [`GetTypingString`](GetTypingString)
