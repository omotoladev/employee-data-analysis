# Employee Data Interrogation and Manipulations

[![GitHub](https://img.shields.io/github/license/Tola-Analyst-hub/employee-data-analysis)](LICENSE)

*Structured SQL analytics on employee data for actionable HR insights*

## Overview
This project involves performing structured SQL queries and analytics on an employee dataset to uncover critical workforce patterns such as employee-manager salary relationships, department-level compensation rankings, and headcount distribution. The analysis provides actionable insights to support HR decisions, compensation planning, and leadership visibility.

## Tools & Technologies
- **SQL Server**: Primary tool for data analysis and manipulation
- **SQL Skills Used**:
  - Data Retrieval (`SELECT`): Queried and extracted specific information from the database
  - Data Aggregation (`SUM`, `COUNT`): Calculated totals and counted records to analyze data trends
  - Data Filtering (`WHERE`, `BETWEEN`, `IN`, `AND`): Applied filters to select relevant data
  - Advanced SQL (`SELF JOIN`, `CTEs`, `RANK()`, `DENSE_RANK()`): Used for complex relationship analysis

## Business Objectives
- Support the HR and executive leadership team with data-driven insights
- Identify compensation discrepancies (e.g., employees earning more than their managers)
- Highlight top earners across departments
- Enable departmental headcount planning
- Provide a reusable SQL logic base for scalable employee data analysis

## Dataset Description
The dataset consists of employees' personal and professional data, including:
- Names
- Departments
- Salaries
- Job roles
- Reporting lines (manager-employee relationships)

The data is available in both CSV and Excel formats:
- `Employee_Dataset.csv`
- `Employee_Dataset.xlsx`

## Key Analyses & Outcomes

### 1. Employees Earning More Than Their Managers
Using a self-join on the employee table, we identified discrepancies in the managerial pay hierarchy. This analysis helps HR teams identify potential compensation issues that could affect manager-employee relationships and overall workplace hierarchy.

### 2. Top Earners in Each Department
Using `RANK()` and `DENSE_RANK()` window functions, we extracted the highest and top 3 earners in every department. This provides better compensation visibility for leadership and helps identify:
- Pay disparities across departments
- Top performers by compensation metrics
- Potential outliers in department salary distributions

### 3. Headcount by Department
Applied `GROUP BY` and `COUNT()` to generate workforce distribution reports, which aid in:
- Capacity planning
- Budget allocation
- Organizational restructuring decisions

## Files in This Project
- `Employee.sql` - SQL queries used for data analysis
- `Employee_Dataset.csv` - Dataset in CSV format
- `Employee_Dataset.xlsx` - Dataset in Excel format
- `Headshot.jpg` - Project owner's professional photo

## How to Use
1. Import the dataset (`Employee_Dataset.csv` or `Employee_Dataset.xlsx`) into your SQL Server database
2. Run the queries in `Employee.sql` to perform the analyses
3. Modify the queries as needed to answer additional business questions

## Future Enhancements
Potential extensions to this analysis could include:
- Attrition risk prediction based on compensation patterns
- Compensation equity analysis across demographic factors
- Career progression analysis using historical employee data
- Pay gap analysis by department, role, or tenure
