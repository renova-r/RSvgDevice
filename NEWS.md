# RSvgDevice 0.6.4.4.9002

Platform compatibility patch to Renova release 0.6.4.4.9001, which is based on CRAN RSvgDevice 0.6.4.4 (archived on CRAN 2021-08-20).

- `src/devSVG.c`: `debug = FALSE;` (a logical assigned to the `int *` argument, flagged by clang `-Wnon-literal-null-conversion` on macOS) is now `debug = NULL;`. This is the same zero-pointer assignment written as an explicit null pointer constant, so the compiled behaviour is unchanged (including the existing edge case when `debug` is `NA`); it only silences the warning.
- `DESCRIPTION`: `Title` is now "An R SVG Graphics Device" (no trailing period, title case; R CMD check NOTEs). The `Date` field (2013-07-02, not read by any R code or help page) was removed because it made R CMD check report an outdated date. Metadata only.
- No R code, `NAMESPACE` or help page changed.
- `DESCRIPTION`: `Version` set to `0.6.4.4.9002`. `README.md` and `NEWS.md` updated.

# RSvgDevice 0.6.4.4.9001

Renova release, based on CRAN RSvgDevice 0.6.4.4 (archived on CRAN 2021-08-20).

- `src/devSVG.c`: `Calloc(1, NewDevDesc)` is now `R_Calloc(1, NewDevDesc)`.
- No R code, `NAMESPACE`, `DESCRIPTION` field or help page changed.
- `DESCRIPTION`: `Version` set to `0.6.4.4.9001`; "Compatibility updates by Renova." appended to `Description`.
- The stale `MD5` file was removed.
- `COPYING` (GNU GPL text) was added; the `License` field is unchanged.
- `README.md` was replaced by a short Renova README and `.Rbuildignore` keeps `README.md` and `NEWS.md` out of the built package.
