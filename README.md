# 🏥 Hospital Emergency Room Dashboard

> **Interactive Power BI dashboard for analyzing Emergency Room patient volume, wait times, satisfaction, referrals, admissions, demographics, and operational patterns.**



## 📌 Project Overview

The **Hospital Emergency Room Dashboard** is an end-to-end Power BI analytics project designed to help hospital stakeholders monitor Emergency Room performance and identify operational patterns.

The dashboard analyzes **9,216 patient records** covering **April 2023 to October 2024** and provides both high-level KPIs and patient-level details.

The solution was developed around four dashboard views:

1. **Monthly View**
2. **Consolidated View**
3. **Patient Details**
4. **Key Takeaways**

The project follows a complete analytics workflow from requirements gathering and data preparation through data modeling, DAX calculations, dashboard development, and insight generation.

---

## 🎯 Business Objective

The main objective is to provide a data-driven view of Emergency Room operations so stakeholders can:

- Monitor patient volumes and trends.
- Understand average patient waiting time.
- Track patient satisfaction.
- Analyze admission patterns.
- Identify departments receiving the highest number of referrals.
- Understand patient demographics.
- Identify busy days and hours.
- Monitor the percentage of patients seen within 30 minutes.
- Drill down to individual patient records when required.
- Generate actionable operational insights.

---

## 📊 Key KPIs

| KPI | Overall Result |
|---|---:|
| 👥 Total Patients | **9,216** |
| ⏱️ Average Wait Time | **35.3 minutes** |
| ⭐ Average Patient Satisfaction | **4.99 / 10** |
| 🔄 Patients Referred | **3,816** |
| 🏥 Admitted Patients | **4,612** |
| 🚪 Non-Admitted Patients | **4,604** |
| ⏱️ Patients Seen Within 30 Minutes | **40.68%** |
| ⏱️ Patients Not Seen Within 30 Minutes | **59.32%** |

> **Note:** The dashboard's satisfaction KPI is displayed on a 10-point scale, while the source field contains the underlying patient satisfaction scores.

---

# 📑 Dashboard Views

## 1. 📅 Monthly View

The Monthly View provides a detailed analysis for a selected year and month.

### Key analysis areas

- Patient Admission Status
- Patient Age Distribution
- Department Referrals
- Percentage of Patients Seen Within 30 Minutes
- Gender Distribution
- Patient Race Distribution
- Patient Volume by Day and Hour
- Monthly patient volume
- Average wait time trend
- Patient satisfaction trend
- Referral trend


---

## 2. 📈 Consolidated View

The Consolidated View provides a holistic summary for a selected date range.

### Key analysis areas

- Total number of patients
- Average wait time
- Patient satisfaction
- Number of referred patients
- Admission vs. non-admission
- Patients seen within 30 minutes
- Age-group distribution
- Gender distribution
- Department referrals
- Patient race
- Patient volume by day and hour



---

## 3. 👤 Patient Details

The Patient Details page provides a granular patient-level view for detailed analysis and troubleshooting.

### Fields included

- Patient ID
- Patient Name
- Patient Gender
- Patient Age
- Patient Admission Date
- Patient Race
- Patient Wait Time
- Department Referral
- Admission Status



---

## 4. 💡 Key Takeaways

The Key Takeaways page converts dashboard results into a concise descriptive analysis for stakeholders.

The analysis covers:

- Patient wait time and satisfaction
- Department referrals
- Peak patient periods
- Patient demographics
- Race distribution
- Admission patterns
- Overall operational summary



---

# 🔎 Key Insights

Based on the dashboard and source dataset:

### ⏱️ Wait Time

The average patient wait time is approximately **35.3 minutes**.

The dashboard also tracks whether patients were seen within the 30-minute target. In the source data, approximately **40.68%** of patients had a wait time of 30 minutes or less.

### ⭐ Patient Satisfaction

The overall average patient satisfaction score is approximately **4.99**.

The dashboard uses the satisfaction trend to identify changes in patient experience over time.

### 🏥 Admission Pattern

The dataset contains almost an even split between admitted and non-admitted patients:

- **4,612 admitted**
- **4,604 non-admitted**

This represents approximately **50.04% admitted** and **49.96% non-admitted**.

### 🔄 Department Referrals

Out of 9,216 patients, **3,816** have a department referral.

The highest referral categories are:

| Department | Patients |
|---|---:|
| General Practice | 1,840 |
| Orthopedics | 995 |
| Physiotherapy | 276 |
| Cardiology | 248 |
| Neurology | 193 |
| Gastroenterology | 178 |
| Renal | 86 |

A further **5,400** records have no department referral.

### 👥 Age Distribution

The **30–39** age group has the highest number of patients with **1,200** records, followed by:

- 20–29: 1,188
- 10–19: 1,179
- 60–69: 1,154
- 70–79: 1,153
- 50–59: 1,151
- 40–49: 1,135
- 0–9: 1,056

### 🌎 Race Distribution

The largest patient race groups are:

| Race | Patients |
|---|---:|
| White | 2,571 |
| African American | 1,951 |
| Two or More Races | 1,557 |
| Asian | 1,060 |
| Declined to Identify | 1,030 |
| Pacific Islander | 549 |

