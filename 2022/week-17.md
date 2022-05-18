
2022-04-25 -- 2022-05-01

## Goals for the week:

- cli release, or close to it
- tidy upkeep for two packages
- publish GH actions blog post
- update to R 4.2 on R-hub

## GitHub

### r-lib/actions

- Do not pin `release` to R 4.1.3 any more, on Linux:
  https://github.com/r-lib/actions/commit/9ea29bb8182371e811c469f947bc64ac054b557f
- Version 2.2.2: https://github.com/r-lib/actions/releases/tag/v2
- Discuss lintr example update to error on failure by default:
  https://github.com/r-lib/actions/issues/537

### r-lib/pak

- Fix nightly build on Windows:
  https://github.com/r-lib/pak/commit/4b1ca346cf5bf4107aec0d72839a4be62c0a891a
- Investigate an install failure:
  https://github.com/r-lib/pak/issues/339#issuecomment-1108281044

### r-lib/testthat

- PR reviews:
  https://github.com/r-lib/testthat/pull/1608
  https://github.com/r-lib/testthat/pull/1609

### r-lib/roxygen2

- PR review:
  https://github.com/r-lib/roxygen2/pull/1335

### r-hub/rhub

- Investigate a submission failure:
  https://github.com/r-hub/rhub/issues/293#issuecomment-1107532688

### r-lib/cli

- Finish CRAN release 3.3.0:
  https://github.com/r-lib/cli/issues/451
- Think about exporting `fmt()`:
  https://github.com/r-lib/cli/issues/454
- Merge get_ppid() PR:
  https://github.com/r-lib/cli/pull/453
- Started working on auto-linked code:
  https://github.com/r-lib/cli/pull/455
- Started working again on https://github.com/r-lib/cli/issues/370
  This is really hard to fix, and to fix it properly, we need to
  abandon glue and write our own parser. It is impossible to parse the 
  `{}` and `{.}` cli expressions with glue. This is the conclusion after
  a lot of ideas and tries, and this is now shelved for later. So new
  cli release is abandoned as well, for now.
- Some new ansi functions: `ansi_grep()`, `ansi_grepl()`, `ans_nzchar()`:
  https://github.com/r-lib/cli/pull/458
- Allow styling in `cli_dl()` labels:
  https://github.com/r-lib/cli/commit/072ed21823cdedb5eb63adcc9dbd2685c8252383
- Make inline styles more predictable:
  https://github.com/r-lib/cli/commit/7ed73e318c1083a7fa14716a5f7f9b4ca99203e4

### r-lib/urlchecker

- Think about adding hyperlinks:
  https://github.com/r-lib/urlchecker/issues/23

## r-hub/r-minimal

- Fix building R-next:
  https://github.com/r-hub/r-minimal/commit/a85b3ccdc62ea5e9fbcfe7276bffe73eaa2020e4
- Rerunning nightly manually, apparently GHCR had some issues

## gaborcsardi/keypress

Started to fix this up, evantually it will be in cli.

- Fix up and merge character leaking issue:
  https://github.com/gaborcsardi/keypress/pull/11
- Fix `keypress(block = FALSE)` on Windows:
  https://github.com/gaborcsardi/keypress/pull/8


## r-lb/ps

- Fix compilation on unsupported platforms:
  https://github.com/r-lib/ps/commits?author=gaborcsardi&since=2022-04-24&until=2022-05-01

## Others

- helped track down a bug on M1 R-devel in
  https://github.com/tidymodels/multilevelmod/
