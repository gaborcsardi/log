
2022-05-16--2022-05-22

## Goals for the week:

- Further improve rig before meeting with sol eng team

## GitHub

### r-lib/rig

- Rename rim to rig, including homebrew, scoop, choco packages
- macOS menu bar app improvements:
  * put in /Applications
  * rename to Rig.app
  * do not crash if no R is installed
  * app icon
  * show exact version numbers
  * better error messages, get them from rust:
    https://github.com/r-lib/rig/pull/61
- Install arm64 R on arm64 OS by default
- Use logging for messages
- Lots of refactoring for better rust code and de-duplication
