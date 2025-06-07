---
sidebar_position: 1
title: About DSL
pagination_label: About DSL
sidebar_label: About
description: "Derpy's Script Loader (DSL) is a script loader for Bully: Scholarship Edition (PC). It allows you to run scripts, access Lua's standard library, and provides many features to enhance the modding experience."
---

# Derpy Script Loader

Derpy's Script Loader (DSL) is a script loader for Bully: Scholarship Edition (PC).
It can be downloaded [here](/docs/miscellaneous/downloads/dsl), and installation is covered by the included `readme.txt`.
Here are a few of the things that DSL excels at doing, and how they help the overall modding process.

- Load scripts directly from a folder with the simple loading system, or even from a zip archive.
- Skip compiling as Lua's parser is now patched in, letting scripts run from source.
- Unlimited amount of scripts thanks to a custom script manager that still emulates game script objects.
- Access the full Lua standard library, but stay safe with optional system security settings.
- Group scripts together into script collections that can be started, stopped, and restarted on the fly while playing.
- Save and load an arbitrary amount of lua data in actual save game files for any large projects.
- Stop guessing what went wrong with your script, and just see it in a nice convenient console with detailed error reporting.
- Register scriptable commands that can be used with the console to do anything you want... on command!
- Use the custom per-frame renderer that gives you a huge amount of powerful lower-level drawing functions.
- Run scripts earlier than normally possible with conventional STimeCycle.lur replacements, or even on the main menu.
- Replace and register new localized text entries, letting you print any text you want anywhere you want.
- Hook into base game scripts with ease using events that callback your code as soon as a native script loads.
- Use a large majority of new DSL functionality from base game scripts if you need to replace normal scripts.
- Take advantage of more new functions that are too numerous to list here!

## Derpy Script Server

Derpy's Script Server is the server version of DSL. It can be downloaded [here](/docs/miscellaneous/downloads/dsl).
If you want to know more about making network scripts for DSL see [network scripting](network-scripting).
A server can send scripts to players and facilitate communication between players via scripting.
No form of game sync is done by DSL or the server itself. Here are some things you can expect from the server.

- Start and stop script collections using the server console just like you would in the client DSL console.
- Send client scripts to players, including updated scripts when the script collection is restarted.
- Make server scripts that have access to most of the same DSL functions as the client.
- Use network events to send arbitrary Lua data between client and server scripts.

## Getting Started

Use the navigation bar on the left if you are looking for DSL functions.

All mods that you make or install with DSL are put in the `_derpy_script_loader/scripts` folder, and are technically called [script collections](collections).

If you already know how to script mod but are new to DSL, the quickest way to learn is to just make a new file in DSL's `scripts` folder and call it something like `mymod.lua`. Open it in your favorite editor, and make a script like you normally would with a `MissionSetup`, `main`, and `MissionCleanup` function. Unlike replacing a built-in script like `ArcRace1.lur`, your script will run as soon as the game starts. It is for this reason that you will need to wait for [`SystemIsReady`](/docs/game-reference/global-functions/SystemIsReady) to return true before doing most things to avoid any crashes. For the most part, it should be just like making a `STimeCycle.lur` mod. Unlike normal scripting you will not need to compile your script, just start the game! Open the console (using ~ by default) to see if you got any errors, and type `/restart mymod.lua` to restart your script.

## Version History

Versions are represented using a single number that goes up with every full release. Some early versions were called alpha, but the number was still just going up by 1 each version.

If a version only provides small fixes and doesn't add new features, it may be released as a patch with a decimal part (like **7.1**).

### version 9

- 184 client functions, 83 server functions.
- Added the IsHash function.
- Added the GetHash function.
- Added support for console input on Linux servers.
- Added the console_no_input option (but didn't change config version so it won't reset your config).
- Added another argument to the PlayerConnecting event.
- Updated example scripts and extra scripts.
- Removed the ability to start local scripts while on a server.
- Improved console behavior on both server versions.
- Intalled the server_browser by default.
- Fixed a crash when using StopCurrentScriptCollection in a script's initial run.
- Fixed a crash when the server generated its default config.
- Fixed an issue that would make players invalid during certain events.
- Fixed the ScriptDestroyed and ScriptShutdown events.
- Fixed and adjusted a few other things.

### version 8

