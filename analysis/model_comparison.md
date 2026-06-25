# Model Comparison

I compared four simple models with one multiple regression model.

| Model | Variables used | R-squared | Useful variables | Business read |
| --- | --- | ---: | --- | --- |
| Simple: marketing spend | marketing_spend | 0.167 | marketing_spend | Useful as a single-driver check. |
| Simple: footfall | footfall | 0.736 | footfall | Useful as a single-driver check. |
| Simple: inventory availability | inventory_availability_pct | 0.013 | inventory_availability_pct | Statistically visible, but weak by itself. |
| Simple: customer rating | customer_rating | 0.001 | None at 5% | Weak alone; more useful after controls. |
| Multiple: sales drivers | marketing_spend, footfall, avg_discount_pct, staff_count, inventory_availability_pct, competitor_distance_km, holiday_flag, customer_rating, region_North, region_South, region_West, store_type_Airport, store_type_Mall, store_type_Residential | 0.855 | marketing_spend, footfall, staff_count, inventory_availability_pct, competitor_distance_km, holiday_flag, customer_rating, region_North, region_South, region_West, store_type_Airport, store_type_Mall, store_type_Residential | Best model for the recommendation. |

The multiple regression is the final model. It has the highest R-squared at 0.855 and compares store drivers in the same equation. The simple models are still useful because they show the raw one-variable relationship before controls are added.

Limitations:
- This is monthly store data, not a controlled experiment.
- Some variables may move together, so a coefficient should not be read as pure causation.
- The p-values are approximate normal-approximation p-values from the computed regression output, not a direct Excel ToolPak export.
