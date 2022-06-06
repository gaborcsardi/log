
2022-05-23--2022-05-29

## Goals for the week:

- Keep improving rig, work towards new release
- Work with Romain on RStudio detection in R packages

## GitHub

### r-lib/rig

- More refactoring, avoid panics on errors
- `rig add` does not change default R version on macOS (!!!)
- Much improved messages:
  https://github.com/r-lib/rig/pull/69
- `rig list`: skip directories that are not R
- JSON output with `--json`:
  https://github.com/r-lib/rig/pull/70
- Library support:
  https://github.com/r-lib/rig/pull/71
- Automatic sysreqs install on Linux:
  https://github.com/r-lib/rig/pull/72
- Rig.app: support library switching
- Start using a configuration file, to avoid having to look up
  user library location all the time. Config file is JSON, learn how to
  parse JSON in rust.
- Second iteration of library support:
  https://github.com/r-lib/rig/pull/75

### r-lib/cli

- Better RStudio pane detection (in nightly):
  https://github.com/r-lib/cli/pull/471
- Avoid red text in build pane, etc: 
  https://github.com/r-lib/cli/commit/5fb5dc12d47696f0dfb86f666e7000d9c7128f36

