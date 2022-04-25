
# 2022-03-14 -- 2022-03-20

## GitHub, 160 commits in 26 repos

### https://github.com/r-lib/whoami/commits?author=gaborcsardi&since=2022-03-13&until=2022-03-20

- tidy upkeep and issue triage

### https://github.com/r-lib/urlchecker/commits?author=gaborcsardi&since=2022-03-13&until=2022-03-20

- tidy upkeep and issue triage
- update base R code
- fix URL fragments
- create and submit base R patch for the same:
  https://github.com/gaborcsardi/r-source/pull/10
  
### https://github.com/r-lib/oskeyring/commits?author=gaborcsardi&since=2022-03-13&until=2022-03-20

- tidy upkeep and issue triage

### https://github.com/r-lib/pkgcache/commits?author=gaborcsardi&since=2022-03-13&until=2022-03-20

- tidy upkeep and issue triage

### https://github.com/r-lib/pak/commits?author=gaborcsardi&since=2022-03-13&until=2022-03-20

- fix bundling and repo tests on R 3.4 and Windows
- use dev pkgdepends for solver improvements

### https://github.com/r-lib/rim/commits?author=gaborcsardi&since=2022-03-13&until=2022-03-20

- print debug info on GHA fail
- fix older Windows download URLs, the changed again
- cannot use 4-number version numbers, must be semver
- experiment with auto-building/publishing homebrew tap for rim,
  could not make it work, so this will be manual for now
- create homebrew tap manually, update installation instructions in README
- work out how to update R to allow debugging and core dumps and add to rim:
  `rim system allow-debugger` and `rim system allow-core-dumps`

### https://github.com/r-lib/processx/commits?author=gaborcsardi&since=2022-03-13&until=2022-03-20

- fix a silly race condition in the SIGCHLD handler, that caused 
  crashes: https://github.com/r-lib/processx/pull/330

### https://github.com/r-lib/pkgdepends/commits?author=gaborcsardi&since=2022-03-13&until=2022-03-20

- Fix a bug in loading the install plan
- Improved solver heuristics more multiple big repos:
  https://github.com/r-lib/pkgdepends/pull/277

### https://github.com/r-hub/r-minimal/commits?author=gaborcsardi&since=2022-03-13&until=2022-03-20

- Work out how to install readxl on Alpine:
  https://github.com/tidyverse/readxl/pull/687
- Fix R-patched build

### https://github.com/r-lib/cli/commits?author=gaborcsardi&since=2022-03-13&until=2022-03-20

- Work on RStudio hyperlinks with Romain:
  https://github.com/r-lib/cli/pull/438

### https://github.com/r-lib/filelock/commits?author=gaborcsardi&since=2022-03-13&until=2022-03-20

- Switch to testthat 3

### https://github.com/r-hub/sysreqsdb/commits?author=gaborcsardi&since=2022-03-13&until=2022-03-20

- small fix

## Issues and PRs

- Report macOS environment issue to psutil:
  https://github.com/giampaolo/psutil/issues/2084

## community.rstudio.com

helped with one issue
