---
description: This function was added in DSL 10
sidebar_class_name: hidden
---

# PedGetActionNode

## Description

Captures the current action node of the specified ped.

```lua
function PedGetActionNode(ped, data) --[[ ... ]] end
```

## Parameters

- `ped`: _`number`_ - The ID of the created ped.
- `data`: _`table`_ - A table containing plaintext strings.

:::info
Plaintexts are only required if you want the function to return a readable action node name, as seen in uncompiled .cat files. If not needed, you may leave the data table empty.
:::

## Return Values

`actionNode`: _`string`_ - The current action node in either its plaintext form or as a hash string.

:::info
If a matching plaintext is found for the hash, the function will return it. Otherwise, it will return a string in the format of unknown hash `#XXXXXXXX` (hexadecimal). The hash is still a valid action node and can be used for other purposes.
:::

## Example

Captures the player's current action node and replays it later.
```lua
local Data = {
  'Global', 'Player', 'Default_Key', -- plaintexts
}
local Node = ''
while true do
  -- Capture the current action node when pressing T
  if IsKeyBeingPressed('T') then
    Node = PedGetActionNode(gPlayer, Data)
  end
  
  -- Replay the captured action node when pressing Y
  if string.len(Node) > 0 and IsKeyBeingPressed('Y') then
    ForceActionNode(gPlayer, Node, 'Player.act')
  end
  
  -- Display current status on screen
  DrawTextInline('Node: '..Node..'\n[T] Capture | [Y] Play', 0, 2)
  Wait(0)
end
```
