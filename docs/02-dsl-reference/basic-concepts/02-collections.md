---
sidebar_position: 2
pagination_label: Script Collections
sidebar_label: Script Collections
description: Script collections are a way to group scripts together, allowing for easier management and organization of mods in DSL.
---

# Script Collections

A _script collection_ (sometimes shortened to collection) is, as the name suggests, a collection of scripts. All scripts that DSL load are contained within a collection, even if they are the only script in said collection. This grouping is useful for being able to start and stop multiple related scripts at once, and for simplifying what counts as a single "mod". In general, each script collection can be considered a different mod.

## Types

:::info

- **(DSL 4)** Support for zip files is only in version 4 and beyond.
- **(DSL 7)** Support for categories is only in version 7 and beyond.

:::

A script collection simply represents one of the things placed in DSL's `scripts` folder. There are 3 ways to define a script collection.
Placing other file types in the `scripts` folder is valid and they will be ignored, but having other folders not representing a script collection will raise errors.

- A folder is known as a _normal_ collection.
- A script file (ending in `.lua` / `.lur`) is known as a _standalone_ collection.
- A zip archive (ending in `.zip`) is known as a _zipped_ collection, and mostly behaves like a _normal_ collection.

### Zipped Collections

If you decide to zip your collection up for release, it can be installed by simply putting the zip archive in the `scripts` folder. The structure of your zip archive is very important, your files (such as your config and main script unless changed in the config) must appear in the root of the zip.

For example, if you have a normal collection as a folder (say `Some Mod`) and want to make `Some Mod.zip` then it is important you do not add the folder to the zip. Instead, the contents of the folder are what should be in the root of the zip. Basically put, make sure your config file can be found in the zip at `config.txt` rather than `Some Mod/config.txt`.

### Collection Categories

Normally you just put script collections in the root of DSL's `scripts` folder, but you can also organize them inside category folders. starting and ending with square brackets (such as `[CATEGORY]`). A collection's category has no effect on how it is used or treated by DSL and is only meant to help organization.

Usually script collections should not be released inside any category folder. This feature is only meant for the end-user to organize the scripts they've downloaded.

## Config

:::info

- **(DSL 4)** This feature was introduced in version 4. Older versions used "main.lua" as the name for main scripts, and the concepts of _init & pre-init_ scripts were not yet a thing.

:::

Collections that are not standalone are able to have a `config.txt` file that determines when the collection should run, what requirements are needed (such as DSL version and the presence of other collections), and allows extra functionality not possible without a config file. This config can also be accessed by scripts for any reason, so custom values can be put in if desired by the author. If a config does not exist in a normal collection, a default one will be generated.

All values are optional, and only `main_script` will get a default value (except on the server version where there can be zero main scripts). Standalone collections obviously use their own name for the main script, and other collections will default to using "main.lua". Since the file generated is self-explanatory and there are no hidden options, most of it will not be explained here.

Please note that any requirements dealing with a version number only use the integer version number. This means you should never require something like version `7.1`, but instead just require version `7`.

## Startup

:::info

- **(DSL 4)** A second starting point is supported using a `init_script`.
- **(DSL 5)** A third starting point is supported using a `pre_init_script`.

:::

There are three distinct points that collections can be automatically started \*if\* they have at least one relevant script defined. If a collection does not start automatically, it will have to be started by a command or loaded as a dependency of another collection. In between each of these _stages_, DSL is reset and all collections are instantly killed (without ever calling `MissionCleanup`).

| Script Stage      | Description                                                                                                                         |
| ----------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| `pre_init_script` | Runs once when the game starts. Rendering is not allowed during this stage, and game functions are unavailable.                     |
| `init_script`     | Runs once when the game is loaded, which is when the main menu is reached for the first time. Game functions are unavailable.       |
| `main_script`     | Runs right after the game's script manager is setup, and before the game's `main.lur` starts. Happens again when the game restarts. |

As for actual scripts, there are only 2 ways that one can be started.

- Automatically when a collection starts, if defined in the collections's config.
- Manually when started by a DSL function.

Collections are only automatically started if DSL's global config doesn't have `dont_auto_start` set to true \*or\* the collection's config has an `auto_start` override set to true. If a collection's config defines `auto_start`, then this preference will be overridden. If however DSL's global config has `force_auto_start_pref` set to true, then the collection's `auto_start` is completely ignored. To put it a little more simply, the auto-start behavior is checked like this.

1. Does DSL's config have `force_auto_start_pref` enabled? Then only auto-start if DSL's dont_auto_start is false.
2. Does the collection have `auto_start` defined? Then only auto-start if it says to.
3. Fallback to only auto-starting if DSL's `dont_auto_start` is false.

## Commands

:::info

- **(DSL 4)** Although all of these commands were available since version 1, the `*` option is only available in version 4 and beyond.

:::

All known collections can be shown using the `/list` command. All collections are shown with the names that other collection commands expect. More specific information can be shown using the `/check` collection command, where collection is some collection name.

Starting (or restarting) a collection can be done using `/start collection`, or `/start *` to start / restart all collections. Restarting can also be done using `/restart collection`, and `/restart *` restarts all collections that were already running.

Stopping a collection is done using `/stop collection` or `/stop *` for all collections. This will not instantly kill scripts completely. Instead it starts the graceful shutdown process by killing all active threads and creating the cleanup thread (meaning `MissionCleanup`). The shutdown process will not be considered finished until all cleanup threads are dead.
