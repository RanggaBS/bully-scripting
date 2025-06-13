---
description: Register a localized text entry with a custom label and length.
sidebar_class_name: hidden
---

# RegisterLocalizedText

> **_This function was added in DSL 4_**

## Description

:::warning
Localized text functions are considered experimental, and may not work reliably.

Do not use a label that already exists within the base game.
:::

Register a localized text entry with a custom `label` and a pre-determined maximum `length` within the game's localized text.

You can call this function as often as you like, but text can only be registered once. If `label` was already registered to have a smaller length, then this function will fail. If it was already registered to be the same length or bigger, then the function will just do nothing.

```lua
function RegisterLocalizedText(label, length) --[[ ... ]] end
```

## Parameters

- `label`: _`string`_ - The label to register. This is the key that will be used to retrieve the localized text.
- `length`: _`integer`_ - The maximum length of the localized text. This is the maximum number of characters that can be stored for this label.

## Return Values

None.

## Example

Print the target ped's name using [`TextPrint`](/docs/game-reference/global-functions/TextPrint).

```lua
RegisterLocalizedText('TARGET_PED_NAME', 100)

function main()
  while not SystemIsReady() do
    Wait(0)
  end
  while true do
    local target = PedGetTargetPed(gPlayer)
    if PedIsValid(target) then
      ReplaceLocalizedText('TARGET_PED_NAME', PedGetName(target))
      TextPrint('TARGET_PED_NAME', 0, 1)
    end
    Wait(0)
  end
end
```

## See Also

- DSL
  - [`GetLocalizedText`](./GetLocalizedText)
  - [`ReplaceLocalizedText`](./ReplaceLocalizedText)
  - [`TextPrint`](/docs/game-reference/global-functions/TextPrint)
