# RSvgDevice

An R graphics device that writes plots as W3C Scalable Vector Graphics (SVG) files.

Compatibility updates by Renova.

Version 0.6.4.4.9001 replaces the deprecated `Calloc` memory macro with `R_Calloc` in `src/devSVG.c`, so the device builds with current R headers. No R function was changed.

## Install

```r
install.packages("RSvgDevice", repos = c(
  Renova = "https://renova-r.r-universe.dev",
  CRAN = "https://cloud.r-project.org"
))
```

Or install this exact release from its tag:

```r
install.packages("remotes")
remotes::install_github("renova-r/RSvgDevice@renova-0.6.4.4.9001")
```

[Release notes](NEWS.md) · [Renova package directory](https://github.com/renova-r/revival-catalog)

RSvgDevice is by T Jake Luciani, Matthieu Decorde (maintainer) and Vaudor Lise; the original project is at <https://github.com/mdecorde/RSvgDevice>. The device source retains its original notices (T Jake Luciani 2002, Tony Plate 2008, Matthieu Decorde 2012, and the R Core graphics code of Robert Gentleman and Ross Ihaka). License: GPL (>= 2); see [COPYING](COPYING).
