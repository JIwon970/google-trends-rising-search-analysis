# Google Trends Rising Search Analysis

This project analyzes rising Google search terms using a Power BI–centric workflow, with intentional DAX measure design for trend behavior analysis.

The main objectives of this project were to:

- Understand how search interest behaves over time (week-to-week patterns)
- Separate short-term spikes from sustained growth behavior
- Evaluate rank stability and movement across weeks
- Compare trends across regions (DMA)
- Build an interactive Power BI dashboard driven by DAX measures
- Summarize findings in a final PDF report

---

## Project Stack
BigQuery → CSV Export → Excel (Validation Only) → Power BI (DAX) → GitHub
- BigQuery: Data source (Google Trends Public Dataset)
- CSV Export: Local export from BigQuery
- Excel: Structure check and basic data validation only (no analysis)
- Power BI: Data model + DAX measures + interactive dashboard
- GitHub: Portfolio publishing and version control

---

## Dataset
- Source: Google Trends Public Dataset (BigQuery)
- Table: top_rising_terms
- Time period: 1 year
- Rows: ~17,000
- Columns:
  - week
  - dma_name
  - term
  - rank
  - percent_gain

---

## Excel File Policy (Important)
- Excel was used only to validate the exported dataset and remove obvious unusable values.
- No pivot tables, no KPI calculations, and no analysis were done in Excel.
- All metrics and insights were created inside Power BI using DAX.

---

## Project Structure  
/data - Cleaned Excel dataset used for Power BI import  
/sql - Optional validation queries for cross-checking  
/powerbi - Power BI dashboard file (.pbix)  
/visuals - Power BI dashboard overview screenshot  
/report - Final PDF analysis report  

Each folder contains its own README file for detailed explanations.

---

## Power BI Analysis Summary
All analysis was performed in Power BI using DAX measures.
- Interactive filtering supports insight exploration by:  
  - DMA (region)
  - Week
  - Search term
- Trend behavior analysis focuses on:  
  - Sustained growth vs short-lived spikes
  - Rank stability vs volatile movement
  - Week-to-week change patterns and momentum
  - Regional differences in trend behavior

Power BI file location:  
/powerbi/Google_Trends_Rising_Search_Dashboard.pbix

---

## Final PDF Report
A full project report was created to summarize:
- Dataset scope and validation steps
- Power BI modeling approach
- DAX measure logic (key measures used)
- Main insights and interpretations
- Dashboard overview and usage notes

PDF report location:  
/report/Google_Trends_Rising_Search_Analysis_Report.pdf

---

## Key Skills Demonstrated
- Working with real-world public datasets (BigQuery export workflow)
- Data validation and cleaning checks in Excel (validation only)
- Power BI data modeling and interactive dashboard building
- Intentional DAX measure design (filter-aware metrics)
- Trend behavior analysis (patterns, stability, and momentum)
- GitHub repository structuring and documentation

---

## Notes
- The raw BigQuery CSV export is not included in this repository.
- This project is for educational and professional demonstration only.

---

## Author
Analyst: Jiwon Yang  
Project: Google Trends Rising Search Analysis  
Year: 2025  
