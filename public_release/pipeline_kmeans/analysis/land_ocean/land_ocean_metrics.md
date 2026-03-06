# Continental vs Oceanic comparison (land_ocean)

**Model:** correlation `log10(q)` vs `log10(dist_min_km + 1)` by domain.

**Land mask:** Natural Earth polygons loaded from local repository assets (no online downloads).

**p-values:** two-sided p computed in log-space with robust fallback (Student-t logsf; fallback Normal logsf for extreme tails).

- **Physical distance cut:** 110 km
- **Outlier threshold (global log-IQR):** log10(q) ≥ 2.432

| domain      |   N_total |   N_used_reg |   r_log10q__log10dist1 |   log10_p_value | p_value_str   |   outliers_logIQR_ge110_pct |   q_median_mWm2 |   q_p90_mWm2 |   dist_min_median_km |
|:------------|----------:|-------------:|-----------------------:|----------------:|:--------------|----------------------------:|----------------:|-------------:|---------------------:|
| continental |     54223 |        54223 |                -0.2952 |      -1125.7137 | < 1e-1126     |                      0.3375 |         64.0000 |     127.4000 |             205.7909 |
| oceanic     |     36836 |        36836 |                -0.3273 |       -961.2438 | < 1e-962      |                      1.8650 |         71.0000 |     295.0000 |             153.5227 |
