# Cofactors (protocol-aligned)

## Availability

- ocean_age: MISSING/FAIL
- elevation: MISSING/FAIL
- litho_proxy: OFF/MISSING/FAIL
- is_land: not present

## Base protocol

- Cut: dist_min_km ≥ DIST_CUTOFF_KM km
- Rows after cut: 53420
- Rows after cofactor NA filtering: 53420

## Model

### OLS with spline bases (fallback)

- Predictors: logdist1 + (no extra cofactors)
- N: 53420
- R²: 0.068

#### Top terms by |t|

|              |         coef |         se_HC3 |   pval |
|:-------------|-------------:|---------------:|-------:|
| s_logdist1_5 | -0.325515    |    4.51511e-10 |      0 |
| s_logdist1_3 | -0.187817    |    4.31254e-10 |      0 |
| s_logdist1_6 | -0.303923    |    7.12273e-10 |      0 |
| s_logdist1_4 | -0.19739     |    4.65545e-10 |      0 |
| s_logdist1_2 | -0.120074    |    6.36442e-10 |      0 |
| s_logdist1_7 | -0.0917964   |    1.01756e-09 |      0 |
| s_logdist1_1 |  2.07502e+11 | 4541.16        |      0 |
| const        | -2.07502e+11 | 4541.16        |      0 |
