---
description: Replace localized text with new text.
sidebar_class_name: hidden
---

# ReplaceLocalizedText

> **_This function was added in DSL 4_**

## Description

:::warning
Localized text functions are considered experimental, and may not work reliably.
:::

Replace localized text with new text.

This can be used with text that exists in the base game, or with text registered using [`RegisterLocalizedText`](RegisterLocalizedText). Text made by the base game is not always loaded until it is needed. You may have to take extra care to wait for certain text to be loaded before replacing it.

```lua
function ReplaceLocalizedText(label, text) --[[ ... ]] end
```

## Parameters

- `label`: _`string`_ - The label of the localized text to replace. This should match a label registered with [`RegisterLocalizedText`](RegisterLocalizedText) or an existing base game label.
- `text`: _`string`_ - The new text to replace the localized text with. This should be a string that fits within the constraints of the label's length.

## Return Values

None.

## Example

```lua
ReplaceLocalizedText('EXAMPLE_LABEL', 'This is the new localized text.')
```

## See Also

- DSL
  - [`GetLocalizedText`](./GetLocalizedText)
  - [`ReplaceLocalizedText`](./ReplaceLocalizedText)
  - [`TextPrint`](/docs/game-reference/global-functions/TextPrint)
