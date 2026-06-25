# Final Recommendation

Use the multiple regression model as the main prioritization tool. It explains much more of the variation in monthly sales than the simple models, with R-squared of 0.855 and adjusted R-squared of 0.848. The simple footfall model is useful as a quick read, but the final model is better because it compares store conditions in the same equation.

The strongest driver is footfall. Its standardized effect is about 0.652, and one additional footfall unit is associated with about $27.11 more monthly sales, holding the other variables constant. Marketing spend is the second clearest driver, with a standardized effect of about 0.237 and about $1.23 more monthly sales per additional marketing-spend unit. These two variables should get the first leadership attention.

Recommended actions:
1. Protect high-footfall stores first. Check whether the best stores have enough staff, stock, and checkout capacity before adding more promotion.
2. Use marketing spend where the store already has enough footfall or a clear acquisition path. The model supports marketing, but footfall is the larger signal.
3. Review staffing and inventory next. Staff count and inventory availability both remain useful after controls, so weak stores may need operating fixes before more media spend.
4. Review store format and region effects. Airport and Mall stores are positive versus High Street, while Residential stores are about $18.6K lower than High Street after controls. West, South, and North are positive versus East in the final model.
5. Use the residual list for store audits. Stores far above prediction may have local practices worth copying; stores far below prediction need checks on inventory gaps, competitor pressure, local execution, and whether recorded footfall is converting.

Do not over-interpret average discount. Its final-model p-value is weak, so discounts should not be treated as the main lever from this analysis. Inventory availability is statistically visible in the simple model, but the simple R-squared is only 0.013, so inventory by itself explains little sales variation. Customer rating is weak alone, but becomes useful in the multiple model after controlling for store size, traffic, location, and format; that suggests ratings matter more as part of the store-quality picture than as a standalone explanation.

Regression shows association. It does not prove that changing one variable will automatically cause sales to move by the coefficient amount. Marketing, footfall, staffing, and inventory can influence each other, and some local store conditions are not in the file. My recommendation is to prioritize from the final model, then validate actions with controlled pilots or before-and-after tracking.
