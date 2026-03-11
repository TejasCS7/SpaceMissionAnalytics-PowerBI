# 🚀 Exploratory Data Analysis on Space Exploration Missions

> A comprehensive **Power BI** dashboard project that transforms complex space mission datasets into actionable insights — built as part of the **Infosys Next Gen Employability Program**.

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Dashboard Preview](#-dashboard-preview)
- [Key Metrics](#-key-metrics)
- [Problem Statement](#-problem-statement)
- [Project Objectives](#-project-objectives)
- [Proposed Solution](#-proposed-solution)
- [Technology Used](#-technology-used)
- [Dashboard Features](#-dashboard-features)
- [Data Pipeline](#-data-pipeline)
- [Insights & Findings](#-insights--findings)
- [Conclusion](#-conclusion)
- [Getting Started](#-getting-started)
- [Author](#-author)

---

## 🌟 Overview

This project leverages **Microsoft Power BI** to perform Exploratory Data Analysis (EDA) on a historical dataset of global space exploration missions. It addresses the challenges of data integration, cleansing, visualization, and predictive modelling specific to space mission datasets — providing a powerful tool for mission planning, risk analysis, and strategic decision-making.

The interactive dashboard enables analysts to quickly uncover patterns, trends, and anomalies across 1,265 recorded space missions spanning over six decades.

---

## 📊 Dashboard Preview

![Space Missions Interactive Dashboard](Interactive_Dashboard.png)

*Interactive Power BI dashboard showcasing mission outcomes, budget analysis, company performance, and launch trends across global space programs.*

---

## 📈 Key Metrics

| Metric | Value |
|--------|-------|
| 🛸 **Total Missions** | 1,265 |
| ✅ **Success Missions** | 1,197 |
| ❌ **Failure Missions** | 48 |
| ⚠️ **Partial Failure Missions** | 19 |
| 🚫 **Prelaunch Failure Missions** | 1 |
| 🟢 **Active Rockets** | 867 |
| 🔴 **Retired Rockets** | 398 |
| 💰 **Total Budget (Sum)** | $13.96 Trillion |

> 📌 **94.62%** of all recorded missions were successful — a testament to the precision of modern space engineering.

---

## ❓ Problem Statement

> *"To develop and demonstrate the effectiveness of Power BI as a comprehensive tool for exploratory data analysis on space exploration missions — addressing the challenges of data integration, cleansing, visualization, and predictive modelling specific to space mission datasets, ultimately enhancing decision-making processes and advancing our understanding of space exploration endeavours."*

Space mission data is inherently complex: multi-source, multi-format, and laden with high-stakes variables. Traditional spreadsheet analysis fails to surface the relationships and patterns needed for informed mission planning. This project bridges that gap with an end-to-end Power BI solution.

---

## 🎯 Project Objectives

```
┌─────────────────────────────────────────────────────────────────┐
│                     PROJECT OBJECTIVES                          │
│                                                                 │
│  1. 📥  Data Integration    →  Consolidate multi-source data    │
│  2. 🧹  Data Cleansing      →  Ensure quality and consistency   │
│  3. 📊  Visualization       →  Uncover patterns and trends      │
│  4. 🔬  Diagnostic Analysis →  Identify failure root causes     │
│  5. 🔮  Predictive Modelling→  Forecast mission parameters      │
│  6. ⚡  Streamlined EDA     →  Enable faster insight extraction  │
└─────────────────────────────────────────────────────────────────┘
```

---

## 💡 Proposed Solution

The project was executed in four structured phases:

### Phase 1 — Data Import, Pre-Processing & Modelling
- Imported raw space mission datasets into Power BI
- Performed data type corrections, null handling, and normalization
- Built a relational data model connecting missions, rockets, companies, and locations

### Phase 2 — DAX Measures & Dashboard Development
- Authored custom **DAX (Data Analysis Expressions)** measures for:
  - Mission success rates
  - Budget aggregations by location/company
  - Year-over-year mission growth
- Designed the interactive dashboard layout

### Phase 3 — Advanced Visualization & Interactivity
- Applied **filters and slicers** for dynamic data exploration
- Added cross-filtering between visuals for drill-down analysis
- Created calculated columns and measures to enrich charts

### Phase 4 — Formatting, Testing & Validation
- Validated all visual outputs against raw data
- Tested filter interactions and edge cases
- Polished formatting for presentation readiness

---

## 🛠️ Technology Used

<div align="center">

| Tool | Purpose |
|------|---------|
| ![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat&logo=powerbi&logoColor=black) **Microsoft Power BI** | Primary tool for data modelling, DAX, and visualization |
| **Power Query** | Data transformation and ETL pipeline |
| **DAX (Data Analysis Expressions)** | Custom measures and calculated columns |
| **Excel / CSV** | Source data format for space mission datasets |

</div>

---

## 📊 Dashboard Features

### 🏆 KPI Cards (Top Row)
Six summary cards provide an instant snapshot of the entire dataset:
- Total Missions, Success Count, Failure Count
- Partial Failures, Prelaunch Failures, Active/Retired rocket counts

### 📅 Total Missions by Year & Mission Status
A time-series line chart reveals the explosive growth in space missions post-2000, with a dramatic spike toward 2020 driven largely by commercial spaceflight.

### 🏢 Success Missions by Company
A horizontal bar chart ranking top performers:
- **CASC** (China Aerospace Science and Technology Corporation) — #1
- **SpaceX** — #2
- **NASA** — #3

### 🚀 Total Missions by Rocket
Orange bar chart highlighting the most-deployed rockets:
- **Falcon** series (SpaceX) — most active
- **Ariane** series — second
- **Long March** series — third

### 🌍 Budget vs. Missions by Location
A bubble scatter plot mapping launch sites by total budget spend and mission volume, revealing cost-efficiency differences across global spaceports.

### 🍩 Mission Status Distribution (Donut Chart)
Clear visual breakdown of outcomes:
- 🟣 **Success: 94.62%**
- 🔵 **Failure: 3.79%**
- 🔵 **Partial Failure: ~1.5%**
- 🟠 **Prelaunch: ~0.08%**

---

## 🔄 Data Pipeline

```
Raw Dataset (CSV/Excel)
        │
        ▼
  Power Query Editor
  ┌─────────────────────────────────┐
  │  • Remove nulls & duplicates    │
  │  • Normalize date formats       │
  │  • Parse rocket & company data  │
  │  • Categorize mission status    │
  └─────────────────────────────────┘
        │
        ▼
  Data Model (Star Schema)
  ┌───────────────┐    ┌───────────────┐
  │  Missions     │───▶│  Rockets      │
  │  (Fact Table) │    └───────────────┘
  │               │───▶┌───────────────┐
  │               │    │  Companies    │
  │               │    └───────────────┘
  │               │───▶┌───────────────┐
  └───────────────┘    │  Locations    │
                       └───────────────┘
        │
        ▼
  DAX Measures & Calculated Columns
        │
        ▼
  Interactive Power BI Dashboard
```

---

## 🔍 Insights & Findings

### 1. Mission Success Has Never Been Higher
Over 94.6% of all recorded missions were successful, with modern missions (post-2010) having even higher success rates thanks to refined engineering and commercial competition.

### 2. Commercial Space is Exploding
The timeline chart shows a dramatic inflection point around 2015–2020, driven primarily by SpaceX's reusable rocket program dramatically lowering launch costs and increasing frequency.

### 3. CASC Leads in Volume
The China Aerospace Science and Technology Corporation (CASC) leads all organizations in raw mission success count, reflecting China's aggressive and sustained space program investment.

### 4. Budget ≠ Success
The budget-vs-location scatter plot reveals that some smaller-budget launch sites achieve comparable success rates to high-spend locations, suggesting operational efficiency plays a key role.

### 5. Rocket Reliability Matters
The Falcon 9 dominates active launches, validating SpaceX's strategy of perfecting a single rocket platform rather than maintaining a large diverse fleet.

---

## 🏁 Conclusion

The application of Power BI in space exploration data analysis offers a **transformative approach** to handling complex mission datasets. Through robust capabilities in data integration, visualization, and analytical modelling, this dashboard:

- ✅ Streamlines the EDA process from raw data to insight
- ✅ Enables rapid pattern recognition across 60+ years of missions
- ✅ Provides decision-makers with a clear view of budget efficiency
- ✅ Highlights key players and technologies shaping modern space exploration
- ✅ Demonstrates the power of self-service BI in scientific domains

As space exploration accelerates in the commercial era, tools like Power BI will be increasingly essential in unlocking discoveries and ensuring the success of future missions.

---

## 🚀 Getting Started

### Prerequisites
- Microsoft Power BI Desktop (free download from [powerbi.microsoft.com](https://powerbi.microsoft.com))
- The space missions dataset (CSV format)

### Steps to Run

```
1. Download and install Power BI Desktop
2. Clone or download this repository
3. Open Power BI Desktop
4. File → Open → Select SpaceMissions.pbix
5. If prompted, update the data source path to your local CSV file
6. Click "Refresh" to reload data
7. Explore the interactive dashboard using slicers and filters
```

### Interacting with the Dashboard

| Action | How |
|--------|-----|
| Filter by Company | Click a bar in the "Success by Company" chart |
| Filter by Year Range | Use the timeline slicer |
| Filter by Status | Click a segment in the donut chart |
| Reset all filters | Click the eraser icon in the filter pane |
| Drill down | Right-click any visual → Drill down |

---

## 👤 Author

**Tejas Gaikawad**
- 🏫 Shri Sant Gajanan Maharaj College of Engineering
- 🆔 Student ID: STU64c414be227ae1690571966
- 🏢 Infosys Next Gen Employability Program

---

## 📜 Program

This project was submitted as a **Capstone Project** for the:

> 🎓 **Infosys Next Gen Employability Program**
> *Creating a Future-Ready Workforce*

---

<div align="center">

Made with 📊 Power BI & 🚀 Curiosity

⭐ Star this repo if the dashboard inspired you!

</div>
