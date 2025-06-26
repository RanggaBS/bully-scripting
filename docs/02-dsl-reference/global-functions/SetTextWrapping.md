---
description: Enables word wrapping for text drawing within a specified width.
sidebar_class_name: hidden
---

# SetTextWrapping

## Description

Enables word wrapping for text drawing, automatically breaking lines to fit within the specified normalized width. When word wrapping is enabled, text will automatically flow to new lines when it would exceed the wrapping boundary. Word wrapping and text clipping are not compatible - using one will disable the other.

```lua
function SetTextWrapping(width) --[[ ... ]] end
```

## Parameters

- `width`: _`number`_ - The width for word wrapping (0.0 to 1.0). Use 0 to disable word wrapping

## Return Values

None.

## Example

```lua
-- Enable word wrapping for left half of screen
-- highlight-next-line
SetTextWrapping(0.5)
SetTextPosition(0.0, 0.1)
SetTextAlign("left", "top")
SetTextScale(0.8)
DrawText("This is a very long piece of text that will automatically wrap to new lines when it reaches the specified width boundary, creating a nice text block.")
```

```lua
-- Create a news ticker with wrapping
local function displayNews(newsText, x, y, width)
-- highlight-next-line
    SetTextWrapping(width)
    SetTextPosition(x, y)
    SetTextAlign("left", "top")
    SetTextScale(0.6)
    SetTextColor(255, 255, 200, 255)
    SetTextOutline(0, 0, 0) -- Black outline for readability
    DrawText(newsText)
    SetTextWrapping(0) -- Reset wrapping
end

-- Usage
displayNews("BREAKING: Scientists discover new species of butterfly in remote rainforest. The discovery sheds new light on biodiversity in the region and highlights the importance of conservation efforts.", 0.05, 0.85, 0.4)
```

- DSL
  - [`SetTextPosition`](./SetTextPosition)
  - [`SetTextFormatting`](./SetTextFormatting)
  - [`SetTextClipping`](./SetTextClipping)