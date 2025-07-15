# 📊 COVID-19 Data Analysis Project

This project performs an in-depth analysis of COVID-19 data to explore the spread, severity, and economic impact across continents and countries. The project integrates data cleaning, exploratory data analysis (EDA), statistical summaries, feature engineering, visualization, and predictive modeling using Python.

---

## 📁 Dataset

- **Source:** [COVID-19 Dataset](https://raw.githubusercontent.com/SR1608/Datasets/main/covid-data.csv)
- **Description:** Contains global COVID-19 data including:
  - Location and continent
  - Date-wise cases and deaths
  - Economic indicators (GDP per capita, Human Development Index)

---

## 🎯 Objectives

- Analyze COVID-19 spread and mortality across continents.
- Explore correlations between socio-economic factors and COVID-19 metrics.
- Engineer new features to enhance understanding.
- Build a regression model to predict deaths.
- Visualize key trends and relationships.

---

## 🛠️ Project Workflow

### 1️⃣ Data Loading
- Imported the dataset using Pandas.

### 2️⃣ Data Cleaning
- Removed duplicates.
- Handled missing values.
- Converted date columns to datetime format.
- Selected relevant columns.
- Extracted month from date.

### 3️⃣ Exploratory Data Analysis
- High-level summaries (mean, median, variance, skewness).
- Quartile and correlation analysis.
- Unique counts and continent-level aggregations.

### 4️⃣ Feature Engineering
- Created:
  - `total_deaths_to_total_cases` ratio.
  - `case_growth_rate`.
  - Monthly extraction for time series analysis.

### 5️⃣ Predictive Modeling
- Trained a Linear Regression model to predict `total_deaths` based on:
  - `total_cases`
  - `gdp_per_capita`
  - `human_development_index`
- Evaluated model performance using RMSE.

### 6️⃣ Visualizations
- Histograms of GDP per capita.
- Scatter plots (Cases vs GDP).
- Pairplots.
- Correlation heatmaps.
- Boxplots of deaths by continent.
- Bar charts of total cases.

---

## 📈 Key Findings

- Significant variation in total cases and deaths across continents.
- Positive correlation between total cases and total deaths.
- Higher GDP per capita and HDI are generally associated with lower case fatality ratios.
- Predictive modeling demonstrates that cases and economic indicators can reasonably estimate total deaths.

---

## 🗂️ Files

- **`covid_analysis.ipynb`** — Jupyter Notebook with full code.
- **`df_groupby.csv`** — Aggregated dataset saved for reference.
- **`README.md`** — Project documentation.
- **`presentation.pptx`** — Optional presentation slides summarizing findings.

---

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/covid19-data-analysis.git
   cd covid19-data-analysis

