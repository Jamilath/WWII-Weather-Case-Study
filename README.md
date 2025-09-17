📊 Project Overview
This repository explores and analyzes historical weather data from World War II, focusing on predicting maximum and minimum daily temperatures using regression techniques and delivering actionable insights through an interactive Power BI dashboard.

Python: Data preparation, EDA, statistical modeling & predictions

Power BI: Executive dashboard for visualization and interactive insights

🌐 Problem Statement
Objective:
Investigate weather reports from World War II to compare with aerial bombing operations, and develop a model to predict maximum and minimum daily temperatures based on weather conditions.

Dataset:
Daily weather observations collected from global weather stations during WWII, provided by the US National Oceanic and Atmospheric Administration (NOAA). Features include precipitation, snowfall, temperatures, wind speed, presence of poor weather conditions, and station metadata (location, etc.).

Goal:

Predict maximum and minimum temperatures from available parameters

Uncover key drivers of temperature variation

Present findings via data visualizations for business and historical insight

🛠️ Workflow
1. Data Cleaning & Preparation (Python)
Import raw datasets (weather records, locations, data dictionary)

Data corrections:

Replace "T" trace values in Precip and Snowfall with 0.01

Convert relevant columns to numeric types

Fill missing numeric values with column averages

Handle missing/blank categorical values

Convert date columns to datetime format

Remove duplicates, drop unused columns (Fahrenheit, etc.)

Feature engineering:

Calculated TempRange = MaxTemp - MinTemp

Merge weather and location metadata for geographic context

Save WeatherDataCleaned.csv for downstream analytics

2. Exploratory Data Analysis (Python)
Statistical summaries, group-by analysis (ex: temperature by weather condition or station)

Correlation matrix to identify relationships among features

Visualizations using matplotlib/seaborn (scatterplots, trendlines, etc.)

3. Predictive Modeling (Python)
Linear regression (scikit-learn) for both MaxTemp and MinTemp

Model performance metrics (e.g., MSE)

Interpretation of feature importances

4. Executive Dashboard (Power BI)
Import cleaned data and Python modeling results

Key dashboard features:

KPI cards for average/max/min temperature, precipitation, poor weather days, etc.

Trend analysis over years, temperature and wind metrics

Scatterplots to analyze relationships (e.g., Precip vs. MaxTemp)


📁 Files
ML-Case-Study-Regression.pdf: Project problem statement and context

python-weather_analysis.ipynb: Complete data cleaning, EDA, and modeling in Python

WeatherDataCleaned.csv: Processed dataset (generated after running the notebook)

PowerBI_Dashboard.pbix: Final interactive dashboard (not included, for privacy—build instructions below)

Sample dashboard screenshots in /assets (optional for portfolio/demo)

🚀 How to Run
Clone the repository

Open and run python-weather_analysis.ipynb to prepare/clean data and generate insights

Open Power BI Desktop, load WeatherDataCleaned.csv, and reference provided DAX for measure creation and dashboard building

Review the dashboard for insights and executive-ready visualizations

🎯 Key Insights
The dashboard summarizes weather trends over WWII, highlighting regional and temporal patterns

Regression reveals which weather features most influence temperature extremes

Visuals enable policymakers, historians, or analysts to quickly interpret large-scale historical weather patterns


Geographical map: Avg MaxTemp by station location

Consistent theme and intuitive layout for stakeholders
