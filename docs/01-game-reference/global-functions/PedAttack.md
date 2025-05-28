---
description: Makes a ped attack another ped, with a configurable aggression priority.
sidebar_class_name: hidden
---

# PedAttack

## Description

Commands one ped to attack another. The priority value affects how committed the attacker is to the target.

```lua
function PedAttack(ped, victim, priority) --[[ ... ]] end
```

## Parameters

- `ped`: _`integer`_ - The attacker ped.
- `victim`: _`integer`_ - The target ped to be attacked.
- `priority`: _`integer`_ - Determines how focused the attacker is:

1: Low priority (can be distracted).

3: High priority (relentless aggression).

## Return Values

None.

## Example

None.

