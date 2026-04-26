# NHS-A-E-Performance
A data analysis and dashboard project using NHS England A & E performance data to evaluate 4-hour waiting-time performance across providers over a 12-month period.

## Project Overview

This project analyses NHS Accident & Emergency (A&E) performance data to understand how provider-level 4-hour performance varied across a 12-month period.

The project focuses on:
- identifying the worst-performing providers in a selected month
- identifying the best-performing providers in a selected month
- analysing national 4-hour performance trends over time
- finding providers that consistently appeared among the worst and best performers
- identifying the overall best and worst providers across the full 12-month period using providers with complete 12-month coverage

## Business Questions

The project was designed to answer the following questions:

1. Which NHS providers had the worst 4-hour A&E performance in a selected month?
2. Which NHS providers had the best 4-hour A&E performance in a selected month?
3. How did national 4-hour A&E performance change over the 12-month period?
4. Did national performance improve or worsen over time?
5. Which providers appeared most often among the worst performers?
6. Which providers appeared most often among the best performers?
7. Which providers had the best and worst overall performance across the full 12-month period among providers with complete 12-month coverage?


## Data Source

The data used in this project comes from the NHS England **A&E Attendances and Emergency Admissions** statistical publication.

Main dataset used:
- 12 monthly provider-level A&E files covering a 12-month period

Additional file downloaded:
- Monthly A&E Time Series workbook (kept as an optional validation/reference source)

Important note:
- The final provider-level dashboard dataset was built from the 12 monthly provider files
- The separate Monthly A&E Time Series file was downloaded but was **not included** in the final provider-level dataset
Source: NHS England – A&E Attendances and Emergency Admissions


## Tools Used

- **Python** (pandas, Jupyter Notebook) for data cleaning, transformation, and analysis
- **Power BI** for dashboard creation and visual storytelling
- **GitHub** for project documentation and portfolio presentation


## Method

The project was completed in the following stages:

1. Downloaded 12 monthly NHS A&E provider-level Excel files
2. Inspected file structure and identified the correct provider-level worksheet
3. Cleaned and transformed the data in Python using pandas
4. Removed non-provider rows, blank rows, and unnecessary columns
5. Standardised column names and converted numeric fields
6. Calculated provider-level 4-hour performance metrics
7. Combined all 12 monthly files into one analysis-ready dataset
8. Calculated national monthly 4-hour performance trends
9. Identified best and worst providers for selected months
10. Identified providers that were repeatedly among the best and worst performers
11. Calculated overall best and worst provider performance across the full 12-month period using providers with complete 12-month coverage
12. Built a Power BI dashboard to present the findings


## Key Insights

- National 4-hour performance showed month-to-month variation across the 12-month period, highlighting changing operational pressure over time.
- Some providers appeared repeatedly in the monthly bottom 10, suggesting persistent performance challenges rather than one-off poor months.
- Among providers with complete 12-month coverage, the worst overall provider across the full period was **[ East Cheshire NHS Trust ]** with **[ 48.39 % ]** seen within 4 hours.
- Among providers with complete 12-month coverage, the best overall provider across the full period was **The Pinn Unregistered Wic** with **100.0%** of patients seen within 4 hours.


## Dashboard

The dashboard was built in **Power BI** and includes:

- a national 4-hour KPI card
- a 12-month national performance trend line
- a month slicer for interactive filtering
- a Top 10 Worst Performing Providers chart for the selected month
- a Top 10 Best Performing Providers chart for the selected month

### Dashboard Link
[View the Power BI dashboard here](PASTE_LINK_HERE)


## Future Improvements

Possible future enhancements include:
- adding regional comparisons
- incorporating map-based provider views if geographic reference data is added
- validating national trends against the NHS Monthly A&E Time Series file
- expanding analysis to include seasonal patterns and year-on-year comparisons


## Repository Structure

nhs-ae-dashboard/
│
├── notebooks/
├── data/
│   ├── raw/
│   └── cleaned/
├── power-bi
├── README.md

## Why This Project Matters

This project demonstrates the ability to work with real UK public-sector healthcare data, clean and transform messy Excel files, calculate meaningful performance KPIs, and present findings in an interactive dashboard. It also shows an understanding of NHS context, which is especially relevant for UK data analyst roles.
