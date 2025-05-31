---
description: Draws text on the screen in a specified style for a given duration.
sidebar_class_name: hidden
---

# DrawTextInline

> **_This function was added in DSL 1_**

## Description

Draws text on the screen in a specified style for a given duration.

This function is useful for displaying temporary messages or objectives to the player.

```lua
function DrawTextInline(text, duration, style) --[[ ... ]] end
```

## Parameters

- `text`: _`string`_ - The text to be drawn.
- `duration`: _`number`_ - The duration for which the text should be displayed, in seconds.
- `style`: _`1|2`_ - The style of the text:
  - _`1`_: Objective style (yellow text, top-center)
  - _`2`_: Subtitle style (white text, small, bottom-center)

## Return Values

None.

## Example

Displays "Hello, world!" for 5 seconds in objective style

```lua
DrawTextInline('Hello, world!', 5, 1)
```

## See Also

- Game's Native
  - [`TextPrintString`](../../game-reference/global-functions/TextPrintString)
