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

- Average length of stay

- Average overall rating

- Appointment completion rate

- Total patients
- Total Appointments



## 📊 Dashboards & Visuals
<img width="985" height="547" alt="Screenshot (78)" src="https://github.com/user-attachments/assets/3a2cc3fe-b008-425e-ab36-d589a51cbc48" />






## 🧠 Key Learnings

- Proper data modeling is critical for healthcare analytics

- Measures should handle business logic, not columns

- Incremental table loading improves performance

- Star schemas scale better than flat models

- Healthcare dashboards must balance insight with data privacy

