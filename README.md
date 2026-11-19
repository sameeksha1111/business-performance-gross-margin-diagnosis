# Maven Toys — Business Performance & Gross Margin Diagnosis | Python & Power BI

**An end-to-end retail business performance analytics project using Python, Pandas, Power BI, and DAX to investigate declining gross profit margins despite revenue growth, identify sales-mix drivers, and support data-driven business decisions.**

## 1. Project Overview

This project analyzes **829,262 historical sales transactions** from Maven Toys, a fictional toy retail chain operating across Mexico, covering January 2022 to September 2023.

I used **Python (Pandas and NumPy)** to inspect, clean, integrate, and analyze sales data, followed by **Power BI and DAX** to develop an interactive three-page business performance dashboard.

The analysis focuses on comparing **January–September 2022 with January–September 2023** to understand why revenue increased while gross profit margin declined.

The dashboard helps management monitor financial performance, explore category and store profitability, identify products contributing to margin deterioration, and evaluate opportunities to improve the sales mix.

## 2. Tech Stack

- **Python:** Data inspection, cleaning, integration, exploratory data analysis, and financial analysis.
- **Pandas:** Data validation, merging, grouping, aggregation, revenue-share comparisons, and profitability analysis.
- **NumPy:** Numerical analysis and product profitability classification.
- **Matplotlib:** Visualization of product-level margin contributions and sales-mix effects.
- **Power BI:** Interactive three-page dashboard and business performance reporting.
- **Power Query:** Data loading, transformation, and dimensional table preparation.
- **DAX:** Financial KPIs, year-over-year comparisons, revenue-share calculations, and gross margin decomposition.

## 3. Data Source

**Dataset:** Mexico Toy Sales

**Source:** Maven Analytics — Data Playground

