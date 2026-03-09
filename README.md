# countyhealthR
An R package for programmatic access to archived County Health Rankings & Roadmaps (CHR&R) data, modeled after the simplicity of the `tidycensus` package.

[![CRAN Version](https://www.r-pkg.org/badges/version/countyhealthR)](https://cran.r-project.org/package=countyhealthR)
[![CRAN Downloads](https://cranlogs.r-pkg.org/badges/grand-total/countyhealthR)](https://cran.r-project.org/package=countyhealthR)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](https://countyhealthrankings.github.io/welcome/contribute.html#countyhealthr-package)

The current version of **countyhealthR** includes four functions to interact with CHR&R data:
1.  **list_chrr_measures**: see all the measures that are available for a selected release year.
2.  **get_chrr_measure_data**: download all data for a selected measure of health.
3.  **get_chrr_county_data**: download all measures for a selected geographic area.
4.  **get_chrr_measure_metadata**: access additional details about a selected measure, such as the measure's position within the [UWPHI Model of Health](https://www.countyhealthrankings.org/resources/2025-uwphi-model-of-health)

You can learn more about each function and its arguments by checking out the [reference manual](https://cran.r-project.org/web/packages/countyhealthR/countyhealthR.pdf).
---

## Install

### Install the stable CRAN version

```r
install.packages("countyhealthR")
```

### Install the development version (GitHub) 
```r
# install.packages("devtools") # if needed 
devtools::install_github("countyhealthrankings/countyhealthR")
``` 

## Quick Start 
```r
library(countyhealthR)

# Example: Load county-level premature death data for the 2024 release
get_chrr_measure_data(
  geography = "county",
  measure = "premature death",
  release_year = 2024
)
``` 
