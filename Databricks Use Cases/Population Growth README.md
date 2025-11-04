
# 📊 Afghanistan Population Growth Analysis (2000–2016)

This Databricks notebook investigates **Afghanistan’s population growth and density surge** between 2000 and 2016 using data from the World Bank. It compares Afghanistan’s growth against the global average and explores the implications of rapid urbanization.

## 🔍 Key Questions
- How fast did Afghanistan’s population grow from 2000 to 2016?
- How does this growth compare to the global average?
- What are the implications for population density and urban planning?

## 🧠 Key Insights
- **Afghanistan's population grew significantly faster** than the global average (confirmed with a statistical test).
- **Population density increased sharply**, suggesting growing pressure on land and resources.
- Urbanization trends indicate potential **stress on housing, transport, and water infrastructure**.

## 🧪 Methodology
- Cleaned and transformed World Bank population data using PySpark and pandas.
- Computed growth rates and densities across all countries.
- Performed a **one-sample t-test** to assess whether Afghanistan’s growth was statistically higher than the global mean.
- Presented findings using Databricks visualizations and Markdown storytelling.


## 🛠️ Tools & Technologies
- **Databricks** (Spark + Notebooks)
- **PySpark & pandas** for data wrangling
- **matplotlib** for optional density charts
- **scipy.stats** for hypothesis testing

## 💡 Next Steps
- Forecast future population and density trends with time series models.
- Integrate land-use and migration data to simulate urban stress.
- Extend analysis to neighboring countries for regional planning insights.


> 🧠 “Urban growth isn’t just about numbers — it’s about planning for people.”  
>
> This project was built to demonstrate real-world data analysis using Databricks, and how we can extract actionable insights from global development data.
