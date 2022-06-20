
2022-06-13--2022-06-19

## Goals for the week:

- Finish up rig issues, rig release
- Start releasing packages with new `errors.R`
- Fix pak nightly builds

## GitHub

### r-lib/rig

- Finish and merge `add-pak` fix: 
  https://github.com/r-lib/rig/pull/92
- Support installing w/o translation on Windows: 
  https://github.com/r-lib/rig/pull/93
- Windows: no desktop icon by default
- Windows: `rig system update-rtools40`.
- `rig sysreqs` for macOS, with gfortran, tidy, pkgconfig, checkbashisms:
  https://github.com/r-lib/rig/pull/94
- `rig system allow-debugger-rstudio` on macOS:
  https://github.com/r-lib/rig/pull/96
- Better subprocess output, include within `[INFO]` like the other messages:
  https://github.com/r-lib/rig/pull/97
- `rig rstudio` now errors if R is not orthogonal
- warn if deleting the default version
- macOS: (re)craete /usr/local/bin links if missing
- improve deleting the default version: better cleanup
- start renv projects: `rig rstudio <renc-lock-file>`
- Release rig 0.5.0

### r-lib/pak

- Fix nightly builds for arm64-linux
- Fixes to avoid loading tibble, rlang, etc. the subprocess

### r-lib/cli

- Fix bright escape codes: 
  https://github.com/r-lib/cli/pull/485

### r-lib/ps

- Fix memory error in `ps_loadavg()` on Linux
- Fix `ps()` with both `user` and `after`.
- Relase 1.7.1 to return data frames instead of tibbles. This is to fix
  a bad issue in pak, when it loaded tibble + dependencies in the
  subprocess, causing issues on Windows because of the DLL locking.

### r-lib/processx

- `errors.R` improvements, update callr, pkgsearch, etc. again
- New patch release 3.6.1 to fix a serious resource leak in the previous 
  version.

### rstudio/rstudio

- Allow debugging R by lldb in RStudio:
  https://github.com/rstudio/rstudio/pull/11428
