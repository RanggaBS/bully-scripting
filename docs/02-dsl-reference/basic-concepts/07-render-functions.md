---
sidebar_position: 7
pagination_label: Render Functions
sidebar_label: Render Functions
description: Render functions are used to draw things on the screen, such as text, images, and shapes. They can be used in any script type, but are most commonly used in drawing scripts.
---

# Render Functions

All of DSL's render functions follow some general rules. Unless otherwise noted by the function's documentation, you can assume the following concepts.

## Normalized Coordinates

Rendering functions that take coordinates or sizes (width / height) expect them to be _normalized_. This means a position of _(0, 0)_ defines the top left of the screen, and _(1, 1)_ is the bottom right. Similarly, a size of _1 x 1_ will be as big as the entire screen. Because of this it is important you make proper use of [`GetDisplayAspectRatio`](/docs/dsl-reference/global-functions/GetDisplayAspectRatio) when you need to draw something that should appear the same size on any aspect ratio. For preserving the aspect ratio of textures, you can use the height multiplied by [`GetTextureDisplayAspectRatio`](/docs/dsl-reference/global-functions/GetTextureDisplayAspectRatio) as the width of your texture draw.

## Color Ranges

Colors values are expected to be in the range of _[0, 255]_, where an RGB value of _0, 0, 0_ is pure black and _255, 255, 255_ is pure white. The alpha value sometimes comes after works the same way, where _0_ is fully transparent and _255_ is fully opaque. If a value given is not an integer, it will be rounded down. Optional color values will always default to _255_.

## Text Formatting

Text formatting for the [`DrawText`](/docs/dsl-reference/global-functions/DrawText) and [`MeasureText`](/docs/dsl-reference/global-functions/MeasureText) functions are done using multiple function calls. Before drawing (or measuring) text, you should be calling any of the text formatting functions to define how you want your text to look. If you end up deciding not to draw text after setting up the format for it, you should call [`DiscardText`](/docs/dsl-reference/global-functions/DiscardText) to get rid of it so it doesn't affect the next time text is drawn. You could also call [`PopTextFormatting`](/docs/dsl-reference/global-functions/PopTextFormatting) to discard the current text but also return a value for later use with [`SetTextFormatting`](/docs/dsl-reference/global-functions/SetTextFormatting). For simple text draws, you can consider using [`DrawTextInline`](/docs/dsl-reference/global-functions/DrawTextInline) as a quick alternative to the normal method.

## Cached Drawing

Things can only technically be drawn in a _drawing_ thread (those with a [type](scripts#thread-types) of `DRAWING`, `POST_WORLD`, or `PRE_FADE`). You are still able to use all rendering functions (unless otherwise noted by the function) at any point, which will simply _cache_ the drawing operation to be done later. The time at which a _cached_ draw is actually drawn is determined by the current _layer_, which is set using [`SetDrawLayer`](/docs/dsl-reference/global-functions/SetDrawLayer). If a measurement is meant to be returned by the function that gets cached, a measurement is still done without actually drawing anything yet.