**Dataset link:** [https://mavenanalytics.io/data-playground/mexico-toy-sales](https://mavenanalytics.io/data-playground/mexico-toy-sales)

The dataset contains historical sales, product, store, inventory, and calendar information for a fictional toy retailer operating in Mexico.

**Main source files:**
- `sales.csv`
- `products.csv`
- `stores.csv`
- `inventory.csv`
- `calendar.csv`
- `data_dictionary.csv`

**Sales records analyzed:** 829,262  
**Products:** 35  
**Stores:** 50  
**Data period:** January 2022 – September 2023

The analysis primarily uses sales, product, store, and calendar data. The source data was integrated and prepared using Python before being imported into Power BI.

The dataset was originally provided by Maven Analytics. This project uses a separately defined business problem focused on profitability and sales-mix changes.

## 4. Features & Highlights

### Business Problem

Maven Toys experienced revenue growth while its gross profit margin declined.

Although higher sales indicate growing business activity, declining margins suggest that the company is generating less gross profit relative to each dollar of revenue.

Without understanding the underlying drivers, management may prioritize revenue growth without recognizing changes in product and category profitability.

**Project Goal:** Identify why gross profit margin declined despite revenue growth, quantify the contribution of category and product sales-mix changes, and recommend three business actions to improve profitability.

### Python Data Preparation & Exploratory Analysis

**Data Preparation**

Used Python and Pandas to inspect and prepare the raw data for analysis.

- Examined dataset structure, data types, missing values, and duplicates.
- Validated numerical fields, transaction dates, and product/store identifiers.
- Standardized product prices, costs, and date columns.
- Integrated sales, product, and store datasets.
- Created calculated financial columns for Revenue, Cost of Goods Sold (COGS), and Gross Profit.
- Exported the prepared dataset for Power BI reporting.

**Analysis 1 — Category Profitability & Sales Mix**

Compared category-level revenue, gross profit margins, and revenue-share changes between January–September 2022 and 2023.

Identified categories gaining or losing revenue share and investigated whether the changing category mix was associated with declining company profitability.

**Analysis 2 — Product Profitability & Sales Mix**

Analyzed product-level revenue, gross profit margins, and changes in revenue contribution.

Identified products gaining or losing sales share and highlighted potential sources of margin dilution.

**Analysis 3 — Store-Level Profitability**

Compared store-level revenue contributions and gross margins across the two periods.

Investigated whether margin deterioration was concentrated in a few stores or observed more broadly across the store network.

**Analysis 4 — Gross Margin Contribution & Root-Cause Analysis**

Quantified the overall gross margin change and decomposed it into two components:

- **Category-Mix Effect:** Changes in revenue allocation between product categories.
- **Within-Category Product-Mix Effect:** Changes in the composition of products sold within each category.

Calculated individual product margin contributions in percentage points and validated that the decomposition reconciled with the overall company gross margin change.

### 5. Key Dashboard Visuals

**Page 1 — Executive Summary**

Provides a management-level overview of the profitability problem and recommended actions.

- **KPI Cards:** Total Revenue, Revenue Growth %, Gross Margin %, and Gross Margin Change (pp).
- **Gross Margin Drivers:** Summarizes the category-mix and within-category product-mix effects.
- **Key Product Findings:** Highlights major product-level contributors, including Colorbuds and Magic Sand.
- **Management Recommendations:** Presents three actions for investigating and improving the sales mix.

**Page 2 — Business Performance**

Explores revenue growth and profitability changes across months, product categories, and stores.

- **KPI Cards:** Total Revenue, Gross Profit, Gross Margin %, and Units Sold.
- **Monthly Revenue Trend:** Compares revenue performance across January–September 2022 and 2023.
- **Monthly Gross Margin Trend:** Shows changes in monthly profitability across the same periods.
- **Category Revenue Comparison:** Compares category sales performance between the two years.
- **Store Profitability Analysis:** Examines store revenue and gross margins to identify areas requiring investigation.

**Page 3 — Margin Root-Cause Diagnosis**

Investigates the factors contributing to the decline in company gross profit margin.

- **KPI Cards:** Gross Margin Change, Category-Mix Effect, and Within-Category Product-Mix Effect.
- **Product Margin Contribution Analysis:** Identifies products whose changes in sales share reduced overall profitability.
- **Gross Margin Decomposition:** Compares the category-mix and within-category product-mix effects.
- **Category Margin Drivers Matrix:** Displays category-level contributions to margin changes with conditional formatting.

### 6. Business Insights & Impact

The analysis revealed that Maven Toys' revenue increased by approximately **30.86%**, while its gross profit margin declined from **29.55% to 26.20%**, a decrease of **3.35 percentage points**.

The gross margin decomposition identified two primary drivers:

- **Category-Mix Effect:** Approximately −1.55 percentage points.
- **Within-Category Product-Mix Effect:** Approximately −1.79 percentage points.

Changes in product mix within categories had a slightly larger negative impact than changes in revenue allocation between categories.

At the product level, two significant negative contributors were:

- **Colorbuds (−2.675 pp):** A high-margin product that experienced a substantial decline in revenue share.
- **Magic Sand (−2.116 pp):** A lower-margin product that gained substantial revenue share.

Other product-level movements partially offset these negative contributions.

The store-level analysis also found that **49 out of 50 stores experienced gross margin deterioration**, indicating that the profitability issue was widespread across the retail network.

**Business Value:** The dashboard provides management with a consolidated view of revenue growth, profitability performance, and sales-mix drivers. It helps distinguish revenue growth from profitable growth and identify products, categories, and stores that warrant further investigation.

### Business Recommendations

**1. Investigate opportunities to recover high-margin product demand**

Examine the decline in Colorbuds' revenue share and identify opportunities to improve profitable sales through assortment, availability, and targeted marketing initiatives.

**2. Review the profitability of growing low-margin products**

Evaluate Magic Sand's pricing, promotional activity, and sales contribution to determine whether its growth can be supported while improving gross profit margins.

**3. Optimize category and store-level product assortment**

Use product profitability and margin-contribution analysis to identify opportunities to improve the sales mix across categories and stores without unnecessarily sacrificing revenue or demand.

These recommendations are proposed management actions based on historical findings and should be evaluated before implementation

### 7.screenshots
https://github.com/sameeksha1111/business-performance-gross-margin-diagnosis/blob/main/screenshots/summary.png - summary
