---
sidebar_position: 3
title: Scripts & Threads
pagination_label: Scripts & Threads
sidebar_label: Scripts & Threads
description: DSL scripts and threads act similarly to normal scripts, with some additional features and functions. This guide covers script flow, environments, thread types, order, and compatibility with the base game.
---

# Scripts & Threads

For the most part, DSL scripts and threads act the same as normal scripts. This means you should mostly be able to do anything you normally could in a base game script replacement, but as discussed in 'Game Compatibility' section below, there may be a few cases where this is not the case.

## Script Flow

There can be 4 special functions defined in your script that DSL will use to make `GAME` threads at certain times. All of them are optional, and will just be skipped if not present.

| Function Name    | Description                                                                                        |
| ---------------- | -------------------------------------------------------------------------------------------------- |
| `gamemain`       | Only once immediately after scripts are initialized, before the base game's `main.lur` is created. |
| `MissionSetup`   | When the script starts. If an error occurs, the whole script is shut down.                         |
| `main`           | After `MissionSetup` is completed, or right away if it doesn't exist.                              |
| `MissionCleanup` | On script shutdown. This thread is considered a _cleanup_ thread.                                  |

The `gamemain` function is special because along with running when normal game threads run, it will also be updated once as soon as it is created. This emulates the way `gamemain` works in the base game's `main.lur`, and also gives you a way to do things that need to be done ASAP.

_Cleanup_ threads will keep a script from being fully shutdown, also keeping the collection stuck in the "STOPPING" state if it's shutting down. Any thread created by a cleanup thread also becomes a cleanup thread. Usually this is only to allow something like a quick area transition to happen as part of cleanup.

## Script Environments

When a DSL script starts, it is given its own environment just like the game's normal mission scripts. The only thing set by DSL in this environment is `ImportScript`, imitating the way the game normally works. This means that all globals you set in your script will be limited to only being seen by said script, even though you can of course still access the global environment. Things can be shared between scripts in a collection using `GetScriptSharedTable` to get a table that all scripts in the collection can access. For a wider scope, you can use the `shared` table to pass things around (the way that normal game scripts do it). If you need to add something to the global environment, you can use `_G` (the global environment table).

## Thread Types

Normally there is only one type of thread, but in DSL there are many thread types. The type of a thread determines when it will be run. Game threads are created using `CreateThread`, and the other "main" thread types also have their own dedicated functions. For any other type of function, you will need to use `CreateAdvancedThread`.

| Thread Type              | Description                                                                 |
| ------------------------ | --------------------------------------------------------------------------- |
| `GAME`                   | runs immediately after base game scripts normally run.                      |
| `SYSTEM`                 | runs each frame before anything else, even before input.                    |
| `DRAWING`                | runs right before the game is presented, allowing you to draw on top of it. |
| **(DSL 4)** `POST_WORLD` | runs after the world is drawn but before HUD is drawn.                      |
| **(DSL 4)** `PRE_FADE`   | runs before the game draws camera fade.                                     |
| **(DSL 6)** `GAME2`      | runs immediately after normal `GAME` threads.                               |
| **(DSL 8)** `PRE_GAME`   | runs immediately before normal `GAME` threads.                              |

## Thread Order

:::info
**(DSL 4)** Prior to version 4, script cleanup was done in order rather than unwinding.
:::

Any time there is a _thread update_, it is done in a specific but very simple order. All collections are run in the order they were created, meaning each script belonging to the collection is run in order, meaning each thread belonging to the script is run in order.

The only exception to this rule is that the script order is reversed when a collection shuts down, as if the scripts are being "unwound".

## Game Compatibility

Since DSL uses its own improved script management system rather than loading scripts directly into the (very limited) normal script pool, things do not \*always\* perfectly work out. 99% of functions will not be affected by this, but a few (namely _button sequence_ functions) will cause issues due to the way they work. Another notable example is `BlipAddXYZ`, a function that mostly works fine but will fail to draw a ground blip by default in DSL. A few _compatibility_ functions (like `CallFunctionFromScript`) exist to help this by calling certain script functions while setting a different base game script as "active". If all else fails though, you can still mod the old fashioned way by replacing base game scripts while still being allowed to make use of most DSL functions.
