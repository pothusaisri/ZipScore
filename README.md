# ZipScore

## Title: ZipScore: Regional Desirability & Socioeconomic Dashboard

### Project Overview
ZipScore is an interactive data visualization dashboard designed to evaluate and compare zip codes within a selected region (state and county) based on key socioeconomic variables. The dashboard calculates a composite "desirability score" for each zip code, enabling users to assess factors such as education, income, employment, housing, and population demographics. This tool is ideal for policymakers, real estate professionals, or residents seeking data-driven insights into regional livability.

### Key Features
##### Composite Desirability Score:

Each zip code is assigned a score (0–1) based on five weighted variables:

Median Household Income (20%)

Education Attainment (% with Bachelor’s Degree or Higher, 20%)

Employment Rate (20%)

Housing Affordability (Median Housing Value, 20%)

Population Age Distribution (Diversity Index, 20%)

Scores are normalized and aggregated using equal weighting for simplicity and transparency.

##### Interactive Map Visualization:

Color-coded map of zip codes (darker hues = higher scores).

Click on zip codes to filter charts and tables.

##### Variable-Specific Visualizations:

Bar charts for income distribution and education levels.

Heatmap for population density.

Pie charts for employment sector breakdown.

##### Score Breakdown Table:

Interactive table showing how each variable contributes to the composite score for selected zip codes.

### Data Sources
All data is sourced from publicly available U.S. Census Bureau datasets. Example citations (APA format):

U.S. Census Bureau. (2023). American Community Survey 1-Year Estimates: Employment Status (Table S240G7). Retrieved from https://data.census.gov/table/ACSST1Y2023_S240G7

U.S. Census Bureau. (2023). American Community Survey 1-Year Estimates: Population by Age (Table S0101). Retrieved from https://data.census.gov/table/ACSST1Y2023_S0101

##### Methodology
Data Collection: Variables are extracted from Census tables and cleaned (e.g., removing outliers, standardizing formats).

Normalization: Each variable is scaled to a 0–1 range using min-max normalization.

Weighted Aggregation: Scores are calculated as (Income × 0.2) + (Education × 0.2) + (Employment × 0.2) + (Housing × 0.2) + (Age Diversity × 0.2).

##### Screenshot
<img width="1258" alt="Screenshot 2025-02-18 at 2 31 00 PM" src="https://github.com/user-attachments/assets/f1c3b9c8-2152-4981-a735-0edadd7ac50e" />

License
This project is licensed under the MIT License. Data sourced from the U.S. Census Bureau is free for public use.