### 📅 Patient Volume by Day

Based on the source data, the highest patient volumes occur on:

| Day | Patients |
|---|---:|
| Saturday | 1,377 |
| Thursday | 1,332 |
| Sunday | 1,318 |

This can help hospital management evaluate staffing and resource allocation by day.

---

# 🛠️ Tools & Technologies

- **Microsoft Power BI**
- **DAX**
- **CSV**
- Data Cleaning & Quality Checks
- Data Modeling
- Data Visualization
- Business Requirements Analysis

---

# 🔄 Project Workflow

The project follows an end-to-end BI development process:

```text
Requirement Gathering
        ↓
Business Requirements
        ↓
Data Walkthrough
        ↓
Data Connection
        ↓
Data Cleaning / Quality Check
        ↓
Data Modeling
        ↓
Data Processing
        ↓
DAX Calculations
        ↓
Dashboard Layout
        ↓
Charts Development & Formatting
        ↓
Dashboard / Report Development
        ↓
Insights Generation
```

---

# 📋 Business Requirements

## KPI Requirements

### Number of Patients
Measure the total number of patients visiting the Emergency Room and display the trend over time.

### Average Wait Time
Calculate the average time patients wait before being attended to by medical staff and identify periods with higher waiting times.

### Patient Satisfaction Score
Analyze average patient satisfaction over time to evaluate service quality and identify potential operational issues.

### Number of Patients Referred
Track patients referred from the Emergency Room to different departments and identify departments with high referral volumes.

---

# 🧩 Data Fields

The source dataset contains **12 fields**:

| Field | Description |
|---|---|
| Patient Id | Unique identifier for each patient |
| Patient Admission Date | Date and time of ER admission |
| Patient First Initial | First initial used in the patient record |
| Patient Last Name | Patient last name |
| Patient Gender | Patient gender |
| Patient Age | Patient age at admission |
| Patient Race | Patient race/ethnicity category |
| Department Referral | Department to which the patient was referred |
| Patient Admission Flag | Indicates whether the patient was admitted |
| Patient Satisfaction Score | Patient evaluation of the ER experience |
| Patient Waittime | Time waited before being attended to |
| Patients CM | Case manager-related field |

---

# 🎛️ Dashboard Interactivity

The report includes interactive controls such as:

- Date range selection
- Year selection
- Month selection
- Patient Race filter
- Patient Gender filter
- Patient Satisfaction filter
- Navigation buttons between dashboard pages
- Patient-level filtering and drill-down analysis

These controls allow users to move from an overall hospital view to more detailed operational analysis.

---


# 🚀 How to Use the Project

1. Download or clone this repository.
2. Open the `.pbix` file using **Microsoft Power BI Desktop**.
3. If required, update the CSV data source path.
4. Refresh the dataset.
5. Use the navigation buttons to move between:
   - Monthly View
   - Consolidated View
   - Patient Details
   - Key Takeaways
6. Apply filters to explore different patient groups and time periods.

---

# 📌 Project Highlights

- End-to-end Power BI dashboard project.
- 9,216 patient records analyzed.
- Four interactive report pages.
- KPI-driven Emergency Room analysis.
- Patient-level drill-down capability.
- Demographic and referral analysis.
- Day and hour-based patient volume analysis.
- 30-minute patient response-time analysis.
- DAX-based KPI calculations.
- Actionable insights for operational decision-making.

---

# 💼 Business Value

The dashboard can support hospital management in:

- **Staffing:** Identifying high-volume days and hours.
- **Patient Flow:** Monitoring wait times and 30-minute response performance.
- **Resource Allocation:** Understanding referral demand by department.
- **Patient Experience:** Tracking satisfaction levels.
- **Capacity Planning:** Understanding admission and patient-volume patterns.
- **Operational Monitoring:** Providing a centralized view of ER performance.
- **Detailed Investigation:** Reviewing patient-level records when anomalies or operational issues require investigation.

---

# 📸 Dashboard Preview

### Consolidated View
![Alt text](https://github.com/Panchal-sunil/Hospital-Emergency-Room-Project/blob/main/Images/Consolidated_View_Chart.png)

### Monthly View
![Alt text](https://github.com/Panchal-sunil/Hospital-Emergency-Room-Project/blob/main/Images/Monthly_View_Chart.png)

### Patient Details
![Alt text]( https://github.com/Panchal-sunil/Hospital-Emergency-Room-Project/blob/main/Images/Patient_Details.png)

### Key Takeaways
![Alt text](https://github.com/Panchal-sunil/Hospital-Emergency-Room-Project/blob/main/Images/Key_Takeaway.png)

---

# 📚 Documentation

The project documentation includes the business requirements, dashboard objectives, KPI requirements, and data terminology used for the analysis.

---

## 👨‍💻 Project

**Hospital Emergency Room Dashboard**

**Technology:** Microsoft Power BI | DAX | Data Analysis | Data Visualization

**Dataset:** Hospital Emergency Room patient data

**Analysis Period:** April 2023 – October 2024

---

⭐ **If you find this project useful, consider giving the repository a star.**
