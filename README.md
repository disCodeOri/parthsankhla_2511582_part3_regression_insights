# Part 3: Regression-Based Business Insights and Model Interpretation

## Business Problem
Leadership wants to know which store factors are most associated with monthly sales. The goal is to decide where to focus action: marketing, footfall, inventory, discounts, staffing, store type, or region.

## Dataset
- Source file: `data/business_regression_data.xlsx`
- Rows analyzed: 320
- Dependent variable: `monthly_sales`
- Optional secondary metric: `monthly_profit`

## Variables Reviewed
Numerical variables: marketing_spend, footfall, avg_discount_pct, staff_count, inventory_availability_pct, competitor_distance_km, holiday_flag, customer_rating.

Categorical variables: region, store_type.

Variables used mainly for ID or context: `store_id`, `month`, and `monthly_profit`.

## Regression Approach
I ran four simple regressions and one multiple regression. The multiple model includes at least three numerical predictors and dummy variables for region and store type.

## Dummy Variable Approach
Region uses East as the reference category. Store type uses High Street as the reference category. The reference category is left out so the model does not double-count categories.

## Model Comparison Summary
The final model is the multiple regression. It has R-squared 0.855 and adjusted R-squared 0.848. The strongest standardized effects are footfall and marketing_spend.

## Business Recommendation
Focus on the useful drivers from the multiple model and review the largest residual stores before taking action. The model is good for prioritization, but it is not causal proof.

## Assumptions and Limitations
- P-values are approximate.
- The data is observational.
- Some useful local factors may be missing.
- Dummy variables compare each category to the selected reference category.

## Screenshots Included
- `screenshots/simple_regression_output.png`
- `screenshots/multiple_regression_output.png`
- `screenshots/residuals_preview.png`
- `screenshots/model_comparison_preview.png`
