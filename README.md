This project demonstrates a comprehensive **time series analysis** of electricity **consumption and production data**. 
It covers **exploratory data analysis (EDA)**, **visualizations**, and **forecasting** using models such as **ARIMA** and **SARIMA**. 
The project is part of a portfolio to showcase skills in data preprocessing, analysis, and modeling of time-dependent data.

---

## Project Structure
```
├── data/
│   └── Electricity.csv         # Raw dataset
├── notebooks/
│   └── Time_Series_Analysis.ipynb
├── reports/
│   └── Time Series Analysis Portfolio Project.pdf
├── README.md
└── requirements.txt
```

---

## Dataset

The dataset contains **hourly electricity consumption and production data** from **January 1, 2019, to March 31, 2024**.

| Column Name   | Description                              |
|---------------|------------------------------------------|
| DateTime      | Timestamp (hourly data)                  |
| Consumption   | Total electricity consumption (MW)       |
| Production    | Total electricity production (MW)        |
| Nuclear       | Nuclear power production (MW)            |
| Wind          | Wind power production (MW)               |
| Hydroelectric | Hydroelectric power production (MW)      |
| Oil and Gas   | Oil and gas power production (MW)        |
| Coal          | Coal power production (MW)               |
| Solar         | Solar power production (MW)              |
| Biomass       | Biomass power production (MW)            |

**Date Range:**  
- Start: 2019-01-01 00:00:00  
- End: 2024-03-31 23:00:00  
- Total Records: 46,011

---

## Steps Performed

### 1. Data Preprocessing
- Converted DateTime column to pandas datetime format.
- Handled missing values and ensured time-based indexing.
- Extracted date-related features like Year, Month, Weekday, and Hour.

### 2. Exploratory Data Analysis (EDA)
- Identified trends and seasonality using visualizations and decomposition.
- Analyzed correlations using heatmaps.
- Aggregated daily and monthly statistics for insights.

### 3. Data Visualization
- Time series plots for consumption vs. production.
- Rolling averages for smoothing trends.
- Faceted charts for production sources.

### 4. Statistical Tests
- Conducted Augmented Dickey-Fuller (ADF) test for stationarity.
- Applied differencing techniques to stabilize variance.

### 5. Modeling & Forecasting
- ARIMA for baseline forecasting.
- SARIMA for incorporating seasonality.

### 6. Evaluation
- Residual analysis and error metrics like MAE, MSE, and RMSE.

---

## Key Insights
- Strong daily and seasonal consumption patterns.
- Increased solar and wind energy production in certain months.
- SARIMA outperformed ARIMA due to its ability to model seasonality.

---

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Statsmodels
- SciPy

---

## How to Run the Project
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/time-series-analysis.git
   cd time-series-analysis
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

---

## Future Work
- Explore deep learning models like LSTM and GRU.
- Automate hyperparameter tuning for ARIMA/SARIMA.
- Build a real-time dashboard.


