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

```text
patients ──< appointments >── doctors ──> departments
patients ──< admissions >──── doctors
                  │
                  ├──────────> departments
                  └──< treatments
