## Vendor_Performance_Analysis
### 📊 Project Overview
This project provides an end-to-end data-driven evaluation of vendor performance for a retail/wholesale environment. By combining Python-based data cleaning with Interactive Tableau Dashboard, the analysis identifies key financial trends, inventory risks, and high-potential brands.

The primary goal is to move beyond basic sales tracking and use statistical thresholds to categorize vendors by their efficiency and scale, then guide strategic marketing and procurement decisions.

<a href="[https://public.tableau.com/app/profile/tran.le6814/viz/VendorPerformanceDashBoard_17417387208030/VendorPerformanceDashboard](https://public.tableau.com/app/profile/tran.le2329/viz/VendorPerformanceDashBoard/Dashboard2?publish=yes)" target="_blank">
  <img src="https://img.shields.io/badge/View%20Live%20Dashboard-Tableau-blue?style=for-the-badge&logo=tableau" alt="Tableau Dashboard">
</a>

### 🛠️ Tech Stack
+ Data Processing: Python (Pandas, NumPy, Scipy)
+ Business Intelligence: Tableau Desktop
+ Database Management: Custom Python ingestion scripts (ingestion_db.py)
+ Environment: Jupyter Notebook, macOS (Apple Silicon), Git/GitHub

### 📂 Repository Structure
**Vendor Performance Analysis.ipynb**: Core analytical notebook containing data cleaning, outlier detection, and the calculation of performance tiers.
**Exploratory Data Analysis.ipynb**: Initial discovery phase focused on distribution of sales, profit margins, and correlation analysis.
**get_vendor_summary.py**: Modular script used to aggregate raw transaction data into vendor-level summaries.
**EDA insights.docx.pdf**: Executive summary documenting key business findings and strategic recommendations.

### 📈 Key Analytical Features
#### 1. Operational KPIs
The analysis tracks five critical metrics displayed in the dashboard:
Total Sales: $441.41M
Total Purchase: $307.34M
Gross Profit: $134.07M
Average Profit Margin: 38.72%
Unsold Capital: $2.71M 

#### 2. Performance Tier Logic
Using advanced calculations in Tableau and Python, vendors are categorized dynamically:
High-Potential Brands: Brands in the bottom 15% of sales volume but the top 15% of profit margin. These represent high-efficiency growth opportunities.
Standard Performers: Brands maintaining consistent volume and average market margins.

#### 3. Interactive Visualizations
The dashboard includes:
Viz-in-Tooltip: Hovering over a brand in the scatter plot reveals a secondary chart of "Sales by Order Size."
Highlight Actions: Selecting a top vendor automatically highlights their specific brands across all performance charts.

### 💡 Strategic Insights
Identified $2.71M in capital currently tied up in slow-moving inventory.
Discovered that Diageo North America leads in total contribution (24.81%), but smaller vendors like M S Walker Inc show higher potential for margin-driven growth.
Streamlined the ingestion of raw vendor data into a clean, queryable format using automated Python scripts.
