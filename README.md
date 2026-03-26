# 📊 HR Analytics Dashboard — Employee Attrition Analysis

![Power BI](https://img.shields.io/badge/Tool-Power%20BI-F2C811?logo=powerbi&logoColor=black)
![Excel](https://img.shields.io/badge/Data-Excel-217346?logo=microsoftexcel&logoColor=white)
![DAX](https://img.shields.io/badge/Formula-DAX-0078D4)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---

## 📌 Project Overview

This Power BI dashboard analyzes **employee attrition** to help HR teams understand **why employees are leaving** and **which groups are most at risk**. Built using real IBM HR data, it transforms raw employee records into clear, actionable business insights.

> **Business Question:** *Why is the company losing employees — and what can be done about it?*

---

## 🖼️ Dashboard Preview

> 📌 **Click on the image to view full size**

[![HR Analytics Dashboard]([screenshots/dashboard_preview.png)](screenshots/dashboard_preview.png](https://github.com/mahesh735-ai/HR-Analytics-Dashboard/blob/main/dashboard_preview.png))

---

## 🎯 Key KPIs

| Metric | Value |
|---|---|
| Total Employees | 1,470 |
| Attrition Count | 237 |
| **Attrition Rate** | **16.1%** |
| Average Age | 37 Years |
| Average Salary | 6.5K |
| Avg Years at Company | 7.0 Years |

---

## 📈 Key Insights

- 🔴 **1 in every 6 employees** is leaving — attrition rate is 16.1%
- 👶 **Age 26–35** has the highest attrition (116 employees) — early-career dissatisfaction
- 💰 **Salary below 5K** is the biggest driver — 163 out of 237 exits
- 📅 Most attrition happens at **Year 1 (59 employees)** — onboarding and early experience issue
- 🧪 **Laboratory Technicians (62)** and **Sales Executives (57)** are highest-risk roles
- 🎓 **Life Sciences (37.6%)** background employees leave the most
- 👨 **Male attrition (140)** is higher than **Female (79)**

---

## 🔄 Project Workflow

### Step 1 — Excel (Data Understanding)
- Explored dataset using filters and pivot tables
- Identified key columns for analysis
- Removed unnecessary columns not needed for dashboard

### Step 2 — Power BI (Data Transformation)
- Loaded data into Power BI Desktop
- Checked and fixed data types in Power Query
- Replaced unclear values with meaningful labels
- **Created new column:** Attrition Count → `Yes = 1`, `No = 0`
- Removed unnecessary columns in Power Query

### Step 3 — DAX Measures
```DAX
Attrition Rate = SUM([Attrition Count]) / SUM([Employee Count])
```

### Step 4 — Dashboard
- No data modeling required (single table)
- Added 6 KPI Cards across the top
- Built 6 interactive charts
- Added **Slicers** for Department (Human Resources / R&D / Sales) and Age Group

---

## 📊 Charts Used

| Chart Type | Used For | Key Finding |
|---|---|---|
| Donut Chart | Attrition by Education | Life Sciences = 37.6% |
| Bar Chart | Attrition by Age Group | 26–35 = highest (116) |
| Matrix Table | Attrition by Job Role × Satisfaction Level | Lab Technician = 62 total |
| Bar Chart | Attrition by Salary Slab | Below 5K = 163 exits |
| Line / Area Chart | Attrition by Years at Company | Year 1 = 59 (peak) |
| Bar Chart | Attrition by Job Role | Lab Tech > Sales Exec > Research Sci |

---

## 💡 Business Recommendations

1. **Improve salary** for employees earning below 5K
2. **Strengthen onboarding** and engagement in first 1–2 years
3. **Reduce workload pressure** for Laboratory Technicians and Sales Executives
4. **Provide career growth** paths for employees aged 26–35
5. Implement **retention programs** targeted at Life Sciences background employees

---

## ⚠️ Challenges Faced & Solutions

| Challenge | How I Solved It |
|---|---|
| Identifying key columns from raw data | Used Pivot Tables in Excel to analyze each column |
| Converting Attrition (Yes/No) to numeric | Added calculated column in Power Query: Yes=1, No=0 |
| Building correct Attrition Rate | Used DAX: SUM(Attrition Count) / SUM(Employee Count) |
| Keeping dashboard clean & readable | Limited to 6 visuals + 3 department slicers |

---

## 🛠️ Tools & Technologies

- **Microsoft Excel** — Data exploration & Pivot analysis
- **Power BI Desktop** — Transformation, DAX, Dashboard creation
- **Power Query** — Data cleaning & column operations
- **DAX** — KPI & Attrition Rate calculation

---

## 📁 Repository Structure

```
HR-Analytics-Dashboard/
│
├── dataset/
│   └── HR_Analytics.csv                     # Source dataset
│
├── dashboard/
│   └── HR_Analytics_Dashboard.pbix          # Power BI file
│
├── screenshots/
│   └── dashboard_preview.png                # Dashboard screenshot
│
├── documentation/
│   └── HR_Analytics_Documentation.docx      # Full project notes
│
└── README.md                                # Project overview
```

---

## 🏁 Conclusion

This dashboard reveals that **low salary, early-career experience gap, and high-pressure roles** are the key drivers behind the company's **16.1% attrition rate**.

By acting on these insights, HR teams can reduce attrition, improve satisfaction, and **save significant hiring and training costs**.

---

## 👤 Author

**Mahesh**
- 💼 LinkedIn: [Mahesh Thakare](https://www.linkedin.com/in/mahesh-thakare-75817b2a7)
- 🐙 GitHub: [mahesh735-ai](https://github.com/mahesh735-ai)

---

> ⭐ *If you found this project helpful, please give it a star!*  
> 💬 *Open to feedback and suggestions for my next project!*
