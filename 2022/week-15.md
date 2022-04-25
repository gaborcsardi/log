
# 2022-04-11 -- 2022-04-17

Mostly on holiday.

## GitHub, 38 issues in 8 repos

### https://github.com/r-lib/pak/commits?author=gaborcsardi&since=2022-04-10&until=2022-04-17

- push 'stable' packages to 'rc' as well, so now we have 
  stable <= rc <= devel, which makes a lot of sense
- CRAN release pak 0.3.0, now the windows and RSPM binaries all work fine
- investigating why we cannot build the builder containers is separate
  jobs, and the answer is simple. You cannot push arches separately into a
  multi-arch registry. Which is pretty messed up TBH. I'll have to use 
  different tags for different arches as a workaround.

### https://github.com/r-lib/ps/commits?author=gaborcsardi&since=2022-04-10&until=2022-04-17

- work on `ps_memory_full_info()`

### https://github.com/r-lib/archive/commits?author=gaborcsardi&since=2022-04-10&until=2022-04-17

- use new libarchive

## Other

- help Hadley with roxygen2 release
