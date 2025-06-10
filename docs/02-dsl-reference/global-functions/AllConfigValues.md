---
description: Iterates over all values in a configuration object for a given key.
sidebar_class_name: hidden
---

# AllConfigValues

> **_This function was added in DSL 1_**

## Description

Returns an iterator function designed for use in a _for loop_ that returns each value associated with `key`.

Iterates over all values in a configuration object for a given key. This function is useful for retrieving all values associated with a specific key in a configuration, allowing for easy access to multiple values without needing to know the exact structure of the configuration.

```lua
function AllConfigValues(config, key) --[[ ... ]] end
```

## Parameters

- `config`: _`userdata`_ - The configuration object to iterate over.
- `key`: _`string`_ - The key to look up in the configuration.

## Return Values

- `iterator`: _`function`_ - An iterator function that returns the next value in the configuration for the given key.

## Example

Give the player each weapon listed in a `gConfig`, which is presumed to already exist as a `Config` object.

### script

```lua
-- highlight-next-line
for weapon in AllConfigValues(gConfig, 'weapon_model') do
  local model = tonumber(weapon)
  if model then
    PedSetWeapon(gPlayer, 50)
  else
    PrintWarning('expected number for weapon ('..weapon..')')
  end
end
```

### config

```ini
# List as many weapon models as you want to be used with AllConfigValues
weapon_model 301 # fire crackers
weapon_model 305 # spud gun
weapon_model 307 # bottle rocket launcher
```
