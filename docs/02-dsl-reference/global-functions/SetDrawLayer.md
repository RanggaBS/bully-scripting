---
description: Set the current drawing layer used by cached draws.
sidebar_class_name: hidden
---

# SetDrawLayer

> **_This function was added in DSL 5_**

## Description

Set the current drawing layer used by [cached draws](/docs/dsl-reference/basic-concepts/render-functions#cached-drawing).

This value is reset every time the current thread changes, so you will only need to re-apply it once before a large amount of drawing as long as you know it is all done without the thread yielding (waiting).

If you need to draw something somewhere other than a thread, you should call this function even if it is just to apply the default setting.

```lua
function SetDrawLayer(layer) --[[ ... ]] end
```

## Parameters

- `layer`: _`string`_ - The layer to set. This can be one of the following values:
  - `POST_WORLD`
  - `PRE_FADE`
  - `POST_FADE`

### Layers

- `POST_WORLD`: after the world is drawn, but before HUD is drawn.
- `PRE_FADE`: (default) after HUD is drawn, but before fading is applied.
- `POST_FADE`: after fading is drawn, immediately before the game is actually drawn.

## Return Values

None.

## Versions

- **DSL 4** - Although layers were not implemented until this version, cached draws used to be drawn at the same time as the `POST_FADE` layer rather than `PRE_FADE` (which is the new default).
- **DSL 5** - This function now works as intended, and does not wrongly raise an error when setting any layer besides `POST_FADE`.

## Example

```lua
SetDrawLayer('POST_WORLD')
-- Draw something...
```
