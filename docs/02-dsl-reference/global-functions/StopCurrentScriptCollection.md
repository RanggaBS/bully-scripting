---
description: Stop the current script collection.
sidebar_class_name: hidden
---

# StopCurrentScriptCollection

> **_This function was added in DSL 7_**

## Description

Stops the current script collection.

Similar to [`TerminateCurrentScript`](TerminateCurrentScript), this will not _instantly_ take control from your script.

The most common use for this function is to mark the script collection as **INACTIVE**, which does not happen automatically when your scripts die.

```lua
function StopCurrentScriptCollection() --[[ ... ]] end
```

## Parameters

None.

## Return Values

None.

## Example

```lua
StopCurrentScriptCollection()
```

## See Also

- DSL
  - [TerminateCurrentScript](TerminateCurrentScript)
