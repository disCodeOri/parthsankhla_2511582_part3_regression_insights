# Model Equations

## Simple Regression Equations
- Simple: marketing spend: monthly_sales = 560777.35 + 2.1296 * marketing_spend
- Simple: footfall: monthly_sales = 446410.58 + 35.6780 * footfall
- Simple: inventory availability: monthly_sales = 484814.26 + 2217.8319 * inventory_availability_pct
- Simple: customer rating: monthly_sales = 703800.86 + -5446.2660 * customer_rating

## Multiple Regression Equation
monthly_sales = 79601.24 + 1.2258 * marketing_spend + 27.1107 * footfall + -30937.3040 * avg_discount_pct + 3721.2197 * staff_count + 2785.9192 * inventory_availability_pct + -3524.8379 * competitor_distance_km + 14036.1537 * holiday_flag + 12753.2669 * customer_rating + 13670.8901 * region_North + 24922.2941 * region_South + 28392.3395 * region_West + 23957.2860 * store_type_Airport + 12091.5548 * store_type_Mall + -18644.0623 * store_type_Residential

## Dummy Variables
Region uses East as the reference category. Store type uses High Street as the reference category. I did not include every category, because that would duplicate the intercept and make the model redundant.

## Coefficient Read
The coefficient tells the expected change in monthly sales when that predictor increases by one unit, holding the other variables in the model constant.

Examples from the final model:

- One additional footfall unit is associated with about $27.11 more monthly sales, holding the other variables constant.
- One additional marketing-spend unit is associated with about $1.23 more monthly sales, holding the other variables constant.
- One more staff member is associated with about $3,721 more monthly sales, after controlling for the other store factors.
- One percentage-point-style increase in inventory availability is associated with about $2,786 more monthly sales in this model.
- One more kilometer of competitor distance is associated with about $3,525 lower monthly sales. I would treat this carefully because competitor distance may also be standing in for local market type.
- A holiday month is associated with about $14,036 higher monthly sales.
- One additional rating point is associated with about $12,753 higher monthly sales after controls. This is different from the simple model, where customer rating is weak by itself.
- North, South, and West stores are higher than East stores, with West the largest regional coefficient at about $28,392.
- Airport stores are about $23,957 higher than High Street stores, Mall stores about $12,092 higher, and Residential stores about $18,644 lower.

The largest standardized effects in the final model are footfall (0.652) and marketing_spend (0.237). These are the clearest drivers in this dataset. The p-values in the workbook are approximate normal-approximation p-values from the computed regression output, so I use them as a practical significance screen rather than as exact ToolPak output.

## Final Model Selected
I selected the multiple regression model. It explains more sales variation than the simple models and includes both numeric store drivers and dummy variables for store categories.
