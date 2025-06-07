---
sidebar_position: 5
pagination_label: Relative Paths
sidebar_label: Relative Paths
description: Relative paths in DSL scripts allow you to access files within the collection or game's Scripts folder. This guide explains how relative paths work, file security, and handling zip files.
---

# Relative Paths

Many DSL functions will take something known as a _relative_ path. This means that the path you give is relative to the running collection, or the game's `Scripts` folder if a DSL is not running (meaning the function was called from a base game script). For example you request a file named `file.txt` from a normal collection named `Collection`, then the real path used will end up being something like `_derpy_script_loader/scripts/Collection/file.txt`.

## File Security

If system access is not enabled (see `allow_system_access` in DSL's config), then an error will occur when trying to access a file that is not in a "safe" path. Anywhere in DSL's `scripts` folder and `packages` folder is considered safe, but in general you shouldn't be accessing anything outside of your own collection.

## Zip Files

If the running collection is a _zipped_ collection, then the file is retrieved from the zip archive. In this case, there is no way to refer to a file that is not in said zip archive.
