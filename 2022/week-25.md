
2022-06-20--2022-06-26

## Goals for the week:

- Start releasing packages with new `errors.R`, really
- R release this week:
  * actions
  * R-hub

### r-lib/callr

- Issue triage, prepare for release

### r-lib/asciicast

- Complete rewrite of recording with embedded R process. This has lots of
  advantages:
  * easier recording
  * potential Windows support
  * more accurate recording, separate input, output, prompt
  * faster recording, no need to do it in real time any more
  https://github.com/r-lib/asciicast/pull/31
- SUpport themes for SVGs as well.
- Better defaults for asciicast in knitr

### r-lib/processx

- Cross platform FIFO implementation to help with asciicast on Windows:
  https://github.com/r-lib/processx/pull/340

### r-lib/actions

- v2.2.3, to temporalily fix the R version to 4.2.0 for Linux
