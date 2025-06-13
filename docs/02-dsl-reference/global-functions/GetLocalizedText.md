---
description: Return the localized `text` associated with a certain `label`.
sidebar_class_name: hidden
---

# GetLocalizedText

> **_This function was added in DSL 5_**

## Description

Return the localized `text` associated with a certain `label`.

```lua
function GetLocalizedText(label) --[[ ... ]] end
```

## Parameters

- `label`: _`string`_ - The label to look up in the localization files. This is typically a key that corresponds to a specific text string in the localization system.

## Return Values

- `text`: _`string | ' '`_ - The localized text associated with the provided label. If the label does not exist, it returns a space character (`' '`).

## Example

```lua
local text = GetLocalizedText('EXAMPLE_LABEL')
if text ~= ' ' then
  print('Localized text: ' .. text)
else
  print('Label not found.')
end
```

## See Also

- DSL
  - [`GetLocalizedText`](./GetLocalizedText)
  - [`ReplaceLocalizedText`](./ReplaceLocalizedText)
  - [`TextPrint`](/docs/game-reference/global-functions/TextPrint)
