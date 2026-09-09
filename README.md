# E-Commerce Sales Analytics & Performance Dashboard

## Project Overview
This project delivers an end-to-end data analytics workflow on an E-commerce sales dataset containing 1,200 transaction records. It encompasses data ingestion, automated cleaning, Exploratory Data Analysis (EDA), advanced data visualizations using Python (Pandas, Seaborn, Matplotlib), and an interactive Power BI Dashboard.

---

## Problem Statement
The primary goal is to analyze customer transaction behavior, evaluate product performance across sales channels, and identify key operational bottlenecks affecting revenue realization. The business currently suffers from a high cancellation/return rate, severely eroding bottom-line profitability.

---

## Dataset Description
- **Source:** `Dataset for Data Analytics.csv`
- **Volume:** 1,200 records | 14 variables
- **Key Columns:** `OrderID`, `Date`, `CustomerID`, `Product`, `Quantity`, `UnitPrice`, `ShippingAddress`, `PaymentMethod`, `OrderStatus`, `TrackingNumber`, `ItemsInCart`, `CouponCode`, `ReferralSource`, `TotalPrice`.

---

## Tools Used
- **Version Control:** Git & GitHub
- **Data Analysis & Cleaning:** Python (Pandas, NumPy) in Google Colab
- **Data Visualization:** Matplotlib, Seaborn
- **Business Intelligence:** Power BI Desktop (DAX, Slicers, Interactive Dashboards)

---

## Data Cleaning Process
1. **Missing Value Imputation:** Handled 309 missing values in `CouponCode` by filling them with `'None'` to explicitly reflect non-discounted transactions.
2. **Type Casting:** Converted string dates to proper `datetime64` data types for time-series aggregation.
3. **Integrity Audit:** Verified 0 duplicate rows across all 1,200 records.
4. **Export:** Exported sanitized output as `Cleaned_ECommerce_Dataset.csv`.

---

## Exploratory Data Analysis (EDA)
- **Descriptive Metrics:** Gross transaction volume reached **$1,264,761.96** with an Average Order Value (AOV) of **$1,053.97**.
- **Correlation Analysis:** Identified a strong positive correlation between `UnitPrice` and `TotalPrice` ($r = 0.72$), proving product price drives transaction value more significantly than volume ($r = 0.62$).
- **Outlier Detection:** IQR analysis identified 8 legitimate high-value transactions peaking at **$3,456.40**.

---

## Visualizations & Dashboard
- **Python Charts:** Evaluated monthly revenue trends, product category totals, order status distributions, AOV across payment options, and price-quantity relationships.
- **Power BI Dashboard (`(Week 6) Task 6.pbix`):** Features dynamic slicers, KPI summary cards, revenue trend lines, donut breakdowns, and channel column charts.

---

## Conclusion
By bridging Python-based statistical analysis with Power BI visual analytics, this capstone project pinpoints core operational vulnerabilities and provides a complete data pipeline to analyze sales revenue and customer transactions.
