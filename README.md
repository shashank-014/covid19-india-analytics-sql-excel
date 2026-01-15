# 🦠 Pandemic Patterns: COVID-19 Analytics for India  
### SQL + Excel Data Analytics Project

## 📌 Project Overview
This project analyzes India’s COVID-19 pandemic using **SQL-based ETL** and **Excel-driven analytics and dashboards**.  
The objective was to transform large, fragmented public health datasets into **structured insights** covering case trends, testing efficiency, vaccination progress, recovery outcomes, and risk classification across Indian states.

The project combines **backend data processing (SQL)** with **front-end analytics and visualization (Excel dashboards)** to demonstrate end-to-end analytical thinking.

---

## 🛠 Tools & Technologies
- **SQL (PostgreSQL)** – Data cleaning, joins, feature engineering
- **Microsoft Excel**
  - PivotTables & PivotCharts
  - Advanced formulas (INDEX, MATCH, MAXIFS)
  - Conditional formatting
  - Time-series forecasting (ETS)
  - Interactive dashboards with slicers

---

## 📂 Datasets Used
- `covid_19_india.csv` – Daily state-level COVID-19 case data  
- `covid_vaccine_statewise.csv` – Vaccination progress by state and age group  
- `StatewiseTestingDetails.csv` – State-level COVID-19 testing data  

All datasets were kept **raw and unaltered** during ingestion to preserve data integrity.

---

## 🧪 Part 1: ETL & Feature Engineering (SQL)
The ETL pipeline was implemented using SQL in a **PostgreSQL / Google Colab** environment.

### Key ETL Steps
- Standardized dates and normalized state names
- Integrated case, testing, and vaccination datasets
- Engineered analytical metrics:
  - Daily new cases using `LAG()`
  - Case Fatality Rate (CFR)
  - Test positivity rate
  - Vaccination rate
  - Active cases
  - Risk classification (High / Medium / Low)
- Created a consolidated `covid_summary` table
- Exported final dataset to Excel for analysis

🔗 **SQL Notebook**  
https://colab.research.google.com/drive/10dnmxWzPtzsyP3MnQobY_ZxTNbWrFpVl

---

## 📊 Part 2: Excel Data Analysis
The cleaned dataset was analyzed in Excel to extract trends and insights.

### Key Analyses Performed
- State-wise and national case trends
- Daily and monthly COVID-19 case progression
- Testing volume vs positivity rate analysis
- Vaccination coverage and age-group analysis
- Recovery rate vs vaccination rate comparison
- Risk assessment using CFR and active cases
- Hotspot detection using conditional formatting
- Time-series forecasting using **FORECAST.ETS**

All missing or zero values were handled **contextually**, not imputed, to avoid analytical distortion.

---

## 📈 Part 3: Interactive Excel Dashboard
An interactive dashboard was built to present insights in a single view.

### Dashboard Features
- KPI summary (cases, recoveries, deaths, tests, vaccinations)
- State-wise comparisons
- Trend analysis over time
- Risk classification (High / Medium / Low)
- Forecasted case trends
- Slicers for state and date filtering

📸 Dashboard screenshots are available in the `/screenshots` folder.

---

## 🔍 Key Insights
- COVID-19 impact varied significantly across Indian states
- Higher testing volumes correlated with higher detected cases
- Vaccination rollout contributed to reduced severity and risk levels
- Recovery rates remained consistently high across states
- Operational anomalies were episodic rather than systemic
- Forecasting highlights increasing uncertainty over time

---

## 🧠 Learnings
- Importance of **ETL and data modeling before visualization**
- Handling real-world dirty data without over-cleaning
- Using Excel as a serious analytical tool beyond basic reporting
- Communicating uncertainty clearly in forecasts
- Translating analysis into business and policy insights

---

## 📁 Repository Structure
