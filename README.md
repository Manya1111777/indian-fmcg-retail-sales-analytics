# indian-fmcg-retail-sales-analytics
# Indian FMCG Retail Sales Analytics Dashboard

## 📊 Project Overview

This project analyzes **Indian FMCG retail sales data for 2024** to understand sales performance, revenue trends, profitability, customer behavior, and inventory-related patterns.

The project combines **Python, SQL, and Power BI** to demonstrate an end-to-end data analytics workflow.

> **Current status:** The Power BI dashboard is under development. Page 1 (Executive Overview) has been completed for the initial submission, and additional pages and refinements will be added.

---

## 🎯 Project Objectives

- Analyze overall retail sales and revenue performance
- Identify high-performing product categories and brands
- Compare online and offline sales channels
- Analyze profitability and overall margin
- Study monthly revenue trends
- Explore customer and loyalty-related patterns
- Analyze inventory and stock-related risks
- Build an interactive Power BI dashboard for business reporting

---

## 🗂️ Dataset

**Dataset:** Indian FMCG Retail Sales – Customer – Inventory (2024)

The dataset contains **100,000 retail transaction records** and **21 columns**.

### Key Columns

- `Invoice_ID` – Unique transaction identifier
- `Invoice_Date` – Transaction date and time
- `City` – Sales city
- `Store_Format` – Store type
- `Category` – Product category
- `Brand` – Product brand
- `Channel` – Online/Offline sales channel
- `Payment_Mode` – Payment method
- `Units` – Units sold
- `Cost_Price` – Product cost price
- `Selling_Price` – Product selling price
- `Revenue` – Transaction revenue
- `Cost` – Transaction cost
- `Margin` – Transaction margin
- `Margin_%` – Margin percentage
- `Stock_On_Hand` – Available stock
- `Reorder_Level` – Reorder threshold
- `Lead_Time_Days` – Inventory lead time
- `Customer_Age` – Customer age
- `Customer_Gender` – Customer gender
- `Loyalty_Flag` – Loyalty customer indicator

---

## 🧹 Data Cleaning & Preparation

Initial data exploration and cleaning were performed using **Python and Pandas**.

Key activities included:

- Checked dataset structure and data types
- Identified missing values
- Checked categorical values for consistency
- Checked for duplicate records
- Converted `Invoice_Date` to datetime format
- Handled missing `Customer_Gender` values by assigning `Unknown`
- Investigated missing `Customer_Age` values
- Checked numerical distributions and potential outliers
- Performed basic consistency checks between Revenue, Cost, and Margin
- Exported the cleaned dataset for further analysis

---

## 🐍 Python Exploratory Data Analysis

Python was used to explore the data and identify business patterns.

### Analysis Performed

- Revenue by product category
- Revenue and margin by brand
- Sales channel performance
- Customer gender analysis
- Revenue distribution and outlier analysis
- Category-level margin analysis
- Correlation analysis
- Loyalty vs non-loyalty customer analysis
- Monthly revenue trends

### Python Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## 🗄️ SQL Analysis

SQL was used to answer business-focused questions and perform aggregation-based analysis.

Key concepts applied:

- `SELECT` and `WHERE`
- `GROUP BY`
- `HAVING`
- Aggregate functions
- `COUNT` and `COUNT DISTINCT`
- `SUM`, `AVG`, `MIN`, `MAX`
- `CASE WHEN`
- Conditional aggregation
- Subqueries
- Percentage contribution
- Top-N analysis
- Sorting and filtering

---

## 📈 Power BI Dashboard

The Power BI report is being developed as a **3-page business dashboard**.

### Page 1 – Executive Overview

The current completed page provides a high-level view of business performance.

#### KPI Cards

- **Total Revenue:** 39.34M
- **Total Units Sold:** 300K
- **Total Cost:** 31.46M
- **Total Margin:** 7.87M
- **Overall Margin:** 20.02%

#### Visualizations

### 1. Monthly Revenue Trend

- Visual: Line chart
- X-axis: Month
- Y-axis: Total Revenue

**Business question:** How did revenue change over the year?

### 2. Revenue by Category

- Visual: Column chart
- X-axis: Category
- Y-axis: Total Revenue

**Business question:** Which product categories generate the most revenue?

### 3. Revenue by Channel

- Visual: Bar chart
- Category: Channel
- Value: Total Revenue

**Business question:** How does revenue compare across sales channels?

### 4. Top 5 Brands by Revenue

- Visual: Horizontal bar chart
- Category: Brand
- Value: Total Revenue

**Business question:** Which brands contribute the most revenue?

---

## 📌 Planned Dashboard Pages

### Page 2 – Sales & Customer Analysis

Planned analysis includes:

- Revenue by City
- Revenue by Store Format
- Payment Mode analysis
- Loyalty vs Non-Loyalty customers
- Customer Gender analysis
- Average Transaction Value

### Page 3 – Inventory & Business Insights

Planned analysis includes:

- Stock on Hand by Category
- Stock vs Reorder Level
- Low-stock products/brands
- Lead Time analysis
- Inventory risk indicators
- Business recommendations

---

## 🧮 Key DAX Measures

Example measures used in the Power BI dashboard:

```DAX
TOTAL_REVENUE = SUM('Table'[Revenue])

TOTAL_UNIT_SOLD = SUM('Table'[Units])

TOTAL_COST = SUM('Table'[Cost])

TOTAL_MARGIN = SUM('Table'[Margin])

OVERALL_MARGIN % = DIVIDE([TOTAL_MARGIN], [TOTAL_REVENUE])

Tools & Technologies
Tool	Purpose
Python	Data cleaning & exploratory data analysis
Pandas	Data manipulation
NumPy	Numerical analysis
Matplotlib	Data visualization
Seaborn	Statistical visualization
SQL	Business analysis & aggregation
Power BI	Interactive dashboard & reporting
Power Query	Data transformation
GitHub	Project documentation & portfolio
🔄 Project Workflow
Raw Dataset
     ↓
Python / Pandas
     ↓
Data Cleaning & EDA
     ↓
SQL Business Analysis
     ↓
Power BI / Power Query
     ↓
Dashboard
     ↓
Business Insights & Recommendations
