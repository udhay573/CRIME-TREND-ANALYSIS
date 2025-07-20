# 🕵️ Crime Trend Analysis 


🔍 Overview
This project analyzes Los Angeles crime data from Jan 2020 to Oct 2023 to identify crime trends, seasonal effects, hotspot regions, and forecast future crime incidents using statistical models.


📁 Data Summary
Source: Los Angeles Open Data Portal
https://data.lacity.org/Public-Safety/Crime-Data-from-2020-to-Present/2nrs-mtv8/about_data

Time Frame: Jan 2020 – Oct 2023

Total Columns: 28

Important Fields:

DATE OCC – Crime occurrence date

TIME OCC – Crime occurrence time

AREA NAME – Location

CRM CD DESC – Crime description

VICT SEX, VICT AGE, VICT DESCENT – Victim demographics



🧹 Data Cleaning
Excluded 2023 (partial year)

Filled missing values with "Unknown"

Cleaned inconsistent gender entries

Converted date fields to datetime format

Verified no duplicate rows





📊 Key Findings



📈 Crime Trends
Overall crime grew at 8.38% CAGR (2020–2022)

Top Crime: Vehicle Theft

Fastest Growing: Identity Theft (8.5k → 22k)


📆 Seasonality & Timing
No strong seasonality; minor dip in February

Crimes peak on Fridays and Saturdays

Most active times: Afternoons and late nights


📍 Regional Crime Distribution
Highest Crime Area: Central (~42k crimes)

Lowest: Foothill (~22k crimes)

Average per area: ~31k


👤 Victim Analysis
Top male-targeted crime: Aggravated Assault

Top female-targeted crime: Intimate Partner Assault

Common to both: Battery - Simple Assault


🧨 External Event Impacts
COVID-19: Sharp drop during lockdowns

Elections: Temporary crime dip due to high security

Juvenile Crime Spike: Notable increase post-March 2022


📈 Forecasting
Model Used: ARIMA (30, 0, 30)

Forecast Horizon: 90 days

Accuracy:

R² = 55.7%

MSE = 5034.67

Model shows decent performance and captures recent trends


🧰 Tools & Libraries
Language: Python

Libraries:

pandas, numpy – Data handling

matplotlib, seaborn – Visualization

statsmodels – ARIMA modeling

sklearn – Metrics & preprocessing

