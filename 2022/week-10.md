
# 2022-03-07 -- 2022-03-13

## GitHub, 150 commits in 13 repos

### https://github.com/r-lib/pak/commits?author=gaborcsardi&since=2022-03-06&until=2022-03-13

- our CRAN repo now also creates a main metadata file, looks like this:
  https://github.com/r-lib/r-lib.github.io/blob/gh-pages/p/pak/devel/metadata.json
  This is already useful as a summary, and has lots of potential use cases,
  e.g. generating a web page with a table of version, querying it from pak
  when updating, etc.
- nightly builds: make the manual trigger (much) better: now we can select
  which archs and oses to build, and whether to deploy or not.
  This is really challenging to do with GHA's current syntax, which is
  pretty lacking, so it took a lot of tries.
- other nightly build fixes
- `push_packages()`: tag automatically based on version number. 9999 is rc,
  otherwise 4 parts is devel, 3 parts is stable.
- fix/reqrite `pak_update()` completely, now that I figured out how 
  stable/rc/devel should work
- rewrite the bundling on install completely, to make it as safe possible.
  It is also (somewhat) tested now.
- Fail `R CMD check` on failing tests. Is a good idea. There were basically
  no tests before, so it did not matter much.
- Fix test cases.
- Dev lib must be arch dependent. Only matters for dev using a multi-arch
  platform.
- Fix testing for dev lib setup. Now we always create dev lib at the start
  of the tests, unless private lib is embedded. A waste of time, but safer.
- Add `BuildResaveData: no` to `DESCRIPTION`. This is safer if CRAN or someone
  runs `R CMD build`.
- Fix `push_packages()` retry, there is another potential git error on which
  we need to retry.
- Update versioned dependencies.
- Work around URL error by ignoring README.md in package. We can't unclude
  the link to package manager otherwise.
- Update NEWS based on new embedded packages.
- pak is 0.2.1.9999 (RC) now
- investigating a nasty crash on aaarch64 Linux, in openssl, and another in
  libcurl

### https://github.com/r-lib/gitcreds/commits?author=gaborcsardi&since=2022-03-06&until=2022-03-13

- tidy upkeep and issue triage
- updates for `manager` not being the default credential helper on Windows 
  any more

### https://github.com/r-lib/cleancall/commits?author=gaborcsardi&since=2022-03-06&until=2022-03-13

- tidy upkeep and issue triage
- CRAN release 0.1.2

### https://github.com/r-lib/pkgbuild/commits?author=gaborcsardi&since=2022-03-06&until=2022-03-13

- tidy upkeep and issue triage

### https://github.com/r-lib/callr/commits?author=gaborcsardi&since=2022-03-06&until=2022-03-13

- tidy upkeep and issue triage

### https://github.com/r-lib/actions/commits?author=gaborcsardi&since=2022-03-06&until=2022-03-13

- temporarily fix release to 4.1.2, until our 4.1.3 Linux builds are ready

### https://github.com/r-lib/oskeyring/commits?author=gaborcsardi&since=2022-03-06&until=2022-03-13

- fix crash on macOS
- CRAN release 0.1.3

### https://github.com/r-lib/fs/commits?author=gaborcsardi&since=2022-03-06&until=2022-03-13

- two small PRs

### https://github.com/r-hub/sysreqsdb/commits?author=gaborcsardi&since=2022-03-06&until=2022-03-13

- small fix

## Issue discussions

Too many to collect now...

## community.rstudio.com

- help with four issues

## Issues and PRs

- investigating an rmarkdown issue, which turned out to be 
  https://github.com/rstudio/rmarkdown/issues/2324
- think about how we can depend on pak:
  https://github.com/r-lib/actions/issues/522
- think about smoother R release transition on GHA:
  https://github.com/r-lib/actions/issues/519
  https://github.com/r-lib/actions/issues/520
  https://github.com/r-lib/actions/issues/521

## Other

- Deleting UTM from both my macOS laptops, they just stopped working.
  Starting to use multipass instead.
