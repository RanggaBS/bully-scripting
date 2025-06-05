---
description: Physical state (or condition to be precise) of the player.
---

# Physical States

The in-game mechanisms that trigger yawning and passing out are not solely controlled by the in-game clock. It has been observed that these behaviors are also influenced by the player’s physical state, which reflects conditions such as being well-rested, physically exhausted, or sleepy.

Example:
Setting the player’s physical state to `2` will cause the player character to pass out within a few real-time minutes, regardless of the in-game time.

Known usage in the base game functions:
- [`PlayerChangePhysicalState`](/docs/game-reference/global-functions/PlayerChangePhysicalState)
- [`PlayerGetPhysicalState`](/docs/game-reference/global-functions/PlayerGetPhysicalState)
- [`PlayerRefreshPhysicalState`](/docs/game-reference/global-functions/PlayerRefreshPhysicalState)
- [`PlayerResetPhysicalState`](/docs/game-reference/global-functions/PlayerResetPhysicalState)

:::info
The names of physical states mentioned are arbitrarily defined for clarity and ease of understanding. They do not represent official terminology used by the game engine or internal development tools.
:::
| State ID | Description  |
| -------: | :----------- |
|        0 | Well-rested  |
|        1 | Exhausted    |
|        2 | Sleepy       |
