# 🏥 HealthCare Data Analysis using SQL

> **Note:** This project is based on a synthetic dataset not derived from real-world data. Please do not use the results for decision-making or factual analysis.

## 📑 Overview

This project demonstrates exploratory data analysis and insights extraction using **SQL** on a simulated **HealthCare** database. It includes data manipulation, aggregation, ranking, filtering, and stored procedure logic to mimic real-world analytical scenarios in the healthcare domain.

## 📂 Dataset Information

The database contains anonymized patient records with the following key attributes:

- **Patient Demographics**: Name, Age, Blood Type
- **Medical Data**: Medical Condition, Test Results, Medication, Doctor
- **Hospitalization Info**: Hospital, Admission & Discharge Dates
- **Insurance Details**: Insurance Provider, Billing Amount

## 🧠 Objectives

The goal was to extract meaningful insights from healthcare data using SQL queries, such as:

- Hospital & Insurance performance
- Patient demographic distribution
- Treatment duration & cost
- Risk categorization and donor matching
- Custom procedure to match universal donors with universal recipients

---

## ⚙️ Project Setup

1. **Create and use the database**:
   ```sql
   CREATE DATABASE Healthcare;
   USE Healthcare;
   ```

## 📂 Assumptions

- The table is **pre-populated** with simulated healthcare records.
- All queries assume the existence of a table named `Healthcare`.

---

## 🔍 Key Analytical Queries

### 🧾 Demographic & Statistical Analysis

- ✅ Total patients, average & maximum age  
- ✅ Age-wise distribution of hospitalized patients  
- ✅ Frequency of each medical condition  

### 🏥 Hospital & Insurance Insights

- ✅ Most preferred hospital and insurance provider  
- ✅ Billing amount per insurance provider  
- ✅ Average billing by medical condition  

### 🧪 Medical Treatment Insights

- ✅ Hospitalization duration and test results  
- ✅ Medication rankings per condition  
- ✅ Categorizing patients based on test outcomes  

### 🩸 Blood Type Analysis

- ✅ Count of each blood type  
- ✅ Count of universal donors (`O-`) and recipients (`AB+`)  
- ✅ Distribution of blood types among age group 20–45  

### 🔁 Stored Procedure

- ✅ A stored procedure `Blood_Matcher()` was created to find universal donors (`O-`) for recipients (`AB+`) prioritizing:
  1. **Same hospital**
  2. **Then different hospitals**

### 📅 Temporal Analysis

- ✅ Hospital admission counts by year (2024 & 2025)

---

## 📊 Results Summary

- 🏥 Identified high-admission hospitals and popular insurance providers  
- 💊 Mapped medication preference per condition  
- 💸 Extracted patterns in hospitalization cost and stay duration  
- 🩸 Created procedure to match blood donors and recipients  
- 🚦 Categorized patient conditions for better decision-making  

---

## 🛠 Tools & Technologies

- **SQL** (MySQL / MariaDB flavor)  
- **Relational Database** design principles  
- **Stored Procedures**  
- **Window Functions** (RANK, DENSE_RANK)  
- **Aggregations, Joins, and Grouping**  

---

## 📌 Conclusion

This project highlights the power of **SQL** in extracting actionable insights from structured health data. It simulates practical use cases such as:

- Hospital operations tracking  
- Insurance provider billing analysis  
- Patient treatment profiling  
- Donor-recipient matching logic  

By building logical queries and leveraging SQL’s full capabilities, we can translate raw healthcare records into meaningful intelligence for informed decision-making.

---
