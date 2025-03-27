# mstats
`scipy.stats.mstats` as a separate package.

The SciPy project assigned "legacy" status to `scipy.stats.mstats` as of
SciPy version 1.16.0; the sub-package will no longer be developed, and all
functions will eventually be deprecated and removed. This `mstats` package
is provided separately to minimize disruption to dependent code: simply
install `mstats` and import functions from `mstats` instead of
`scipy.stats.mstats` to avoid the warnings and eventual errors.

Note that `scipy.stats.mstats` is no longer being developed due to serious
deficiencies, such as NumPy masked arrays automatically masking the result
of invalid operations that would otherwise result in NaNs. Code that uses
`mstats` will still be subject to these issues, whereas code that follows
the recommendations provided by `scipy.stats.mstats` deprecation messages
will be improved.

At this time, this project does not provide independent rendered documentation;
instead, see the rendered SciPy 1.15.2
[`scipy.stats.mstats`](https://docs.scipy.org/doc/scipy-1.15.2/reference/stats.mstats.html)
documentation.
