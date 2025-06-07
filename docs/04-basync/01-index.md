---
slug: .
description: Basync is a script collection designed to provide basic extensible sync to your DSL server.
---

# BASYNC

## Summary

Basync is a script collection designed to provide basic extensible sync to your DSL server. The target audience for these doc pages are people who are already familiar with the basics of setting up a server, using scripts, and making their own scripts. If you're just getting started and aren't confident doing those things yet then you should consider checking out the DSL [server manual](/docs/miscellaneous/resources/dsl-server-manual).

Basync and its modules (discussed later) can be downloaded on the [GitHub page](https://github.com/derpy54320/dss-extras) for extra DSS scripts. Since basync is just a script collection, installation is as simple as dropping it in your server's `scripts` folder and getting some [basync modules](/docs/basync/modules) to go with it. Just make sure not to change the name from "basync" since other scripts will expect it to be named that (when requiring dependencies or using `net.basync`).

## Modularity

One of the main principles behind basync's design is staying basic on its own but being extensible and modular through _other_ scripts. Instead of trying to be perfect and do everything, basync lets you (the server owner and/or scripter) decide what you want synced by basync and leaves the rest up to other scripts.

On its own, basync provides some basic world sync and manages the existance of **peds** & **vehicles**. Both of these entities have their name, model, area, and position synced. Peds can also be assigned to vehicle seats, and basync controls putting peds in and out of said vehicles.

Other scripts can make use of certain basync functions to add their own bits of sync, such as trying to sync action nodes or action throttle (what makes peds walk / run). Many scripts like this are developed alongside basync, and are usually referred to as [basync modules](/docs/basync/modules).

Even basync's core behaviors can be configured if needed, just by editing its `config.txt` file.

## Documentation

More specific documentation is available in the following pages.

| Page                                | Description                                             |
| ----------------------------------- | ------------------------------------------------------- |
| [global api](/docs/basync/api)      | global server functions that mock client functions      |
| [functions](/docs/basync/functions) | basync functions that you can use in your scripts       |
| [objects](/docs/basync/objects)     | info about various basync objects and their methods     |
| [events](/docs/basync/events)       | basync events that you can use in your scripts          |
| [modules](/docs/basync/modules)     | basync modules that extend entity sync                  |
| [examples](/docs/basync/examples)   | some basic examples of how other scripts can use basync |
