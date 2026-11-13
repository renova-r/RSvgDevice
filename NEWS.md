# RSvgDevice 0.6.4.4.9001

Renova release, based on CRAN RSvgDevice 0.6.4.4 (archived on CRAN 2021-08-20).

- `src/devSVG.c`: `Calloc(1, NewDevDesc)` is now `R_Calloc(1, NewDevDesc)`.
- No R code, `NAMESPACE`, `DESCRIPTION` field or help page changed.
- `DESCRIPTION`: `Version` set to `0.6.4.4.9001`; "Compatibility updates by Renova." appended to `Description`.
- The stale `MD5` file was removed.
- `COPYING` (GNU GPL text) was added; the `License` field is unchanged.
- `README.md` was replaced by a short Renova README and `.Rbuildignore` keeps `README.md` and `NEWS.md` out of the built package.
