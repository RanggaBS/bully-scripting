---
description: Iterates over all values in a configuration object for a given key, parsing each value as a string.
sidebar_class_name: hidden
---

# AllConfigStrings

> **_This function was added in DSL 1_**

## Description

Similar to [`AllConfigValues`](AllConfigValues), except it also parses each value like [`GetConfigString`](GetConfigString) would.

```lua
function AllConfigStrings(config, key) --[[ ... ]] end
```

## Parameters

- `config`: _`userdata`_ - The configuration object to iterate over.
- `key`: _`string`_ - The key to look up in the configuration.

## Return Values

- `iterator`: _`function`_ - An iterator function that returns the next value in the configuration for the given key, parsed as a string.

## Example

```lua
-- highlight-next-line
for value in AllConfigStrings(gConfig, 'some_key') do
  print('Value: ' .. value)
end
```

## See Also

- DSL
  - [`AllConfigValues`](AllConfigValues)
  - [`GetConfigString`](GetConfigString)
