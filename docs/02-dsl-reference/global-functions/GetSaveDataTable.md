---
description: Get a save data table by its ID.
sidebar_class_name: hidden
---

# GetSaveDataTable

> **_This function was added in DSL 1_**

## Description

Get a _save data table_ given a _`saveDataID`_. If one does not exist, an empty one will be generated. The same restrictions apply to the table as with tables packed using [`PackTable`](./PackTable).

Save data can only be assumed to be ready by the time the first [**`GAME`** thread](/docs/dsl-reference/basic-concepts/scripts#thread-types) runs. This basically means that you shouldn't get save data until your script's `MissionSetup` or `main` function.

All modifications you make to your _save data table_ will be saved in the normal file used to save game progress, giving you a way to save things that should be tied to the playthrough.

:::tip
_`saveDataID`_ should be unique enough that other developers are not likely to use it by mistake. Prefixing it with your username is often a good way to avoid conflicts.
:::

```lua
function GetSaveDataTable(saveDataID) --[[ ... ]] end
```

## Parameters

- `saveDataID`: _`string`_ - The ID of the save data table to get. This is case-sensitive and must match the ID used when saving the data.

## Return Values

- `saveData`: _`table`_ - The save data table associated with the given ID. If it does not exist, an empty table will be returned.

## Versions

- **DSL 4** - Save data is now more reliable, and accurately reports when it is not ready.

## Example

```lua
local mySaveData = GetSaveDataTable('myUniqueSaveDataID')
mySaveData.myValue = 42 -- Set a value in the save data table
```

Remember how many apples Jimmy eats and show it to the player at all times.

```lua
-- _derpy_script_loader/scripts/remember_apples.lua

function MissionSetup()
  gSaveData = GetSaveDataTable('test_saving_system')
end

function main()
  local eating = false

  while not SystemIsReady() do
    Wait(0)
  end

  -- make an initial value for our apple count if one does not exist in our save data table
  if not gSaveData.apples then
    gSaveData.apples = 0
  end

  while true do
    if PedMePlaying(gPlayer, 'EatDirect', true) and PedGetWeapon(gPlayer) == 310 then
      eating = true -- remember that we started eating so we can increment our count when we're done eating
    elseif eating then
      eating = false
      -- increment our apple count (since we're editing it in the save table, it will save with the game)
      gSaveData.apples = gSaveData.apples + 1
    end
    drawText('[saving example]\nJimmy has consumed ' .. gSaveData.apples .. ' apples.')
    Wait(0)
  end
end

function drawText(text)
  SetTextFont('Georgia')
  SetTextBold()
  SetTextShadow()
  SetTextScale(1.2)
  SetTextPosition(0.5, 0.9)
  SetTextColor(191, 191, 191, 255)
  DrawText(text)
end
```
