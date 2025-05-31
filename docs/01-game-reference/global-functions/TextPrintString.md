---
description: ...
sidebar_class_name: hidden
---

# TextPrintString

## Description

Prints non-localised text on the screen.
<br/>Every game version other than PS2 prints text in red regardless of style.

:::info

- **(DSL 10)** style now follows PS2 colours.

:::

```lua
function TextPrintString(text, duration, style) --[[ ... ]] end
```

## Parameters

- `text`: _`string`_ - The text to be drawn.
- `duration`: _`number`_ - Text duration, in seconds.
- `style`: _`1|2`_ - The style of the text:
  - _`1`_: Objective style (yellow text, top-center)
  - _`2`_: Subtitle style (white text, small, bottom-center)

## Return Values

...

## Example

Displays "Hello, world!" for 5 seconds in objective style

```lua
TextPrintString('Hello, world!', 5, 1)
```

