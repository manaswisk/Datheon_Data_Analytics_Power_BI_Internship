# Task 4: Corporate Financial & Profitability Performance Dashboard

## Project Overview

This project analyzes the Microsoft Financial Sample dataset using Power
BI. The dashboard presents sales, profit, discounts, cost of goods sold
(COGS), product performance, country performance, customer segments,
monthly trends, and an interactive sales-growth scenario.

## Dataset

-   **Source file:** `financial_sample.xlsx`
-   **Worksheet:** `Sheet1`
-   **Records:** 700
-   **Period covered:** 2013--2014
-   **Key fields:** Segment, Country, Product, Discount Band, Units
    Sold, Manufacturing Price, Sale Price, Gross Sales, Discounts,
    Sales, COGS, Profit, Date, Month Number, Month Name, and Year.

Blank values in `Discount Band` were labelled `Unknown` so that records
were retained.

## Dashboard Features

-   KPI cards for Total Sales, Total Profit, Total Gross Sales, Total
    COGS, Total Discounts, and Profit Margin.
-   Yearly Sales & Profit Performance.
-   Sales Performance by Country.
-   Sales by Product.
-   Sales & Profit by Customer Segment.
-   Monthly Sales Trend.
-   Sales & Profit by Discount Band.
-   Interactive slicers for Year, Country, Product, and Segment.
-   A What-if `Sales Growth %` parameter ranging from -20% to +20%.

## Key DAX Measures

The report includes measures for: - Total Sales, Total Profit, Total
Gross Sales, Total Discounts, and Total COGS. - Total Units Sold and
Total Transactions. - Profit Margin, COGS Ratio, Discount Rate, and
Gross Profit Margin. - Scenario Sales, Scenario Profit, Sales Variance,
and Sales Variance %.

### Scenario Analysis Assumption

Scenario Sales applies the selected growth rate to current Total Sales.
Scenario Profit applies the same growth rate to current Total Profit,
which assumes the current profit margin remains constant. This is a
what-if illustration, not a statistical forecast.

## Important Data Notes

-   The source dataset covers 2013--2014; the monthly trend reflects
    those historical records.
-   The dataset does not provide a separate budget or target field.
    Sales Variance is therefore calculated against actual sales using
    the user-selected what-if growth scenario, not against an externally
    supplied budget.
-   `Total Sales` is the net sales field after discounts. Gross Sales
    and Discounts are shown separately.
-   The `Gross Profit` measure in this report is calculated as net Sales
    minus COGS.

## Tools Used

-   Microsoft Power BI Desktop
-   Power Query for data preparation
-   DAX for measures and scenario calculations
-   Microsoft Excel (`.xlsx`) as the source dataset

## Deliverables

-   Power BI report:
    `Task4_Corporate_Financial_Performance_Dashboard.pbix`
-   PDF export: `Task4_Corporate_Financial_Performance_Dashboard.pdf`
-   Source dataset: `financial_sample.xlsx`

## Conclusion

The dashboard provides an interactive view of financial performance
across time, countries, products, and customer segments. The What-if
parameter allows users to explore the impact of different sales-growth
assumptions on projected sales and profit.
