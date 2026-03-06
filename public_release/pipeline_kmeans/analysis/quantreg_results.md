# Quantile regression results

Model: `log10(q) ~ log10(dist_min_km + 1)`.

| domain      |    tau |    beta |   ci_low |   ci_high |     N | method   | note   |
|:------------|-------:|--------:|---------:|----------:|------:|:---------|:-------|
| continental | 0.5000 | -0.0642 |  -0.0663 |   -0.0621 | 54223 | QuantReg |        |
| continental | 0.9000 | -0.2182 |  -0.2225 |   -0.2140 | 54223 | QuantReg |        |
| global      | 0.5000 | -0.0876 |  -0.0895 |   -0.0857 | 91059 | QuantReg |        |
| global      | 0.9000 | -0.3224 |  -0.3270 |   -0.3178 | 91059 | QuantReg |        |
| oceanic     | 0.5000 | -0.1472 |  -0.1513 |   -0.1430 | 36836 | QuantReg |        |
| oceanic     | 0.9000 | -0.4132 |  -0.4237 |   -0.4027 | 36836 | QuantReg |        |
