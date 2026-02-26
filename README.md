# HR Analytics Dashboard — Power BI Project

## 📊 Project Overview

This project presents an **end-to-end HR Analytics solution** built using **Power BI** to analyze employee attrition patterns and provide actionable workforce insights.

The dashboard enables HR teams and business leaders to:

* Monitor employee attrition trends
* Identify high-risk employee segments
* Analyze attrition drivers
* Support data-driven HR decision-making

---

## 🎯 Business Problem

Employee attrition impacts organizational productivity, hiring costs, and team stability.
The objective of this project is to analyze historical HR data and answer:

* Which employees are most likely to leave?
* What factors influence attrition?
* Which departments and roles experience higher turnover?
* How salary, age, and experience impact retention?

---

## 🧱 Solution Architecture

```
Raw HR Dataset
      ↓
Data Cleaning & Transformation
      ↓
Data Modeling (Star Schema)
      ↓
DAX Measures & KPIs
      ↓
Interactive Power BI Dashboard
```

---

## 📁 Dataset Information

The dataset contains employee demographic, compensation, and job-related attributes.

### Columns Used

EmpID, Age, AgeGroup, Attrition, BusinessTravel, DailyRate, Department, DistanceFromHome, Education, EducationField, EmployeeCount, EmployeeNumber, EnvironmentSatisfaction, Gender, HourlyRate, JobInvolvement, JobLevel, JobRole, JobSatisfaction, MaritalStatus, MonthlyIncome, SalarySlab, MonthlyRate, NumCompaniesWorked, Over18, OverTime, PercentSalaryHike, PerformanceRating, RelationshipSatisfaction, StandardHours, StockOptionLevel, TotalWorkingYears, TrainingTimesLastYear, WorkLifeBalance, YearsAtCompany, YearsInCurrentRole, YearsSinceLastPromotion, YearsWithCurrManager

---

## 🧹 Data Preparation

Data preparation steps included:

* Removed duplicate Employee IDs
* Standardized categorical values
* Created Age Groups
* Derived Salary Slabs
* Handled missing values
* Converted data types
* Validated attrition labels

Tools used:

* Power Query (ETL)
* SQL (optional preprocessing)

---

## 📐 Data Model

A simplified analytical model was designed:

* Employee table as primary fact dataset
* Calculated columns for segmentation
* Optimized relationships for performance

---

## 📊 Dashboard Features

### KPI Summary

* Total Employees
* Attrition Count
* Attrition Rate
* Average Age
* Average Salary
* Average Years at Company

### Analytical Visuals

* Attrition by Education
* Attrition by Age Group
* Attrition by Salary Slab
* Attrition by Gender
* Attrition Trend Over Time
* Attrition by Job Role
* Department Filters

---

## 📈 Key Insights

* Highest attrition observed among employees aged **26–35**
* Lower salary slabs show significantly higher turnover
* Sales and Laboratory roles show elevated attrition risk
* Overtime correlates strongly with attrition

---

## 🛠️ Tools & Technologies

| Tool        | Purpose               |
| ----------- | --------------------- |
| Power BI    | Dashboard Development |
| Power Query | Data Transformation   |
| DAX         | KPI & Measures        |
| SQL         | Data Preparation      |
| GitHub      | Version Control       |

---

## 🧮 Key DAX Measures

### Attrition Count

```DAX
Attrition Count =
CALCULATE(COUNT(Employee[EmpID]),
Employee[Attrition] = "Yes")
```

### Attrition Rate

```DAX
Attrition Rate =
DIVIDE([Attrition Count], COUNT(Employee[EmpID]))
```

### Average Salary

```DAX
Avg Salary =
AVERAGE(Employee[MonthlyIncome])
```

---

## 🖼 Dashboard Preview

![Dashboard Preview]("C:\Users\Joy\Pictures\Screenshots\HR-analytical-dashboard.png")

---



## 📌 Project Outcomes

* Built an HR analytics reporting solution
* Improved workforce visibility
* Demonstrated business intelligence lifecycle
* Delivered executive-level dashboard design

---

## 🔮 Future Improvements

* Predictive attrition model (Machine Learning)
* Automated data refresh using Power BI Service
* Department-level forecasting
* HR KPI scorecards

---

## 👤 About me 

I am **Johnson Sukumar**, a Data Analyst with 4 years of professional experience working with data to support business analysis and decision-making.

---

## 📄 License

This project is licensed under the MIT License.
