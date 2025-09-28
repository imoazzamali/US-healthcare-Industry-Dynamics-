# US-healthcare-Industry-Dynamics-
A Power BI project analyzing U.S. healthcare trends from 2019–2020, covering hospitals, patients, payers, and providers. Includes schema, PBIX source file, and PDF report for insights into costs, payments, patient demographics, and provider performance.


# U.S. Healthcare Dynamics Dashboard (2019–2020)

## 📊 Project Overview
This repository contains a **Power BI project** designed to analyze the **U.S. healthcare system** between **2019 and 2020**.  
It provides deep insights into **hospitals, patients, payers, and providers** through an interactive data model and visual dashboards.

The aim is to empower **healthcare decision-makers, analysts, and policymakers** by uncovering financial, demographic, and operational patterns in healthcare delivery.

---

## 📂 Repository Contents
- `dashboards.pbix` → Power BI source file containing the interactive dashboards  
- `report.pdf` → Exported report with visualizations and insights  
- `schema.png` → Data model schema (fact & dimension tables)  

---

## 🏥 Key Analysis Areas
### 1. **Executive Summary**
- High-level healthcare trends (patients, expenses, payments, revenues).  
- Year-over-year comparisons.  

### 2. **Hospital Analysis**
- Performance metrics: AR ratio, IPTP ratio, bad debts.  
- Expense and CPT unit distribution by hospital.  
- Identification of critical hospitals requiring attention.  

### 3. **Patient Analysis**
- Demographics (gender, blood group, lifestyle).  
- Patient distribution across states and regions.  
- Trends in patient outcomes and enrollment.  

### 4. **Payer-Provider Analysis**
- Relationship between payers and providers.  
- Revenue streams (insurance vs. patient).  
- Regional specialty distribution and provider activity.  

### 5. **Financial Insights**
- Monthly gross and adjusted expenses.  
- Adjustment factors and debt impact.  
- Revenue trends (insurance, patient, total).  

---

## 🗂 Data Model
The solution is built on a **star schema** in Power BI:  

- **Fact Table**: Transactions (expenses, revenue, adjustments, CPT units).  
- **Dimension Tables**:  
  - `Patient_Lookup` (demographics, health factors)  
  - `Hospital_Lookup` (hospital details)  
  - `Physician_Lookup` (provider info, specialties)  
  - `Speciality_Lookup` (provider specialty types)  
  - `Payer_Lookup` (payer details)  
  - `CptCode_Lookup` (procedure codes)  
  - `DiagnosisCode_Lookup` (diagnosis codes)  
  - `DimDate` (date dimension for time-series analysis)  
  - `Adjustment Factor (%)` (financial adjustment ratios)  
  - `BadDebtTable` & `Transaction_Lookup` (financial integrity checks)  

