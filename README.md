# Sales & Performance Analytics Dashboard (Power BI)

## 📌 Project Overview
This is an **End-to-End Power BI Business Intelligence** project designed to replicate a real-world corporate analytics environment. The primary objective is to track and analyze the company's **Sales, Revenue, Profitability, and Time-Intelligence Trends (YTD, LY)**.

The project covers the entire BI lifecycle: from data transformation and building a clean **Star Schema Data Model** to creating advanced **DAX Measures** and delivering highly interactive, executive-level visualizations.

---

## 🏗️ Data Architecture & Modeling
To optimize dashboard performance and follow industry best practices, the data model is built using a **Star Schema (1:Many Relationships)**. This infrastructure ensures fast query processing and clean data granularity.

* **Fact Table (`FACT_SALES`):** Stores all core transactional metrics including `Gross_Revenue_INR`, `Net_Profit_INR`, `Product_Cost_INR`, and `Units_Sold`. It serves as the centralized repository for all explicit measures.
* **Dimension Tables (Lookup Tables):**
  * `DIM_PRODUCT`: Contains granular product details such as `Product_ID`, `Product_Name`, `Category`, and `Sub_Category`.
  * `DATE_CALNDER`: A dedicated, continuous date dimension table engineered to support precise time-intelligence calculations, linked to the fact table via a `1 to *` relationship.

---

## 📈 Key KPIs & Business Metrics Captured
The top analytical panel showcases high-level executive KPIs:
* **Total Profit:** ₹720.57M
* **Total Revenue:** ₹2.41bn
* **Total Units Sold:** 124K
* **Revenue YTD (Year-To-Date):** ₹1.26bn

---

## 📊 Analytical Insights & Visualizations
The layout is optimized for decision-makers to extract **Actionable Insights** instantly:
1. **Revenue YTD by Month (Bar Chart):** Tracks the month-on-month revenue acceleration and fiscal trends.
2. **Total Revenue by Product Name (Horizontal Bar Chart):** Identifies top-performing products, highlighting **Laptops** as the primary driver (₹1.3bn), followed by **Smartphones**.
3. **Total Profit by Sub-Category (Donut Chart):** Pinpoints profit centers, demonstrating that **Computers** and **Mobiles** drive over **52%** of the total ₹720.57M profit.
4. **Total Revenue by Category (Pie Chart):** Provides a portfolio overview, revealing that the **Electronics** segment dominates with **94.14%** of total revenue.
5. **YTD Revenue VS Previous Year (Matrix Table & Trend Line):** 
   * A critical time-intelligence visual comparing **Current Year YTD** against the **Previous Year (Revenue LY)** on a monthly granularity.
   * Enables stakeholders to monitor Year-over-Year (YoY) growth patterns and identify seasonal fluctuations.

---

## ⚡ Technical Skills Demonstrated
* **Data Cleaning & ETL:** Conducted data profiling, type casting, and schema validation inside **Power Query**.
* **Advanced DAX Formulas:** Implemented robust time-intelligence calculations:
  * Used `TOTALYTD` and `DATESYTD` expressions to capture dynamic financial year progress.
  * Leveraged `SAMEPERIODLASTYEAR` and `DATEADD` functions to benchmark performance against historical periods.
  * Formulated **Explicit Measures** instead of implicit ones to enforce analytical rigor and speed up report rendering.

---

## 🚀 How to Explore this Project
1. Download the `.pbix` file from this repository.
2. Open it using **Power BI Desktop**.
3. Interact with the dynamic **Year Slicers (2024, 2025)** located in the top-right corner to see the entire data model adjust instantly.

---
*Developed with a focus on Corporate Data Standards, Data Modeling Integrity, and Executive-Level Storytelling.*
