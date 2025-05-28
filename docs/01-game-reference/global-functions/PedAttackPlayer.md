---
description: Makes a ped attack the player with a specified priority level.
sidebar_class_name: hidden
---

# PedAttackPlayer

## Description

Commands a ped to attack the player. Functions similarly to [**PedAttack**](https://bully-scripting.vercel.app/docs/game-reference/global-functions/PedAttack), but targets the player directly.

```lua
function PedAttackPlayer(ped, priority) --[[ ... ]] end
```

## Parameters

- `ped`: _`integer`_ - The pedestrian who will attack the player.
- `priority`: _`integer`_ - Determines how focused the attacker is:

1: Low priority (can be distracted).

3: High priority (relentless aggression).

## Return Values

None.

## Example

None.

