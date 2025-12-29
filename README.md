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

- Medications

- Imaging

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

- Unique Patients

- Total Encounters
- Total Male Patients
- Total Female Patients
- Average BMI
- Female Diagnosis %
- Male Diagnosis %

- Inventory KPIs

- Total Inventory Items

- Low Stock Items (calculated using StockLevel ≤ ReorderLevel)

- Low Stock Rate (%)

# Clinical KPIs

- Total Lab Tests

- Average Systolic BP

- Average Heart Rate

- Total Diagnoses

- Total Procedures

## 📊 Dashboards & Visuals

<img width="912" height="505" alt="Screenshot (59)" src="https://github.com/user-attachments/assets/5b8811fb-47f1-4c7c-a5de-60fc042a934b" />
<img width="910" height="506" alt="Screenshot (56)" src="https://github.com/user-attachments/assets/3e39b191-3602-4db9-9392-892d11ba9e6d" />
<img width="913" height="505" alt="Screenshot (58)" src="https://github.com/user-attachments/assets/e00dea31-d613-4894-ab14-0dc57c3f8f91" />
<img width="912" height="503" alt="Screenshot (60)" src="https://github.com/user-attachments/assets/002d7287-0532-4311-8969-f557c3c546bf" />



## 🧠 Key Learnings

- Proper data modeling is critical for healthcare analytics

- Measures should handle business logic, not columns

- Incremental table loading improves performance

- Star schemas scale better than flat models

- Healthcare dashboards must balance insight with data privacy

