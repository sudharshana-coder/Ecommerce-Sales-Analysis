# E-Commerce Sales Data Cleaning and Visualization

## Project Overview
This project focuses on cleaning, analysing, and visualizing real-world e-commerce transaction data using Python. The objective is to identify data-quality issues, handle missing values and duplicates, investigate outliers, and discover business insights through data visualization.

## Dataset
- **Dataset:** Online Retail II
- **Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/502/online+retail+ii)
- **Period:** December 2009 – December 2011
- **Original Records:** 1,067,371
- **Columns:** 8

## Technologies Used
- Python 3.10
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- VS Code

## Data Cleaning
- Identified and removed 34,335 duplicate records.
- Filled 4,382 missing product descriptions with "Unknown".
- Retained missing Customer IDs.
- Excluded records with zero or negative quantities and non-positive prices from sales analysis.
- Converted Customer ID into a nullable integer type.
- Created a Sales column using Quantity × Price.

**Final cleaned records:** 1,007,914

## Outlier Detection
Used the Interquartile Range (IQR) method.

| Column | Outliers Identified |
|---|---:|
| Quantity | 53,061 |
| Price | 79,000 |
| Sales | 84,955 |

Outliers were identified but not automatically removed because some extreme values may represent genuine transactions.

## Visualizations
1. Monthly Sales Trend
2. Top 10 Products by Quantity Sold
3. Top 10 Countries by Sales (excluding the UK)
4. Distribution of Product Quantities
5. Distribution of Product Prices
6. Sales by Day of the Week

## Key Business Insights
- Total Sales: 20,476,634.02
- Total Invoices: 40,078
- Unique Products: 5,399
- Customers with an available ID: 5,878
- Top-selling Product: WORLD WAR 2 GLIDERS ASSTD DESIGNS
- Highest Sales Country: United Kingdom
- Best Sales Month: November 2011
- Highest Sales Weekday: Thursday
- Average Invoice Value: 510.92

*Sales values are in GBP. Returns, cancellations and non-positive prices are excluded from this sales analysis.*

## Conclusion
This project demonstrates how Python can transform raw e-commerce transaction data into meaningful business insights. It provided practical experience in data cleaning, exploratory data analysis, outlier detection, and data visualization.
