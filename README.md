# Hidden Groundwater Contamination Patterns in Tamil Nadu Using Python

## Project Overview

This project analyzes groundwater quality data across Tamil Nadu using Python to identify variations in chemical concentrations, understand relationships between groundwater parameters, and highlight locations that may require additional monitoring.

The analysis uses **433 groundwater records from 25 districts**, covering the data acquisition period **2020–2023**.

## Dataset Information

- **Source:** Central Ground Water Board (CGWB), Government of India — National Water Data Portal
- **Region:** Tamil Nadu, India
- **Period:** 2020–2023
- **Original Dataset:** 433 rows and 47 columns
- **Cleaned Dataset:** 433 rows and 35 columns, including engineered features
- **Domain:** Environmental Data Analytics / Groundwater Quality

The dataset contains chemical measurements such as pH, Electrical Conductivity (EC), Total Dissolved Solids (TDS), Total Hardness, Calcium, Magnesium, Chloride, Sulphate, and Uranium.

## Project Objectives

1. Analyze groundwater quality across districts in Tamil Nadu.
2. Identify districts with higher chemical concentrations.
3. Study relationships between major groundwater chemical parameters.
4. Identify unusual groundwater measurements and suggest areas requiring further monitoring.

## Tools and Technologies

- Python
- Google Colab
- Pandas and NumPy
- Matplotlib and Seaborn
- GitHub

## Project Methodology

### Stage 1 — Data Import and Initial Exploration

Imported the groundwater dataset and examined its structure, data types, missing values, and descriptive statistics.

### Stage 2 — Data Cleaning and Transformation

- Checked and handled duplicate records.
- Identified and treated missing values where appropriate.
- Standardized district names and converted date information.
- Created additional features for year, month, and pH categories.
- Retained chemical parameters with substantial missing values without inventing measurements.

### Stage 3 — Statistical Analysis and Visualization

Performed descriptive statistics, distribution analysis, correlation analysis, and district-wise comparisons.

Created **12 visualizations**:

**Univariate Analysis**
1. pH Distribution
2. TDS Distribution
3. Uranium Distribution
4. Groundwater Sample Count by District
5. pH Category Distribution

**Bivariate Analysis**
6. District-wise Median Hardness
7. Electrical Conductivity vs TDS
8. Year-wise Median Hardness
9. District-wise Median Uranium

**Multivariate Analysis**
10. Chemical Parameter Correlation Heatmap
11. District-wise Normalized Chemical Profile Heatmap
12. District-Year Median Hardness Heatmap

### Stage 4 — Findings and Recommendations

Summarized key findings, explained the types of analysis, recommended monitoring priorities, and identified future improvements.

## Key Findings

- **pH:** 431 out of 433 groundwater samples (99.54%) were within the selected pH reference range of 6.5–8.5.
- **Hardness:** Dharmapuri and Salem showed relatively high district-wise median groundwater hardness.
- **Uranium:** Most available measurements were low, but some unusually high concentrations were observed, reaching approximately 0.19 mg/L.
- **Chemical Relationships:** Electrical Conductivity and TDS demonstrated a very strong positive correlation.
- **Sampling Coverage:** Records were unevenly distributed across districts and years, limiting direct comparisons and long-term trend conclusions.

## Recommendations

- Prioritize additional groundwater testing in locations with elevated chemical measurements.
- Investigate unusually high uranium measurements through confirmatory testing.
- Use EC measurements alongside laboratory TDS analysis for monitoring dissolved minerals.
- Improve sampling coverage across districts and years.
- Compare measurements with applicable water-quality standards before making drinking-water safety conclusions.

## Limitations

- Groundwater records are unevenly distributed across districts and years.
- TDS and uranium measurements are unavailable for many records.
- Year-based features are derived from the data acquisition date and may not represent actual sampling dates.
- Elevated chemical concentrations alone do not establish that groundwater is unsafe.
- Predictive machine learning models were not developed as part of this project.

## Future Enhancements

- Expand the dataset with more recent groundwater measurements.
- Develop automated data analysis and interactive dashboards.
- Explore machine learning models for groundwater quality prediction.
- Integrate GIS-based mapping for spatial analysis.

## Project Notebook

[View the Python Analysis Notebook](Tamil_Nadu_Groundwater_Analysis.ipynb)

## Conclusion

This project demonstrates how Python-based data cleaning, statistical analysis, and visualization can help identify groundwater quality patterns across Tamil Nadu.

The results provide a foundation for further environmental monitoring, improved data collection, and evidence-based groundwater management decisions.