- 182 client functions, 81 server functions (count no longer includes replaced functions or standard Lua functions).
- Added the PRE_GAME thread type.
- Added the ScriptShutdown and ScriptDestroyed events.
- Added the ServerShutdown event.
- Added the GetCurrentScript function.
- Added the ObjectNameToHashID function on the server, which acts just like the client one.
- Added the QuitServer command on the server for graceful shutdown.
- Added the GetScriptNetworkTable function for sharing values between network scripts.
- Added global net table for accessing shared network tables.
- Added the CreateAdvancedThread function to the server version.
- Added the /quit command on servers for graceful shutdown.
- Added a SIGTERM signal handler for graceful shutdown on Linux servers.
- Added a server config option for showing performance warnings (it was always shown before, now it is off by default).
- Re-organized client config options so that networking options are at the top (but there aren't new options).
- Removed the SetScriptCleanup function as it was broken and has been superseded by ScriptShutdown.
- Fixed the GetScriptFilePath function.

### version 7.1

- Fixed scripted text entry (pasting the clipboard would cause issues after StartTyping was called).
- Fixed script collection discovery for Linux servers.

### version 7

- 197 total functions.
- Servers can now be run on Linux.
- Added ped throttle functions and events.
- Added global dsl table for accessing shared tables.
- Added categories for script collections to help organize large amounts of mods.
- Added the PlayerBuilding event so that scripts can cancel the rebuilding of the player model.
- Added the StopCurrentScriptCollection function so collections can set themselves as fully inactive.
- Added the ability to serialize light userdata for the sake of hashes returned by some game functions.
- Missing scripts are no longer included when \* is used for a command.
- The StartTyping function can now take an initial string instead of always starting blank.
- Improved error reporting when unable to open a file.
- For security, scripts can no longer write files at all after connecting to a server.
- Added a function to check if scripts are allowed to write files.
- Added the AllowOnServer header function to do the same thing as allow_on_server from collection config.
- Reworked client events related to server connections, no longer passing the address more than needed.
- An error is now raised if SendNetworkEvent is called with an unconnected player.
- The client now filters out files based on their type, only allowing whitelisted extensions.
- The require function now properly sets \_REQUIREDNAME in the same way the standard version did.
- Fixed even more issues related to DrawTextInline, including some related to inline texture drawing.
- Fixed an issue that let you restart network scripts after disconnecting.
- Fixed stand-alone server scripts.
- Fixed an issue where scripts loaded as a dependency would still get auto-started.
- Fixed excessive CPU usage by the server.
- Like always, many more small fixes.

### version 6

- 192 total functions.
- OpenFile supports the "ab" mode.
- Fixed function hook and replacement functions.
- The loadfile function doesn't raise an error if the path is unsafe (instead it returns nil + an error).
- Optimized network messages slightly.
- Fixed a problem that could happen when passing nil to compatibility functions.
- A missing main_script will no longer raise an error if there are other types of scripts.
- Fixed a crash related to the command parser.
- Some script cleanup tasks now happen when the script is shutdown rather than when it is fully destroyed.
- Fixed a couple memory leaks.
- Removed the broken DisableController function and replaced it with the ZeroController function.
- Added a message to tell the user if Lua has had an unrecoverable error.
- Added pool functions to check or require pool sizes.
- Added the SetScriptCleanup function for things that need to be cleaned up instantly rather than in a thread.
- Added the CameraFaded event.
- Added the GAME2 thread type.
- Lots of other little fixes and changes as always.

### version 5

- 183 total functions.
- The server version has been released, allowing players to connect to it and communicate through scripted events.
- More local events have been added that offer scripts greater control over the game.
- A new global function hook and replacement system has been created.
- More input functions have been added to modify controller state.
- A significant amount of small changes and patches.

### version 4

- 130 total functions.
- Added an event system, providing scripts with a way to influence game behavior and trigger their own events.
- Argument checking is a little more strict to help the debugging process rather than just taking bad values.
- Collections can now be installed as a zip archive by simply putting a zip with the mod files into the scripts folder.
- Collections have their own config files where custom settings, requirements, or script names can be specified.
- Commands can now have help text associated with them.
- Console output has been improved, such as now showing the collection and thread names in errors.
- Countless major under-the-hood changes to generally improve DSL.
- Direct input keyboard scan codes are now used instead of virtual key codes.
- Dynamic textures were introduced, allowing you to do things like draw the game's current back buffer onto a texture to draw later.
- ImportScript is now supported in a way that mimics the base game, allowing you to import scripts from Scripts.img into your script.
- Improved the way normal script objects are emulated to be more accurate.
- Inline text now has an optional width argument that goes before the text.
- Localized text can now be replaced with new text, and new text entries can be registered.
- More thread types were made for improved control with rendering functions.
- Patched the custom save data system heavily, as it was pretty broken before.
- Persistent data tables have been added as a way for scripts to store information in between DSL resets.
- Pre-init scripts are now a thing, allowing you to run scripts much earlier than normal even if in a limited way.
- Render cache functions now draw before camera fade is applied, but this can be scripted using the new draw layer system.
- Significant additions to the library of script functions, and many improvements to already existing ones.
- Standard file input / output functions have been added for a safer alternative to allowing full system access.
- Smaller things that are too numerous to list fully here.

### alpha 3

- 90 total functions.
- Scripts do not shutdown when main returns anymore, as this design seems better.
- There is a package system now so anyone can neatly add C functions to use in lua if system access is on.
- Config is generated instead of released with updates so that updating is a simple drag/drop/replace.
- The loadlib function is now allowed when system access is turned on in config.
- DrawTextInline can now draw "directly" instead of only allowing one text at a time per-style.
- DrawTextInline doesn't round down duration and the texture alpha has been fixed.
- DrawTextInline preserves formatting on new lines.
- DrawTexture2 can draw a centered texture with optional rotation.
- IsGamePaused returns true if the game is paused.
- GetPackageFilePath returns a file name relative to the "packages" directory.
- SetTextFormatting can take a style number like the ones given to DrawTextInline.
- Other small fixes too minor to list.

### alpha 2

- 87 total functions.
- Temporarily added allow_mouse to loader config, so that mouse-related issues can be narrowed down and reported by those who have problems.
- Added SetTextBold, SetTextItalic, SetTextClipping, PopTextFormatting, and DrawTextInline.

### alpha 1

- 82 total functions.
- The first public release.

### pre-alpha (0)

- Pre-alpha versions were only shared between a tight group of testers, and are only listed here for the sake of completeness.
