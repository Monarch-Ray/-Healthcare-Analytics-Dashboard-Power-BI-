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

- Appointments per Provider

- Inventory KPIs

- Total Inventory Items

- Low Stock Items (calculated using StockLevel ≤ ReorderLevel)

- Low Stock Rate (%)

# Clinical KPIs

- Total Lab Tests

- Abnormal Lab Results

- Average Heart Rate

- Total Diagnoses

- Total Procedures

## 📊 Dashboards & Visuals

<img width="929" height="495" alt="Screenshot (54)" src="https://github.com/user-attachments/assets/c8c3bc86-2e15-4a16-a427-7d20760fec54" />
<img width="928" height="500" alt="Screenshot (53)" src="https://github.com/user-attachments/assets/4424e633-e369-4f8e-bee1-7900e8c46dda" />
<img width="929" height="507" alt="Screenshot (50)" src="https://github.com/user-attachments/assets/3539e9c6-909f-4fc6-9716-9e257234184d" />


## 🧠 Key Learnings

- Proper data modeling is critical for healthcare analytics

- Measures should handle business logic, not columns

- Incremental table loading improves performance

- Star schemas scale better than flat models

- Healthcare dashboards must balance insight with data privacy

