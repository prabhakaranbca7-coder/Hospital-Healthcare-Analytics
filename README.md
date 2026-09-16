# Hospital Healthcare Analytics

## Project Overview

This is an end-to-end healthcare analytics project focused on analyzing hospital operations, patients, appointments, admissions, treatments, doctors, and department performance.

The project follows a complete Data Analyst workflow:

**Data Cleaning → Python/Pandas Analysis → PostgreSQL → SQL Analysis → Power BI Dashboard → Business Insights**

The objective is to transform hospital data into meaningful insights that can support operational and management decisions.

---

## Business Objectives

- Analyze patient and hospital activity.
- Understand appointment performance and status.
- Identify departments with high appointment and admission volumes.
- Analyze appointment waiting time.
- Measure appointment completion rate.
- Analyze hospital readmission rates.
- Understand average length of hospital stay.
- Analyze treatment costs and treatment outcomes.
- Evaluate department performance.
- Analyze doctor workload.
- Identify useful business insights from healthcare data.

---

## Dataset

The project contains six cleaned datasets:

| Dataset | Records | Description |
|---|---:|---|
| Patients | 12,000 | Patient demographic and registration information |
| Doctors | 80 | Doctor details, specialization, experience, and employment type |
| Departments | 8 | Department capacity, staffing, beds, and occupancy |
| Appointments | 45,000 | Appointment details, status, waiting time, and satisfaction |
| Admissions | 9,000 | Hospital admission, discharge, department, and readmission information |
| Treatments | 12,892 | Treatment details, costs, duration, diagnosis, and outcomes |

**Total Records Analyzed: 87,972**

> The datasets used in this portfolio project are cleaned/anonymized project data and do not contain real patient-identifying information.

---

## Data Cleaning

Data cleaning and preparation were performed using Python and Pandas.

The cleaning process included:

- Dataset dimension checks
- Missing-value analysis
- Duplicate detection
- Date validation
- Data type validation
- Numerical range validation
- Categorical value validation
- Invalid relationship checks
- Missing waiting-time handling
- Treatment-date validation
- Length-of-stay calculation
- Outlier identification
- Dataset merging
- Exporting cleaned datasets

Outliers were identified during analysis and retained where they could represent genuine hospital cases rather than obvious data-entry errors.

---

## Python / Pandas Analysis

Python and Pandas were used for data cleaning, validation, exploratory analysis, and data preparation.

### Main Python Tasks

- Data loading
- Data profiling
- Missing-value analysis
- Duplicate detection
- Data validation
- Group-by analysis
- Statistical analysis
- Correlation analysis
- Dataset merging
- Feature creation
- Cleaned dataset generation

### Analysis Performed

- Patient age analysis
- Insurance-type analysis
- Appointment status analysis
- Appointment waiting-time analysis
- Department occupancy analysis
- Admission analysis
- Length-of-stay analysis
- Treatment cost analysis
- Treatment outcome analysis
- Doctor and department analysis

---

## PostgreSQL & SQL Analysis

The cleaned datasets were imported into PostgreSQL for relational analysis.

### Database

**Database:** `Advanced_analysis`

### Table Relationships

text
patients ──< appointments >── doctors ──> departments
patients ──< admissions >──── doctors
                  │
                  ├──────────> departments
                  └──< treatments

## SQL Analysis Included

The SQL analysis focused on intermediate and advanced analytical concepts:

- JOINs
- Aggregations
- GROUP BY
- HAVING
- Subqueries
- CASE statements
- Common Table Expressions (CTEs)
- Window functions
- Ranking
- Percentage calculations
- Conditional filtering
- Department-level analysis
- Doctor workload analysis
- Readmission analysis
- Treatment analysis
- Monthly trend analysis

A total of **30 SQL analytical questions** were completed, followed by a practical SQL assessment.

---

## Power BI Dashboard

An interactive Power BI dashboard was created to present the major findings.

### Key Performance Indicators

