# BrightTV Viewership Analytics
### Customer Value Management (CVM) Case Study | BrightLearn 2026

**Author:** Siyakha Ntuli  
**Date:** June 2026  
**Data Period:** January – March 2026  

---

## Overview

BrightTV is a South African subscription television broadcaster offering multiple channels to its subscriber base. The CEO commissioned this analytics case study to provide insights that would assist the Customer Value Management (CVM) team in growing the company's subscription base for the current financial year.

The dataset provided contained two raw tables — subscriber user profiles and viewership transaction records — covering January to March 2026, encompassing 10,000 viewing sessions across 4,386 unique subscribers.

---

## Business Questions

The following four questions guided the entire analysis:

1. What are the user and usage trends of BrightTV?
2. What factors influence consumption?
3. What content would you recommend to increase consumption on low consumption days?
4. What initiatives would you recommend to grow BrightTV's user base?

---

## How the Case Study Was Done

The project followed a structured 7-phase analytical approach:

**Phase 1 — Business Understanding**  
Defined the CEO's objective, identified the four business questions and documented stakeholder questions that would be asked before starting any analysis.

**Phase 2 — Data Understanding**  
Explored two raw Excel tables in Databricks. Identified 7 data quality issues including ghost profiles, duplicate columns, UTC timestamps, duration stored as timestamp format and missing demographic values.

**Phase 3 — Data Preparation**  
Built a master SQL view (`bright_tv_master`) in Databricks that joins both raw tables, applies all cleaning and transformation logic and exposes clean columns for analysis. Key transformations included UTC to SA time conversion, duration to minutes conversion, age group segmentation and demographic standardisation.

**Phase 4 — Analysis**  
Wrote 12 analytical SQL queries covering user demographics, time trends and content performance — each directly answering one of the four business questions.

**Phase 5 — Visualisation**  
Built three themed interactive dashboard pages in Databricks, with the same dashboards replicated in Power BI, Google Looker Studio and Excel for cross-tool validation.

**Phase 6 — Insights and Recommendations**  
Synthesised findings from all dashboards into evidence-based recommendations answering all four business questions.

**Phase 7 — Presentation**  
Delivered a professional Word document report and PowerPoint presentation structured for a CEO audience.

---

## Key Insights Found

### Demographics
- BrightTV has **4,386 unique subscribers** generating **10,000 viewing sessions** and **87,210 total minutes** watched across 3 months
- The subscriber base is **84.88% male** and only **11.13% female** — a 7:1 gender imbalance representing the single largest growth opportunity
- **Adults (30-59)** dominate with 5,756 subscribers, followed by Youth (3,601)
- **Gauteng** leads province viewership, with Northern Cape, Free State and North West as the lowest performing provinces
- Race distribution mirrors SA's general population demographics

### Time Trends
- Consumption grew by **192% from January to March 2026** — a strong positive trajectory
- **Peak viewing window is 17:00–18:00 SA time** consistently across all three months
- **Saturday is the strongest viewing day** every month without exception
- **Monday and Tuesday are consistently the weakest days** — attributed to the Monday blues effect
- January dominates the 10 lowest consumption days — a post-holiday slow start effect

### Content and Channels
- **ICC Cricket World Cup 2011** is the most watched channel at 24,080 minutes — but represents a critical overreliance risk on a single 15-year-old replay title
- **Female subscribers prefer:** Trace TV, SuperSport Live Events, Cartoon Network
- **Male subscribers prefer:** ICC Cricket World Cup 2011, Channel O, SuperSport Blitz
- **Mpumalanga** shows high consumption relative to subscriber count — high engagement per subscriber
- Bottom performing channels (Wimbledon, Vuzu, MK, M-Net, SawSee) require strategic scheduling intervention

---

## Recommendations Summary

1. **Female acquisition campaign** — target the 88.87% male-dominated subscriber gap
2. **Teen girl targeting** — only 14 female teenagers subscribing, massive untapped segment
3. **Family bundle** — 174 kids accounts with incomplete profiles indicate families already watching
4. **Kids content partnerships** — partner with SA children's show producers
5. **Bottom 3 province campaign** — Northern Cape, Free State, North West need regional targeting
6. **Mpumalanga growth investment** — proven high engagement, prime acquisition target
7. **Multilingual content** — Zulu, Afrikaans, Sotho, Hindi content for inclusive positioning
8. **Reduce cricket dependency** — invest in live sports rights or current content titles
9. **Invest in Trace TV** — appeals to Youth, Kids, Teenagers and Females simultaneously
10. **Lead-in/Lead-out programming** on Monday and Tuesday to lift low consumption days
11. **Premium content at 17:00–19:00** daily to maximise peak window viewership

> *"BrightTV has a loyal but narrow subscriber base — predominantly male, adult, Gauteng-based and cricket-dependent. The opportunity to double the subscriber base exists by targeting females, teenagers, kids and bottom 3 provinces with the right content, campaigns and partnerships."*

---

## Tools Used

| Tool | Purpose |
|---|---|
| **Databricks SQL** | Data ingestion, cleaning, transformation, analysis and dashboards |
| **Microsoft Excel** | Pivot tables, charts and cross-tool validation |
| **Power BI** | Interactive dashboard visualisation |
| **Google Looker Studio** | Dashboard visualisation |
| **Miro** | Project planning and process flow diagram |
| **GitHub** | Version control and portfolio management |
| **Microsoft Word** | Professional findings report |
| **PowerPoint** | CEO presentation deck |

---

## Repository Structure

```
BrightTV-Viewership-Analytics/
│
├── README.md
│
├── 01_project_description/
│   ├── BrightTV_Case_Study.pdf          # Original case study brief
│   └── BrightTV_Raw_Data.csv            # Raw dataset
│
├── 02_project_planning/
│   └── BrightTV_Miro_Flowchart.png      # Project flow diagram
│
├── 03_data_processing/
│   ├── BrightTV_Viewership_Analysis_2026.sql   # Full annotated SQL notebook
│   └── BrightTV_Excel_Analysis.xlsx            # Pivot tables and charts
│
└── 04_project_presentation/
    ├── BrightTV_Presentation.pptx               # CEO presentation deck
    ├── BrightTV_Viewership_Analytics_Report.docx # Findings report
    └── dashboards/
        ├── databricks_demographics.png
        ├── databricks_time_trends.png
        ├── databricks_content_channels.png
        ├── powerbi_demographics.png
        ├── powerbi_time_trends.png
        ├── powerbi_content_channels.png
        ├── looker_demographics.png
        ├── looker_time_trends.png
        └── looker_content_channels.png
```

---

## Skills Demonstrated

**Technical:** SQL, Data Engineering, EDA, Time Series Analysis, Content Performance Analysis, KPI Design, Dashboard Development, Excel Pivot Tables

**Tools:** Databricks, Power BI, Google Looker Studio, Excel, Miro, GitHub

**Business:** CVM Strategy, Audience Segmentation, Content Scheduling, Lead-in/Lead-out Programming, Subscriber Growth Strategy, Data Storytelling

---

*BrightLearn Data Analytics Programme | 2026*
