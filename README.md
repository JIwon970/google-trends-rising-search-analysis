# Google Trends Rising Search Analysis

This project analyzes rising Google search terms using a Power BI–centric workflow, with intentional DAX measure design for trend behavior analysis.

A final written report was also produced to document the workflow, DAX measures, and key findings.

---

## The main objectives of this project were to:
- Understand how rising search terms behave over time across weeks  
- Separate short-term spikes from sustained growth behavior  
- Compare persistence (active weeks) against growth intensity (average percent gain)  
- Build an interactive Power BI dashboard driven by DAX measures  
- Summarize findings in a final PDF report

---

## Project Stack
**BigQuery → CSV Export → Excel (Validation Only) → Power BI (DAX) → Report (PDF) → GitHub**

- **BigQuery:** Data source (Google Trends Public Dataset)  
- **CSV Export:** Local export from BigQuery  
- **Excel:** Structure check and basic data validation only (no analysis)  
- **Power BI:** Data model + DAX measures + interactive dashboard  
- **Report (PDF):** Final written analysis and documentation  
- **GitHub:** Portfolio publishing and version control  

---

## Dataset
- **Source:** Google Trends Public Dataset (BigQuery)  
- **Table:** `top_rising_terms`  
- **Time period:** 1 year  
- **Rows:** ~17,000  
- **Columns:**
  - `week`
  - `dma_name`
  - `term`
  - `rank`
  - `percent_gain`

---

## Excel File Policy (Important)
Excel was used only to validate the exported dataset and remove obvious unusable values.

- No pivot tables  
- No KPI calculations  
- No analysis in Excel  

All metrics and insights were created inside Power BI using DAX.

---

## Project Structure
- `/data` - Cleaned Excel dataset used for Power BI import  
- `/powerbi` - Power BI dashboard file (.pbix)  
- `/visuals` - Power BI dashboard overview image  
- `/report` - Final PDF analysis report  

Each folder contains its own README file for detailed explanations.

---

## Power BI Analysis Summary
All analysis was performed in Power BI using DAX measures.

### Dashboard focus
The dashboard is designed to help identify whether a rising
- **A short-lived spike** (high intensity but low persistence), or  
- **A sustained rising trend** (active across multiple weeks)

### Key metrics used
- **Active Weeks (Persistence)**  
- **Average Percent Gain (Growth Intensity)**  
- **Average Rank (Context / Top 20 selection)**  

### Interactive filtering
The final dashboard uses minimal slicers to keep exploration clean:
- **Week**

**Power BI file location:**  
`/powerbi/Google_Trends_Rising_Search_Dashboard.pbix`

---

## Report Writing (Included)
A final PDF report was written as the formal documentation of this project.

### What the report covers
- Dataset scope, filters, and validation steps  
- Data preparation workflow (BigQuery export → Excel validation → Power BI import)  
- Data model design and key DAX measures (with explanations)  
- Dashboard design decisions and usage notes  
- Key findings and interpretation (spikes vs sustained trends)  
- Limitations and next-step improvement ideas  

**PDF report location:**  
`/report/Google_Trends_Rising_Search_Analysis_Report.pdf`

---

## Key Skills Demonstrated
- Working with real-world public datasets (BigQuery export workflow)  
- Data validation and cleaning checks in Excel (validation only)  
- Power BI data modeling and interactive dashboard building  
- Intentional DAX measure design (filter-aware metrics)  
- Trend behavior analysis using persistence vs intensity  
- Report writing and insight communication (PDF deliverable)  
- GitHub repository structuring and documentation  

---

## Notes
- The raw BigQuery CSV export is not included in this repository.  
- This project is for educational and professional demonstration only.  

---

## Author
- **Analyst:** Jiwon Yang  
- **Project:** Google Trends Rising Search Analysis  
- **Year:** 2025  
