---
description: Draws a rectangle on the screen.
sidebar_class_name: hidden
---

# DrawRectangle

> **_This function was added in DSL 1_**

## Description

Draws a rectangle on the screen with the specified position, size, and color.

Position and size in normalized coords, relative to the screen, 0-1.

Keep the [general rules](/docs/dsl-reference/basic-concepts/render-functions) of rendering in mind. _`x`_ and _`y`_ define the top left of the rectangle.

```lua
function DrawRectangle(x, y, width, height, red, green, blue, alpha) --[[ ... ]] end
```

## Parameters

- `x`: _`number`_ - The x-coordinate of the rectangle's top-left corner (0-1).
- `y`: _`number`_ - The y-coordinate of the rectangle's top-left corner (0-1).
- `width`: _`number`_ - The width of the rectangle (0-1).
- `height`: _`number`_ - The height of the rectangle (0-1).
- `red?`: _`number|nil`_ - (Optional) The red component of the rectangle's color (0-255), default 255.
- `green?`: _`number|nil`_ - (Optional) The green component of the rectangle's color (0-255), default 255.
- `blue?`: _`number|nil`_ - (Optional) The blue component of the rectangle's color (0-255), default 255.
- `alpha?`: _`number|nil`_ - (Optional) The alpha component of the rectangle's color (0-255), default 255.

## Return Values

None.

## Versions

- **DSL 4** - _`alpha`_ is now optional, and `255` will be used if it is not present.

## Example

Draws a red rectangle at (10%, 10%) with size (20%, 20%)

```lua
DrawRectangle(0.1, 0.1, 0.2, 0.2, 255, 0, 0, 255)
```
