# Amazon Product Pricing & Review Analytics

## Project Overview

This project analyzes Amazon product listings to understand pricing patterns, discounts, product categories, and customer ratings. Python was used for data cleaning, exploratory data analysis, and visualizations. SQL was used to investigate data quality and perform product-level and category-level analysis, while Microsoft Power BI was used to build an interactive dashboard.

## Objectives

- Analyze product listings across categories.
- Compare actual and discounted prices.
- Identify products with the highest listed discounts.
- Understand customer rating distributions.
- Explore the relationship between discounts and ratings.
- Clean duplicate records and validate data quality using SQL.
- Perform category-wise pricing and discount analysis.
- Rank products within categories using advanced SQL queries.

## Tools & Technologies

- **SQL:** SQLite, DB Browser for SQLite
- **Python:** Pandas, NumPy, Matplotlib, Seaborn
- **Environment:** Google Colab
- **Business Intelligence:** Microsoft Power BI
- **Data Transformation:** Power Query

## SQL Analytics

SQL was used to perform data validation, cleaning, and business analysis on the Amazon product dataset.

### SQL Tasks Performed

- Inspected table structure and column data types.
- Checked for missing and blank values.
- Identified duplicate product IDs and investigated exact duplicate records.
- Created a cleaned table named `amazon_clean`.
- Analyzed the top 10 products by listed discount percentage.
- Compared average discounts and ratings across product categories.
- Grouped products into discount ranges to compare average ratings.
- Calculated absolute price reductions from actual and discounted prices.
- Used Common Table Expressions (CTEs) and window functions to rank products within categories.

### SQL Data Cleaning Results

| Metric | Result |
|---|---:|
| Original records | 1,465 |
| Records after exact duplicate removal | 1,355 |
| Exact duplicate rows removed | 110 |
| Missing or blank values detected | 0 |

The original `amazon` table was preserved, and a separate `amazon_clean` table was created for analysis.

### Key SQL Findings

- Electronics contained 497 product listings in the broad-category analysis, with an average listed discount of 49.64% and average rating of 4.08.
- Home contained 451 product listings, with an average listed discount of 40.23% and average rating of 4.03.
- Products with discounts below 20% had an average rating of 4.14, while products with discounts between 20% and 49% had an average rating of 4.12.
- One Sony Bravia television listing had an actual price of ₹1,39,900 and a discounted price of ₹77,990, representing a listed price reduction of ₹61,910.

These findings describe the analyzed listings and do not establish that discounts cause changes in customer ratings or sales.

## Python Analysis

Python and Pandas were used to prepare and analyze the dataset. Exploratory data analysis and visualizations were created to investigate:

- Product category distribution.
- Actual versus discounted prices.
- Discount percentage distribution.
- Customer rating distribution.
- Relationship between discount percentages and ratings.
- Products with the highest listed discounts.

## Key Findings

- Electronics has the highest number of product listings in the category analysis.
- Average listed discount: approximately 47.69%.
- Average customer rating: approximately 4.10 out of 5.
- Discount percentage and rating have a weak negative correlation of approximately -0.155.
- Some listings have discounts between 90% and 94%.

The Python findings summarize the original analysis; the SQL findings reflect the cleaned table and the category grouping used in the SQL queries.

## Power BI Dashboard Features

The interactive dashboard includes:

- Total product count.
- Average customer rating.
- Average discount percentage.
- Average discounted price.
- Category-wise product analysis.
- Rating distribution.
- Actual versus discounted price comparison.
- Discount versus rating analysis.
- Top discounted products.

## Project Files

- `amazon_product_analysis.ipynb` — Python data cleaning, analysis, and visualizations.
- `Amazon_Product_Analytics.pbix` — Interactive Power BI dashboard.
- `amazon_ecommerce_analytics.sql` — SQL queries for data validation, cleaning, and business analysis.
- `Amazon_dashboard.png` — Power BI dashboard preview.

## Dataset

[Amazon Sales Dataset on Kaggle](https://www.kaggle.com/datasets/karkavelrajaj/amazon-sales-dataset)

The dataset contains product listing information, including product identifiers, categories, prices, discounts, and customer ratings.

## Limitations

- The dataset contains product listings and review information, not verified transaction records.
- Actual sales, revenue, profit, and purchasing behavior cannot be determined from these fields alone.
- Listed discounts do not necessarily represent actual customer savings.
- Customer ratings and discounts show an association in the analyzed data, not a causal relationship.
- Duplicate removal was based on identical records across the available columns; repeated product IDs were not automatically treated as duplicate records.

## Dashboard Preview

[View the Power BI Dashboard](https://github.com/vidya-cse-dev/amazon-product-pricing-analytics/blob/main/Amazon_dashboard.png)

[View Dashboard Image](https://github.com/vidya-cse-dev/amazon-product-pricing-analytics/raw/main/Amazon_dashboard.png)

## Conclusion

This project demonstrates an end-to-end product analytics workflow using Python, SQL, and Power BI. It combines data cleaning, exploratory analysis, SQL-based business queries, price and discount comparisons, and interactive visualization to derive insights from Amazon product listings.

## Author

[Vidya — GitHub Profile](https://github.com/vidya-cse-dev)
