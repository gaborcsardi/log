
2022-05-09--2022-05-15

## Goals for the week:

- rim talk was postponed, so keep adding new features before next week
- rim menu bar app

## GitHub

### r-lib/rim

- Release rim 0.3.0
- Link statically to MSVC runtime, so it is really dependency free on
  Windows: 
  https://github.com/r-lib/rim/pull/57
- macOS menu bar app, and lots of learning for that:
  * how to create a rust library 
  * how to call rust library from C
  * survey on tools to create a menu bar app
  * learn more Swift and AppKit
  * how to call C (rust really) library from Swift
  * `DirectoryWatcher()` in Swift to watch a directory for changes
  * "launch at login" and "preferences" functionality in macOS apps
