
# 2022-04-18 -- 2022-04-24

## GitHub, 75 commits in 13 repos

### https://github.com/r-lib/cli/commits?author=gaborcsardi&since=2022-04-17&until=2022-04-24

- `ansi_*()` functions handle hyperlinks now
- turning off ANSI colors also turns off hyperlinks
- related fixes in roxygen2 and testthat
- stop special casing Rstudio in `cli@@symbol`, it just made things worse
- submit new cli 3.3.0 to CRAN, stuck at a revdep false positive
- Add internal get_ppid() function: https://github.com/r-lib/cli/pull/453

### https://github.com/r-lib/ps/commits?author=gaborcsardi&since=2022-04-17&until=2022-04-24

- finish `ps_memory_full_info()`
- implement getting/setting the cpu affinity
- CRAN release 1.7.0

### https://github.com/r-lib/actions/commits?author=gaborcsardi&since=2022-04-17&until=2022-04-24

- fix release to 4.1.2 on Linux, temporarily

### https://github.com/r-lib/pak/commits?author=gaborcsardi&since=2022-04-17&until=2022-04-24

- use different tags for different arches for the builder containers,
  so all builds finally work well.

### https://github.com/r-lib/gh/commits?author=gaborcsardi&since=2022-04-17&until=2022-04-24

- small PR from Maelle: https://github.com/r-lib/gh/pull/167

### https://github.com/r-hub/macoscheck/commits?author=gaborcsardi&since=2022-04-17&until=2022-04-24

- fix R-hub's M1 builder, need to add R's arm64 binary directory to the PATH

### https://github.com/r-hub/node-rversions/commits?author=gaborcsardi&since=2022-04-17&until=2022-04-24

- fix windows URL, the tag is uppercase, the file name is lowercase, because
  why not?

### https://github.com/r-hub/rversions.app/commits?author=gaborcsardi&since=2022-04-17&until=2022-04-24

- use new rversions for the fix just above

### https://github.com/r-hub/api.app

- start reading about how we could do zero downtime deployments

### Other

- discussing RStudio environment detection:
  https://github.com/rstudio/rstudio/pull/11040
- discussion RStudio hyperlinks and ANSI colors:
  https://github.com/rstudio/rstudio/pull/11009
