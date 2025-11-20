# Manufacturing Downtime Analysis w/ Power BI
### Digital Egypt Pioneers Initiative (DEPI) - Capstone Project

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Power Query](https://img.shields.io/badge/Power_Query-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)

## Executive Summary
This project delivers a rigorous analysis of industrial production line data to monitor and evaluate **'Downtime'**. Utilizing **Microsoft Power BI**, the project focuses on assessing operational efficiency, identifying root causes of delays, and providing actionable insights to minimize waste and boost productivity.

The analysis is based on a real-world dataset covering a **5-day production cycle**, including 61 downtime incidents across 38 batches and 4 operators.

## Objectives
* **Performance Assessment:** Identify gaps in the manufacturing line's overall performance.
* **Root Cause Analysis:** Correlate human error vs. technical machine failures to pinpoint specific training needs.
* **Product Efficiency:** Analyze time utilization per Product type and Batch.
* **Data Modeling:** Build a structured schema for scalable analysis.

## Technical Architecture

### 1. Data Preparation (ETL)
Data transformation was performed using **Power Query (M Language)**:
* **Data Cleaning:** Standardized units (e.g., converting "1 L" to "1000 ml") and corrected Operator IDs.
* **Unpivoting:** Transformed `Line Downtime` columns into a long-format structure for granular analysis.
* **Fact & Dimension Tables:** Created a star schema structure separating metrics (`fLineProductivity`) from attributes (`dProducts`, `dOperators`).

### 2. Data Modeling
The project utilizes a **Fact Constellation (Galaxy) Schema** with selective Snowflaking. This approach supports model purity and ensures accurate filtering across multiple fact tables.

### 3. UI/UX Design
* **Design System:** A Dark Industrial Theme with gold accents was chosen to reduce eye fatigue and highlight KPIs.
* **Prototyping:** Wireframes were created in **Draw.io** and high-fidelity mockups were designed in **Figma** before implementation.

## Dashboard Overview
The interactive dashboard includes the following pages:
1.  **Home Page:** Central navigation hub.
2.  **Production Overview:** High-level KPIs including Efficiency Rate, Net Run Time, and Availability.
3.  **Downtime Analysis:** Breakdown of downtime causes (Machine vs. Operator) and trends.
4.  **Operator Performance:** Benchmarking operator efficiency and error rates.
5.  **Drill-through Details:** Granular views for specific Products and Operators.

*(Optional: Add your dashboard screenshots here)*
`![Dashboard Screenshot](path/to/image.png)`

## Key Insights
* **Critical Downtime:** Total downtime reached **36%**, reducing line availability to **64%**.
* **Main Driver:** **Operator Errors** accounted for **54%** of all downtime incidents.
* **Top Machine Issue:** "Machine Adjustment" was the leading mechanical cause of delays.
* **Product Sensitivity:** "Cola 2L" and "Cola 600ml" showed the highest recurring downtime frequency.

## Recommendations
* **Operator Training:** Conduct targeted retraining for operators (specifically Mac & Dennis) on setup and calibration.
* **Preventive Maintenance:** Implement a structured PM plan for machines showing instability (Adjustment & Failure).
* **Inventory Control:** Update SOPs for batch changeovers to mitigate "Inventory Shortage" delays.

## The Team (CLS-CA13-DAT2-G5-T1)
This project was created under the supervision of **Eng. Mahmoud Seraj**.

* **Hamza Bahgat**
* **Hussien Habashy**
* **Kareem AbdelHamied**
* **Mohammed Ali**
* **Mohammed Ezzat**
* **Sohaib Atef**

---
*Developed as part of the Digital Egypt Pioneers Initiative (DEPI) - 2024/2025.*