- Total Patients — **12,000**
- Total Appointments — **45,000**
- Total Admissions — **9,000**
- Total Treatments — **12,892**
- Completion Rate — **77.94%**
- Readmission Rate — **9.16%**
- Average Waiting Time — **28.75 minutes**
- Average Length of Stay — **4.01 days**
- Average Treatment Cost — **₹3,925.36**

### Dashboard Analysis

The dashboard includes:

- Appointment Status
- Monthly Appointment Trend
- Appointment Volume by Department
- Admissions by Department
- Readmission Rate by Department
- Treatment Outcomes
- Average Treatment Cost by Treatment Type
- Average Waiting Time by Department
- Average Length of Stay by Department
- Treatment Outcome Distribution
- Department Performance
- Doctor Workload

### Interactive Filters

The dashboard contains slicers for:

- Department
- Appointment Status
- Appointment Type
- Appointment Date

These filters allow users to interactively explore the hospital data.

---

## Key Business Insights

### 1. Pediatrics Readmission Rate

Pediatrics recorded the highest department-level readmission rate at **10.49%**, with **1,296 admissions** and **136 readmissions**.

### 2. General Medicine Admissions

General Medicine recorded the highest number of admissions with **1,374 admissions**.

### 3. Appointment Completion Rate

The overall appointment completion rate was **77.94%**.

### 4. Average Waiting Time

The overall average appointment waiting time was approximately **28.75 minutes**.

### 5. Average Length of Stay

The average hospital length of stay was approximately **4.01 days**.

### 6. Treatment Outcomes

**Improved** was the most common treatment outcome, accounting for approximately **68.02%** of treatments.

### 7. Treatment Cost

**Medication** had the highest average treatment cost among the treatment types, at approximately **₹3,970.72**.

---

## Tools & Technologies

### Programming & Data Analysis

- Python
- Pandas
- Jupyter Notebook

### Database

- PostgreSQL
- pgAdmin

### Data Visualization

- Microsoft Power BI
- DAX

### Other Tools

- GitHub
- VS Code
Hospital-Healthcare-Analytics/
│
├── Python/
│   └── Hospital analysis.ipynb
│
├── SQL/
│   └── SQL analysis.sql
│
├── PowerBI/
│   └── Hospital_dashboard.pbix
│
├── Cleaned_Data/
│   ├── patients_clean.csv
│   ├── doctors_clean.csv
│   ├── departments_clean.csv
│   ├── appointments_clean.csv
│   ├── admissions_clean.csv
│   └── treatments_clean.csv
│
├── Screenshots/
│   └── hospital_dashboard.png
│
└── README.md
## Project structure 
Raw Hospital Data
       ↓
Data Cleaning & Validation
       ↓
Python / Pandas Analysis
       ↓
Cleaned CSV Datasets
       ↓
PostgreSQL Database
       ↓
SQL Analysis
       ↓
Power BI Data Model
       ↓
DAX Measures
       ↓
Interactive Dashboard
       ↓
Business Insights
## Project Workflow 
Raw Hospital Data
       ↓
Data Cleaning & Validation
       ↓
Python / Pandas Analysis
       ↓
Cleaned CSV Datasets
       ↓
PostgreSQL Database
       ↓
SQL Analysis
       ↓
Power BI Data Model
       ↓
DAX Measures
       ↓
Interactive Dashboard
       ↓
Business Insights
## Conclusion

This project demonstrates an end-to-end Data Analyst workflow for healthcare data, covering data cleaning, exploratory analysis, SQL-based analysis, and interactive Power BI reporting.

The analysis provides insights into patient activity, appointment performance, hospital admissions, readmissions, treatment outcomes, waiting time, length of stay, treatment costs, department performance, and doctor workload.

By combining **Python, Pandas, PostgreSQL, SQL, Power BI, and DAX**, the project transforms raw healthcare data into structured analysis and meaningful business insights.

Overall, this project demonstrates practical skills in **data preparation, analytical SQL, data visualization, dashboard development, and business insight generation**.
