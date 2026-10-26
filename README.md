# COVID-19 Global Impact Analysis

## 📌 Project Overview

The **COVID-19 Global Impact Analysis** project explores the global impact of the COVID-19 pandemic using data analysis and visualization. The project focuses on reported COVID-19 cases, deaths, trends over time, and vaccination indicators across countries.

The goal is to clean the dataset, perform exploratory data analysis, calculate useful metrics, and prepare an interactive dashboard using Power BI.

## 🎯 Objectives

- Clean and prepare the COVID-19 dataset for analysis.
- Identify missing values, empty columns, and duplicate records.
- Analyze reported COVID-19 cases and deaths over time.
- Calculate a 7-day rolling average of new cases.
- Calculate the case fatality rate (CFR).
- Estimate doubling time when the available data supports the calculation.
- Compare reported cases per million people across countries.
- Explore vaccination coverage where data is available.
- Present insights through visualizations and a Power BI dashboard.

## 🛠️ Tools and Technologies

- **Microsoft Excel** — Dataset preparation and inspection.
- **Python** — Data cleaning, analysis, and visualization.
- **Pandas** — Data manipulation and analysis.
- **NumPy** — Numerical calculations.
- **Matplotlib** — Data visualization.
- **Google Colab / Jupyter Notebook** — Running Python analysis.
- **Power BI** — Interactive dashboard development.

## 📂 Project Structure

```text
COVID-19-Global-Impact-Analysis/
│
├── README.md
├── Covid-19 data.xlsx
├── COVID19_Cleaned_Data.xlsx
├── COVID19_Global_impact_analysis_with_insights.ipynb
└── PowerBI_Dashboard/
```

*Note: Include only the files and folders that are actually present in your GitHub repository. Add your Power BI `.pbix` file to the folder if you have created and saved the dashboard.*

## 📊 Dataset Overview

The initial dataset inspection reported:

| Description | Result |
|---|---:|
| Original rows | 28,240 |
| Original columns | 61 |
| Missing cells | 961,867 |
| Completely empty columns removed | 7 |
| Duplicate rows detected | 0 |
| Duplicate country-date records detected | 0 |

The dataset includes country-level time-series information related to COVID-19 cases, deaths, testing, vaccination, and other indicators.

## 🧹 Data Cleaning

The following cleaning steps were performed using Python:

1. Loaded and inspected the dataset.
2. Checked the dataset dimensions and data types.
3. Identified missing values and duplicate records.
4. Removed columns that were completely empty.
5. Filled missing continent labels only when a known continent was available for the same country.
6. Sorted records by country and date.
7. Retained other missing values instead of automatically replacing them with zero.

These steps helped prepare the data for further analysis while preserving the available reported information.

## 📈 Analysis and Visualizations

The project includes the following analyses:

### 1. Daily COVID-19 Cases
Examines changes in daily reported cases over time.

### 2. Seven-Day Rolling Average
Smooths daily fluctuations to make broader case trends easier to observe.

### 3. Total Reported Deaths
Explores cumulative reported deaths over time.

### 4. Cases per Million People
Supports comparisons between countries while accounting for differences in population size.

### 5. Vaccination Coverage
Explores vaccination indicators for countries and dates where suitable data is available.

## 🧮 Key Metrics

**Case Fatality Rate (CFR)**

The percentage of reported cases that resulted in reported deaths:

```text
CFR = (Total Reported Deaths / Total Reported Cases) × 100
```

**Seven-Day Rolling Average**

The average of daily new cases over a seven-day window, calculated separately for each country.

**Estimated Doubling Time**

An estimate based on comparing cumulative cases with the value seven days earlier. It is calculated only when both values are positive and cases have increased.

## 📊 Power BI Dashboard

The planned dashboard can include:

- KPI cards for reported cases and deaths.
- Daily cases and seven-day rolling average trend charts.
- Country-level comparisons.
- Vaccination coverage visualizations.
- Date and country filters for interactive exploration.

The dashboard should use consistent date filters and avoid double-counting country totals if a global aggregate row is included.

## 🔍 Key Findings

- The original dataset contains 28,240 rows and 61 columns.
- A substantial amount of data is missing, so results must be interpreted carefully.
- Seven completely empty columns were removed during cleaning.
- No duplicate rows or duplicate country-date records were identified by the checks.
- Rolling averages help make broader changes in daily case reports easier to interpret.
- Country comparisons should consider population size, testing availability, reporting practices, and data completeness.

Specific country rankings and final totals should be reported only after verifying the values from the cleaned dataset.

## ⚠️ Limitations

- Missing values may affect comparisons and visualizations.
- COVID-19 reporting practices vary between countries and over time.
- Reported cases do not necessarily represent all infections.
- Vaccination indicators may not be available for every country or date.
- The case fatality rate is a descriptive ratio of reported data, not an individual's probability of death.


## 🏁 Conclusion

This project demonstrates how Python and data visualization tools can be used to clean and explore COVID-19 data. The analysis establishes a foundation for understanding reported case trends, deaths, and vaccination indicators and for presenting the results in an interactive Power BI dashboard.

dashboard development.
