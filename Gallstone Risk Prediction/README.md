
# Gallstone Risk Prediction | Use Case 2

## 🧠 Overview

A data science project to assess and predict gallstone risk using clinical features such as visceral fat, body fat percentage, BMI, gender, age, and weight. Built in a Databricks notebook, the analysis combines statistical testing, visualizations, and SQL modeling to derive actionable health insights.

### 👩‍💼 Business Context

* Identify key predictors influencing gallstone formation
* Deliver clinical and strategic recommendations for targeted screening programs
* Support health teams with interpretable risk scores and visual storytelling


### 1. Data Loading & Exploration

* Loaded data from `personal_catalog.gallstone_risk_prediction.gallstone_data` in Databricks
* Inspected schema, row counts, and class distribution (gallstone positive vs negative)

### 2. Exploratory & Statistical Analysis

* Calculated summary statistics on numeric variables
* Visualized mean differences between patient groups for BMI, age, TBFR, VFR, weight
* Conducted hypothesis testing (two‑sample t‑tests and chi‑square tests) to assess significance

  ✅ Approach leveraged: **Problem‑solving mindset**, **logical reasoning**, and **statistical rigor**.

### 3. Visualization & Interpretation

* Created bar charts and annotated results with p‑values
* Added clinical thresholds (e.g. BMI = 25; VFR = 10), mean differences, and labels
* Used heatmaps to illustrate correlation strengths between features and gallstone status

  🎯 Focused on **choosing the right visual or metric** to communicate findings effectively.

### 4. Statistical Findings

* **Strongest predictors**: VFR and TBFR (correlation ≈ 0.24 each, statistically significant)
* **Moderate**: BMI (≈ 0.18)
* **Low impact**: age and weight (≈ 0.04 correlation)
* **Gender significant**: higher gallstone prevalence in women (chi‑square p < 0.05)

  Provided insights bridging data patterns and clinical relevance.

### 5. SQL-Based Risk Modeling

* Computed feature means by group and base risk in SQL
* Derived normalized coefficients from group differences
* Built a logistic‑style risk score to calculate a predicted gallstone probability
* Classified patients into **High (🔴), Medium (🟡),** or **Low (🟢)** risk based on probability thresholds (>70%, 30–70%, <30%)

  This demonstrates **accuracy in handling data**, and **deep understanding of both statistical modeling and business context**.

---

## 🧩 Core Skills Demonstrated

* **Problem‑solving mindset**: Tackled missing data, adapted to Databricks’ environment, and structured analyses around clinical hypotheses
* **Critical thinking & logical reasoning**: Framed clear hypotheses (e.g. BMI increases risk), tested statistically, and interpreted results correctly
* **Data manipulation & cleaning precision**: Handled null values, removed outliers, and standardized variable names for clarity
* **Accuracy in data handling**: Ensured consistent numeric encoding, correct group aggregation, and reproducible SQL logic
* **Understanding business context**: Translated statistical findings into actionable health‑screening strategies and interventions
* **Choosing the right visual or metric**: Used bar charts, heatmaps, and annotated visuals to tell the data story effectively

---

## 📊 Key Insights & Strategic Recommendations

| Risk Factor             | Findings             | Recommendation                        |
| ----------------------- | -------------------- | ------------------------------------- |
| **Visceral Fat & TBFR** | Strongest predictors | Prioritize abdominal fat screenings   |
| **BMI**                 | Moderate association | Include in risk score, monitor trends |
| **Weight & Age**        | Low impact           | Focus resources elsewhere             |
| **Gender**              | Women at higher risk | Consider gender-adjusted thresholds   |

* **High Risk (🔴 >70%)** → Immediate ultrasound & clinical review
* **Medium Risk (🟡 30–70%)** → Diet counseling & 6‑month follow-up
* **Low Risk (🟢 <30%)** → General wellness advice annually


## 📌 Summary

This project combines **statistical analysis**, **clean data pipelines**, **clear visual communication**, and **business-savvy risk modeling** to evaluate and classify gallstone risk among patients. Foundation is built on hypothesis testing and real-world context, offering interpretable insights and practical recommendations.

