---
description: Draws text on the screen in a specified style for a given duration.
sidebar_class_name: hidden
---

# DrawTextInline

> **_This function was added in DSL 2_**

## Description

Draws text on the screen with a specified duration, alignment, and formatting. Unlike the [`DrawText`](/docs/dsl-reference/global-functions/DrawText) function, this function allows you to embed all formatting options directly within the string. In contrast, `DrawText` requires you to set each formatting option separately before calling the function.

Format specifiers:
| Specifier         | Description                                                                 |
|-------------------|-----------------------------------------------------------------------------|
| `~b~`             | Makes the text **bold**.                                                    |
| `~i~`             | Makes the text *italic*.                                                    |
| `~xy~`            | Sets the text position. Takes two arguments: `number, number`.              |
| `~scale~`         | Sets the text scale. Takes one argument: `number`.                          |
| `~rgb~`           | Sets the text color using RGB values. Takes three arguments: `number, number, number`. |
| `~alpha~`         | Sets the text transparency (alpha/opacity). Takes one argument: `number`.   |
| `~width~`         | Sets the text width. Takes one argument: `number`.                          |
| `~height~`        | Sets the text height. Takes one argument: `number`.                         |
| `~font~`          | Sets the text font. Takes one argument: `string`.                           |
| `~white~`         | Changes the text color to white.                                            |
| `~yellow~`        | Changes the text color to yellow.                                           |
| `~cyan~`          | Changes the text color to cyan.                                             |
| `~t~` or `~texture~` | Draws a texture. Takes one argument: `userdata`.                         |

:::info
To use multiple specifiers more conveniently, you can combine them with `+` instead of writing each one separately. For example, `~xy~~scale~~font~` can be written as `~xy+scale+font~`.
:::

Pre-defined styles:
| Style | Description                                                                 |
|-------|-----------------------------------------------------------------------------|
| 1     | Displays the text as an objective task (yellow, centered, and at the top).  |
| 2     | Displays the text as a subtitle (white, centered, and at the bottom).       |
| 3     | Aligns the text to the left.                                                |
| 4     | Aligns the text to the right.                                               |
| 5     | Aligns the text to the center.                                              |

```lua
function DrawTextInline(text, [format specifier arguments], duration, style) --[[ ... ]] end
```

## Parameters

- `text`: _`string`_ — The text to be displayed, including any format specifiers.
- `[format specifier arguments]`: _`number`, `string`, or `userdata`_ — Optional arguments, depending on the format specifiers used.
- `duration`: _`number`_ — Duration in seconds for which the text should be displayed.
- `style`: _`number`_ — A pre-defined style index.

## Return Values

None.

## Example

Displays "Hello, world!" for 5 seconds in objective style:
```lua
DrawTextInline('Hello, world!', 5, 1)
```

Displays "Hello, world!" at the top-left of the screen for 5 seconds, with each word shown in a different color:
:::warning
The following code is only an example to demonstrate how format specifiers work. However, using it similarly or exactly as shown may cause a significant performance hit. Use it wisely and only when necessary.
:::
```lua
DrawTextInline('~xy+yellow~Hello~cyan~, ~white~world~rgb~!', 0.1, 0.1, 255, 50, 32, 5, 1)
```

Displays button information for 5 seconds at the bottom-left:
```lua
local Texture = GetHudTexture('Button_Enter')
DrawTextInline('~xy+scale+white+t~ - Enter something.', 0.02, 0.95, 0.8, Texture, 5, 3)
```

## See Also

- Game's Native
  - [`TextPrintString`](/docs/game-reference/global-functions/TextPrintString)
  - [`TextPrint`](/docs/game-reference/global-functions/TextPrint)
