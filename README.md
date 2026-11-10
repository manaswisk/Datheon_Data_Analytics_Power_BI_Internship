# Superstore Sales & Profit Executive Dashboard

## Project Overview

This project presents an interactive Power BI dashboard built using the
Superstore Retail Sales dataset. It provides an executive-level view of
sales performance, profitability, regional results, product performance,
and customer segments.

## Objectives

-   Summarize overall sales, profit, order volume, and profit margin.
-   Explore sales performance over time.
-   Compare profit across regions.
-   Analyze sales across product categories.
-   Highlight the top 10 products by sales.
-   Enable interactive exploration using report slicers.

## Tools & Technologies

-   Microsoft Power BI Desktop
-   Power Query for data preparation
-   DAX (Data Analysis Expressions) for measures
-   CSV dataset

## Dataset

**File:** `superstore_sales.csv`

The report uses the valid Superstore sales records after removing
appended non-sales rows during data preparation. The expected cleaned
dataset contains 9,994 sales rows and 21 columns.

The dataset's monetary values are presented in **US dollars (USD, \$)**.

## Dashboard Contents

### Key Performance Indicators

-   Total Sales
-   Total Profit
-   Total Orders
-   Profit Margin

### Visual Analysis

-   Sales performance over time
-   Profit by Region
-   Sales by Category
-   Top 10 Products by Sales

### Interactive Filters

-   Region
-   Category
-   Segment
-   Order Date

## DAX Measures

``` dax
Total Sales = SUM('superstore_sales'[Sales])

Total Profit = SUM('superstore_sales'[Profit])

Total Orders = DISTINCTCOUNT('superstore_sales'[Order ID])

Profit Margin = DIVIDE([Total Profit], [Total Sales], 0)

Total Quantity = SUM('superstore_sales'[Quantity])

Average Order Value = DIVIDE([Total Sales], [Total Orders], 0)

Total Customers = DISTINCTCOUNT('superstore_sales'[Customer ID])
```

## Validation Benchmarks

With all filters cleared and all 9,994 valid records included, the
expected results are:

  KPI               Expected value
  --------------- ----------------
  Total Sales       \$2,297,200.86
  Total Profit        \$286,397.02
  Total Orders               5,009
  Profit Margin             12.47%

## Project Files

Place these files in the project folder:

-   `Superstore_Dashboard.pbix` --- editable Power BI report
-   `Superstore_Dashboard.pdf` --- exported dashboard report
-   `dashboard_screenshot.png` --- dashboard preview image
-   `superstore_sales.csv` --- source dataset
-   `README.md` --- project documentation

## How to Use

1.  Open `Superstore_Dashboard.pbix` in Power BI Desktop.
2.  If prompted, locate `superstore_sales.csv` and update the data
    source path.
3.  Select **Refresh** if needed.
4.  Use the Region, Category, Segment, and Order Date slicers to explore
    the report.
5.  Clear slicer selections to return to the full-dataset KPI values.

## Notes

-   KPI validation values are expected values for the unfiltered
    dataset; selected slicers will change the results.
-   The report is intended for sales and profitability analysis and
    executive-level exploration.

## Author

Data Analytics Internship Project
