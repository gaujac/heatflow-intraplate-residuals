# Random-lines placebo vs. real distance model

Pearson correlation between `log10(q)` and `log10(distance + 1)`.

p-values computed in log-space (two-sided) to avoid underflow.

| config               |         r | p_value_str   |      log10_p |     slope |   intercept |     N |
|:---------------------|----------:|:--------------|-------------:|----------:|------------:|------:|
| REAL_min(GEM,PB2002) | -0.295073 | < 1e-1888     | -1887.838424 | -0.129227 |    2.156366 | 91059 |
| PLACEBO_random_lines | -0.299199 | < 1e-1947     | -1946.165944 | -0.129248 |    2.067463 | 91059 |
