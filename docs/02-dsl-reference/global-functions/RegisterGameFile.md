---
description: Registers a file for replacement in the game archives.
sidebar_class_name: hidden
---

# RegisterGameFile

> **_This function was added in DSL 5_**

## Description

Registers a file for replacement in the game archives.

Register some file for replacement given a [relative path](/docs/dsl-reference/basic-concepts/relative-paths). This can usually only be called in a [pre_init_script](/docs/dsl-reference/basic-concepts/collections#startup). It is usually simpler to register the file using your collection's [`config.txt`](/docs/dsl-reference/basic-concepts/config-files#example-configuration) instead.

```lua
function RegisterGameFile(archive, path) --[[ ... ]] end
```

## Parameters

- `archive`: _`string`_ - The name of the archive to register the file in.
- `path`: _`string`_ - The relative path to the file within the archive.

### Archives (for the `archive` argument)

- `ACT.IMG`
- `CUTS.IMG`
- `TRIGGER.IMG`
- `IDE.IMG`
- `SCRIPTS.IMG`
- `WORLD.IMG`

## Return Values

None.

## Example

```lua
RegisterGameFile('ACT.IMG', 'path/to/file')
```
