---
description: ...
sidebar_class_name: hidden
---

# SoundPlayAmbientSpeechEventSpecific

## Description

:::info
`lineid` matches the line number in `audio\PLAYLIST\Speech.lst` minus 1.
:::

```lua
function SoundPlayAmbientSpeechEventSpecific(ped, speechid, lineid) --[[ ... ]] end
```

## Parameters

- `ped`: _`integer`_ - The ped to make talk.
- `speechid`: _`string`_ - The speech event name.
- `lineid`: _`integer`_ - The line to play.

## Return Values

...

## Example

Makes Jimmy say his Jimmy_PIDLER_v1 line, or "Freaking garbage weather.".

```lua
SoundPlayAmbientSpeechEventSpecific(gPlayer, 'PLAYER_IDLE_RAIN', 34011)
```