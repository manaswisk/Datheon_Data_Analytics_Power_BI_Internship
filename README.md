# Task 3: Customer Cohort \& Churn Analytics

## Project Overview

This project analyzes customer churn and retention patterns using the
IBM Telco Customer Churn dataset. The goal is to identify customer
groups with higher churn rates and recommend practical actions to
improve customer retention.

The analysis was completed using Python in Google Colab and an
interactive dashboard in Microsoft Power BI.

## Objectives

* Measure overall customer churn and retention rates.
* Segment customers by tenure groups.
* Compare churn across contract types and payment methods.
* Identify high-risk customer segments.
* Present findings through charts, a churn heatmap, and a Power BI
dashboard.
* Recommend data-informed customer retention strategies.

## Dataset

* **Dataset:** `telco\_customer\_churn.csv`
* **Source:** [Datheon -- Telco Customer Churn
Dataset](https://www.datheon.in/datasets/telco_customer_churn.csv)
* **Records:** 7,043 customers
* **Columns:** 21

The dataset includes customer demographics, subscribed services,
contract details, payment methods, tenure, monthly charges, total
charges, and churn status.

## Tools and Technologies

* Python
* Pandas and NumPy
* Plotly
* Google Colab
* Microsoft Power BI Desktop
* DAX

## Methodology

1. Loaded the Telco Customer Churn CSV dataset into Pandas.
2. Inspected the dataset structure, data types, missing values, and
duplicate rows.
3. Converted `TotalCharges` to numeric and handled blank values as
zero.
4. Calculated baseline churn and retention rates.
5. Grouped customers into tenure bands: 0--12, 13--24, 25--36, 37--48,
49--60, and 61--72 months.
6. Analyzed churn by contract type and payment method.
7. Compared churn rates across contract and payment method
combinations.
8. Created visualizations and exported analysis tables for reporting
and dashboard use.

**Cohort interpretation:** This dataset is a one-time customer snapshot.
The tenure groups in this project are tenure-based segments, not true
acquisition-month cohorts or month-by-month retention curves.

## Key Findings

Metric / Segment                                                Result

\---

Total customers                                                  7,043
Churned customers                                                1,869
Retained customers                                               5,174
Overall churn rate                                              26.54%
Overall retention rate                                          73.46%
Month-to-month contract churn                                   42.71%
One-year contract churn                                         11.27%
Two-year contract churn                                          2.83%
Electronic-check payment churn                                  45.29%
Highest-risk combination: month-to-month + electronic check     53.73%

### Tenure-Based Churn Pattern

Churn was highest among customers with 0--12 months of tenure
(approximately 47.4%) and declined across longer-tenure groups, reaching
approximately 6.6% for customers with 61--72 months of tenure.

## Power BI Dashboard

The Power BI report includes:

* KPI cards for Total Customers, Churned Customers, Churn Rate, and
Retention Rate.
* Customer churn rate by contract type.
* Customer churn rate by payment method.
* Customer churn rate by tenure cohort.
* Customer retention rate by tenure cohort.
* A matrix heatmap comparing churn by contract and payment method.
* Slicers for Contract, Payment Method, Gender, and Tenure Cohort.

## Strategic Retention Recommendations

1. **Improve early customer engagement:** Strengthen onboarding,
service education, and first-year support because churn is highest
among newer customers.
2. **Encourage longer contracts:** Test appropriate annual-plan
incentives and loyalty benefits for month-to-month customers.
3. **Investigate electronic-check churn:** Review the payment
experience and customer feedback, and make convenient automatic
payment options easy to adopt.
4. **Prioritize high-risk segments:** Focus retention outreach on
month-to-month customers using electronic checks, while evaluating
individual customer needs before offering incentives.
5. **Monitor retention performance:** Track churn and retention metrics
regularly and compare results across customer segments.

These findings show associations in the dataset; they do not establish
that contract type or payment method causes churn.

## Project Files

The project folder is intended to contain these deliverables (file names
may vary slightly depending on saved exports):

* `Task3\_Customer\_Cohort\_Churn\_Analysis.ipynb` --- Python analysis
notebook.
* `Task3\_Customer\_Churn\_Dashboard.pbix` --- Power BI report.
* `Task3\_Customer\_Churn\_Dashboard.pdf` --- exported dashboard report.
* `Task3\_Dashboard\_Screenshot.png` --- dashboard screenshot.
* `telco\_customer\_churn.csv` --- source dataset.
* `Task3\_Analysis\_Outputs.zip` --- exported analysis tables and
cleaned dataset.
* `README.md` --- project documentation.

The analysis ZIP contains the cleaned dataset and exported tables for
tenure cohort, contract churn, payment churn, high-risk segments,
retention recommendations, and heatmap data.

## How to Use

1. Download or clone the project files.
2. Open the `.ipynb` notebook in Google Colab or Jupyter.
3. Run the notebook cells in order. The notebook loads the source CSV
from the dataset URL shown in the notebook.
4. Open the `.pbix` file in Power BI Desktop to explore the dashboard
and slicers.
5. Refer to the PDF export and screenshot for a static view of the
dashboard.

## Conclusion

This project demonstrates an end-to-end customer churn analysis
workflow, from data inspection and preprocessing through segmentation,
visualization, and business recommendations. The results highlight the
importance of early customer engagement, contract strategy, and payment
experience in customer retention analysis.

\---

**Project:** Data Analytics Internship -- Task 3  
**Topic:** Customer Cohort \& Churn Analytics

