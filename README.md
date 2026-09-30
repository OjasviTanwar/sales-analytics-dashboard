# Sales Analytics Dashboard

End-to-end sales analytics on a 3,900-row retail dataset: Python ETL, MySQL business queries, and an interactive Power BI dashboard.

## Dataset

`customer_shopping_behavior__1.csv` — 3,900 transactions × 18 columns: customer demographics (age, gender, location), product details (item, category, size, color, season), purchase amount, review rating, subscription status, shipping type, discounts, promo usage, payment method, and purchase frequency.

## What's Inside

| File | Description |
|------|-------------|
| `Customer_Shopping_Behavior_Analysis.ipynb` | Pandas ETL: null handling (median imputation of review ratings by category), snake_case standardization, feature engineering (age bands, purchase frequency in days), exploratory analysis |
| `customer_behavior_sql_queries.sql` | 10 business queries — revenue by gender, discount behavior, top-rated products, shipping comparison, subscriber spend, discount rates, customer segmentation (CTEs), top products per category (window functions), repeat-buyer analysis, revenue by age group |
| `customer_behavior_dashboard__1.pbix` | Interactive Power BI dashboard (19 visuals): customer counts, revenue, subscription mix, category/country/device breakdowns, slicers for filtering |

## Tech Stack

Python (Pandas, NumPy) · MySQL · Power BI

## Key Analyses

- Revenue comparison across gender, shipping type, and subscription status
- Discount effectiveness: which products sell most on discount
- Customer segmentation into New / Returning / Loyal via CTEs
- Top 3 products per category using `ROW_NUMBER()` window functions
- Repeat-buyer vs subscription correlation

## Author

Ojasvi Tanwar — B.Tech Computer Science & Engineering (2026)
