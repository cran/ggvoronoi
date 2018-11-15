# ggvoronoi: Voronoi Diagrams and Heatmaps with 'ggplot2'

## Overview

'ggvoronoi' is an R package that allows for easy creation and manipulation of Voronoi diagrams, which are tools for determining nearest neighbor regions for a given set of points. 
Voronoi diagram regions are calculated using the R package 'deldir' by Rolf Turner. 
The output from 'deldir' is converted to the spatial object format provided by the 'sp' package from Edzer Pebesma and Roger Bivand.
This allows for additional functionality beyond what is provided in 'deldir': diagrams can now be extended to heatmaps and users can now specify a bounding region for the diagram.
From there, visualization capabilities are implemented using the framework of 'ggplot2', a popular graphics package for R created by Hadley Wickham, 
or the user can analyze the diagram using any of R's spatial data analysis packages.

## Installation

To install 'ggvoronoi' from CRAN:

```r
install.packages("ggvoronoi")
```

Or install the latest development version from this repository:

```r
devtools::install_github("garretrc/ggvoronoi",build_vignettes = TRUE)
```

Finally, with either verison you can load the R package with the typical method:

```r
library(ggvoronoi)
```

## Getting Started

With the vignette, you can view some examples and create your first Voronoi diagram!

```r
vignette("ggvoronoi")
```

Alternatively, the vignette is available [here.](http://htmlpreview.github.io/?https://github.com/garretrc/ggvoronoi/blob/master/vignettes/ggvoronoi.html)

## Contact info

For questions about usage/syntax or for reporting bugs, email Robert Garrett at garretrc@miamioh.edu or raise an issue on this repository. 

To contribute to the package, follow the procedures outlined in CONTRIBUTING.md

## Changes

v0.8.2: Added unit tests using 'testthat' and 'vdiffr'. Minor improvements to vignette and README.md

v0.8.1: Fixed bug when using a discrete value for fill mapping. Removed google maps API call in the vignette.
