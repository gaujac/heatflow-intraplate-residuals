# Regressions log10(q) × log10(dist_min_km + 1) by cluster (k=4)

- Intraplate subset: dist_min_km ≥ 110 km, q > 0.
- Features: log10(q), log10(dist_min_km + 1), scaled (StandardScaler), weights W_DIST=1.0, W_Q=1.0.
- K-Means: k=4, random_state=42, n_init=50.

| Cluster   |     N |   slope |   intercept |       r |      p |
|:----------|------:|--------:|------------:|--------:|-------:|
| 0         |  9341 |  0.0197 |      1.5100 |  0.0225 | 0.0300 |
| 1         | 16925 | -0.0375 |      2.0255 | -0.0658 | 0.0000 |
| 2         |  1484 |  0.0404 |      2.5630 |  0.0236 | 0.3632 |
| 3         | 25670 | -0.0840 |      2.0003 | -0.1264 | 0.0000 |
| Global    | 53420 | -0.1568 |      2.2263 | -0.2440 | 0.0000 |
