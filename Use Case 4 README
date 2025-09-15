# Use Case 4: Climate Change CO2 Emissions Analysis

## Overview
This project explores global factors influencing per-capita CO2 emissions using climate and environmental data. The goal is to demonstrate **data science rigor**, including hypothesis testing, feature engineering, regression modeling, and business-oriented insights.

---

## Dataset
- **Source:** Global climate dataset (1,000 country-year observations)
- **Key Features:**
  - Year, Country
  - Avg Temperature (°C)
  - CO2 Emissions (Tons per Capita)
  - Sea Level Rise (mm)
  - Rainfall (mm)
  - Population
  - Renewable Energy (%)
  - Extreme Weather Events
  - Forest Area (%)

---

## Workflow

### 1. Data Loading & Cleaning
- Loaded dataset from Delta table `climate_change_dataset`.
- Standardized column names, handled missing values, ensured correct data types, and removed duplicates.

### 2. Exploratory Data Analysis (EDA)
- Visualized distributions for Population, CO2 Emissions, Renewable Energy %, and Avg Temperature.
- Scatter plots and boxplots:
  - CO2 vs Renewable Energy adoption
  - CO2 emissions for high vs low renewable countries
- Identified skewed Population distribution → candidate for log transformation.

### 3. Hypothesis Testing
- **Question:** Do countries with high renewable energy adoption have lower CO2 emissions per capita?
- **Levene’s Test:** Variances are equal (p = 0.8412)
- **Independent Samples t-test:** No significant difference (t = 1.6211, p = 0.1053)
- **Conclusion:** Renewable energy alone does not significantly explain CO2 differences, aligning with visual trends from EDA.

### 4. Regression Analysis
- **Single-factor regression:** CO2 ~ Renewable_Energy_Pct
- **Multi-factor regression:** CO2 ~ Renewable_Energy_Pct + Population + Forest Area + Extreme Weather + Avg Temperature
- **Initial findings:** Low R², numeric instability due to highly skewed Population.

### 5. Feature Engineering
- Log-transformed Population to reduce skew and stabilize computations.
- Created interaction term: Renewable_Energy_Pct × Avg_Temperature_C.
- Verified no strong multicollinearity using correlation matrix.
- Refined regression model with engineered features:
  - Slight improvement in numeric stability
  - Predictors remain statistically insignificant

### 6. Insights & Business Implications
- CO2 emissions per capita are influenced by more complex factors (e.g., industrial activity, transportation, economic structure) not captured here.
- Emphasis on statistical rigor:
  - Diagnosing model issues
  - Iteratively improving features
  - Transparent communication of results
- Recommendation: enrich dataset with additional predictors to derive actionable business insights.

---

## Visualizations
1. Scatter plot: CO2 Emissions vs Renewable Energy %
2. Correlation matrix of predictors
3. Log-transformed Population distribution
4. Final refined regression model results

---

## Key Takeaways
- **Failed experiments can be highly instructive** when analyzed rigorously.
- Statistical testing and feature engineering are critical tools to **turn unexpected results into meaningful insights**.
- Communicating limitations and methodology clearly is essential for business impact.

---

## Technologies & Libraries
- Python (pandas, numpy, statsmodels, matplotlib, seaborn)
- PySpark & Databricks
- Delta Tables for clean data storage
