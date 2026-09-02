 # Employee Analytics Dashboard — Power BI

## 📊 Project Overview
This project analyzes employee data using **Microsoft Power BI**. It demonstrates data cleaning with Power Query, DAX measures, KPI creation, interactive charts, and dashboard design.

The dataset contains **20,300 employee records and 12 columns** covering employee details, salary, department, job role, joining date, city, experience, and performance.

## 🎯 Objectives
- Clean and transform an unclean employee dataset
- Handle missing and inconsistent values
- Standardize text categories
- Correct data types
- Create DAX measures and KPIs
- Build an interactive employee analytics dashboard
- Generate business insights from employee data

## 🗂️ Dataset Columns

| Column | Description |
|---|---|
| Employee_ID | Unique employee identifier |
| Name | Employee name |
| Age | Employee age |
| Gender | Employee gender |
| Department | Employee department |
| Job_Role | Employee job role |
| Salary | Employee salary |
| Joining_Date | Employee joining date |
| City | Employee city |
| Email | Employee email |
| Experience_Years | Years of experience |
| Performance_Score | Employee performance rating |

## 🧹 Data Cleaning

The source data contains realistic quality issues such as:
- Missing Age, Gender, and Performance Score values
- Leading/trailing spaces
- Inconsistent capitalization
- Department variations such as `IT`, `it`, ` IT ` and `H.R`
- Job-role capitalization differences
- City variations such as `Hyd` and `Hyderabad`
- Experience values containing formats such as numeric values and `5 years`
- Columns requiring appropriate numeric/date data types

### Power Query Cleaning Steps
1. Trim unnecessary spaces
2. Clean hidden characters
3. Standardize text capitalization
4. Replace inconsistent category values
5. Handle missing values
6. Correct invalid values
7. Convert Age to Whole Number
8. Convert Salary to numeric
9. Convert Joining_Date to Date
10. Convert Experience_Years to numeric
11. Standardize Performance_Score

## 📌 KPIs
- Total Employees
- Average Salary
- Total Salary
- Average Experience
- Employees Rated

### Example DAX Measures

```DAX
Total Employees =
DISTINCTCOUNT('Employee'[Employee_ID])

Average Salary =
AVERAGE('Employee'[Salary])

Total Salary =
SUM('Employee'[Salary])

Average Experience =
AVERAGE('Employee'[Experience_Years])
```

> Replace `'Employee'` with your actual Power BI table name if different.

## 📈 Dashboard Visualizations

### Employees by Department
Shows employee count by department.

### Average Salary by Department
Compares average salary across departments.

### Employees by Gender
Shows the gender distribution.

### Average Salary by Job Role
Compares compensation across job roles.

### Employees by City
Shows employee distribution by location.

### Employee Performance
Displays the distribution of performance ratings.

### Hiring Trend
Shows hiring patterns over time using Joining_Date.

### Experience vs Salary
Explores the relationship between experience and salary using a scatter chart.

## 🎛️ Interactive Slicers
Recommended slicers:
- Department
- Gender
- City
- Job Role
- Performance Score
- Joining Date

## 🛠️ Tools
- Microsoft Power BI
- Power Query
- DAX
- CSV

## 🔄 Project Workflow

```text
Raw CSV
   ↓
Power BI
   ↓
Power Query Cleaning
   ↓
Data Type Correction
   ↓
Data Standardization
   ↓
Data Model
   ↓
DAX Measures
   ↓
KPIs
   ↓
Interactive Charts
   ↓
Professional Dashboard
```

## 💡 Business Questions
- How many employees are in the organization?
- Which department has the most employees?
- Which department has the highest average salary?
- Which job roles have the highest average salary?
- How are employees distributed across cities?
- What is the average experience?
- Is there a relationship between experience and salary?
- What is the performance distribution?
- How has hiring changed over time?

## 📁 Recommended GitHub Structure

```text
employee-analytics-powerbi/
│
├── README.md
├── data/
│   └── employee_dataset.csv
├── powerbi/
│   └── Employee_Analytics_Dashboard.pbix
├── screenshots/
│   └── dashboard.png
└── documentation/
    └── data-cleaning-steps.md
```

## 🚀 How to Use
1. Clone or download the repository.
2. Open the `.pbix` file in Power BI Desktop.
3. Review the Power Query transformations.
4. Refresh the data if required.
5. Explore the dashboard using slicers and charts.

## 📚 Skills Demonstrated
- Data Cleaning
- Power Query
- Data Transformation
- Data Modeling
- DAX
- KPI Development
- Data Visualization
- Dashboard Design
- Business Analysis
- Interactive Reporting

## 👤 Author
**Vignesh**

A portfolio project demonstrating practical **Power BI Data Analyst** skills.
