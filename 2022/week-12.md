
# 2022-03-21 -- 2022-03-27

## GitHub, 79 commits in 15 repositories

### https://github.com/r-lib/processx/commits?author=gaborcsardi&since=2022-03-20&until=2022-03-27

- investigating interrupt issues on Windows, in the end there is nothing
  we can do to fix the weird exit status in powershell
- avoid short path for `wd` on Windows to fix
  https://github.com/r-lib/processx/issues/313
- fix many test cases on Windows
- docs updates
- CRAN release 3.5.3

### https://github.com/r-lib/rim/commits?author=gaborcsardi&since=2022-03-21&until=2022-03-27

- Build R on arm64 using https://github.com/rstudio/r-builds, all R 
  versions from R 3.3.0, put at at https://github.com/r-hub/R/releases
  They are not auto-built yet.
- Support arm64 Linux in rim, using the builds above.
- Update `system add-pak` to allow arm64 Linux.
- Better R-devel URLs on macOS.
- Add Debian 11 support.
- Clean up on self-hosted runner.
- Add Rtools42 support.
- Support deleting rtools with `rim rm`
- Update docs.
- Release rim 0.2.1.

### https://github.com/r-lib/pak/commits?author=gaborcsardi&since=2022-03-20&until=2022-03-27

- suffering with crashes on arm64 Linux. Seems to work now, with some 
  openssl and libcurl tinkering.
- update deploy process to make latest build compatible with R-devel

### https://github.com/r-hub/cranatgh/commits?author=gaborcsardi&since=2022-03-20&until=2022-03-27

- fix all failed packages at https://github.com/cran

### https://github.com/r-lib/fs/commits?author=gaborcsardi&since=2022-03-20&until=2022-03-27

- small PR

### https://github.com/r-lib/crayon/commits?author=gaborcsardi&since=2022-03-20&until=2022-03-27

- small build bug fix
- CRAN version 1.5.1

### https://github.com/r-hub/rtools42/commits?author=gaborcsardi&since=2022-03-20&until=2022-03-27

- create a repo for Rtools42, with a stable download URL, at 
  https://github.com/r-hub/rtools42/
- setup a watch for the CRAN web page, so when they have a new Rtools42 
  build, I can update this manually

### https://github.com/r-hub/r-minimal/commits?author=gaborcsardi&since=2022-03-20&until=2022-03-27

- fix download URL again, this time for R-devel

## community.rstudio.com

helped with one issue

