# Manufacturing Downtime Analysis w/ Power BI
### Digital Egypt Pioneers Initiative (DEPI) - Capstone Project

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Power Query](https://img.shields.io/badge/Power_Query-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)

## Project Overview
This project conducts a rigorous analysis of industrial production line data to monitor and evaluate **'Downtime'**. Utilizing **Power BI**, the project focuses on assessing operational efficiency, identifying root causes of delays, and providing actionable insights to minimize waste and boost productivity.

This analysis is based on a real-world dataset covering a **5-day production cycle** for a single manufacturing line.

## Objectives
* [cite_start]**Performance Assessment:** Identify gaps in the manufacturing line's overall performance[cite: 81].
* [cite_start]**Root Cause Analysis:** Correlate human error vs. technical machine failures to pinpoint training needs[cite: 82].
* [cite_start]**Product Efficiency:** Analyze time utilization per product type and batch[cite: 83].
* [cite_start]**Data Modeling:** Build a scalable schema for repeatable analysis[cite: 84].

## Data Scope
The analytical sample includes:
* [cite_start]**1** Production Line[cite: 88].
* [cite_start]**6** Different Products[cite: 89].
* [cite_start]**38** Distinct Batches[cite: 89].
* [cite_start]**4** Operators[cite: 90].
* [cite_start]**61** Recorded Downtime Incidents[cite: 91].

## Tools & Methodology

### 1. Data Preparation (Power Query)
Data cleaning and transformation were performed using **M Language** in Power Query:
* [cite_start]**Unpivoting Data:** Transformed `Line Downtime` into a long format for better granularity[cite: 132].
* [cite_start]**Standardization:** Cleaned Product names (e.g., converting "1 L" to "1000 ml") and Operator IDs[cite: 145, 171].
* [cite_start]**Fact & Dimension Tables:** Separated data into Facts (`fLineProductivity`, `fLineDowntime`) and Dimensions (`dProducts`, `dOperators`, `dDowntimeFactors`)[cite: 197, 201].

### 2. Data Modeling
[cite_start]The model follows a **Fact Constellation (Galaxy) Schema** with selective Snowflaking to ensure model purity and accurate filtering[cite: 194].

*(You can add a screenshot of your Model View here)*
`![Data Model Screenshot](path/to/your/image.png)`

### 3. UI/UX Design
* [cite_start]**Theme:** Dark Industrial Theme with Gold Accents for high contrast[cite: 260].
* [cite_start]**Tools:** Wireframes designed in **Draw.io** and high-fidelity mockups in **Figma**[cite: 217].

## Dashboard Features
The interactive dashboard consists of:
1.  **Home Page:** Navigation hub.
2.  [cite_start]**Production Overview:** High-level KPIs (Efficiency Rate, Net Run Time, Total Downtime)[cite: 275].
3.  [cite_start]**Downtime Analysis:** Deep dive into machine failures vs. operator errors[cite: 280].
4.  [cite_start]**Operator Performance:** Benchmarking operator efficiency and error rates[cite: 286].
5.  [cite_start]**Drill-through Pages:** Detailed views for specific Products and Operators[cite: 282].

*(Add a GIF or Screenshot of your Dashboard here)*
`![Dashboard Overview](path/to/your/dashboard_image.png)`

## Key Insights
* [cite_start]**High Downtime:** Total downtime reached **36%**, reducing line availability to **64%**[cite: 293].
* [cite_start]**Primary Cause:** **Operator Errors** accounted for **54%** of downtime incidents[cite: 294].
* [cite_start]**Machine Issues:** "Machine Adjustment" was the leading mechanical cause of delays[cite: 296].
* [cite_start]**Product Sensitivity:** "Cola 2L" and "Cola 600ml" faced the most recurring downtime[cite: 297].

## Recommendations
* [cite_start]**Targeted Training:** Retraining required for specific operators (e.g., Mac & Dennis) on setup and calibration[cite: 311].
* [cite_start]**Preventive Maintenance:** Implement a structured PM plan for machines showing instability[cite: 314].
* [cite_start]**SOPs:** Update Standard Operating Procedures for batch changeovers to reduce "Inventory Shortage" delays[cite: 320].

## The Team
This project was created by **CLS-CA13-DAT2-G5-T1** under the supervision of **Eng. [cite_start]Mahmoud Seraj**[cite: 6, 8].

* **Hamza Bahgat**
* **Hussien Habashy**
* **Kareem AbdelHamied**
* **Mohammed Ali**
* **Mohammed Ezzat**
* **Sohaib Atef**

---
*Created as part of the Digital Egypt Pioneers Initiative (DEPI) - 2024/2025.*