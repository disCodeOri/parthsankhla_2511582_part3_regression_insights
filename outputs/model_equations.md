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

The largest standardized effects in the final model are footfall (0.652) and marketing_spend (0.237). These are the clearest drivers in this dataset.

## Final Model Selected
I selected the multiple regression model. It explains more sales variation than the simple models and includes both numeric store drivers and dummy variables for store categories.
