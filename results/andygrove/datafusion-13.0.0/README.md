# DataFusion 13.0.0 Benchmark Results

Notes

- DataFusion 13.0.0 uses a schema using Float64 rather than Decimal128

## SF=1 TBL, partitions=2

```bash
./target/release/tpch benchmark datafusion --query 1 --path ./benchmarks/data --format tbl --iterations 3 --debug
```

Results are average of 3 iterations.

| Query | Time    | Notes                                                       |
| ----- | ------- | ----------------------------------------------------------- |
| 1     | 4534.90 | Results not verified                                        |
| 2     | 1027.20 | Results not verified                                        |
| 3     | 3762.85 | Results not verified                                        |
| 4     | 3032.46 | Results not verified                                        |
| 5     | 3259.11 | Results not verified                                        |
| 6     | 3903.56 | Results are not correct due to rounding errors in predicate |
| 7     | 5650.35 | Results not verified                                        |
| 8     | 3277.19 | Results not verified                                        |
| 9     | 4540.22 | Results not verified                                        |
| 10    | 4123.24 | Results not verified                                        |
| 11    | 843.72  | Results not verified                                        |
| 12    | 3749.11 | Results not verified                                        |
| 13    | 624.44  | Results not verified                                        |
| 14    | 3202.08 | Results not verified                                        |
| 15    | 4402.84 | Results not verified                                        |
| 16    | 519.70  | Results not verified                                        |
| 17    | 7047.43 | Results not verified                                        |
| 18    | 5491.99 | Results not verified                                        |
| 19    | 3413.83 | Results not verified                                        |
| 20    | 3617.21 | Results not verified                                        |
| 21    | 4104.39 | Results not verified                                        |
| 22    | 503.52  | Results not verified                                        |

## SF=1 TBL, partitions=24

```bash
./target/release/tpch benchmark datafusion --query 1 --path ./benchmarks/data --format tbl --iterations 3 --debug --partitions 24
```

Results are average of 3 iterations.

| Query | Time    | Notes                                                       |
| ----- | ------- | ----------------------------------------------------------- |
| 1     | 4850.23 | Results not verified                                        |
| 2     | 931.62  | Results not verified                                        |
| 3     | 3872.02 | Results not verified                                        |
| 4     | 3076.35 | Results not verified                                        |
| 5     | 3296.85 | Results not verified                                        |
| 6     | 3914.90 | Results are not correct due to rounding errors in predicate |
| 7     | 4406.20 | Results not verified                                        |
| 8     | 3471.94 | Results not verified                                        |
| 9     | 4455.66 | Results not verified                                        |
| 10    | 4303.69 | Results not verified                                        |
| 11    | 835.63  | Results not verified                                        |
| 12    | 3812.34 | Results not verified                                        |
| 13    | 570.06  | Results not verified                                        |
| 14    | 3167.84 | Results not verified                                        |
| 15    | 4511.69 | Results not verified                                        |
| 16    | 448.15  | Results not verified                                        |
| 17    | 6091.42 | Results not verified                                        |
| 18    | 5132.89 | Results not verified                                        |
| 19    | 3595.37 | Results not verified                                        |
| 20    | 3427.55 | Results not verified                                        |
| 21    | 3838.73 | Results not verified                                        |
| 22    | 447.21  | Results not verified                                        |
