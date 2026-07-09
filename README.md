Overview

This project performs an Exploratory Data Analysis (EDA) on an e-commerce order dataset containing 1200 records. The goal is to understand the basic patterns, trends, and distributions in the data before any further modeling or visualization work. Analysis covers descriptive statistics, outlier detection, category breakdowns, missing value checks, correlation analysis, and revenue summaries.

Tools & Methods

All analysis was done in Excel using built-in formulas:
AVERAGE, MEDIAN — central tendency
QUARTILE — IQR-based outlier detection
COUNTIF, SUMIF, AVERAGEIF — category-wise counts and totals
COUNTBLANK — missing value checks
CORREL — correlation between Quantity and TotalPrice

Analysis Steps


Basic Statistics: Calculated mean, median, min, and max for Quantity, UnitPrice, and TotalPrice.
Outlier Check (IQR Method): Computed Q1, Q3, and IQR for TotalPrice to flag outliers outside the lower/upper limits.
Category Counts: Counted records by Product, Payment Method, and Order Status.
Missing Values Check: Verified completeness of key columns using COUNTBLANK.
Correlation: Measured the relationship between Quantity and TotalPrice.
Product-wise Totals: Aggregated quantity sold, total sales, and average price per product.
Order Analysis: Summarized total orders, revenue, and order value stats, broken down by order status and payment method.

Key Findings


TotalPrice is right-skewed: the mean (1053.97) is higher than the median (823.62), driven by a small number of high-value orders.
8 outliers were detected in TotalPrice using the IQR method (values above 3330.41), likely bulk orders or data entry errors.
No missing values were found in any of the key columns across all 1200 records.
Quantity and TotalPrice show a moderate positive correlation (r = 0.62).
Chair and Printer are the top-performing products by total sales; Desk has the lowest average price.
Cancelled orders generate the highest total revenue among all order statuses.
Revenue is fairly evenly distributed across the five payment methods (Debit Card, Online, Credit Card, Gift Card, Cash).

Outcome


The EDA confirmed that the dataset is clean and analysis-ready, with no missing values across all 1200 records. It revealed a right-skewed TotalPrice distribution with 8 statistical outliers, a moderate positive relationship between Quantity and TotalPrice (r = 0.62), and clear leaders in product sales (Chair and Printer). These insights provide a solid, validated foundation for the next phase of the project — visualization and deeper statistical modeling — without needing further data cleaning.
