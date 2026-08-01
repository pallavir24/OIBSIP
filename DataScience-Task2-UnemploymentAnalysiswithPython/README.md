# Task 2: Unemployment Analysis with Python 📈

## 📌 Overview
This project performs an **Exploratory Data Analysis (EDA)** on India's unemployment dataset using Python. The objective is to uncover regional and temporal trends in unemployment across various Indian states, with a specific focus on evaluating the sharp impact of the **COVID-19 pandemic** on key labor market metrics:
* **Unemployment Rate (%)**
* **Estimated Employed**
* **Estimated Labour Participation Rate (%)**

---

## 🛠️ Tech Stack & Libraries
* **Language:** Python
* **Environment:** Jupyter Notebook
* **Data Processing:** `pandas`, `numpy`
* **Data Visualization:** `matplotlib`, `seaborn`

---

## 📊 Dataset Information
* **Source:** Kaggle — *Unemployment in India* dataset
* **Attributes Covered:**
  * `States`: Regions/States in India
  * `Date`: Observation date
  * `Frequency`: Monthly / Quarterly records
  * `Estimated Unemployment Rate (%)`: Percentage of unemployed workforce
  * `Estimated Employed`: Total count of employed individuals
  * `Estimated Labour Participation Rate (%)`: Percentage of total population in the labor force

---

## 📋 Task Checklist & Features

- [x] **Data Loading & Inspection:** Shape inspection, missing value verification, column renaming, and datetime type conversion.
- [x] **Exploratory Data Analysis (EDA):** Region-wise average unemployment calculation and month-over-month trend extraction.
- [x] **Time-Series Line Chart:** Comparative analysis of unemployment rates over time across major Indian states.
- [x] **Bar Chart Visualization:** Identification and ranking of the **Top 10 states** with the highest average unemployment rate.
- [x] **Correlation Analysis (Heatmap):** Analysis of inter-relationships between Unemployment Rate, Employed Population, and Labour Participation Rate.
- [x] **Pre-COVID vs. Post-COVID Impact Analysis:** Splitting data by key time periods to calculate and contrast mean indicator values before and after lockdown implementation.
- [x] **Insights & Documentation:** Markdown commentary explaining findings between each visualization.

---

## 🔍 Key Insights & Observations

1. **Impact of COVID-19:** 
   * A severe surge in unemployment rates occurred starting around April–May 2020 due to nationwide lockdowns.
2. **Regional Disparities:** 
   * Certain states consistently experienced significantly higher baseline unemployment rates compared to the national average.
3. **Labour Participation Correlation:** 
   * A drop in employment numbers during lockdown periods directly correlated with sharp shifts in the overall labor participation rate across major regions.
4. **Labor Force Shrinkage:** 
   * Beyond rising unemployment rates, a significant drop in the overall Labour Participation Rate during peak disruption periods indicates that many individuals temporarily stopped actively seeking employment altogether, understating the total economic strain.

---


