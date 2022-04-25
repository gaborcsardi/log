
# 2022-02-28 -- 2022-03-06

## GitHub, 223 commits in 24 repos

### https://github.com/r-lib/desc/commits?author=gaborcsardi&since=2022-02-27&until=2022-03-06

- tidy upkeep and issue triage
- switch crayon -> cli
- CRAN release 1.4.1

### https://github.com/r-lib/pak/commits?author=gaborcsardi&since=2022-02-27&until=2022-03-06

- Working on nightly builds. Update to new rim version in nightly builds.
- Start using a self-hosted M1 runner for arm64 macOS builds.
- Start using a self-hosted runner for Linux aarch64 builds.
- Update table of supported platforms in README
- Fix pushing packages to GHCR, need to retry, sometimes it just fails,
  even if we use the built-in retry of skopeo.
- Suffering with updating image in README. These are cached indefintely,
  so one has to change the URL to clear the cache, e.g. by adding a 
  `?version=n` dummy query parameter.
- Fix authots in DESCRIPTION.

### https://github.com/r-lib/cli/commits?author=gaborcsardi&since=2022-02-27&until=2022-03-06

- Tidy upkeep and issue triage
- Ignore error inspector in condition wrapping, apparently we don't need
  it: https://github.com/r-lib/cli/issues/288
- We need new rlang for the tests, but we cannot require it, because that
  changes rlang behavior, so need to skip the tests that use old rlang.

### https://github.com/r-lib/processx/commits?author=gaborcsardi&since=2022-02-27&until=2022-03-06

- tidy upkeep and issue triage
- suffering with an issue with `kill_tree()` on macOS, because now you cannot
  always read out the environment of another process:
  https://github.com/r-lib/processx/issues/326

### https://github.com/r-lib/rim/commits?author=gaborcsardi&since=2022-02-27&until=2022-03-06

- Set PATH to rim an R on GHA Windows, so rim and R just work ootb.
- Make the tests work on GHA. This is complicated because of interplay
  between bash, powershell and bats. It works if we run the `.bat` files:
  https://github.com/r-lib/rim/commit/86d1aea0d5347a7d3e300ba7174c163a8ebe254f
- Add more Windows tests.
- Better README
- Better messages when we escalate/elevate:
  https://github.com/r-lib/rim/issues/26
- Windows: `rim default <ver>` checks of `ver` is installed.
- Release 0.2.0
- Thinking about how we could support system dependencies in rim, and
  whether we should use Homebrew or Simon's recipes or both.

### https://github.com/r-lib/ps/commits?author=gaborcsardi&since=2022-02-27&until=2022-03-06

- tidy upkeep and issue triage
- Fix a test case

### https://github.com/r-lib/fs/commits?author=gaborcsardi&since=2022-02-27&until=2022-03-06

- tidy upkeep and issue triage

### https://github.com/r-lib/brio/commits?author=gaborcsardi&since=2022-02-27&until=2022-03-06

- tidy upkeep and issue triage

### https://github.com/r-lib/sessioninfo/commits?author=gaborcsardi&since=2022-02-27&until=2022-03-06

- tidy upkeep and issue triage

### https://github.com/r-hub/r-minimal/commits?author=gaborcsardi&since=2022-02-27&until=2022-03-06

- fix aarch64 builds, need pak with the right arch, with the new repo URL.
- try to work around various directory names before R release, R-alpha, 
  R-beta, etc. 
- Document that we support aarch64 packages now.

### https://github.com/r-lib/callr/commits?author=gaborcsardi&since=2022-02-27&until=2022-03-06

- last of master -> main transition

### https://github.com/r-hub/sysreqsdb/commits?author=gaborcsardi&since=2022-02-27&until=2022-03-06

- add some exceptions for the case where a cran packages is neeeded
  through bioc, so we don't pick it up automatically.

### https://github.com/r-lib/revdepcheck/commits?author=gaborcsardi&since=2022-02-27&until=2022-03-06

- last of master -> main transition

### https://github.com/r-lib/rcmdcheck/commits?author=gaborcsardi&since=2022-02-27&until=2022-03-06

- last of master -> main transition

### https://github.com/r-lib/remotes/commits?author=gaborcsardi&since=2022-02-27&until=2022-03-06

- last of master -> main transition

### https://github.com/r-lib/asciicast/commits?author=gaborcsardi&since=2022-02-27&until=2022-03-06

- last of master -> main transition

### https://github.com/r-lib/cleancall/commits?author=gaborcsardi&since=2022-02-27&until=2022-03-06

- last of master -> main transition

### https://github.com/r-lib/filelock/commits?author=gaborcsardi&since=2022-02-27&until=2022-03-06

- last of master -> main transition

### https://github.com/r-lib/zip/commits?author=gaborcsardi&since=2022-02-27&until=2022-03-06

- last of master -> main transition

### https://github.com/r-lib/liteq/commits?author=gaborcsardi&since=2022-02-27&until=2022-03-06

- last of master -> main transition

### https://github.com/r-dbi/odbc

- Fixing LaTeX issues: https://github.com/r-dbi/odbc/pull/487

### Issues and PRs

- https://github.com/ropensci/codemetar/issues/331
- debugging new withr, turns out the handler stack has changed:
  https://github.com/r-lib/withr/issues/197
- opening tidy upkeep issues in all my repos

## Issue discussions

Too many to collect now...

## community.rstudio.com

- help with three issues
