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
[MediCarePlus Semantic Model.png](MediCarePlus%20Semantic%20Model.png)

## Dashboard Overview
The Power BI dashboard includes:
Avg Wait Time
Avg Patient Satisfaction
Total Patient Visits
Wait Time by Doctor
Treatment Duration by Visit Type
Readmission Within 30 Days
Department‑level Visit Volumes
[MediCarePlus_Report.pdf](MediCarePlus_Report.pdf)

## Real‑Time Alerts (Activator)
Two alert rules were configured:
AvgWaitTime > 15 minutes
AvgPatientSatisfaction < 3.5

When triggered, alerts notify me via teams so I can notify relevant stakeholders and staff to intervene immediately.
[MediCarePlus Activator Alert.png](MediCarePlus%20Activator%20Alert.png)

## Key Insights
Doctors with the highest patient load also showed the longest wait times.
Surgical and emergency visits had the longest treatment durations.
Readmissions were concentrated in specific departments and visit outcomes.
Satisfaction scores dropped sharply when wait times exceeded 15 minutes.
Real‑time alerts enabled faster response to operational bottlenecks.

## Business Recommendations
Based on the analysis of patient wait times, treatment durations, satisfaction scores, and readmission patterns, the following recommendations can help MediCare Plus improve operational efficiency and patient experience:

1. Reduce Wait Time Bottlenecks Through Doctor Workload Balancing
High‑volume doctors consistently showed longer wait times. Redistributing patient load across available clinicians or adjusting scheduling blocks can reduce congestion and improve flow.

2. Implement Fast‑Track Protocols for High‑Duration Visit Types
Surgical consultations and emergency visits recorded the longest treatment durations. Introducing pre‑assessment steps, standardized triage, or dedicated procedure slots can shorten overall cycle time.

3. Strengthen Discharge Planning for High‑Risk Visit Categories
Readmissions were concentrated in emergency, surgical, and routine checkup visits. Enhancing discharge instructions, follow‑up reminders, and post‑visit monitoring for these groups can reduce 30‑day readmission rates.

4. Monitor Satisfaction Drivers in Real Time
Satisfaction scores dropped sharply when wait times exceeded 15 minutes. Using Activator alerts to notify supervisors when thresholds are breached enables immediate intervention and improves patient experience.

5. Increase Department‑Level Visibility for Operational Decision‑Making
Departments such as Emergency and General Medicine handle the highest visit volumes. Providing department heads with real‑time dashboards empowers them to allocate staff, adjust workflows, and respond to spikes in demand.

6. Use Predictive Indicators to Prevent Service Delays
Patterns in wait times and treatment durations can be used to forecast peak periods. Integrating predictive analytics into the dashboard can help the hospital proactively staff high‑demand windows.

7. Standardize Data Capture Across Visit Types
Variability in documentation and visit categorization can affect reporting accuracy. Standardizing data entry fields and enforcing consistent visit type definitions will improve the reliability of insights.
