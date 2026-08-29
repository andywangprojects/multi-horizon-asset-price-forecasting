# Multi-Horizon Asset Price Forecasting

**Task 1000 — Predictive Analytics: Stocks & Crypto**

A cross-asset forecasting project that compares traditional time-series modelling
and machine-learning methods across equities and cryptocurrencies over multiple
forecast horizons.

---

## Project Report

The full project report documents the complete workflow, including:

- Exploratory data analysis
- Financial feature engineering
- Multi-horizon target construction
- ARIMA forecasting
- Random Forest regression
- Model evaluation and comparison
- Volatility regime analysis
- Monte Carlo simulation
- Cross-asset analysis
- Final multi-horizon price forecasts
- Model limitations and interpretation

### Full HTML Report

[**Open the Full Project Report →**](https://andywangprojects.github.io/multi-horizon-asset-price-forecasting/report/Task1000_Multi_Horizon_Asset_Forecasting_Report.html)

---

## Project Objective

The objective of this project is to forecast future asset prices across multiple
time horizons while examining how forecasting performance differs between
equities and cryptocurrencies.

Rather than relying on a single modelling framework, the project compares:

- **ARIMA** as a traditional time-series benchmark
- **Random Forest Regressor** as a nonlinear, feature-driven machine-learning model

The project also incorporates financial market characteristics such as momentum,
mean reversion, changing volatility regimes, and cross-asset relationships.

---

## Assets

| Asset | Ticker | Asset Class | Role |
|---|---|---|---|
| Tesla | TSLA | Equity | Forecast Target |
| Alphabet | GOOGL | Equity | Forecast Target |
| Bitcoin | BTCUSD | Cryptocurrency | Forecast Target |
| Ethereum | ETHUSD | Cryptocurrency | Forecast Target |
| Invesco QQQ | QQQ | ETF / Equity Benchmark | Market Benchmark |

QQQ is primarily used as an equity-market benchmark and for market-relative analysis,
rather than as one of the main final forecast targets.

---

## Forecast Horizons

The forecasting framework covers seven horizons:

| Horizon | Purpose |
|---|---|
| 30 Days | Short-term forecast |
| 3 Months | Short-to-medium-term forecast |
| 6 Months | Medium-term forecast |
| 1 Year | Long-term market forecast |
| 3 Years | Long-horizon scenario |
| 5 Years | Long-horizon scenario |
| 10 Years | Structural long-term scenario |

Long-horizon forecasts, particularly 3-year, 5-year, and 10-year estimates,
are interpreted as **model-implied scenarios rather than precise price targets**.

---

## Project Workflow

```text
Raw Historical Data
        ↓
Data Validation & Cleaning
        ↓
Standardized Processed Data
        ↓
Exploratory Data Analysis
        ↓
Financial Feature Engineering
        ↓
Multi-Horizon Target Construction
        ↓
Chronological Train / Test Split
        ↓
ARIMA                 Random Forest
   ↓                         ↓
Forecasts                 Forecasts
        ↓
Model Evaluation
        ↓
Volatility Regime Analysis
        ↓
Monte Carlo Simulation
        ↓
Cross-Asset Comparison
        ↓
Final Multi-Horizon Forecasts


Repository Structure
multi-horizon-asset-price-forecasting/
│
├── data/
│   ├── raw/
│   ├── processed/
│   └── modeling/
│
├── notebooks/
│   └── Asset_Price_Forecasting.ipynb
│
├── src/
│
├── figures/
│
├── results/
│   ├── forecasts/
│   ├── metrics/
│   └── simulations/
│
├── models/
│
├── report/
│   └── Task1000_Multi_Horizon_Asset_Forecasting_Report.html
│
├── README.md
├── requirements.txt
└── .gitignore