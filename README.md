# Manufacturing Downtime Analysis w/ Power BI
# Manufacturing Downtime Analysis
### Digital Egypt Pioneers Initiative (DEPI) - Capstone Project

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Power Query](https://img.shields.io/badge/Power_Query-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)

## Executive Summary
This project delivers a rigorous analysis of industrial production line data to monitor and evaluate **'Downtime'**. [cite_start]Utilizing **Microsoft Power BI**, the project focuses on assessing operational efficiency, identifying root causes of delays, and providing actionable insights to minimize waste and boost productivity[cite: 75, 76].

[cite_start]The analysis is based on a real-world dataset covering a **5-day production cycle**, including 61 downtime incidents across 38 batches and 4 operators[cite: 87, 89, 90, 91].

## Objectives
* [cite_start]**Performance Assessment:** Identify gaps in the manufacturing line's overall performance[cite: 81].
* [cite_start]**Root Cause Analysis:** Correlate human error vs. technical machine failures to pinpoint specific training needs[cite: 82].
* [cite_start]**Product Efficiency:** Analyze time utilization per Product type and Batch[cite: 83].
* [cite_start]**Data Modeling:** Build a structured schema for scalable analysis[cite: 84].

## Technical Architecture

### 1. Data Preparation (ETL)
[cite_start]Data transformation was performed using **Power Query (M Language)**[cite: 104]:
* [cite_start]**Data Cleaning:** Standardized units (e.g., converting "1 L" to "1000 ml") and corrected Operator IDs[cite: 145, 171].
* [cite_start]**Unpivoting:** Transformed `Line Downtime` columns into a long-format structure for granular analysis[cite: 132].
* [cite_start]**Fact & Dimension Tables:** Created a star schema structure separating metrics (`fLineProductivity`) from attributes (`dProducts`, `dOperators`)[cite: 197, 201].

### 2. Data Modeling
The project utilizes a **Fact Constellation (Galaxy) Schema** with selective Snowflaking. [cite_start]This approach supports model purity and ensures accurate filtering across multiple fact tables[cite: 194, 196].

### 3. UI/UX Design
* [cite_start]**Design System:** A Dark Industrial Theme with gold accents was chosen to reduce eye fatigue and highlight KPIs[cite: 260, 266].
* [cite_start]**Prototyping:** Wireframes were created in **Draw.io** and high-fidelity mockups were designed in **Figma** before implementation[cite: 215, 217].

## Dashboard Overview
[cite_start]The interactive dashboard includes the following pages[cite: 71]:
1.  [cite_start]**Home Page:** Central navigation hub[cite: 218].
2.  [cite_start]**Production Overview:** High-level KPIs including Efficiency Rate, Net Run Time, and Availability[cite: 219].
3.  [cite_start]**Downtime Analysis:** Breakdown of downtime causes (Machine vs. Operator) and trends[cite: 279, 280].
4.  [cite_start]**Operator Performance:** Benchmarking operator efficiency and error rates[cite: 285].
5.  [cite_start]**Drill-through Details:** Granular views for specific Products and Operators[cite: 282, 288].

*(Optional: Add your dashboard screenshots here)*
`![Dashboard Screenshot](path/to/image.png)`

## Key Insights
* [cite_start]**Critical Downtime:** Total downtime reached **36%**, reducing line availability to **64%**[cite: 293].
* [cite_start]**Main Driver:** **Operator Errors** accounted for **54%** of all downtime incidents[cite: 294].
* [cite_start]**Top Machine Issue:** "Machine Adjustment" was the leading mechanical cause of delays[cite: 296].
* [cite_start]**Product Sensitivity:** "Cola 2L" and "Cola 600ml" showed the highest recurring downtime frequency[cite: 297].

## Recommendations
* [cite_start]**Operator Training:** Conduct targeted retraining for operators (specifically Mac & Dennis) on setup and calibration[cite: 311].
* [cite_start]**Preventive Maintenance:** Implement a structured PM plan for machines showing instability (Adjustment & Failure)[cite: 314].
* [cite_start]**Inventory Control:** Update SOPs for batch changeovers to mitigate "Inventory Shortage" delays[cite: 308, 320].

## The Team (CLS-CA13-DAT2-G5-T1)
This project was created under the supervision of **Eng. [cite_start]Mahmoud Seraj**[cite: 8, 18].

* **Hamza Bahgat**
* **Hussien Habashy**
* **Kareem AbdelHamied**
* **Mohammed Ali**
* **Mohammed Ezzat**
* **Sohaib Atef**

---
[cite_start]*Developed as part of the Digital Egypt Pioneers Initiative (DEPI) - 2024/2025[cite: 19].*