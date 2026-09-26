# SWYNEX-Exploratory-Data-Analysis

Task 2 of the SWYNEX Data Analyst Internship: perform exploratory data analysis on the cleaned dataset and identify useful insights.

## Dataset
- **Name:** Retail Store Sales (cleaned dataset from Task 1)
- **Size:** 11,971 rows x 11 columns (after cleaning)
- **Source file:** `cleaned_data.csv`

## Tools Used
Python, pandas, NumPy, Matplotlib, Seaborn (Google Colab)

## Approach
1. Loaded the cleaned dataset from Task 1.
2. Calculated summary statistics for the key numeric columns (price, quantity, total spent).
3. Analyzed revenue by category to see which categories perform best.
4. Compared Online vs In-store performance.
5. Studied payment method distribution.
6. Tracked monthly sales trends over time.
7. Detected outlier transactions using the IQR method.
8. Identified the best-selling items by quantity.
9. Measured the impact of discounts on average order value.

All charts referenced below are included as code output inside `EDA_Analysis.ipynb`.

## Key Statistics
- Average transaction value and quantity distribution were calculated using `describe()`.
- Dataset covers 200 unique items across 8 categories, 3 payment methods, and 2 sale channels (Online, In-store).

## Charts Included (in the notebook)
- Payment method distribution (pie chart)
- Monthly sales trend (line chart)
- Outlier detection for total spent (boxplot)
- Top 10 best-selling items by quantity (bar chart)
- Average transaction value: discount vs no discount (bar chart)

## Key Insights

1. **All three payment methods are almost equally popular.** Cash accounts for 34.3% of transactions, Digital Wallet for 32.9%, and Credit Card for 32.8%. Customers show no strong preference for any one payment method.

2. **There is no significant seasonal trend in sales.** Monthly sales fluctuated between roughly Rs. 35,000 and Rs. 50,000 from 2022 to 2025, with no consistent upward or downward pattern.

3. **60 outlier transactions were identified** using the IQR method, falling outside the normal range of -160.5 to 403.5. The most extreme values were concentrated in the Furniture category, reaching up to Rs. 410.

4. **Discounts have almost no impact on average order value.** The average transaction value with a discount applied is Rs. 130.49, compared to Rs. 129.95 without a discount, a difference of only Rs. 0.54. This suggests the current discount strategy is not driving higher spending per order.

5. **The single best-selling item is a beverage product (Item_2_BEV), with about 670 units sold**, and the top 10 list is otherwise dominated by Milk Products and Furniture items, showing these categories are popular by volume even though they do not lead in total revenue.

## Files in this Repository
- `cleaned_data.csv` - cleaned dataset used for analysis
- `EDA_Analysis.ipynb` - full analysis notebook (statistics, charts, code, and outputs)
- `README.md` - this file
