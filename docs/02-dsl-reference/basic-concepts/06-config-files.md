---
sidebar_position: 6
title: 'Config Files'
pagination_label: 'Config Files'
sidebar_label: 'Config Files'
description: 'Learn about the DSL, its purpose, and how it can help you in your projects.'
---

# Config Files

Config files in DSL define various settings and behaviors for script collections. They allow you to specify when a collection should run, its requirements, and other custom values that scripts can access.

Starting from DSL 10, configuration files for mods are no longer generated automatically. Instead, you need to create one manually to specify your files, set up the mod, define custom keys, and list any requirements.<br/>You can create a new file named either config.txt (legacy naming convention) or config.ini (new naming convention), and define your configurations within it.

For further documentation: [Script Collections](./02-collections)

## Example

```ini
; DSL Configuration

; if this script collection should automatically start up when the game starts
; only uncomment auto_start if it is necessary to override the preference set by the user

auto_start: true

; it is possible to make a collection that is only meant to register game files but have no scripts
; this will disable normal script loading and suppress the error for having no main script

disable_scripts: false

require_version: 10
require_exact_version: 10
require_system_access: false
require_dependency: MyOtherMod
require_name: MyMod

; main script(s) start when the collection starts (uses main.lua if none are specified)
; if a script ends with .lua and the file does not exist then .lur will be attempted afterwards

main_script: main.lua

; optional initialization script(s) can run during the pause menu before the game starts
; these scripts will only have access to DSL functions and game threads (such as main) will not run

init_script: init.lua

; optional pre-initialization script(s) can run very early during the game's initialization
; these scripts will only have access to DSL functions and cannot render or have any of its threads run

pre_init_script: pre-init.lua

; if this collection is meant to run while connected to servers (no effect on server scripts)
; it will keep the collection from being stopped when connecting to a server and allow control while connected
; this is primarily meant for collections that don't affect gameplay as most servers would see that as cheating

allow_on_server: true

; register game files that should be put in a temporary IMG file (no effect on server scripts)
; files are only registered once when the game starts regardless of if the collection is started or not

act_file: AI.cat
cuts_file: 1-01.dat
trigger_file: MisTrig.dat
ide_file: default.idb
scripts_file: main.lur
world_file: MG_Biology.nft

; Mod Configuration

vertical_position: top
horizontal_position: right
scale: 1.5
font: Consolas
```
