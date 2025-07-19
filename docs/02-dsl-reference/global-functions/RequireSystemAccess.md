---
description: Ensure that system access is enabled.
sidebar_class_name: hidden
---

# RequireSystemAccess

> **_This function was added in DSL 1_**

## Description

Ensure that system access is enabled.

This is a _header_ function, meaning it is meant to go on the top of your main script as an alternative to using [config.txt](/docs/dsl-reference/basic-concepts/collections#config).

This function makes sure that system access is enabled (see `allow_system_access` in DSL's config). If system access is not enabled, then this script will be shutdown, execution will instantly stop, and the console will inform the user that they need system access enabled to continue. If a main script of a collection is shutdown as a result of calling this function, the entire collection will also be shutdown.

```lua
function RequireSystemAccess() --[[ ... ]] end
```

## Parameters

None.

## Return Values

None.

## Example

```lua
-- highlight-next-line
RequireSystemAccess()

function main()
  while not SystemIsReady() do
    Wait(0)
  end
  -- ...
end
```
