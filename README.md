🕵️ Crime Trend Analysis – Los Angeles Crime Data Analytics

📁 Dataset
* **Source:** Los Angeles Open Data Portal
* **URL:** https://data.lacity.org/Public-Safety/Crime-Data-from-2020-to-Present/2nrs-mtv8/about_data
* **Time Period:** January 2020 – October 2023
* **Total Features:** 28 columns
* **Key Fields:**
   * DATE OCC, TIME OCC: Temporal data
   * AREA NAME: Geographic location
   * CRM CD DESC: Crime classification
   * VICT_SEX, VICT_AGE, VICT_DESCENT: Demographics

🧹 Data Preprocessing
* **Year Filtering:** Excluded 2023 (partial year data)
* **Missing Values:** Filled with "Unknown" category
* **Data Cleaning:** Standardized inconsistent gender entries
* **Type Conversion:** Datetime formatting for temporal analysis
* **Deduplication:** Verified no duplicate records

🔍 Analytical Insights
* **Growth Rate:** 8.38% CAGR (2020-2022)
* **Top Crime Type:** Vehicle Theft
* **Fastest Growing:** Identity Theft (8.5k → 22k incidents)
* **Temporal Patterns:**
   * Peak Days: Fridays & Saturdays
   * Peak Hours: Afternoons & late nights
   * Seasonal: Minor dip in February

📍 Geographic Distribution
| Area | Crime Count | Status |
|------|-------------|---------|
| **Central** | **~42,000** | **Highest** |
| Average | ~31,000 | Baseline |
| Foothill | ~22,000 | Lowest |

👥 Victim Demographics
* **Male-targeted:** Aggravated Assault (most common)
* **Female-targeted:** Intimate Partner Assault (most common)
* **Both genders:** Battery - Simple Assault

🌊 External Impact Analysis
* **COVID-19 Lockdowns:** Sharp crime reduction
* **Election Periods:** Temporary dips due to increased security
* **Post-March 2022:** Notable juvenile crime surge

📈 Forecasting Model & Results
| Model | Parameters | Horizon | R² Score | MSE |
|-------|------------|---------|----------|-----|
| **ARIMA** | **(30, 0, 30)** | **90 days** | **55.7%** | **5034.67** |

**Model Performance:** Decent accuracy with good recent trend capture

🧰 Tools & Technologies
* **Programming:** Python
* **Data Processing:** pandas, numpy
* **Visualization:** matplotlib, seaborn
* **Statistical Modeling:** statsmodels (ARIMA)
* **Metrics & Evaluation:** scikit-learn

✅ Key Conclusions
* Crime shows a consistent upward trend with 8.38% annual growth
* Vehicle theft remains the dominant crime category
* Identity theft is experiencing explosive growth (158% increase)
* Geographic disparities persist, with the  Central area most affected
* External events significantly impact crime patterns

🚀 Future Enhancements
* **Advanced Models:** LSTM/Prophet for better time series forecasting
* **Real-time Analysis:** Streaming data pipeline integration
* **Predictive Policing:** ML models for crime prevention strategies
* **Demographic Deep Dive:** Intersectional analysis of victim patterns
* **Cross-city Comparison:** Benchmark against other major US cities
