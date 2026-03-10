## Resubmission

This resubmission addresses a NOTE raised by CRAN's incoming checks
indicating that more than two CPU cores were used during examples.

The cause was multithreaded parsing in readr when reading CSV files.  
`read_csv_zenodo()` now explicitly sets `num_threads = 1` to ensure single-threaded execution.

All examples that require internet access are wrapped in `\donttest{}` to comply with CRAN policies.

## R CMD check results

0 errors | 0 warnings | 1 note

* checking for future file timestamps ... NOTE
  unable to verify current time

This NOTE is a known harmless issue related to time verification on some systems and does not affect package functionality.

## Downstream dependencies

None.
