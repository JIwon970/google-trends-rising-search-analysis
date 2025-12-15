#Google Trends Rising Search Analysis
##Overview
This project analyses rising Google search terms to understand how trends change over time across different regions.

The main focus of this project is analytical thinking and DAX measure design in Power BI, rather than Excel-based reporting.

Unlike Project 1, this project uses real-world public data and performs all calculations and analysis inside Power BI.

---

##Purpose

This project was created to:
-Demonstrate analytical thinking beyond simple reporting
-Design and use DAX measures for trend analysis
-Identify pattern differences such as:
--Short-term spikes vs sustained growth
--Rank stability over time
--Week-to-week trend behaviour
-Complement Project 1 by focusing on analysis design, not just dashboards

---

##Data Source
-Dataset: Google Trends Public Dataset
-Platform: Google BigQuery
-Table: top_rising_terms

##Data Scope
-Time period: 1 year
-Rows: ~17,000
-Key fields:
--week
--dma_name
--term
--rank
--percent_gain

---

##Data Preparation
###BigQuery → Excel
-Data was exported from BigQuery as CSV
-The CSV was opened in Excel only for validation purposes

##Excel Usage (Validation Only)
Excel was used strictly for data checking, not analysis:
-Structure and column validation
-Date and data type checks
-Removal of obvious invalid or unusable values

❌ No pivot tables
❌ No calculations
❌ No analysis in Excel

The cleaned Excel file is stored in the repository for transparency.

---

##Analysis Approach
All analysis was performed in Power BI.

###Key Characteristics
-Excel-based reporting ❌
-Power BI + DAX–driven analysis ⭕

###Focus Areas
-Trend behaviour over time
-Ranking movement patterns
-Growth consistency vs one-off events
-Regional (DMA-level) differences

---

##Power BI & DAX
###DAX Usage
Custom DAX measures were designed to:
-Track week-over-week changes
-Compare rank behaviour over time
-Distinguish sustained growth from short-term spikes
-Support interactive filtering and comparisons

All metrics are filter-aware and respond dynamically to:
-Time
-Region (DMA)
-Search term

---

##Deliverables
-Interactive Power BI dashboard
-Analytical report explaining:
-Methodology
-Key findings
-Interpretation of trends

---

##Repository Structure
'google-trends-rising-search-analysis/
├─ data/
│  └─ google_trends_rising_terms_clean.xlsx
├─ sql/
│  └─ validation_queries.sql   (optional)
├─ powerbi/
│  └─ Google_Trends_Rising_Search_Dashboard.pbix
├─ visuals/
│  └─ powerbi_dashboard_overview.png
├─ report/
│  └─ Google_Trends_Rising_Search_Analysis_Report.pdf
└─ README.md'

---

##Tools Used
-Google BigQuery (data source)
-Excel (data validation only)
-Power BI Desktop
-DAX

---

##Key Takeaway
This project demonstrates the ability to:
-Work with real-world datasets
-Design analysis logic before visuals
-Use DAX intentionally for analytical questions
-Move beyond descriptive reporting into trend analysis
