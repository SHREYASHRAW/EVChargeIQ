# EVChargeIQ — EV Charging Business Analytics

> **Data-driven analysis of public EV charging demand, station performance, charging economics, and infrastructure utilization using real-world city-scale charging data.**

---

## 📌 Project Overview

**EVChargeIQ** is a data analytics project focused on understanding how public electric vehicle charging infrastructure is being used at city scale.

The project analyzes real-world public EV charging transaction and station infrastructure data from **Beijing, China**, covering **January and July 2025**.

The goal is to transform raw charging data into actionable business insights that can support decisions related to:

* Charging demand
* Station performance
* Infrastructure utilization
* Charging economics
* Spatial demand patterns
* Seasonal differences
* Demand forecasting
* Infrastructure planning and optimization

---

## 🎯 Business Problem

As electric vehicle adoption increases, charging companies need to understand whether existing infrastructure is being used efficiently and where operational improvements may be more valuable than simply adding new charging capacity.

EVChargeIQ aims to answer:

> **When, where, and under what conditions is public EV charging infrastructure most heavily utilized, and what business decisions can be supported by these patterns?**

The analysis will investigate charging demand, station characteristics, utilization, charging costs, and spatial patterns to identify opportunities for better infrastructure planning and operational efficiency.

---

## 📊 Dataset

The primary dataset is the **city-scale public electric vehicle charging transactions and infrastructure dataset** released by Wang et al. in *Scientific Data* in 2026.

The dataset contains:

* **8.544 million charging transactions**
* Approximately **8,553 public charging stations**
* Transaction-level charging records
* Station-level infrastructure attributes
* January 2025 transaction data
* July 2025 transaction data
* An anonymized `station_id` for linking transaction and station tables
* Charging energy and duration information
* Electricity and service fee information
* Charging equipment information
* Station infrastructure information
* Anonymized spatial grid information

### Important Dataset Limitation

The dataset contains observations from **January and July 2025 only**.

Therefore, this project will **not interpret the data as a complete annual time series** or claim full-year seasonal trends.

Instead, January and July will be treated as two observed periods for comparative analysis.

### Source

Wang, Q., Liu, S., Su, Z. et al. *A city-scale dataset of public electric vehicle charging transactions and infrastructure.* Scientific Data, 2026.

Dataset DOI: `10.6084/m9.figshare.31952289`

---

## 🔍 Key Business Questions

### 1. Charging Demand

* When does charging demand peak?
* How does charging activity vary throughout the day?
* How does charging behavior differ between January and July?

### 2. Station Performance

* Which stations handle the highest charging activity?
* Which station characteristics are associated with higher utilization?
* Which stations appear underutilized?

### 3. Infrastructure Utilization

* How efficiently are charging connectors being used?
* How does utilization vary by station characteristics?
* Are some areas potentially over-supplied relative to observed demand?

### 4. Charging Economics

* How much revenue is generated from charging activity?
* What proportion of charging cost comes from electricity versus service fees?
* How does charging price relate to energy consumed per session?

### 5. Spatial Analysis

* Which spatial areas have greater charging activity?
* How does charging demand relate to infrastructure density?
* Where are potential infrastructure optimization opportunities?

### 6. Predictive Analytics

* Can charging demand patterns be predicted?
* Which factors are associated with higher charging demand?
* Can analytical results support infrastructure planning decisions?

---

## 🛠️ Technology Stack

| Category              | Tools                  |
| --------------------- | ---------------------- |
| Programming           | Python                 |
| Data Manipulation     | Pandas, NumPy          |
| Data Visualization    | Matplotlib             |
| Database Analysis     | SQL                    |
| Business Intelligence | Power BI               |
| Machine Learning      | Scikit-learn           |
| Notebook Environment  | Jupyter / Google Colab |
| Version Control       | Git & GitHub           |
| Data Format           | Parquet                |

---

## 🏗️ Project Structure

```text
EVChargeIQ/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   ├── 01_data_audit.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_eda_and_kpis.ipynb
│   ├── 04_station_analysis.ipynb
│   └── 05_demand_analysis.ipynb
│
├── sql/
│   ├── 01_business_queries.sql
│   ├── 02_station_performance.sql
│   └── 03_demand_analysis.sql
│
├── dashboard/
│   └── EVChargeIQ.pbix
│
├── reports/
│   └── EVChargeIQ_Report.pdf
│
├── src/
│
├── README.md
└── .gitignore
```

---

## 📈 Planned Analysis

The project will follow this analytical workflow:

```text
Raw EV Charging Data
        ↓
Data Audit
        ↓
Data Cleaning & Validation
        ↓
Feature Engineering
        ↓
Exploratory Data Analysis
        ↓
KPI Development
        ↓
SQL Business Analysis
        ↓
Station & Spatial Analysis
        ↓
Charging Economics
        ↓
Demand Analysis
        ↓
Predictive Analytics
        ↓
Power BI Dashboard
        ↓
Business Recommendations
```

---

## 🤖 Predictive Analytics

A predictive component will be developed after the exploratory analysis.

The exact modeling approach will be determined based on the characteristics of the available data rather than assuming a model in advance.

Potential areas include:

* Charging demand prediction
* Station utilization prediction
* Demand pattern classification
* Infrastructure optimization analysis

---

## 📊 Planned Power BI Dashboard

The final dashboard is expected to include:

### Executive Overview

* Total charging sessions
* Total energy consumed
* Total charging fees
* Average session duration
* Station count
* Infrastructure KPIs

### Station Performance

* Station rankings
* Charging activity
* Energy consumption
* Infrastructure characteristics
* Utilization indicators

### Demand Analytics

* Hourly charging patterns
* Daily patterns
* January vs July comparison
* Peak demand periods

### Spatial & Infrastructure Analysis

* Charging activity by spatial grid
* Station density
* Infrastructure distribution
* Potential optimization areas

---

## 💡 Expected Business Outcomes

The final project will aim to provide evidence-based recommendations around:

* Improving station utilization
* Understanding peak charging demand
* Identifying operational inefficiencies
* Evaluating charging economics
* Supporting infrastructure planning
* Identifying areas where optimization may be preferable to capacity expansion

Recommendations will be based on the analysis rather than predefined assumptions.

---

## ⚠️ Data & Privacy

The released dataset uses anonymized station identifiers and spatial information.

The project will not attempt to identify individual users, original station names, operators, or precise locations.

No customer-level identities will be fabricated or inferred where the dataset does not provide them.

---

## 📚 Reference

Wang, Q., Liu, S., Su, Z. et al.
**A city-scale dataset of public electric vehicle charging transactions and infrastructure.**
*Scientific Data*, 2026.

Dataset DOI: `10.6084/m9.figshare.31952289`

---

## 🚧 Project Status

**Current Stage:** Project Setup & Dataset Audit

### Progress

* [x] GitHub repository initialized
* [x] Project structure created
* [x] Dataset selected
* [x] Dataset source documented
* [ ] Dataset audit
* [ ] Data cleaning
* [ ] Exploratory analysis
* [ ] SQL analysis
* [ ] Station performance analysis
* [ ] Spatial analysis
* [ ] Predictive analytics
* [ ] Power BI dashboard
* [ ] Final report
* [ ] Business recommendations
