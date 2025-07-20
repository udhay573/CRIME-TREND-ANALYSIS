🔍 Crime Trend Analysis (2020–2022)

This project analyzes crime data from Jan 2020 to Dec 2022 to uncover trends, patterns, and predictive insights using Python and statistical modeling. The analysis was conducted as part of the IE6400 Foundations for Data Analytics course at Northeastern University.


📂 Data Source

The dataset was obtained from a public crime reporting source covering Jan 2020 – Oct 2023. Only full years (2020–2022) were considered for analysis.

🧹 Data Cleaning

Excluded partial data from 2023.

Filled nulls in victim gender, descent, and premises with "Unknown".

Encoded inconsistent gender values ('H', 'Unknown') as 'X'.

Converted date columns to datetime format.

Checked for and removed duplicate records.



📊 Key Insights




📈 Overall Crime Trends


Crimes increased at a CAGR of 8.38% from 2020 (~200K) to 2022 (~234K).


📅 Seasonality & Day-of-Week


No strong monthly seasonality detected.

Fridays and Saturdays show highest crime frequency.

Tuesdays show the lowest.


🚓 Most Common Crimes

Top Crime (All years): VEHICLE – STOLEN

Significant rise in THEFT OF IDENTITY from 2020 to 2022.


🌍 Regional Crime Distribution

Average: ~31K crimes per area.

Central area highest (~42K), Foothill lowest (~22K).


🧒 Demographics & Impact

Males most frequently face ASSAULT WITH DEADLY WEAPON.

Females face more INTIMATE PARTNER - SIMPLE ASSAULT.


📉 Major Event Impacts

Sharp drop in crime during COVID lockdowns (2020).

Rise in juvenile crimes post-2022 linked to policy changes.


📈 Forecasting Future Crime (ARIMA)

Used ACF and PACF to configure ARIMA(30, 0, 30).

Forecasted 90 future days.


Achieved:

MSE: ~5034.67

R² Score: 55.73%


📎 Tools & Technologies

Python (Pandas, Matplotlib, Statsmodels)

Jupyter Notebook

ARIMA for time series forecasting
