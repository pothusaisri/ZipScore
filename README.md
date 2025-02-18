# ZipScore

## Title: ZipScore: Regional Desirability & Socioeconomic Dashboard

### 🗂️ Project Overview
ZipScore is an interactive data visualization dashboard designed to evaluate and compare zip codes within a selected region (state and county) based on key socioeconomic variables. The dashboard calculates a composite "desirability score" for each zip code, enabling users to assess factors such as education, income, employment, housing, and population demographics. This tool is ideal for policymakers, real estate professionals, or residents seeking data-driven insights into regional livability.

### 🎯 Project Objectives

This dashboard empowers users to make data-driven decisions by transforming socioeconomic metrics into actionable insights. Homebuyers and renters evaluate neighborhoods through livability scores based on income, education, and housing affordability. Real estate professionals identify investment opportunities using composite scores and housing trends. Policymakers allocate resources equitably by analyzing underserved regions with low scores, while nonprofits tailor community programs using demographic data. Researchers streamline analysis with preprocessed, transparent Census datasets. Finally, urban planners prioritize infrastructure projects via interactive maps, fostering equitable and sustainable development.

### Data Description

Variables Collected :

Median Household Income
Source: U.S. Census Bureau (Table ACSST1Y2023_S240G7).
Description: Annual median income by zip code.

Education Attainment (% Bachelor’s Degree or Higher)
Source: U.S. Census Bureau (Table ACSST1Y2023_S0101).
Description: Percentage of adults aged 25+ with a bachelor’s degree.

Employment Rate
Source: U.S. Census Bureau (Table ACSST1Y2023_S240G7).
Description: Percentage of working-age population employed.

Housing Affordability
Source: U.S. Census Bureau (Table ACSST1Y2023_S0101).
Description: Median housing value categorized into price ranges.

Population Age Distribution
Source: U.S. Census Bureau (Table ACSST1Y2023_S0101).
Description: Population segmented by age groups (e.g., 25–34, 65+).

### Data Preprocessing:

To ensure accurate and meaningful visualizations, the raw data undergoes rigorous preprocessing:

Outlier Removal:
Anomalous values (e.g., a $10M median income in a low-income zip code) are flagged using interquartile range (IQR) or Z-score thresholds and excluded to prevent skewed analysis.

Missing Value Imputation:
Gaps in data (e.g., unreported housing values) are filled using county-level averages to maintain dataset integrity without introducing bias.

Normalization (0–1 Scale):
Variables like income (20k–200k) and education rates (0–100%) are scaled to a 0–1 range using min-max normalization.
This ensures comparability when aggregating scores (e.g., combining income and education metrics

Integration with Tableau:
Cleaned data is exported as a .csv or connected via Tableau’s data connectors.

### 📊 Visualization Features
Interactive Map:
Color gradients reflect composite scores (darker = higher desirability).
Clickable zip codes to filter downstream charts.

Variable-Specific Charts:
Bar graphs for income brackets and education levels.
Heatmaps for population density.
Pie charts for employment sector breakdown (private, government, self-employed).

##### Data Sources
All data is sourced from publicly available U.S. Census Bureau datasets. Example citations (APA format):

U.S. Census Bureau. (2023). American Community Survey 1-Year Estimates: Employment Status (Table S240G7). Retrieved from https://data.census.gov/table/ACSST1Y2023_S240G7

U.S. Census Bureau. (2023). American Community Survey 1-Year Estimates: Population by Age (Table S0101). Retrieved from https://data.census.gov/table/ACSST1Y2023_S0101

##### Methodology

Weighted Aggregation: Scores are calculated as (Income × 0.2) + (Education × 0.2) + (Employment × 0.2) + (Housing × 0.2) + (Age Diversity × 0.2).

##### Screenshot
<img width="1258" alt="Screenshot 2025-02-18 at 2 31 00 PM" src="https://github.com/user-attachments/assets/f1c3b9c8-2152-4981-a735-0edadd7ac50e" />

##### link to dashboard - 
https://public.tableau.com/app/profile/saisree.pothu8740/viz/ZipcodeDataDashboard2022/Dashboard2

License
This project is licensed under the MIT License. Data sourced from the U.S. Census Bureau is free for public use.
