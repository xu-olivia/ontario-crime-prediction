# Ontario Crime Analysis and Prediction

## 📖 Table of Contents
- [Overview](#overview)
- [Objectives](#objectives)
- [Data Sources](#data-sources)
- [Analytical Approach](#analytical-approach)
- [Key Findings](#key-findings)
- [Recommendations](#recommendations)
- [Output Files](#output-files)
- [Next Steps](#next-steps)

### 📌 Overview
This project explores the relationship between regional crime rates and demographic factors across Ontario. Using publicly available crime statistics and demographic data by health unit, the analysis identifies the key drivers of criminal activity and provides policy-oriented recommendations.

### 🎯 Objectives
- Identify regional and demographic drivers of crime in Ontario.
- Quantify the impact of key features (e.g. family structure, immigration, income) on crime rates using linear regression.
- Examine trial rate variations and their regional distribution.
- Support crime prevention strategy through data-driven insights.

### 📈 Data Sources
- Ontario Crime Dataset: Includes 20 features such as offence type, case disposition status, and trial rate.
- Demographic Dataset: Includes 36 features covering population structure, employment, income, and education at the health unit level.
- [Download Here](https://github.com/xu-olivia/ontario-crime-prediction/blob/main/Ontario%20Crime%20Statistics.xlsx)

### 💻 Analytical Approach
- Data Integration: Merged regional crime and demographic datasets using geographic identifiers.
- Feature Selection: Performed correlation analysis to identify variables with strong relationships to crime cases.
- Modelling: Developed linear regression models to test statistical significance and predictive strength.
- Segmentation: Grouped regions into five zones for deeper geographic insights.

### 📁 Key Findings
- High Crime Drivers are % of female lone-parent families, % of immigrants and % of visible minorities. These variables showed statistically significant correlations (p ≈ 0) and explained up to 72% of crime case variance.
  <img width="660" alt="Key Driver of Crime" src="https://github.com/user-attachments/assets/deea16fb-80e0-4a12-a03c-0dc83628bbdc" />
  <img width="660" alt="Linear Regression" src="https://github.com/user-attachments/assets/a3d987c7-6b6e-4448-b314-4e8ff5cc6f16" />

- Trial Rate: Not significantly predicted by the current features, suggesting the need for additional data.
  <img width="660" alt="Key Driver of Trial Rate" src="https://github.com/user-attachments/assets/793a9543-03b7-4191-9aec-b57f4066684c" />

- Geographic Hotspots: Central Ontario (Toronto, Peel, Durham) accounts for over 40% of all criminal cases.
  <img width="660" alt="Geographic Hotspots" src="https://github.com/user-attachments/assets/2b54f81d-f9b0-4bc1-8afd-7af7fa3515e5" />

### 📑 Recommendations
- Invest in support services for lone-parent families and new immigrants (e.g., counselling, financial aid).
- Promote early intervention programs for youth exhibiting behavioral issues.
- Develop machine learning models for crime prediction and resource allocation.

### 🗄️ Output Files
- [demographics_cleaned.xlsx](https://github.com/xu-olivia/ontario-crime-prediction/blob/main/Demographic_Cleaned.xlsx) – Regional demographic data.
- [criminal offenses_cleaned.xlsx](https://github.com/xu-olivia/ontario-crime-prediction/blob/main/Criminal%20Offenses_Cleaned.xlsx) – Criminal offenses data.
- [data_cleaning.py](https://github.com/xu-olivia/ontario-crime-prediction/blob/main/Data%20Cleaning.ipynb) - Python script for data cleaning.
- [ontario_crime_analysis.py](https://github.com/xu-olivia/ontario-crime-prediction/blob/main/Correlation%20Analysis%20and%20Linear%20Regression.ipynb) – Python script for inferential analysis and data modelling.

### 📍 Next Steps
- Incorporate real-time or multi-year data to capture trends.
- Explore non-linear models or classification approaches for predicting trial outcomes.
- Investigate potential spatial dependencies using geospatial analytics.
