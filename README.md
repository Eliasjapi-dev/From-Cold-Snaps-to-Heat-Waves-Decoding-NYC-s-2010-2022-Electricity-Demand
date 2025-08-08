# From Cold Snaps to Heat Waves: Decoding NYC’s Electricity Demand (2010–2022)

**A comprehensive data exploration and predictive modeling workflow analyzing how weather extremes shape New York City’s electricity consumption, cost, and demand forecasting.**

<p align="center">
  <img src="https://github.com/user-attachments/assets/6b68e230-754b-42d8-9fa3-4aa19c141393" alt="LinkedIn Banner" width="80%"/>
</p>

## 📖 Project Description

Between January 1, 2010, and December 31, 2022, New York City experienced volatile temperature swings—from frigid winter cold snaps to scorching summer heat waves. This Jupyter notebook:

1. **Frames clear research questions** around the relationships between average temperature, heating degree days (HDD), cooling degree days (CDD), and daily electricity demand (MWh) & cost (USD).
2. **Integrates two public datasets**: Central Park’s historical weather (Kaggle) and NYC OpenData’s electricity consumption & cost.
3. **Walks through complete data preparation**: parsing dates, cleaning, aligning multi-year time series, handling missing values, and merging.
4. **Showcases exploratory visualizations**—time-series plots, heatmaps, and distribution charts—to reveal seasonality, trends, and anomalies.
5. **Conducts rigorous statistical analysis**: Pearson & Spearman correlations, hypothesis tests, and rolling-window trend assessments to quantify weather–demand relationships.
6. **Implements predictive models**: trains and evaluates multiple regression algorithms (Linear Regression, Random Forest) to forecast electricity demand based on weather features.
7. **Analyzes feature importance**: interprets model coefficients and Random Forest importances to identify the most influential variables driving consumption.
8. **Summarizes actionable insights** for grid operators and policymakers, highlighting strategic focus areas for demand response and infrastructure planning.

---

## 📈 Key Visualizations & Model Outputs

<p align="center">
  <img src="https://github.com/user-attachments/assets/a9700469-d959-4d73-9b28-905974e04d3e" alt="Monthly Comparison" width="80%"/>
  <br>
  <em>Figure 1. Monthly average temperature vs. electricity consumption (2010–2022).</em>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/983a3ebe-618b-4290-a27b-a25b8f93d133" alt="Pearson Heatmap" width="45%" style="margin-right:5px;"/>
  <img src="https://github.com/user-attachments/assets/c0b429cc-645d-4998-9a8b-0e1d3968c7ab" alt="Spearman Heatmap" width="45%"/>
  <br>
  <em>Figure 2. Pearson correlation matrix &nbsp;&nbsp;|&nbsp;&nbsp; Figure 3. Spearman correlation matrix.</em>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/5201eabd-7904-413d-99d5-e96ed36079e4" alt="Significance Table" width="40%" style="margin-right:5px;"/>
  <br>
  <em>Figure 4. Statistical significance (95% CI) of Pearson  & Spearman correlations.</em>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/f7269df1-3515-4aef-a741-c47008f5e767" alt="Interpretation Table" width="73%"/>
  <br>
  <em>Figure 5. Summary of key correlation coefficients & interpretations.</em>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/e0de9c50-bc0a-4197-a10c-b83f7a20f34c" alt="Model Predictions on Test Data" width="73%"/>
  <br>
  <em>Figure 6. Model predictions vs. actual consumption on test dataset.</em>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/8ec13393-7052-4cdf-aa56-0b1972c7008e" alt="Linear Regression Coefficients" width="25%"/>
  <br>
  <em>Figure 7. Linear Regression coefficients (sorted by absolute magnitude).</em>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/8f3e94c0-9d29-44a4-84c5-8806c5f5c8c9" alt="Top 10 Feature Importances" width="40%"/>
  <br>
  <em>Figure 8. Top 10 feature importances from Random Forest model.</em>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/b0611183-595b-4846-9961-6996f53c505b" alt="Model Performance on Test Data" width="40%"/>
  <br>
  <em>Figure 9. Model performance metrics (R², RMSE, MAE) on test set.</em>
</p>

---

## 🗂 Notebook Structure

```text
1. Project Introduction & Motivation
2. Research Questions & Objectives
3. Data Sources & Ingestion
4. Data Wrangling & Feature Engineering
5. Exploratory Data Analysis (EDA)
6. Statistical & Correlational Analysis
7. Predictive Modeling   
   • Model Selection (Linear Regression, Random Forest)  
   • Train/Test Split & Cross-Validation  
   • Performance Metrics (R², RMSE, MAE)  
8. Feature Importance & Coefficient Interpretation
9. Forecasting Insights & Discussion
10. Conclusions & Next Steps
```

## 📂 Repository Layout

```
├── NYC_Central_Park_weather_1869-2022.csv                               # Daily weather observations
├── Electric_Consumption_And_Cost__2010_-_Feb_2025.csv                   # Daily electricity usage & cost
├── from_cold_snaps_to_heat_waves_nyc_electricity_demand_2010-2022.ipynb # Analysis notebook
├── README.md                                                            # Project overview & instructions
└── requirements.txt                                                     # Python dependencies
```

---

## Data Sources

| Dataset                          | Provider               | Period            | Link                                                                                         |
|----------------------------------|------------------------|-------------------|----------------------------------------------------------------------------------------------|
| **Central Park Weather History** | Kaggle (NOAA)          | 2010–2022 (subset)| https://www.kaggle.com/danbraswell/new-york-city-weather-18692022                           |
| **Electric Consumption & Cost**  | NYC OpenData           | 2010–Feb 2025     | https://data.cityofnewyork.us/Housing-Development/Electric-Consumption-And-Cost-2010-Feb-2025-/jr24-e7cr |

---

## 🚀 How to Run

1. **Clone the repository**:

   ```bash
   git clone https://github.com/Eliasjapi-dev/From-Cold-Snaps-to-Heat-Waves-Decoding-NYC-s-2010-2022-Electricity-Demand.git
   cd nyc-weather-electricity-analysis
   ```
2. **Install dependencies**:

   ```bash
   pip install -r requirements.txt
   ```
3. **Launch the notebook**:

   * Open `notebooks/from_cold_snaps_to_heat_waves_nyc_electricity_demand_2010-2022.ipynb` in Jupyter Lab or Notebook.
   * Run all cells to reproduce the full analysis, statistical tests, and predictive modeling.

## 🧰 Dependencies

* Python 3.8+
* pandas, numpy, matplotlib, seaborn
* scipy, statsmodels, scikit-learn

## 🤝 Contributing

Contributions, issue reports, and pull requests are welcome! Feel free to:

* Integrate advanced forecasting algorithms (ARIMA, XGBoost)
* Add spatial analysis (borough/district-level load forecasting)
* Develop interactive dashboards (Plotly, Streamlit)

---

*Authored by Elías Jara | Updated: August 2025*
