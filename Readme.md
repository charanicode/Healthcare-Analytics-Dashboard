# 🏥 Healthcare Analytics Dashboard | Power BI

## 📌 Project Overview
The Healthcare Analytics Dashboard is an interactive Power BI project designed to analyze patient admissions, demographics, insurance approvals, billing amounts, and hospital operations. It helps users explore healthcare data and identify meaningful business insights through interactive visualizations.

## 🎯 Project Objectives
- Analyze patient admissions across hospitals.
- Understand patient demographics by age group, gender, and blood type.
- Evaluate insurance approval ratios and billing patterns.
- Compare hospital activity and doctor workloads.
- Analyze patient length of stay and medication trends.

## 🛠️ Tools & Technologies
- **Power BI Desktop** — Dashboard development and data visualization
- **DAX** — Measures and KPI calculations
- **Power Query** — Data preparation and transformation

## 📊 Dashboard Pages

### 1. Healthcare Overview
- Total Admissions
- Total Bill Amount
- Total Approved Amount
- Total Patient Pay
- Monthly Admissions Trend
- Admissions by Admission Type
- Admissions by Hospital

### 2. Patient Demographics
- Admissions by Age Group
- Admissions by Gender
- Admissions by Blood Type
- Admissions by Condition
- Average Patient Age

### 3. Insurance & Billing Analysis
- Insurance Approval Ratio
- Bill Amount vs. Approved Amount by Hospital
- Patient Pay by Hospital
- Average Bill Amount by Admission Type
- Total Patient Pay

### 4. Hospital Operations Analysis
- Average Length of Stay
- Admissions by Doctor
- Admissions by Hospital
- Admissions by Medication
- Admissions by Discharge Month

## 📈 Key Business Insights
Based on the dashboard analysis:
- Acevedo recorded the highest number of patient admissions.
- Elective admissions were the most common admission type.
- Acevedo LLC recorded the highest total bill amount.
- The overall insurance approval ratio was approximately 89%.
- Patients in the 30–40 age group recorded the highest number of admissions.

*Note: These insights reflect the results observed in the analyzed dataset.*

## 📐 Key DAX Measures

**Total Admissions**
```DAX
Total Admissions = COUNTROWS(Healthcare)
```

**Total Bill Amount**
```DAX
Total Bill Amount = SUM(Healthcare[Bill Amount])
```

**Total Approved Amount**
```DAX
Total Approved Amount = SUM(Healthcare[Approved Amount])
```

**Total Patient Pay**
```DAX
Total Patient Pay = SUM(Healthcare[Patient Pay])
```

**Insurance Approval Ratio**
```DAX
Insurance Approval Ratio =
DIVIDE(
    SUM(Healthcare[Approved Amount]),
    SUM(Healthcare[Bill Amount]),
    0
)
```

Format the Insurance Approval Ratio measure as a percentage in Power BI.

## 💡 Key Features
- Interactive dashboard visualizations
- KPI cards for important healthcare metrics
- Hospital-wise and admission-type analysis
- Patient demographic segmentation
- Insurance and billing performance analysis
- Date, hospital, and admission-type filters



## 🚀 How to Explore the Project
1. Download the `.pbix` file from this repository.
2. Open it using Microsoft Power BI Desktop.
3. Explore the four dashboard pages.
4. Use the available filters and slicers to analyze the data.



## 👩‍💻 Author
**Charani**

Aspiring Data Analyst | Power BI | SQL | Data Visualization

---

⭐ If you find this project useful, feel free to explore the repository.
