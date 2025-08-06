---
description: Instantly exit the game's process.
sidebar_class_name: hidden
---

# QuitGame

> **_This function was added in DSL 5_**

## Description

Instantly exit the game's process.

```lua
function QuitGame(status) --[[ ... ]] end
```

## Parameters

- `status`: _`integer`_ - The exit status code. This is typically `0` for a normal exit, but can be any integer value.

## Return Values

This function doesn't return.

## Example

```lua
QuitGame(0)
```
