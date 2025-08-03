---
description: Create a `texture` for later drawing given a relative path of a `.png` file.
sidebar_class_name: hidden
---

# CreateTexture

> **_This function was added in DSL 1_**

## Description

Create a `texture` for later drawing given a [relative path](/docs/dsl-reference/basic-concepts/relative-paths) of a `.png` file.

```lua
function CreateTexture(filename) --[[ ... ]] end
```

## Parameters

- `filename`: _`string`_ - The relative path of the `.png` file to load as a texture. The path should be relative to the folder of your script.

## Return Values

- `texture`: _`userdata`_ - The created texture object that can be used for drawing.

## Example

```lua
-- highlight-next-line
local texture = CreateTexture("my_texture.png")
local x, y = 0.1, 0.1 -- Position to draw the texture (in normalized coordinates)
local w, h = 0.2, 0.3 -- Width and height of the texture (in normalized coordinates)
local r, g, b, a = 255, 255, 255, 255 -- Color and alpha values
DrawTexture(texture, x, y, w, h, r, g, b, a)
```

## See Also

- DSL
  - [`DrawTexture`](./DrawTexture) - Draws the texture on the screen.
  - [`DrawTexture2`](./DrawTexture2) - Draws the texture on the screen, with rotation.
