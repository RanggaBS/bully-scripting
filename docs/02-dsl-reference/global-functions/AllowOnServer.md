---
description: Allow your script to keep running even when connected to a server.
sidebar_class_name: hidden
---

# AllowOnServer

> **_This function was added in DSL 7_**

## Description

This is a _header_ function, meaning it is meant to go on the top of your main script as an alternative to using [config.txt](/docs/dsl-reference/basic-concepts/collections#config).

Similar to setting `allow_on_server` in config (which is usually the better option), this will allow your script to keep running even when connected to a server.

```lua
function AllowOnServer() --[[ ... ]] end
```

## Parameters

None.

## Return Values

None.

## Example

```lua
AllowOnServer()

-- Your script code here

function main()
  -- Your script code here
end
```
