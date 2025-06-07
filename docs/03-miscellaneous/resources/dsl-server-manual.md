---
description: Derpy's Script Server - Server Manual
title: Derpy's Script Server - Server Manual
---

# Derpy's Script Server - Server Manual

## Server Setup

- [1. Getting started](#1-getting-started)
- [2. Setting up a Linux server](#2-setting-up-a-linux-server)
- [3. Configuring your server](#3-configuring-your-server)
- [4. Setting up your scripts](#4-setting-up-your-scripts)
- [5. Hosting your server](#5-hosting-your-server)

## Official Scripts

- [account](#account)
- [admin](#admin)
- [chat](#chat)
- [loadanim](#loadanim)
- [menu](#menu)
- [profanity](#profanity)

## 1. Getting started

Before setting up your server, you should already be familiar with the basics of [derpy's script loader (DSL)](/docs/dsl-reference/basic-concepts/about-dsl) and how [DSL collections](/docs/dsl-reference/basic-concepts/collections) work. Once you are confident with using the loader itself, you should be ready to setup a server (which you can download [here](/docs/miscellaneous/downloads/dsl)).

Once you have the server version, you must decide if you want to run the server using Windows or Linux. If using Windows, you should just be able to run `derpy_script_server.exe`. If using Linux, you should run `./derpy_script_server` but may have to set a few things up first.

The directory (or folder) you run the executable in is where all your files will go. You should at least have the `scripts` folder by the executable before you run it. After you start the server for the first time, a `config.txt` file will be generated and you may configure it before starting again.

## 2. Setting up a Linux server

If you're running Ubuntu, read on for some help getting started. If you're using any other Linux distro, then you're on your own. Since the server is 32 bit, you will need to make sure you can actually run 32 bit code. This usually just means you'll need to install `lib32z1` and `libc6-i386`.

The following code is a list of commands to help you get your Linux server setup using the command line. It downloads version 9 since that is the latest version as of this writing, but you may need to change it to download a later version if there is a newer one available.

```bash
# ubuntu setup (for other linux distros, you're on your own)

# make a new directory for the server somewhere

mkdir my-dss-server
cd my-dss-server

# download and extract the server release

wget -q -O dss.zip https://www.mediafire.com/file_premium/vobshxqcc2kxxa8/derpy_script_server_9_s.zip/file
unzip dss.zip

# install 32 bit packages for your 64 bit system

sudo apt-get install lib32z1
sudo apt-get install libc6-i386

# make the server file an executable

chmod +x derpy_script_server

# run the server so it generates a config

./derpy_script_server

# configure the server

nano config.txt

# and finally run it for real

./derpy_script_server
```

## 3. Configuring your server

For the most part, `config.txt` documents itself and you should be able to figure out what to change. The only things that you should really need to change are `server_name`, `server_info`, and if you'd like you can uncomment `server_icon` and set it to a relative path for a 1:1 PNG that is no more than 100 KiB.

If you are only making this server for a few friends and you want to make sure nobody joins that isn't supposed to, you can setup a whitelist by setting `whitelist_instead` to true and uncommenting `whitelist_ip` and setting it to someone's IP. You can then add as many more IPs as you want by duplicating that line.

## 4. Setting up your scripts

By itself, a server will do nothing to players' games. It is only through scripts that anything happens, including any sort of game sync. Scripts used to come with the server (in an `extras` folder) but are now you will have to download or make any scripts you want. Once you get some scripts you can control them using the same basic commands you'd use on the client.

Official scripts (made or endorsed by _derpy54320_) are available on [GitHub](https://github.com/derpy54320). These scripts all have their own `config.txt` that you should check out and configure if you decide to use them. Some scripts can integrate with each other, but none are configured to do so by default.

While most official scripts are documented here, [basync](/docs/basync) has its own page due to how complex it is. It provides a modular base for multiplayer.

If you are interested in making your own network scripts, you can check out this page to get started.

## 5. Hosting your server

It is usually a good idea to run the server locally on Windows so it is easier to develop it, then move it to a dedicated Linux server when it's ready to be played. There are many services that will let you rent a [VPS](https://en.wikipedia.org/wiki/Virtual_private_server) if you do not have a server yet, [Vultr](https://vultr.com) being a fairly good choice. It is often more cost-effective to rent a Linux server than a Windows one, but either will work of course so you should get whatever is best for you.

Once your server is up, you should be able to connect to it by turning on `allow_networking` in your DSL `config.txt` and then using `/connect` in-game. If everything seems okay, you can share your server's IP with your friends to start playing! It is suggested you restart the server at least every few days to keep it running well.

If you have problems, make sure the port for your server is open (`17017` by default) and that your firewall allows in-bound connections for the server. To test if your server is visible to the internet, consider using [portchecker.co](https://portchecker.co).

## account

### Summary

These scripts make players create an account to play on the server. This ensures that every player has some unique identifier (their username) that other scripts can use when saving data that should be tied to a certain player. Accounts can also have roles attached to them, which other scripts can check for.

### Integrations

- `profanity`: restrict players from creating accounts with profane usernames.

### Commands (server)

- `/check_account <user>`: check if an account exists, is being used, and what roles it has.
- `/check_accounts [count]`: print statistics related to accounts, and optionally list accounts in alphabetical order.
- `/delete_account <user>`: delete a specific account.
- `/demote_account <user> [role]`: strip an account of a specific role or of all roles.
- `/promote_account <user> <role>`: give an account some role that other scripts can check for.
- `/reset_accounts`: reset all account data, totally destroying every account.
- `/unlimit_accounts <player_id>`: temporarily allow a player to make as many accounts as they want.
- `/verify_accounts`: tell all running scripts to verify their account data and cleanup anything related to deleted accounts.

### Local Events (server)

- `account:deleteAccount(user)`: an account has been deleted and all references to this username should be removed.
  Return true to tell the server something failed, which will tell the server owner to try `/verify_accounts`.
- `account:playerSignedIn(player, user)`: a player has signed in and was not signed in before.
  This event is only run when the player is valid and connected.
- `account:playerSignedOut(player)`: a player has signed out (and may not be valid anymore).
  All players are signed out when the account scripts stop or when accounts are reset using `/reset_accounts`.
- `account:playerUpdatedRoles(player)`: a player had their roles changed (happens after a sign-in, sign-out, promotion, or demotion).
  This event is only run when the player is valid and connected.
- `account:scriptStopping`: the account system's script collection is stopping.
  Runs before players are signed out, so you can remove player account references early if desired.
- `account:verifyAccounts(check)`: the server wants all scripts to verify that all their references to usernames are valid (using if check(user) then ...).
  Return true to tell the server something failed, which will tell the server owner to try `/verify_accounts`.

### Shared Functions (server)

- `net.account.all_players()`: returns an iterator for all signed in players (so you can use `for player, user do ...`).
- `net.account.get_player_username(player)`: returns the username of a player if they're signed in (and `nil` otherwise, so you can check if they're even signed in).
- `net.account.is_player_role(player, role)`: returns true if the player is signed in and has the role (and `false` otherwise).

### Shared Functions (client)

- `net.account.get_username()`: returns the username of the player if they're signed in (and nil otherwise, so you can check if they're even signed in).
- `net.account.is_ui_active()`: returns true if the account UI is active (and false otherwise, so you can disable your UI while it is up).

## admin

### Summary

These scripts provide administrative and moderative commands. Players can be authenticated using an IP or an account role if applicable. Commands are only registered for players that are allowed to use them (but even then the server will verify them before doing anything).

### Integrations

- `account`: use roles to determine admins / mods, and show usernames in the `/players` command.

### Commands (client)

- `/ban <id> [reason]`: temporarily ban a player (until the scripts are stopped).
- `/kick <id> [reason]`: kick a player.
- `/players`: list all player IDs.
- `/server [...]`: remotely run a command on the server.

### Local Events (server)

- `admin:playerUpdated(player)`: a player's rank has been updated, so you should update any cached information about their rank.
  This event is only run when the player is valid and connected.

### Shared Functions (server)

- `net.admin.is_player_admin(player)`: returns `true` if the player is an admin, and `false` otherwise.
- `net.admin.is_player_mod(player)`: returns `true` if the player is an admin _or_ moderator, and `false` otherwise.
- `net.admin.update_player(player)`: update the player's rank and trigger an `admin:playerUpdated` event. Usually not needed unless you have a reason.

### Shared Functions (client)

- `net.admin.is_admin()`: returns `true` if the player is an admin, and `false` otherwise.
- `net.admin.is_mod()`: returns `true` if the player is an admin or moderator, and `false` otherwise.

## chat

### Summary

These scripts are for the chat. Press `enter` or `/` to start sending a message or run a command.

### Integrations

- `account`: show usernames instead of player names and ensure proper UI timing.
- `admin`: show player ID numbers to moderators.
- `profanity`: censor profane player messages.

### Commands (server)

`/say <message>`: send a server message to all players.

### Local Events (server)

- `chat:playerMessage(player, msg)`: a player is sending a message. The `msg` table contains data about the message, some of which can be modified.
  Return `true` to not send the message. The `msg` table contains these fields: `name`, `message`, `moderator`, and `color`.

### Shared Functions (server)

- `net.chat.notify(target, message, red, green, blue)`: same as the client version, but takes a target player. Use `-1` for all players.
- `net.chat.say(target, name, message, red, green, blue)`: same as the client version, but takes a target player. Use `-1` for all players.

### Shared Functions (client)

- `net.chat.notify(message, red, green, blue)`: print a notification in the chat, and optionally specify a custom text color.
- `net.chat.say(name, message, red, green, blue)`: print a message in the chat, and optionally specify a custom name color.

## loadanim

### Summary

The same `loadanim.lua` script that normally comes with DSL. Loads all animation groups so other scripts don't have to worry about it.

## menu

### Summary

These scripts are for the server menu. It is totally client side and serves as a central menu system for other scripts to integrate with.

### Local Events (client)

- `menu:openMain(add)`: the main menu is opening and you should add options (using `add("Name", "Description", CB_Function)`).
  Return `true` to stop the menu. The `add` function creates a thread in the handling script that runs when selected.

### Shared Functions (client)

You should usually only create a menu during a callback registered during the `menu:openMain` event. Callbacks run on the same thread as the main menu, so they will properly keep it from being used until your callback returns. If you do make your own menu at a different time, return `true` during `menu:openMain` while it is running.

- `net.menu.create(title, help)`: creates a new `menu` object.
- `net.menu.submenu(title, help)`: creates a new `menu` object that inherits the style of the main menu.
- `net.menu.extend(help)`: creates a new `menu` object that inherits the style of the main menu and draws to the right of it.
- `net.menu.is_active()`: returns `true` if the menu is active.

### Menu Object (client)

The menu system works by adding a bunch of options with `menu:option` and drawing with `menu:draw` each frame. After the menu is drawn, it lets the user control it the next time it is updated (the next frame). When a selection is made, the menu will remember which option it was (based on position and text) and return `true` next time the option is added. This lets you handle your option however you like and also keeps the options past that point from being updated until the menu is drawn again, which helps you not have to worry about control flow as much (which means you can `elseif` options together for convenience).

These are methods for `menu` objects returned by `net.menu.create` and `net.menu.extend`.

- `menu:active()`: returns `true` while the menu is active, and updates the menu if needed.
  Usually you will be simply using this method in a `while` to loop make your menu loop.
- `menu:option(text, right_text, description_text)`: adds an option to the menu, and updates the menu if needed.
  Returns `true` if it was just selected. All arguments are optional and can be skipped using `nil`.
- `menu:alert(text, seconds)`: show some text in the description box. Takes priority over menu and option help text.
  If `seconds` is not given (or isn't positive), it will only be used for one draw.
- `menu:help(text)`: set the help text associated with the menu. Has the lowest priority for the description box.
  This sets the same thing as the `help` argument for menu creation. It can also be `nil`.
- `menu:draw(keep)`: draws the menu, and updates it first if needed. Resets all options and allows input to be processed next menu update. Returns `x, y, w, h`.
  If `keep` is given, options will not reset. If `keep` is given but not a boolean, it updates the `right_text` for the current option to allow a "selector".
- `menu:up()`: uses the menu navigation controls and logic to determine if the user hit up. Also plays a sound.
  There are also methods for `down`, `left`, and `right` that do not explicitly listed here.
- `menu:submenu(help)`: creates and returns a new menu that inherits this menu's `draw_style`.
  The style is copied by value, so you can change it independently of the original.
- `menu:extend(help)`: creates and returns a new menu that inherits this menu's `draw_style` and draws to the right of it.
  Usually it is neater to just make a new menu than to keep extending right.
- `menu:style(name)`: apply a pre-defined style to the menu instead of changing `draw_style` manually.
  As of writing this, options include `'default'` and `'alternate'`.

These are fields in `menu` objects that can be changed (other fields should not be changed).

- `menu.can_exit`: determines if the menu can be exited by pressing left.
  By default this is `true`.
- `menu.fix_camera`: determines if the game's camera will be scripted to not change when hitting up.
  By default this is `true`.
- `menu.title_format`: a text formatting table for the format of title text.
  There are also fields for `option_format` and `description_format`.
- `menu.draw_style`: a table that describes how the menu should be drawn.
  Changing this will require you to look in the source to see how.

```lua
-- menu example: make a new menu that can be accessed from the main menu

RegisterLocalEventHandler("menu:openMain",function(add)
  add("My Menu", "An example sub-menu in the main server menu.", M_MyMenu)
end)

function M_MyMenu()
  local menu = net.menu.create("My Menu")
  while menu:active() do
    if menu:option("Give Spud Gun") then
      PedSetWeapon(gPlayer, 305, 8, false)
    elseif menu:option("Give Bottle Rocket Launcher") then
      PedSetWeapon(gPlayer, 307, 8, false)
    end
    menu:draw()
    Wait(0)
  end
end
```

## profanity

### Summary

These scripts check for profanity. They do not do anything by themselves, and only provide other scripts with a way to check for profanity.

### Shared Functions (server & client)

- `net.profanity.is_dirty_str(str, level)`: returns `true` if the string contains profanity, optionally using a custom profanity level.
- `net.profanity.get_clean_str(str, level)`: returns a censored version of the string (can be slow, so it is suggested you don't use it on the server).
