# 📊 Amazon Sales Data Cleaning & Advanced Analysis in Excel
This project showcases how to clean, explore, and analyze Amazon sales data using
**Microsoft Excel**. It includes data wrangling, Pivot Table mastery, KPI creation, and dynamic reporting to turn raw data into actionable insights. --- 
## 📁 Table of Contents
1. [📘 Project Overview](#-project-overview)
 2. [🧹 Data Cleaning Process](#-data-cleaning-process)
3. [📈 Advanced Analysis & Insights (Pivot Table Breakdown)](#-advanced-analysis--insights-pivot-table-breakdown)
4. 4. [🛠️ Tools & Techniques Used](#️-tools--techniques-used)
 5. [🚀 Final Outcome](#-final-outcome)
 6. [📁 Folder Structure](#-folder-structure) 7. [📎 Resources & References](#-resources--references) --- ## 📘 Project Overview This case study demonstrates cleaning, segmenting, and analyzing an Amazon sales dataset in Excel. Key deliverables include: - 🧹 Data cleaning with Excel functions - 📊 Pivot table insights - 📌 KPI tracking - 📈 Chart visualizations - 📂 Actionable metrics for business use --- ## 🧹 Data Cleaning Process **Tools:** Microsoft Excel **Dataset:** Amazon Sales (Demo Case Study) ### ✅ Product Name - Original product names were long and inconsistent. - Used `=LEFT()` and `=PROPER()` functions to shorten and standardize. ### ✅ Category Column - Category, sub-category, and sub-subcategory were merged in one field. - Used **Text-to-Columns (Delimiter)** to split them into four distinct columns. ### ✅ Duplicate Records - Initial entries: **1,465** - After removing duplicates: **1,351 clean records** --- ## 📈 Advanced Analysis & Insights (Pivot Table Breakdown) ### 📊 Average Discount % by Category **Formula Used:** ```excel = (Actual Price - Discounted Price) / Actual Price * 100 

• Pivot Table: 

• Rows: Category 

• Values: Discount % → Average 

Evaluation:
Camera Accessories and Electronics offer the highest discounts, while Mobile Phones offer the least.
[See](Amazon Case Study 1.xlsx) 

🧮 Product Count by Category 

• Pivot Table: 

• Rows: Category 

• Values: Product Name → Count (Distinct) 

Evaluation:
Electronics and Home Appliances dominate in number, showing market preference.
[See](Amazon Case Study 1.xlsx)
⭐ Total Reviews per Category 

• Pivot Table: 

• Rows: Category 

• Values: Rating Count → Sum 

Evaluation:
Mobile Phones receive the most customer reviews despite fewer SKUs.
[See](Amazon Case Study 1.xlsx)
🥇 Top-Rated Products 

• Pivot Table: 

• Rows: Product Name 

• Values: Average Rating 

• Filter: Top 10 

• Sort: Largest to Smallest 

Evaluation:
Multiple products maintain ratings above 4.5, reflecting high satisfaction. 

💰 Average Actual vs Discounted Price by Category 

• Pivot Table: 

• Rows: Category 

• Values: Average Actual Price, Average Discounted Price 

Evaluation:
Mobiles and Electronics show large price drops due to aggressive discounting.
[See](Amazon Case Study 1.xlsx)
🏆 Most Reviewed Products 

• Pivot Table: 

• Rows: Product Name 

• Values: Rating Count → Sum 

• Filter: Top 10 

Evaluation:
These are likely Amazon's top-selling products.
[See](Amazon Case Study 1.xlsx)
🔻 Products with ≥ 50% Discount 

• Pivot Table: 

• Rows: Product Name 

• Values: Discount % → Sum 

• Applied filter: ≥ 50% 

• Set format: Percentage with 1 decimal 

Evaluation:
719 products have a discount of 50% or more — potential clearance or promo deals.
[See](Amazon Case Study 1.xlsx)
📉 Product Rating Distribution 

• Pivot Table: 

• Rows: Rounded Rating 

• Values: Product Name → Count 

Evaluation:
Majority of ratings cluster between 4.0–4.5 — showing general customer satisfaction.
[See](Amazon Case Study 1.xlsx)
📈 Potential Revenue by Category 

Formula: 

= Actual Price * Rating Count 

• Pivot Table: 

• Rows: Category 

• Values: Potential Revenue → Sum 

Evaluation:
Mobile Phones lead in potential revenue, followed by Electronics.
[See](Amazon Case Study 1.xlsx)
💵 Product Count by Price Bucket 

Formula: 

=IF(Discounted Price < 200, "<₹200", IF(Discounted Price <= 500, "₹200–₹500", ">₹500")) 

• Pivot Table: 

• Rows: Price Bucket 

• Values: Product Name → Count 

Evaluation:
Most products fall into ₹200–₹500 — mid-range pricing is popular. 

📊 Discount Level vs Rating Trend 

Formula for Buckets: 

=IF([@Discount%]<=10,"0–10%", IF([@Discount%]<=20,"11–20%", ...)) 

• Pivot Table: 

• Rows: Discount Bucket 

• Values: Average Rating 

• Chart: Line 

Evaluation:
No direct negative correlation between discount size and rating quality. 

Products with < 1,000 Reviews 

• Pivot Table: 

• Rows: Product Name 

• Values: Rating Count 

• Filter: < 1000 

Evaluation:
1351 products have low engagement — possibly new or under-marketed listings.
[See](Amazon Case Study 1.xlsx)
🏷️ Highest Discount by Category 

• Pivot Table: 

• Rows: Category 

• Values: Discount % → Max 

Evaluation:
Accessories show discounts up to 70% — indicates clearance sales.
[See](Amazon Case Study 1.xlsx)
🥇 Top 5 Products by Combined Score 

Score Formula: 

= Average Rating + (Rating Count / 1000) 

• Pivot Table: 

• Rows: Product Name 

• Values: Score 

• Filter: Top 5 

Evaluation:
Top performers combine excellent ratings with high review volumes.
[See](Amazon Case Study 1.xlsx)
🛠️ Tools & Techniques Used 

• Excel Functions: LEFT, PROPER, IF, calculated fields 

• Pivot Table Strategies: Top N filters, custom field settings, sorting 

• Charts: Line charts, Pie charts, Bar charts 

• Formatting: Custom percentage displays, conditional formatting, decimal precision 

• Data Cleaning Tools: Text-to-Columns, remove duplicates 

🚀 Final Outcome 

• ✅ Delivered an insightful Excel workbook for Amazon sales analysis 

• ✅ Built dynamic, interactive dashboards and KPIs 

• ✅ Identified high-performing products, pricing strategies, and review trends 

• ✅ Ready-to-present format for business or academic purposes
