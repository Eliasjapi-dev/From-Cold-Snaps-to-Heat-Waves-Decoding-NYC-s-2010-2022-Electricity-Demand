# From Cold Snaps to Heat Waves: Decoding NYC’s Electricity Demand (2010–2022)

**A comprehensive data exploration analyzing how weather extremes shape New York City’s electricity consumption and cost.**

## 📖 Project Description

Between January 1, 2010, and December 31, 2022, New York City experienced increasingly volatile temperature patterns—from brutal cold snaps in winter to record-breaking heat waves in summer. This Jupyter notebook:

1. **Frames clear research questions** around how daily average temperature, heating degree days (HDD), and cooling degree days (CDD) relate to city-wide electricity demand (MWh) and cost (USD).
2. **Integrates two public datasets**: Central Park’s historical weather records (Kaggle) and NYC OpenData’s electricity consumption & cost.
3. **Walks through complete data preparation**: cleaning, aligning dates, handling missing values, and merging time series.
4. **Showcases exploratory visualizations**—interactive line charts and heatmaps—to reveal seasonality, trends, and anomalies.
5. **Conducts rigorous statistical analysis**: Pearson & Spearman correlations, hypothesis tests, and rolling-window trend assessments.
6. **Summarizes actionable insights** for grid operators and policymakers, highlighting how air-conditioning loads drive summer peaks and why electric heating plays a smaller role in winter usage.

## 🗂 Notebook Structure

```text
1. NYC Weather & Electricity Consumption Analysis (2010–2022)         # Project context, questions, sources
2. Why this project?                                                # Motivation and scope
3. Research Questions                                               # Key analytical objectives
4. Data Sources                                                     # Datasets descriptions and loading
5. Methodology                                                     # Data wrangling, cleaning, merging
6. Key Findings                                                    # Early insights summary
7. New York Temp Dataset (Kaggle)                                   # Detailed weather data overview
8. Electricity Consumption & Cost (NYC OpenData)                   # Detailed energy data overview
9. Merging of the DataFrames                                        # Aligning weather & energy
10. Graphs                                                          # Time-series plots, seasonal patterns
11. Statistical and Correlational Analysis                          # Correlations, heatmaps, tests
12. Conclusions                                                     # Final takeaways and recommendations
```

## Data Sources

| Dataset                         | Provider               | Period                 | Link                                                                                         |
|---------------------------------|------------------------|------------------------|----------------------------------------------------------------------------------------------|
| **Central Park Weather History**| Kaggle (NOAA)          | 2010–2022 (subset)     | https://www.kaggle.com/danbraswell/new-york-city-weather-18692022                           |
| **Electric Consumption & Cost** | NYC OpenData           | 2010–2022 (subset)     | https://data.cityofnewyork.us/Housing-Development/Electric-Consumption-And-Cost-2010-Feb-2025-/jr24-e7cr |

## 📂 Repository Layout

```
├── data/                                                        # Raw CSV datasets
│   ├── NYC_Central_Park_weather_1869-2022.csv                   # Daily weather observations
│   └── Electric_Consumption_And_Cost__2010_-_Feb_2025.csv       # Daily electricity usage & cost
├── from_cold_snaps_to_heat_waves_nyc_electricity_demand_2010-2022.ipynb
├── README.md                                                    # Project overview & instructions
└── requirements.txt                                             # Python dependencies
```

## 🚀 How to Run

1. **Clone the repository**:

   ```bash
   git clone https://github.com/Eliasjapi-dev/From-Cold-Snaps-to-Heat-Waves-Decoding-NYC-s-2010-2025-Electricity-Demand.git
   cd nyc-weather-electricity-analysis
   ```
2. **Install dependencies**:

   ```bash
   pip install -r requirements.txt
   ```
3. **Launch the notebook**:

   * Open `from_cold_snaps_to_heat_waves_nyc_electricity_demand_2010-2022.ipynb` in Jupyter.
   * Execute all cells to reproduce data preparation, visualizations, and statistical tests.

## 🧰 Dependencies

* Python 3.8+
* pandas, numpy, matplotlib, seaborn
* scipy, statsmodels

## 🤝 Contributing

Contributions, issue reports, and pull requests are welcome! Feel free to:

* Add short-term forecasting modules or machine-learning models
* Explore borough-level or sub-metering data for deeper insights
* Refactor visualizations for interactivity (e.g., Plotly, Bokeh)

---

*Authored by Elías Jara | Updated: August 2025*
