# Outliers vs normals (intraplate domain)

- Distance domain: dist_min_km ≥ 110 km
- Outlier flag: q ≥ 169 mW m⁻² (column: `outlier_relevant_lin`)
- Normals: 51,457
- Outliers: 1,963

## Non-parametric tests (log10 p-values)

_p-values are reported as log10(p) via Normal-tail mapping to avoid underflow._

| test                           |        stat |   log10_p | p_value_str   | note                              |
|:-------------------------------|------------:|----------:|:--------------|:----------------------------------|
| Mann–Whitney U                 | 0           | -1233.74  | < 1e-1234     | normal approx (no tie correction) |
| KS (q)                         | 1           |  -412.333 | < 1e-413      | asymptotic mapping                |
| Mann–Whitney U (log10 q)       | 0           | -1233.74  | < 1e-1234     | normal approx (no tie correction) |
| KS (log10 q)                   | 1           |  -412.333 | < 1e-413      | asymptotic mapping                |
| Mann–Whitney U (dist_km)       | 8.27386e+07 |  -503.515 | < 1e-504      | normal approx (no tie correction) |
| KS (dist_km)                   | 0.499847    |  -104.023 | < 1e-105      | asymptotic mapping                |
| Mann–Whitney U [log10(dist+1)] | 8.27386e+07 |  -503.515 | < 1e-504      | normal approx (no tie correction) |
| KS [log10(dist+1)]             | 0.499847    |  -104.023 | < 1e-105      | asymptotic mapping                |

## Effect size

- Cohen's d in log10(q): 2.225

## Notes

- Mann–Whitney U uses normal approximation (tie correction not applied here).
- KS uses asymptotic mapping for log10(p) reporting.
