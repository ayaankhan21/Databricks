# US Greenhouse Gas Emissions: End-to-End Data Analytics Project Using Databricks

## 📋 Project Overview
This project demonstrates a complete data analytics lifecycle within the **Databricks ** environment. It focuses on transforming raw United States greenhouse gas (GHG) emissions data into actionable insights through SQL-based engineering and interactive data visualization.


---

## 💼 Business Context
The project simulates a real-world scenario where an analyst supports environmental reporting requirements. The goal is to identify emission "hotspots" across the US and calculate normalized metrics (emissions per capita) to understand the impact of population density on environmental footprints.

---

## 🛠️ Tools & Technologies
* **Platform:** Databricks Free Edition (Community Edition)
* **Engine:** Databricks SQL
* **Data Source:** Public EPA Greenhouse Gas Emissions dataset
* **Visualization:** Databricks Dashboards
* **AI Tools:** Databricks AI Assistant for query optimization and debugging

---

## 🎯 Project Objectives
1.  **Ingestion:** Import raw EPA data from GitHub into the Databricks Lakehouse.
2.  **Transformation:** Clean and cast data types for numeric analysis.
3.  **Exploration:** Analyze emissions across states and counties.
4.  **Normalization:** Calculate emissions per person using population data.
5.  **Visualization:** Build a stakeholder-facing dashboard to show geographic patterns.

---

## ⚙️ Data Pipeline & Preparation

The raw data required significant cleaning before analysis:
* **Schema Mapping:** Created a new Databricks catalog and table for the raw CSV data.
* **Data Cleaning:** Removed thousand separators (commas) from text-based numeric fields.
* **Type Casting:** Converted `Emissions` and `Population` columns from `STRING` to `DECIMAL` and `INT`.

---

## 📊 Key SQL Analysis
The analysis provides answers to critical environmental questions:
* **State Analysis:** Total emissions summed by state to identify major contributors.
* **Top 10 Rankings:** Identification of the highest-emitting counties and states.
* **Per Capita Metrics:** `Total Emissions / Total Population` to find high-intensity areas.
* **Geographic Correlation:** Analysis of latitude/longitude to map emission centers.

---

## 📈 Dashboard & Insights
The final interactive dashboard includes a United States emissions map, scatter plots for population analysis, and bar charts for county rankings.

![dashboard databricks](https://github.com/user-attachments/assets/40e05a3b-90ef-4be1-bd37-dc9abcc110df)


### Key Insights:
* **Concentration:** A small number of states account for a large share of total US emissions.
* **Population Paradox:** High-population regions often show lower emissions per person, while some low-population industrial counties show massive
