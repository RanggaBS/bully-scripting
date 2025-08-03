---
description: Returns the local player's username from their configuration.
sidebar_class_name: hidden
---

# GetPlayerName

## Description

Returns the local player's username, as set in their config. If there is no valid username set, "player" is returned. This function is useful for personalizing script output or identifying the player in multiplayer scenarios.

```lua
function GetPlayerName() --[[ ... ]] end
```

## Parameters

None.

## Return Values

- `name` - _`string`_ - Returns the player's username from their configuration, or "player" if no valid username is set.

## Example

```lua
-- Get and display the player's name
local playerName = GetPlayerName()
print("Welcome, " .. playerName .. "!")

-- Use in personalized messages
local name = GetPlayerName()
DrawTextInline("Hello ~g~" .. name .. "~w~, enjoy the game!", 3.0, 1)

-- Use for save data organization
local playerData = GetSaveDataTable(GetPlayerName() .. "_progress")
playerData.level = (playerData.level or 0) + 1
print(GetPlayerName() .. " is now level " .. playerData.level)
```

## See Also

- DSL
  - [`GetPlayerIp`](./GetPlayerIp)