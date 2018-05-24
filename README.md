# Turtl project tracker

This repo exists to track all bugs, issues, features requests, and status for
the entire Turtl project.

The idea is that many times, users/issue reporters don't know which repo to open
the issue on or where to look for project status. This is the attempt to solve
this problem by centralizing everything into one place.

## Turtl components

Here are the main pieces of Turtl and how they all fit together. Note that this
pertains to the v0.7.x release and up, it does not apply to the v0.6 releases or
older.

- [core](https://github.com/turtl/core-rs)  
  The Turtl core houses all the low-level logic for the client app. It runs the
  crypto, the syncing, and the managing of all the user data.
- [server](https://github.com/turtl/server)  
  The Turtl server is a piece separate from the client that's responsible for
  managing user accounts, storing and syncing data, and access restrictions.
  This is the piece the core talks to to log a user in or to grab or update the
  user's profile.
- [js](https://github.com/turtl/js)  
  This is the Turtl HTML5 frontend. It currently serves as the UI for both the
  desktop and mobile clients.
- [desktop](https://github.com/turtl/desktop)  
  This is an Electron wrapper around the [js project](https://github.com/turtl/js)
  that packages Turtl for Windows, Linux, and OSx.
- [mobile](https://github.com/turtl/mobile)  
  This is a Cordova wrapper around the [js project](https://github.com/turtl/js)
  that packages Turtl for Android (and soon iOS).
- [browser-extension](https://github.com/turtl/browser-extension)  
  This is a Firefox/Chrome (and possibly others) browser extension that talks to
  the [desktop](https://github.com/turtl/desktop) app and provides web clipping
  and bookmarking.
- [lib-permissions](https://github.com/turtl/lib-permissions)  
  A small library that allows the [server](https://github.com/turtl/server) and
  the [core](https://github.com/turtl/core-rs) to share a common set of user
  roles and permissions.

