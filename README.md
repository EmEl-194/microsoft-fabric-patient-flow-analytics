## Project Overview
This project delivers an end‑to‑end healthcare analytics solution built using Microsoft Fabric, integrating Lakehouse ingestion, semantic modeling, Power BI reporting, and real‑time Activator alerts.
The goal is to help MediCare Plus Hospital monitor patient wait times, satisfaction, treatment duration, and readmission risks in real time to support operational decision‑making.

## Business Problem
MediCare Plus Hospital was experiencing:
Rising patient wait times
Increasing 30‑day readmission rates
Limited visibility into department‑level performance
No real‑time monitoring or automated alerts
Manual reporting processes that delayed intervention
These challenges affected patient satisfaction, operational efficiency, and regulatory compliance.

## Project Objectives
Build a unified data foundation using Microsoft Fabric Lakehouse
Create a semantic model linking patient visits to doctor data
Develop a Power BI dashboard for real‑time KPI monitoring
Configure Activator alerts for critical thresholds
Provide actionable insights to hospital leadership

## Tools & Technologies
Microsoft Fabric Lakehouse – Data ingestion & storage
Power BI – KPI cards, visuals, and interactive reporting
Semantic Model – Star schema linking fact & dimension tables
Activator Alerts – Automated notifications for KPI breaches
CSV Data – PatientVisits & DoctorData

## Data Model
The semantic model links:
Fact Table: PatientVisits
Dimension Table: DoctorData
Join Key: DoctorID

This structure supports efficient slicing by doctor, department, visit type, and outcome.
[MediCarePlus%20Semantic%20Model.png](MediCarePlus Semantic Model.png)
