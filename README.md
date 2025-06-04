# Ontario Crime Analysis and Prediction

## Table of Contents
- [Overview](#overview)
- [Objectives](#objectives)
- [Data Sources](#data-sources)
- [Analytical Approach](#analytical-approach)
- [Key Findings](#key-findings)
- [Recommendations](#recommendations)
- [Output Files](#output-files)
- [Next Steps](#next-steps)

### Overview
This project explores the relationship between regional crime rates and demographic factors across Ontario. Using publicly available crime statistics and demographic data by health unit, the analysis identifies the key drivers of criminal activity and provides policy-oriented recommendations.

### Objectives
- Identify regional and demographic drivers of crime in Ontario.
- Quantify the impact of key features (e.g. family structure, immigration, income) on crime rates using linear regression.
- Examine trial rate variations and their regional distribution.
- Support crime prevention strategy through data-driven insights.

### Data Sources
- Ontario Crime Dataset: Includes 20 features such as offence type, case disposition status, and trial rate.
- Demographic Dataset: Includes 36 features covering population structure, employment, income, and education at the health unit level.

### Analytical Approach
- Data Integration: Merged regional crime and demographic datasets using geographic identifiers.
- Feature Selection: Performed correlation analysis to identify variables with strong relationships to crime cases.
- Modelling: Developed linear regression models to test statistical significance and predictive strength.
- Segmentation: Grouped regions into five zones for deeper geographic insights.

### Key Findings
- High Crime Drivers are % of female lone-parent families, % of immigrants and % of visible minorities. These variables showed statistically significant correlations (p ≈ 0) and explained up to 72% of crime case variance.

- Trial Rate: Not significantly predicted by the current demographic features, suggesting the need for non-linear modelling or additional contextual data.

- Geographic Hotspots: Central Ontario (Toronto, Peel, Durham) accounts for over 40% of all criminal cases.


### Recommendations
- Invest in support services for lone-parent families and new immigrants (e.g., counselling, financial aid).
- Promote early intervention programs for youth exhibiting behavioral issues.
- Develop machine learning models for crime prediction and resource allocation.


### Output Files
- ontario_crime.xlsx – Raw crime data.
- demographics.xlsx – Regional demographic data.
- ontario_crime_analysis.py – Python script for data cleaning, EDA, modeling, and visualization.
- Ontario Crime Insights.pdf – Summary of insights, visuals, and key conclusions.

### Next Steps
- Incorporate real-time or multi-year data to capture trends.
- Explore non-linear models or classification approaches for predicting trial outcomes.
- Investigate potential spatial dependencies using geospatial analytics.
