## Resubmission

This is a resubmission. The following changes were made in response to CRAN feedback:

* Examples that download data from Zenodo are wrapped in `\donttest{}` as recommended.
* A CRAN-safe caching mechanism was implemented so that during checks data are written only to `tempdir()`, while users can optionally cache data locally outside of CRAN environments.

## R CMD check results

0 errors | 0 warnings | 1 note

* checking for future file timestamps ... NOTE
  unable to verify current time

This NOTE is a known harmless issue related to time verification on some systems and does not affect package functionality.

## Downstream dependencies

None.
