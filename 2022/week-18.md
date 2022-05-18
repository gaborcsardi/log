
2022-05-02--2022-05-08

## Goals for the week:

- Put rim into better shape before showing it at the lab meeeting
- tidy upkeep for two packages

## GitHub

### r-lib/rim

- Lots of refactoring for more idiomatic rust code. Lots of rust learning.
- Implement `rim rstudio`
- Install pak by default, select version: 
  https://github.com/r-lib/rim/pull/47
- `rim switch` alias for `rim default`
- Make default in `rim ls`
- `rim system` prints help if no sub-command
- macOS: ignore `.DS_Store` files
- `rim system allow-debugger`: detect if R is not signed
- only cache downloaded files for a day
- `rim add` sets default if none is set
- add choco package
- `rim add` sets the CRAN mirror
- `rim add` sets up RSPM

### r-lib/archive

Release to make CRAN happy.

## Others

- Fix https://r-pkg.org, had to remove the READMEs temporarily because the
  machine that was producing them was hacked.
