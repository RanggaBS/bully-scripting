---
description: Ensure that the current version of DSL is at least a specific version.
sidebar_class_name: hidden
---

# RequireLoaderVersion

> **_This function was added in DSL 1_**

## Description

Ensure that the current version of DSL is at least a specific version.

This is a _header_ function, meaning it is meant to go on the top of your main script as an alternative to using [config.txt](/docs/dsl-reference/basic-concepts/collections#config).

This function makes sure that the current version of DSL is at least `version`. If `notBackwardsCompatible` is `true`, then it requires that the current version of DSL is the exact version specified. If the current DSL version does not match what is desired, then this script will be shutdown, execution will instantly stop, and the console will inform the user that they do not have the right version. If a main script of a collection is shutdown as a result of calling this function, the entire collection will also be shutdown.

:::info
The version number required here should only be an integer, as any decimal part will be disregarded.
:::

```lua
function RequireLoaderVersion(version, notBackwardsCompatible) --[[ ... ]] end
```

## Parameters

- `version`: _`number`_ - ...
- `notBackwardsCompatible`: _`boolean`_ - ...

## Return Values

None.

## Versions

- **DSL4** - The optional `notBackwardsCompatible` argument was added.

## Example

We can require a certain loader version if we know something will only work in that version.

```lua
-- highlight-next-line
RequireLoaderVersion(4)

RegisterLocalizedText('QUICK_EXAMPLE', 100)
ReplaceLocalizedText('QUICK_EXAMPLE', 'These localized text functions were introduced in DSL4, so it is important we check for that version so anyone running an old DSL version will know they need to upgrade.')

function main()
  while not SystemIsReady() do
    Wait(0)
  end
  Wait(1000)
  TutorialShowMessage('QUICK_EXAMPLE', 5000)
end
```
