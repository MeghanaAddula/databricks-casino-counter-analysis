# databricks-casino-counter-analysis
Databricks Spark SQL assessment project focused on casino mechanical counter analysis, revenue calculation, and business-driven data insights.

# Databricks Spark SQL Assessment - Casino Mechanical Counter Analysis

## Project Overview

This project is a Databricks-based data analysis assessment focused on casino mechanical counter data. The main objective of this project is to analyze cumulative counter readings and calculate key business metrics such as Cash In, Cash Out, and Gross Gaming Revenue (GGR) using Spark SQL.

The analysis was performed by following the given assessment guidelines and applying the required business logic to convert mechanical counter differences into actual monetary values.

## Tools and Technologies Used

- Databricks
- Spark SQL
- SQL
- Data Analysis
- Business Logic Implementation
- GitHub

## Dataset Understanding

The dataset contains mechanical counter readings from casino gaming machines. The important point in this assessment is that the `total_in` and `total_out` columns are not direct money values. They are cumulative counter readings.

To calculate the actual monetary value, the difference between counter readings is multiplied with `DENOMINATIE` and `IMPULS`.

## Business Logic Used

Actual Amount = Counter Reading Difference × DENOMINATIE × IMPULS

Cash In = Difference in total_in × DENOMINATIE × IMPULS

Cash Out = Difference in total_out × DENOMINATIE × IMPULS

Gross Gaming Revenue / Profit = Cash In - Cash Out

## Questions Completed

### Question 1
Calculated Cash In, Cash Out, and GGR using mechanical counter readings.

### Question 2
Question 2 was skipped because the card history / raport_card_history data was considered corrupted or ignored as per the given assessment instruction.

### Question 3
Performed period-based comparison using mechanical counter data and calculated business metrics for the required time periods.

### Question 4
Performed location-level analysis by considering active/full-period locations and comparing performance using Spark SQL.

## Folder Structure

```text
Databricks_Assessment_Addula_Meghana/
│
├── Databricks_Notebook/
│   └── Databricks notebook/source file
│
├── Q1/
│   ├── SQL query
│   ├── Output screenshot
│   └── Explanation
│
├── Q2/
│   └── Note explaining why the question was skipped
│
├── Q3/
│   ├── SQL query
│   ├── Output screenshot
│   └── Explanation
│
├── Q4/
│   ├── SQL query
│   ├── Output screenshot
│   └── Explanation
│
└── Reports/
    ├── Final Technical Report
    └── Personal Development Report
