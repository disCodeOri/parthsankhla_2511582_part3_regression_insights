# Residual Analysis

Residual = actual monthly sales minus predicted monthly sales.

## Largest Positive Residuals
| Store | Region | Store type | Actual sales | Predicted sales | Residual |
| --- | --- | --- | ---: | ---: | ---: |
| STR-1058 | East | High Street | $870,937 | $759,933 | $111,005 |
| STR-1028 | East | Mall | $713,611 | $606,267 | $107,344 |
| STR-1073 | East | Residential | $813,317 | $721,217 | $92,099 |
| STR-1026 | East | Mall | $625,514 | $535,396 | $90,118 |
| STR-1051 | East | Airport | $787,716 | $700,456 | $87,260 |

These stores sold more than the model expected. They may have local advantages not captured in the dataset, such as store execution, nearby events, better merchandising, or stronger repeat customers.

## Largest Negative Residuals
| Store | Region | Store type | Actual sales | Predicted sales | Residual |
| --- | --- | --- | ---: | ---: | ---: |
| STR-1023 | South | Mall | $627,172 | $765,512 | $-138,340 |
| STR-1012 | West | Residential | $595,468 | $713,206 | $-117,738 |
| STR-1017 | West | High Street | $685,379 | $801,191 | $-115,812 |
| STR-1007 | West | Mall | $800,452 | $916,051 | $-115,599 |
| STR-1060 | West | Mall | $721,079 | $808,713 | $-87,633 |

These stores sold less than expected. I would check local inventory problems, competitor activity, staffing quality, and whether the recorded footfall turned into actual purchases.

The residuals do not show one single store type that the model always misses. They do show that some store-months are far from the fitted line, so the model is a guide, not a replacement for store-level review.
