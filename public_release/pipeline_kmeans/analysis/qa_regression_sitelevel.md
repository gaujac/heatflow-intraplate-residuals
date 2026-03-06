# Site-level Regression QA Report

**Model:** `log10(q) ~ log10(dist_min_km + 1)`

- **Global β_logdist:** -0.1129
- **95% CI:** [-0.1161, -0.1096]
- **R²:** 0.096
- **N (sites used):** 58,032

## Sensitivity by grid size (snap to metric grid)

|   snap_km |   beta_logdist |   ci_low |   ci_high |     R2 |          N |
|----------:|---------------:|---------:|----------:|-------:|-----------:|
|    0.5000 |        -0.1233 |  -0.1266 |   -0.1200 | 0.1041 | 61062.0000 |
|    1.0000 |        -0.1129 |  -0.1161 |   -0.1096 | 0.0960 | 58032.0000 |
|    2.0000 |        -0.0970 |  -0.1002 |   -0.0938 | 0.0797 | 54199.0000 |

## Residual map

![Residual map](qa_residual_map.png)


## SR2 Panel

![SR2 panel](sr2_panel_density_and_residuals.png)
