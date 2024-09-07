# E-Commerce Cohort Analysis

## Problem Statement

As e-commerce grows rapidly, traditional brick-and-mortar establishments must enhance their online efforts to compete with leaders like Amazon. To achieve this, understanding customer behavior through data analysis is crucial. This project focuses on cohort analysis to answer the following key questions:

1. How to interpret and clean e-commerce data effectively?
2. How to create a simple cohort analysis to compare metrics across different customer cohorts?

## Solution Overview

### Data Description

The dataset used for this analysis is sourced from the UCI Data Repository and includes 541,909 transactions from a UK-based non-store retailer specializing in all-occasion gifts.

### Approach

1. **Data Cleaning and Preparation**
   - **Handling Missing Data**: Removed records with missing customer IDs as they are essential for cohort analysis.
   - **Refunds Handling**: Separated refunds from the main dataset to ensure accurate sales metrics.
   - **Outliers Detection**: Filtered out extreme values in order quantities and unit prices. Removed non-product related entries such as 'DOTCOM POSTAGE' and 'CRUK Commission' to maintain data relevance.

2. **Feature Engineering**
   - **Total Order Amount**: Added a column for total order amount by multiplying unit price with quantity purchased.
   - **Invoice Period Label**: Created labels representing the year and month of each transaction.
   - **Customer Cohort Labels**: Assigned cohort labels based on the earliest purchase date of each customer.

3. **Cohort Analysis**
   - **Metric Aggregation**: Aggregated metrics across cohort groups and invoice periods to track customer activity over time.
   - **Cohort Duration Label**: Generated labels to represent the number of months since a customer’s first purchase for detailed analysis.

4. **Refund Analysis**
   - Analyzed refunds and cancellations to evaluate their impact on overall sales and customer metrics.

### Outcomes and Results

- **Data Cleanliness**: Enhanced data quality by addressing missing values, outliers, and irrelevant entries.
- **Customer Insights**: Provided valuable insights into customer behavior through cohort analysis, including average order values, retention rates, and customer lifetime value (CLV).
- **Refund Impact**: Identified significant refunds and their impact on sales figures, aiding in operational improvements.

#### Quantitative Results

- **Top Selling Items**: Identified the most significant products by total sales.
- **Average Unit Price**: Calculated the average unit price across different cohorts.
- **Retention Rates**: Analyzed customer retention rates by examining cohort behavior over multiple periods.
- **Refund Analysis**: Detailed significant refunds across various products, revealing insights into potential areas for improvement.
