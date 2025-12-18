# Power BI 

This folder contains the Power BI file for the Google Trends rising search analysis.

## Description
- The cleaned dataset from the /data folder was imported into Power BI.
- A data model was created and all metrics were built using DAX measures.
- The final dashboard focuses on trend behavior analysis:
  - persistence (active weeks) vs growth intensity (average percent gain).

## File Name
`Google_Trends_Rising_Search_Dashboard.pbix`

## Dashboard Features
- Scatter Chart:
  - Active Weeks (Persistence) vs Average Percent Gain (Intensity)
- Table:
  - Top terms with supporting metrics (Avg Rank, Avg Percent Gain, Active Weeks)
- Slicer:
  - Week

## Notes
- Top terms are filtered as Top 20 by Average Rank.
- Rank volatility was not used in the final dashboard because rank movement was minimal within the filtered dataset.
- This PBIX file is the main interactive deliverable for this project.
