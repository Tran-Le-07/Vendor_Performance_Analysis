## Vendor_Performance_Analysis
### 📊 Project Overview
This project provides an end-to-end data-driven evaluation of vendor performance for a retail/wholesale environment. By combining Python-based data cleaning with Interactive Tableau Dashboard, the analysis identifies key financial trends, inventory risks, and high-potential brands.

The primary goal is to move beyond basic sales tracking and use statistical thresholds to categorize vendors by their efficiency and scale, ultimately guiding strategic marketing and procurement decisions.

[🔗 View Interactive Vendor Performance Dashboard](https://public.tableau.com/views/VendorPerformanceDashBoard/Dashboard2)

### ❓Business Problem
**Effective inventory and sales management are critical for optimizing profitability in the retail/wholesale industry. Companies need to ensure that they are not incurring losses due to inefficient pricing, poor inventory turnover, or vendor dependency.**
**The goal of this analysis is to:**
+ Identify underperforming brands that require promotional or pricing adjustments.
+ Determine top vendors contributing to sales and gross profits.
+ Analyze the impact of bulk purchasing on unit costs.
+ Assess inventory turnover to reduce holding costs and improve efficiency.
+ Investigate the profitability variance between high-performing and low-performing vendors.

### 🛠️ Tech Stack
+ **Data Processing**: Python (Pandas, NumPy, Scipy)
+ **Business Intelligence**: Tableau Desktop
+ **Database Management**: Custom Python ingestion scripts (ingestion_db.py)
+ **Environment**: Jupyter Notebook, macOS (Apple Silicon), Git/GitHub

### ⚙️ Project Pipeline
+ **Data Ingestion**: Automated Python scripts aggregate raw transaction logs into vendor-level summaries.
+ **Exploratory Data Analysis (EDA)**: Statistical profiling of sales distributions and outlier detection.
+ **Feature Engineering**: Calculating Unsold Capital and Performance Tiers (Percentile-based logic).
+ **Dashboarding**: Building an interactive BI tool in Tableau for stakeholder reporting.

### 📂 Repository Structure
+ **EDA insights.docx.pdf**: Executive summary documenting key business findings and strategic recommendations.
+ **Vendor Performance Analysis.ipynb**: Core analytical notebook containing data cleaning, outlier detection, and the calculation of performance tiers.
+ **Exploratory Data Analysis.ipynb**: Initial discovery phase focused on distribution of sales, profit margins, and correlation analysis.
+ **get_vendor_summary.py**: Modular script used to aggregate raw transaction data into vendor-level summaries.
+ **ingestion_db.py**: Automates the loading of raw CSV data into a structured format for analysis.

### 📈 Key Analytical Features
#### 1. Operational KPIs
The analysis tracks five critical metrics displayed in the dashboard:
+ Total Sales: **$441.41M**
+ Total Purchase: **$307.34M**
+ Gross Profit: **$134.07M**
+ Average Profit Margin: **38.72%**
+ Unsold Capital: **$2.71M** (highlighting frozen assets in the supply chain)

#### 2. Performance Tier Logic (Percentile-Based)
Using advanced calculations in Tableau and Python, vendors are categorized dynamically:
+ **High-Potential Brands**: Brands in the bottom 15% of sales volume but the top 15% of profit margin. These represent high-efficiency growth opportunities.
+ **Standard Performers**: Brands maintaining consistent volume and average market margins.

#### 3. Interactive Visualizations
The dashboard includes:
+ **Viz-in-Tooltip**: Hovering over a brand in the scatter plot reveals a secondary chart of "Sales by Order Size."
+ **Highlight Actions**: Cross-chart highlighting to track specific brands across all metrics.

### 💡 Strategic Insights
+ **Inventory Optimization**: Identified **$2.71M** in capital currently tied up in slow-moving inventory.
+ **Growth Opportunity**: While Diageo North America leads in total contribution **(24.81%)**, smaller vendors like M S Walker Inc show significantly higher potential for margin-driven growth.
+ **Automayion**: Reduced manual data prep time by implementing automated Python ingestion scripts.
