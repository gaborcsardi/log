
2022-06-06--2022-06-12

## Goals for the week:

- (Try to) finish error object rewrite, start updating other packages
- Fix the more serious rig issues that people found, release update

## GitHub

### r-lib/rig

- better `rig list`, print as table, print real version number as well:
  https://github.com/r-lib/rig/pull/91
- Refactoring for running R form rig
- Working of fixing `add-pak` to fix serious issue: 
  https://github.com/r-lib/rig/issues/84
  https://github.com/r-lib/rig/pull/92

### r-lib/processx, errors

- update `errors.R` in other packages: asciicast, pkgsearch, pkgdepends, callr
- release processx 3.6.0, with the new errors

### r-lib/pkgdepends

- Fix the annoying error when an installation plan failed without telling why:
  https://github.com/r-lib/pkgdepends/commit/84c87d81a3fd949061e92431adef2fce21e80b2b

### r-lib/pak

- Use new `errors.R` and give better errors

### r-lib/callr

- Big rewrite of errors, using new `errors.R`:
  https://github.com/r-lib/callr/pull/227
- Make traceback and frame dump optional, to finally fix
  https://github.com/r-lib/callr/issues/201
  https://github.com/r-lib/callr/commit/bf17b64dec4c8b23a28db16c23d31e97108ddc39

### r-lib/pkgcache

- Update bioc version
- Update `errors.R`

### r-hub/rhub-linux-builders

Update rchk to LLVM-12. We can finally reproduce CRAN's issues now (!!!).
