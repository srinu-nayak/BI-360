# 𝐁𝐮𝐬𝐢𝐧𝐞𝐬𝐬 𝐈𝐧𝐬𝐢𝐠𝐡𝐭𝐬 360 – 𝐀 𝐏𝐨𝐰𝐞𝐫 𝐁𝐈 𝐏𝐫𝐨𝐣𝐞𝐜𝐭 𝐟𝐨𝐫 𝐀𝐭𝐥𝐢𝐐 𝐇𝐚𝐫𝐝𝐰𝐚𝐫𝐞
### Tools Used:
- Data Extraction: MySQL, Excel/CSV
- Data Cleaning & Analysis: Power Query, DAX, DAX Studio
- Data Visualization: Power BI
- Version Control: Git, GitHub
- Microsoft Fabric - Dataflows, Pipeline, APIs, Lake house
- BI Gateways, Incremental Refresh, SharePoint

# Background & Overview
This project provides a comprehensive data analytics solution for AtliQ Hardware, a rapidly expanding global electronics company specializing in PC accessories and components. The objective is to establish a robust, centralized data platform to replace decentralized reporting and support strategic decision-making across all core business functions (Finance, Sales, Marketing, Supply Chain).

The reliance on fragmented, manual data sources (scattered Excel sheets) has resulted in inefficient operational decision-making, leading to significant financial losses and a competitive disadvantage, particularly during critical market expansion initiatives. This analysis addresses the urgent need for data transparency and actionable metrics.

### Project Goals / Key Questions:
- How has Net Sales Growth trended across key geographies (APAC, North America, EU) and product segments over the past five fiscal years?
- What is the current Net Profit Margin {NPM}, and which operational expenditures are primary detractors from overall profitability?
- Which customer segments and sales channels are driving the highest Gross Margin {GM}, and how can discounting strategies be optimized for better performance?
- What is the current Forecast Accuracy {FCA}, and how can supply chain efficiency be enhanced to minimize inventory imbalances (stockouts and excess)?

An interactive PowerBI dashboard can be downloaded here Link [https://app.powerbi.com/view?r=eyJrIjoiMTEzMTY2ZjktOGM4YS00ZjFlLWFjZGMtMjI0NWRmNzc1MmJhIiwidCI6IjFiMTRiNGZmLTMxMWUtNGEyMC1iM2NjLTM0ZGZhNzAxMDI2ZCJ9]

# Data Structure Overview
AtliQ's database structure a seen below consists of multiple tabels:operating expenses, sales targets, and market share data etc., with a total row count of 1,858,329 records.

#### Data Model
<img width="600" height="728" alt="Data Model" src="https://github.com/user-attachments/assets/5ea7078d-2340-4339-bd7d-1af4cec22e3a" />

Prior to beginning the analysis, a variety of checks were conducted for quality control and familiarization with the datasets. The SQL queries utilized to inspect and perform quality checks can be found.

# Executive Summary
Net Sales demonstrated significant compound growth across the analysis period, escalating by approximately 280% in FY 2019, 140% in FY 2020, and reaching a peak increase of roughly 350% in FY 2022. Despite this strong top-line expansion, the company’s Net Profit Margin has remained negative since FY 2020, indicating high operational and marketing expenditure relative to revenue—a common trait for aggressive growth-stage companies. APAC consistently served as the highest-revenue region, led by the Indian market, while Amazon maintained its position as the top global retailer customer. Supply chain efficiency improved, with Forecast Accuracy ($\text{FCA}\%$) recovering from a low of 73% (post-COVID-19 disruption) to 81% in the latest fiscal year, mitigating severe stock imbalance issues.

Below is the overview from the Power BI Dashboard and more example are included throughtout the report. The entire dashboard can be downloaded here [https://app.powerbi.com/view?r=eyJrIjoiMTEzMTY2ZjktOGM4YS00ZjFlLWFjZGMtMjI0NWRmNzc1MmJhIiwidCI6IjFiMTRiNGZmLTMxMWUtNGEyMC1iM2NjLTM0ZGZhNzAxMDI2ZCJ9]


#### Features
<img width="1280" height="741" alt="image" src="https://github.com/user-attachments/assets/c6cdaaf7-6f42-43bf-9c6b-0524e40c1ebb" />

• Finance View: Detailed financial analysis, including revenue, expenses, and profit margins (Explore P&L statements, Net Sales Performance Trend, Top Products and Customers based on NS, GS, GM/%, COGS, NP%, Pre & Post Deductions)
• Sales View: Insights into product and customer performance (Examine Customer and Product Performances, Performance matrix with NS and GM% on customers, Unit economics with COGS and deductions)
• Marketing View: Analytics to enhance marketing strategy (Analyze Product Performance, Market/Regional/Customer Performance, GM% & NP% Performance on Segment, and Unit economics with COGS, Operational expenses, and NP)
• Supply Chain View: Optimization metrics for efficient supply chain management (Investigate Forecast Accuracy, Net Error, ABS Error, Key metrics by Customer based on FA/NE/ABSE, Accuracy/Net Error Trend, and Key metrics by Product)
• Executive View: Metrics critical for top-level decision-makers.

# Insights Deep Dive
• Net Sales grew ~350% (FY 2022), but Net Profit % remained negative due to high expenses.
• APAC led in Net Sales; however, North America had the highest subregional sales with only ~5% market penetration in the PC division.
• Flat discounting was hurting Gross Margins — indicating a need for performance-based discounting.
• Supply chain issues led to stockouts in FY 2021–2022, followed by excess inventory.
• Sales peaked from September to December — pointing to the need for optimized inventory planning.
• High marketing costs in the UK and Germany required a strategic review.

# Recommendations
• Introduce performance-based discounting by product and customer.
• Expand presence in APAC, especially India.
• Integrate real-time forecasting tools to reduce stock imbalances.
• Review and optimize marketing spend in the UK and Germany.
• Align inventory and promotions with peak seasonal demand (Sep–Dec).

# Caveats and Assumptions 
### Limitations
- Data on market share is limited only to the Personal Computer division, restricting a full competitive landscape analysis across all product categories.
- Operating Expense data is aggregated, preventing a granular breakdown of marketing versus general overhead spend to isolate specific cost drivers.
- The Targets dataset is only available for FY 2022, hindering a historical analysis of target attainment and performance variance for previous fiscal years.
- The analysis only covers actual sales up to December 31, 2021, and FY 2022 metrics are based on preliminary or partial data.
  
### Future Work
- Implement Advanced RFM (Recency, Frequency, Monetary) segmentation on the retailer customer base to refine targeted marketing campaigns and loyalty programs.
- Develop an Inventory Optimization Dashboard to forecast stock levels dynamically, incorporating lead times and safety stock calculations.
- Introduce What-If Scenario Analysis in the dashboard to model the impact of varying discounting rates or price changes on the $\text{Gross Margin}$ and $\text{Net Sales}$.
- Integrate unstructured Customer Feedback Data (if available) to gain qualitative insight into product underperformance (e.g., USB flash drives).
- Extend the data model to include Supplier Performance Metrics for a complete 360-degree view of the supply chain value chain.
