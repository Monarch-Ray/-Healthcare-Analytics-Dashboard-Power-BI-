# Healthcare-Analytics-Dashboard-Power-BI-
## 📌 Project Overview

This project is an end-to-end healthcare analytics solution built using Power BI, designed to analyze operational, clinical, and inventory data from a simulated healthcare environment.

- The dashboard supports:

- Executive decision-making

- Operational monitoring

- Clinical insights

- Inventory risk management

The project follows industry best practices including star schema modeling, clean Power Query transformations, and DAX-based KPIs.

## 🎯 Objectives

- Build a scalable healthcare data model

- Visualize appointment and encounter trends

- Analyze clinical data (labs, vitals, diagnoses, procedures)

- Monitor inventory levels and risk

- Create executive-ready KPIs and dashboards

## 🧱 Data Model Design

The project uses a Star Schema for performance and clarity.
# Dimension Tables

- Patients

- Providers

- Departments

- Payers
  
# Fact Tables

- Appointments

- Encounters

- Inventory

- Labs

- Vitals

- Diagnoses

- Procedures

- Satisfaction

All relationships are:

- One-to-many

- Single-direction

- No fact-to-fact joins

## 🔧 Data Transformation (Power Query)

Key transformation principles:

- Remove unnecessary PHI fields

- Enforce correct data types

- Remove duplicates using primary keys

- No business logic stored in columns unless necessary

All inventory risk logic is calculated dynamically using DAX, not Power Query columns.

## 📐 Key DAX Measures
# Operational KPIs

- Total Appointments

- Appointment Completion Rate

- Total Encounters

- Total Patients

- Total Encounters
- Total Male Patients
- Total Female Patients
- Average BMI
- Female Diagnosis %
- Male Diagnosis %
- Average Rating
- Average Staff Rating
- Average Environment Rating

- Inventory KPIs

- Total Inventory Items

- Low Stock Items (calculated using StockLevel ≤ ReorderLevel)

- Low Stock Rate (%)

# Clinical KPIs

- Total Lab Tests

- Average Systolic BP

- Total Patients Discharged Home

- Total Diagnoses

- Total Procedures

## 📊 Dashboards & Visuals

<img width="912" height="505" alt="Screenshot (65)" src="https://github.com/user-attachments/assets/2d2f6ad3-5911-4318-bee7-90e4a8837343" />
<img width="912" height="505" alt="Screenshot (66)" src="https://github.com/user-attachments/assets/ef467603-bbf9-4efc-a773-37f1012cefea" />
<img width="912" height="505" alt="Screenshot (67)" src="https://github.com/user-attachments/assets/a3c1f22d-02bb-4d13-8c39-4863f4986aed" />
<img width="913" height="504" alt="Screenshot (68)" src="https://github.com/user-attachments/assets/b3e1e84d-bc77-45b8-afc5-00b8fac86dec" />
<img width="914" height="503" alt="Screenshot (62)" src="https://github.com/user-attachments/assets/246b6669-d5f2-45c0-b0d7-e413f7eb6de4" />




## 🧠 Key Learnings

- Proper data modeling is critical for healthcare analytics

- Measures should handle business logic, not columns

- Incremental table loading improves performance

- Star schemas scale better than flat models

- Healthcare dashboards must balance insight with data privacy

