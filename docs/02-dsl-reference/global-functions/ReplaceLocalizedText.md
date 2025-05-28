---
description: Replaces a localized text entry with a string.
sidebar_class_name: hidden
---

# ReplaceLocalizedText

## Description

Replaces a localized text entry with a new string. If the replacement string is too long, it will not be copied over in full. If no replacement string is given, the function simply returns the maximum allowed length for that entry.

```lua
function ReplaceLocalizedText(entry,replacement) --[[ ... ]] end
```

## Parameters

- `entry`: _`string`_ - The name of the localized text entry to replace.
- `replacement`: _`string`_ - The new string to set for this entry. Optional; if omitted, no replacement is done.

## Return Values

- `lenght`: _`number`_ - Returns the maximum allowed length of the string for the given entry.

Returns nil if the localized string was not found or is not loaded.

## Example

None.

