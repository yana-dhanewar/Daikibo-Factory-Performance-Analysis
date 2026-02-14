# Daikibo-Factory-Performance-Analysis
Industrial IoT telemetry analysis and interactive dashboard created for the Deloitte Data Analytics Job Simulation
# Daikibo-Factory-Performance-Analysis
Industrial IoT telemetry analysis and interactive dashboard created for the Deloitte Data Analytics Job Simulation
# 🏭 Daikibo Operational Performance Overview
**Industrial IoT Telemetry & Equipment Health Analysis**

### 🎯 Project Objective
This project was completed as part of the **Deloitte Data Analytics Job Simulation**. The objective was to transform raw industrial telemetry data into actionable executive insights for Daikibo, a global manufacturer. I analyzed failure patterns across four international factory locations—**Tokyo, Osaka, Berlin, and Shenzhen**—to identify critical maintenance priorities.

### 📊 Dashboard Preview
<img width="1366" height="720" alt="Screenshot 2026-02-15 014812" src="https://github.com/user-attachments/assets/b80ffbab-531e-4c23-8870-ef6d1a94c87f" />


### 💾 Data Source
The dataset consists of **Industrial IoT telemetry logs** in JSON format, capturing machine status, temperature, and pressure readings from four global sites for the duration of May 2021. 
* **File Type:** `.json`
* **Source:** Deloitte Data Analytics Job Simulation via Forage.

### 🛠️ Technical Workflow (What I Did)
* **Data Ingestion:** Processed a complex JSON dataset containing a month’s worth of telemetry logs.
* **Calculated Fields & Logic:** Engineered a custom metric, `Unhealthy`, using a Tableau calculated field to quantify downtime events:
  `IF [Status] = "unhealthy" THEN 10 ELSE 0 END`
* **Data Visualization:**
    * Developed **"Downtime per Factory"** (Sheet 1) to identify geographical hotspots.
    * Developed **"Downtime per Machine"** (Sheet 2) for granular equipment analysis.
* **Interactive Dashboarding:** Created the **Daikibo Operational Performance Overview**, implementing **Filter Actions** so that factory-level selections dynamically update the machine-level failure data.

### 💡 Key Insights
* **High-Risk Location:** Identified that the **Daikibo-Seiko (Osaka)** factory reported significantly higher unhealthy telemetry signals compared to Berlin or Tokyo.
* **Bottleneck Equipment:** Successfully isolated specific **Device Types** (specifically Laser Cutters) that were consistently underperforming, allowing for targeted maintenance instead of costly site-wide shutdowns.

### 📂 Repository Structure
| File                                  | Description                                              |
| :---                                  | :---                                                     |
| `Daikibo_Factory_Analysis.twbx`       | The full Tableau Packaged Workbook.                      |
| `Factory_Telemetry_Data_May2021.json` | The raw source data used for the analysis.               |
| `Yana_Dhanewar_Daikibo_SOW.pdf`       | Professional Scope of Work (SOW) document.               |
| `README.md`                           | Project summary and technical documentation (this file). |

---
**Tools Used:** Tableau Desktop, JSON Data Parsing, Data Transformation, Statistical Trend Analysis.
