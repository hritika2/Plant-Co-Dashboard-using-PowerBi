# Plant Co. Dashboard using PowerBi

This project presents an end-to-end Power BI solution that transforms raw Excel sales data into a fully interactive analytical dashboard. The dashboard provides actionable insights into sales trends, profitability and account performance, enabling informed decision-making across product, customer, and geographic dimensions.

# Dataset Overview

### 1. Fact Table — fact_sales

  Contains transactional sales data, including:
  - Product ID
  - Sales Quantity
  - Sales Amount
  - Cost of Goods Sold (COGS)
  - Invoice Date
  - Account ID

### 2. Account Dimension — dim_account

Includes customer and geographic details such as:
- Account identifiers
- Location information
- Customer segmentation attributes

### 3. Product Dimension — dim_product

Provides a multi-level hierarchy for product-based analysis:
- Product Family
- Product Group
- Product Name
- Size
- Product Type

### 4. Date Dimension — dim_date

A custom date table covering Jan 2022 – Dec 2024, featuring:
- Calendar columns (Year, Month, Quarter)
- A calculated “in past” flag used for accurate YTD and PYTD logic

### 5. Values Table — dim_values

A helper table enabling dynamic metric selection between:
- Sales
- Gross Profit
- Quantity

# Dashboard Features

### Dynamic KPI Cards:

- Year-to-Date (YTD)
- Prior Year-to-Date (PYTD)
- YTD vs PYTD comparison
- Gross Profit Percentage (GP %)
- Conditional formatting to highlight positive/negative performance

### Interactive Slicers:

- Year selection
- Metric selector (Sales, Quantity, Gross Profit)
- Automatic title updates based on slicer choices

### Visuals Designed for Insight

1. Waterfall Chart
  Breaks down changes between YTD and PYTD to show contributing factors by product type or account.

2. Line & Stacked Column Chart
    Displays monthly performance trends with drill-down to quarter and month, enabling time-based comparison.

3. Tree Map
    Highlights bottom 10 countries by YTD vs PYTD, enabling focus on declining markets.

4. Scatter (Bubble) Chart
    Plots: Gross Profit % (Y-axis) and Selected measure (X-axis)
    Used to segment accounts based on profitability and sales levels, with average lines for benchmarking.
