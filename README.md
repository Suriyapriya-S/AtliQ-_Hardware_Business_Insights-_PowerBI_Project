# AtliQ-_Hardware_Business_Insights-_PowerBI_Project
### 📊 Business Intelligence Dashboard for AtliQ Hardware

**Project Overview:**

   This project simulates a full-scale Business Intelligence (BI) solution for **AtliQ Hardware**, a fictional tech-product company. AtliQ operates in multiple product categories — **Networking, Storage, Desktop, and Notebook** — and distributes products via **Direct, Distributor, and E-commerce channels** across various **regions and markets**.
_____________________________________________________________________________________________________________________________________________________________________________________________________________________
🧠 **Objective**
 
* ✅ **Deliver department-wise insights** through clean, interactive, and intuitive dashboards tailored to the needs of Finance, Sales, Marketing, Supply Chain, and Executive teams.
* 📊 **Enable data-driven decision-making** by visualizing key performance indicators (KPIs), sales trends, forecasts, regional comparisons, and profit/loss analytics.
____________________________________________________________________________________________________________________________________________________________________________________________________________________
📁 ***Dashboard Overview & Insights***

1. 🏠 **Home View**:

    * Central navigation page with clear section links to each dashboard view.
    * Includes Info & Support tabs via bookmarks.
    * Basic dataset and schema descriptions for user context.
     
    ![Image_Alt](https://github.com/Suriyapriya-S/AtliQ-_Hardware_Business_Insights-_PowerBI_Project/blob/9aee3f62eb2f2843e71cb224ee05da867aa8e062/Screenshot%202025-06-20%20190314.png) 
____________________________________________________________________________________________________________________________________________________________________________________________________________________
2. 💰 **Finance View**:
 
*Visuals*:

  * Cards for Net Sales, GM%, NP% (with conditional formatting) 
  * P&L Matrix (Current/LY/Target) 
  * Top/Bottom Products & Customers; Trend Area Chart.
  
 *Insights*:

* NS grew by 140–354% between 2019–2022.
* Despite NS growth, net profit has been negative since 2019, driven by high OpEx (likely linked to aggressive expansion).
  
![Image_Alt](https://github.com/Suriyapriya-S/AtliQ-_Hardware_Business_Insights-_PowerBI_Project/blob/2fd0cd09131b89ba18d68f1f236e93a3aa1f5c9a/Screenshot%202025-06-20%20190349.png) 
____________________________________________________________________________________________________________________________________________________________________________________________________________________

3. 📈 **Sales View**:
 
  *Visuals*:

 * Scatter Chart: Net Sales vs. Gross Margin % with dynamic GM% toggling for deeper profitability analysis.
 
 * Donut Charts: Percentage breakdowns of key metrics:
       Net Sales, Gross Margin, Pre‑ and Post‑Invoice Deductions, COGS (Cost of Goods Sold)
       
 * Matrix: Detailed customer & product-level view of Net Sales and Profitability for drill‑down analysis.

 *Insights*

 * Product Performance: Notebooks dominated product sales in 2022, contributing 42.5% of total sales.
 * Customer Analysis: Amazon topped customer Net Sales at $496.88M, while Relief showed higher GM%.


![Image_Alt](https://github.com/Suriyapriya-S/AtliQ-_Hardware_Business_Insights-_PowerBI_Project/blob/cb259a2f31e8a040c6d93421de84f129149c92a5/Screenshot%202025-06-20%20190413.png)

____________________________________________________________________________________________________________________________________________________________________________________________________________________

4. 📢 **Marketing View**:

 *Visuals*:

* Toggle-enabled Scatter Chart: Compare either Gross Margin % (GM%) or Net Profit % (NP%) against Net Sales.

* Waterfall Chart: Shows how Gross Margin turns into Net Profit after subtracting Operational Expenses (OpEx).

* Pie Chart: Shows the percentage split between Gross Margin and COGS (Cost of Goods Sold).

* Matrix: Shows sales performance across different segments and markets.

 *Insights*

 * In 2022, all regions had negative profitability because Operational Expenses (OpEx) were higher than Gross Margin (GM).

![Image_Alt](https://github.com/Suriyapriya-S/AtliQ-_Hardware_Business_Insights-_PowerBI_Project/blob/848b68979948272d9e95d4d5a13f2b11cabc4de1/Screenshot%202025-06-20%20190440.png)
____________________________________________________________________________________________________________________________________________________________________________________________________________________

5. 🚚 **Supply Chain View**:

*Visuals*:

* New card visuals for Forecast Accuracy %, Net Error, ABS Error.
 
* Matrix breakdown by Customer & Product.

* Line/Column charts for forecast metrics.
 
 *Insights*

* December 2021 had the highest net error with forecast accuracy at 81.5%.

* FY2021 had the highest absolute forecast error (~$10M).

![Image_Alt](https://github.com/Suriyapriya-S/AtliQ-_Hardware_Business_Insights-_PowerBI_Project/blob/34723cf6e4aded2996cea4d8808cae9abceb887e/Screenshot%202025-06-20%20190505.png)  

___________________________________________________________________________________________________________________________________________________________________________________________________________________

6. 🧑‍💼 **Executive View**:
 
 *Visuals*:

* Composite Cards: Show main KPIs with color indicators for growth or decline.

* Charts (Column, Line, Area, Ribbon, Bar): Show multi‑year trends and comparisons.

* Matrix: Shows performance by sub‑region and highlights top and bottom products/customers.

 *Insights*

* Retailers generated 70.5% of total revenue, and the P&A Division contributed about 49.9%.

* Even with some losses, the company managed to capture 6% market share by 2022 because of strategic growth efforts.

  ![Image_Alt](https://github.com/Suriyapriya-S/AtliQ-_Hardware_Business_Insights-_PowerBI_Project/blob/f144c7d115049a0fbd30e52fcad6f59bfeae1fde/Screenshot%202025-06-20%20190522.png)

___________________________________________________________________________________________________________________________________________________________________________________________________________________

🛠️ ***Technical Work & Implementation***


🔗 **Data Connectivity & Preparation**

 *  Connected a MySQL database to Power BI.
   
 *  Checked the data for mistakes, cleaned it, and created fact and dimension tables.
   
 *  Built a special date table with Fiscal Year and Fiscal Month columns.
   
 *  Double‑checked data accuracy using cross‑tab checks and UAT (User Acceptance Testing).
 
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

⚙️ **Data Modeling**

 * Created a snowflake schema with one‑to‑many relationships between tables.
   
 * Turned off loading of unnecessary tables to make the dashboard faster.
   
 * Added YTD (Year-to-Date) and YTG (Year-to-Go) columns to track sales progress.
   
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

📐 **DAX Measures**

Built 25+ custom DAX formulas to calculate:

*KPIs*: Net Sales, Gross Margin, Net Profit, Forecast Accuracy, Net Error, Absolute Error.

*P&L metrics*: Year-over-Year (YoY) changes, Operational Expense, Revenue Contribution %.

*Comparisons*: vs Last Year, vs Target.

*UX features*: Dynamic Titles, Slicer Labels, Toggle Measures, Quarter calculations.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

🧰 **Power BI Features & Tools Used**

*DAX Studio*: To improve performance and reduce file size.

*Bookmarks*: For toggling between views, info tabs, and interactive visuals.

*Dynamic Slicers*: For selecting benchmarks, products, or customer segments.

*Power BI Service*: Published the report, set up a gateway, enabled auto‑refresh, created an App workspace, and tested live data with Excel.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

📈 **Advanced Visuals Used**

  * Waterfall Chart, Ribbon Chart, Area & Line Charts.
   
  * KPI Cards with color indicators.
   
  * Matrix with dynamic column names.
   
  * Tooltips for detailed metrics.

 ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

🎓 **Learnings & Takeaways**

  * Gained hands‑on experience working like a real BI developer—managing stakeholder requests, UAT, and best practices.
   
  * Learned how to build strong data models, improve performance, and design clean visuals.
   
  * Improved skills in DAX to create advanced calculations and interactive dashboards.
