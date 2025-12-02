**🩺 Global Health Index 2024**
A Data-Driven Assessment of Global Healthcare Performance, Efficiency & Regional Disparities
<div align="center">

</div>
📌 Project Overview

This project analyzes global healthcare performance for 2024 using data scraped from CEOWorld and Numbeo. Through interactive Power BI dashboards, the study evaluates:

Overall healthcare quality

Efficiency of healthcare spending

Regional disparities

Benchmark performance across countries

The findings highlight global leaders, inefficient spenders, structural weaknesses, and regions requiring targeted improvement.

🧹 Data Preparation Workflow
🔎 1. Web Scraping

Scraped global health index data using Python.

Extracted indices and expenditure metrics from multiple sources.

🧼 2. Cleaning with Power Query

Removed duplicates

Filled missing values

Countries with no available data were assigned 0 to avoid assumptions

Normalized column names and formats

🧮 3. Feature Engineering (Power BI)

Created essential calculated fields:

Combined Health Score =
([Health Care Index (CEOWorld) 2024] + 
 [Health Care Index (Numbeo) 2024]) / 2

Efficiency Score =
DIVIDE([Combined Health Score], [Health Care Exp Index (Numbeo) 2024])


Also created region grouping with SWITCH() + IN().

📊 4. Dashboard Development

Three dashboards were built:

Benchmark Assessment

Regional Analysis

Efficiency & ROI Analysis

📊 Dashboards Summary
🧭 1. Benchmark Assessment Dashboard

Ranks countries by Combined Health Score

Highlights top & bottom performers

Shows efficiency leaders

Identifies index discrepancies between CEOWorld & Numbeo

🌍 2. Regional Analysis Dashboard

Regional ranking by performance

Efficiency distribution across regions

Healthcare index totals per region

Reveals structural inequalities

💰 3. Efficiency & ROI Dashboard

Spending vs performance

Spending vs efficiency

ROI outliers (efficient vs inefficient systems)

Identifies cost-effective countries

🌎 Key Insights
🏆 Top-Performing Countries

Taiwan

South Korea

Australia

Netherlands

Canada

Sweden

Japan

🚀 High-Efficiency Leaders

Ireland

Malta

Sweden

Australia

Canada

⚠️ Low-Performing Countries

DR Congo

Libya

Paraguay

Bolivia

Honduras

Sudan

🌍 Regional Performance

Europe & Oceania → Best overall performance and efficiency

Africa & Latin America → Lowest scores and highest structural challenges

Asia → Mixed performance

💡 Spending vs Outcome

Higher healthcare expenditure does not always translate to better performance.
Efficiency varies widely → system design and governance matter.

🔚 Conclusion

Global healthcare performance remains unequal across continents.
High-performing countries combine strong outcomes with efficient spending, while many developing regions struggle with limited resources and weak health infrastructure.
The analysis reveals where strategic investment, policy reform, and capacity-building can significantly improve global health outcomes.

💡 Recommendations

Strengthen investment in low-performing systems

Adhere to efficiency-based budgeting

Adopt best practices from top performers

Improve health data quality and reporting

Strengthen primary and preventive healthcare

Deploy digital health systems and monitoring frameworks

🧰 Tools Used
Tool	Purpose
Python	Web scraping
Power Query	Cleaning & transformation
Power BI	Dashboard creation
DAX	Metric & measure calculation
📁 Repository Structure
📦 Global-Health-Index-2024
│
├── data/
│    └── health_index_cleaned.csv
│
├── visuals/
│    └── dashboard_screenshots/
│
├── scraping_script.py
├── PowerBI_Dashboard.pbix
└── README.md

👨‍💻 Author

Joseph Innocent
Data Analyst | Healthcare Insights | Python & Power BI

🔗 GitHub: @youngjon2001

<div align="center">
