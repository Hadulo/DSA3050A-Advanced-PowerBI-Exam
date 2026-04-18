# DSA 3050A Advanced Power BI Exam: Healthcare Analytics Dashboard

## Student Information
- **Student Name:** [Your Full Name]
- **Admission Number:** [Your Admission Number]
- **Course Code:** DSA 3050A
- **Semester:** Spring Semester 2026
- **Institution:** United States International University Africa

---

## Project Overview
An advanced Power BI analytical solution built on a hospital admissions
dataset of 55,500 records spanning 2019 to 2024. The solution covers
billing performance, patient admission trends, clinical outcomes, and
operational efficiency across a network of hospitals.

---

## Problem Statement
Hospital management lacks a structured way to monitor billing revenue,
track admission patterns across medical conditions, evaluate test result
outcomes, and compare performance across insurance providers and time
periods. This dashboard addresses those gaps through an interactive
multi-page Power BI report.

---

## Dataset Description
- **Source:** Kaggle - Healthcare Dataset
- **File:** healthcare_dataset.csv
- **Rows:** 55,500
- **Columns:** 15
- **Date range:** 2019 to 2024
- **Key fields:** Age, Medical Condition, Billing Amount,
  Admission Type, Test Results, Insurance Provider,
  Doctor, Hospital, Discharge Date

---

## Tools Used
- Power BI Desktop
- Power Query (M language)
- DAX (Data Analysis Expressions)
- GitHub

---

## Steps Followed
1. Acquired dataset from Kaggle and inspected raw data
2. Imported into Power BI and opened Power Query Editor
3. Applied 10 transformation steps including removing duplicates,
   fixing data types, handling negative billing values,
   standardising name casing, and creating derived columns
4. Built a star schema with 5 dimension tables, 1 fact table,
   and a DAX-generated Date table
5. Created 8 DAX measures and 3 calculated columns
6. Designed a 3-page interactive dashboard
7. Generated analytical insights and business recommendations
8. Documented all steps in a PDF report and uploaded to GitHub

---

## Dashboard Features
- **Page 1 - Executive Summary:** KPI cards, monthly billing trend,
  billing by condition, year/gender/admission type slicers
- **Page 2 - Detailed Analysis:** Matrix by condition and year,
  drill-down by insurance provider, age vs billing scatter chart,
  top 10 highest billing admissions table
- **Page 3 - Insights and Performance:** YTD billing line chart,
  year-over-year growth chart, abnormal test rate by condition,
  admission type donut chart, page navigation buttons

---

## Key DAX Measures
| Measure | Purpose |
|---|---|
| Total Billing | Sum of all billing amounts |
| Total Admissions | Count of all admission records |
| Avg Billing per Admission | Mean billing cost per visit |
| Distinct Patients | Count of unique patients |
| Emergency Admission % | Proportion of emergency visits |
| YTD Billing | Cumulative billing year to date |
| Billing Growth % | Year-over-year billing change |
| Abnormal Test % | Proportion of abnormal test results |

---

## Key Insights
1. Length of stay is the primary billing driver, not condition type
2. 67% of admissions are unplanned (Emergency or Urgent)
3. Abnormal test rates are uniform at 33% across all conditions
4. 2024 data represents a partial year and should not be compared
   directly to full prior years
5. All five insurance providers show equal admission volumes
   and consistent average billing

---

## Challenges Encountered
[Describe any issues you faced, for example:]
- Negative billing values required filtering before analysis
- 534 duplicate rows were identified and removed
- The flat file required manual splitting into a star schema
- TestResults had to be explicitly retained in Fact_Admissions
  when building dimension tables

---

## Conclusion
This project demonstrates a complete end-to-end Power BI solution
covering data cleaning, star schema modeling, DAX calculations,
interactive dashboard design, and business insight generation.
The solution provides hospital management with actionable visibility
into billing performance, clinical outcomes, and admission trends
across a six-year period.

---
## Power BI File
The .pbix file exceeds GitHub's 25MB upload limit and is
hosted on Google Drive.

[Click here to download the Power BI file](https://drive.google.com/file/d/14WMyOeUWoZKRKoKTnmS9SGY2c4IcV3XT/view?usp=sharing)

> To open: download the file and open with Power BI Desktop.
## Repository Structure
```
DSA3050A-Advanced-PowerBI-Exam/
├── data/               # Raw dataset CSV file
├── screenshots/        # All report screenshots by section
├── report/             # Final PDF submission
└── README.md           # This file
```
