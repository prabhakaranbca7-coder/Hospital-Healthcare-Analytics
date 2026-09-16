# Hospital Healthcare Analytics

## 📌 Project Overview

This is an end-to-end healthcare analytics project designed to analyze hospital operations, appointments, admissions, treatments, patient information, and department performance.

The project follows a complete Data Analyst workflow:

**Data Cleaning → Python/Pandas Analysis → PostgreSQL → SQL Analysis → Power BI Dashboard → Business Insights**

The objective is to transform raw hospital data into meaningful insights that can support operational and management decisions.

---

## 🎯 Business Objectives

The project focuses on answering important healthcare business questions such as:

- How many patients, appointments, admissions, and treatments are recorded?
- Which departments receive the highest number of appointments?
- What is the appointment completion rate?
- Which departments have higher readmission rates?
- What is the average patient waiting time?
- What is the average length of hospital stay?
- Which treatment types have higher average costs?
- What are the most common treatment outcomes?
- How does appointment volume change over time?
- Which doctors have the highest appointment workload?
- Which departments may require further operational attention?

---

## 📊 Dataset

The project contains six cleaned datasets:

| Dataset | Records | Description |
|---|---:|---|
| Patients | 12,000 | Patient demographic and registration information |
| Doctors | 80 | Doctor details, specialization, experience, and employment type |
| Departments | 8 | Department capacity, staffing, beds, and occupancy |
| Appointments | 45,000 | Appointment details, status, waiting time, and satisfaction |
| Admissions | 9,000 | Hospital admission, discharge, department, and readmission information |
| Treatments | 12,892 | Treatment details, costs, duration, diagnosis, and outcomes |

**Total records analyzed: 87,972**

> The datasets used in this portfolio project are cleaned/anonymized project data and should not contain real patient-identifying information.

---

## 🧹 Data Cleaning

Data cleaning and preparation were performed using Python and Pandas.

The cleaning process included:

- Checking dataset dimensions
- Checking missing values
- Detecting duplicate records
- Validating date fields
- Checking invalid relationships between tables
- Handling missing waiting-time values
- Checking treatment-date validity
- Calculating length of stay
- Validating numerical ranges
- Identifying statistical outliers
- Checking categorical values
- Creating cleaned datasets for further analysis

Outliers were identified during analysis and retained where they could represent genuine hospital cases rather than obvious data-entry errors.

---

## 🐍 Python / Pandas Analysis

Python was used for data cleaning, validation, exploratory analysis, and preparation of the datasets.

### Main Python tasks

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
- Exporting cleaned datasets

### Example analyses

- Patient age distribution
- Insurance-type distribution
- Appointment status analysis
- Waiting-time analysis
- Department occupancy analysis
- Admission analysis
- Length-of-stay analysis
- Treatment cost analysis
- Treatment outcome analysis

---

## 🗄️ PostgreSQL & SQL Analysis

The cleaned datasets were imported into PostgreSQL for relational analysis.

### Database

**Database:** `Advanced_analysis`

The project contains relationships between:

```text
patients ──< appointments >── doctors ──> departments
patients ──< admissions >──── doctors
                  │
                  ├──────────> departments
                  └──< treatments
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
