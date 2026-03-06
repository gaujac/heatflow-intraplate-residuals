# Outlier categories summary

Protocol thresholds:
- THR_Q_RELEV = 169.0 mW m^-2
- THR_LOG_RELEV = 2.432
- DIST_CUTOFF_KM = 110.0 km

IQR thresholds computed on valid q>0 rows:
- IQR (linear) upper fence: q ≥ 169.0
- IQR (log10) upper fence : log10(q) ≥ 2.432 (~270)

| Category                   | Flag                 | Cutoff                  |   N_all |   pct_all |   N_dist_ge_cut |   pct_within_dist_domain |
|:---------------------------|:---------------------|:------------------------|--------:|----------:|----------------:|-------------------------:|
| IQR (linear q)             | outlier_linear       | q ≥ 169.0               |   10347 |    11.363 |            1963 |                    3.675 |
| IQR (log10 q)              | outlier_log          | log10(q) ≥ 2.432 (~270) |    5944 |     6.528 |             870 |                    1.629 |
| Extreme (q ≥ 1,000)        | outlier_extreme      | q ≥ 1,000               |    1568 |     1.722 |             226 |                    0.423 |
| Ultra-rare (q ≥ 100,000)   | outlier_ultrarare    | q ≥ 100,000             |      12 |     0.013 |              11 |                    0.021 |
| Relevant (q ≥ 169)         | outlier_relevant_lin | q ≥ 169                 |   10347 |    11.363 |            1963 |                    3.675 |
| Relevant (log10 q ≥ 2.432) | outlier_relevant_log | log10(q) ≥ 2.432        |    5944 |     6.528 |             870 |                    1.629 |
| Any (protocol/value-based) | outlier_any          | -                       |   10347 |    11.363 |            1963 |                    3.675 |
