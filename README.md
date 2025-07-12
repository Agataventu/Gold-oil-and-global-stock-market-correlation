# Oil, Gold, and Global Stock Market Dynamics: An Econometric Analysis

This repository contains the full documentation, code, and results of an econometrics project examining the relationships between gold, oil, and the MSCI World Index. The analysis investigates how these relationships changed before and after the COVID-19 pandemic using advanced time series techniques.

## Overview

We study the dynamic interactions among:
- **Gold Spot Price (USD)**
- **Crude Oil WTI Futures (USD)**
- **MSCI World Index (USD)**

Our objective is to understand whether and how the relationships between these assets evolved over time, particularly across the pre- and post-COVID-19 periods.

## Data

- **Source**: [Investing.com]
- **Period**: January 2013 – December 2024
- **Frequency**: Daily closing prices
- **Variables**: Gold, Oil, and MSCI Index returns

## Methodology

### 1. Preliminary Analysis
- Log-return transformation
- ACF and PACF tests
- Augmented Dickey-Fuller test for stationarity

### 2. Modeling Approach
- **VAR (Vector Autoregression)**:
  - Used to detect interdependencies and Granger causality
  - Separate models estimated for pre- and post-COVID periods
- **DCC-GARCH (Dynamic Conditional Correlation GARCH)**:
  - Captures time-varying volatility and co-movements
  - Allows for different correlation regimes across time
  - Used t-distributed residuals and Exponential GARCH effects

## Key Findings

- **Pre-COVID**:
  - Weak Granger causality
  - Gold modestly predicted oil; oil led MSCI movements
  - Volatility highly persistent; small but significant correlation shocks

- **Post-COVID**:
  - Stronger influence of MSCI and Gold; Oil’s predictive power declined
  - Correlation shocks became larger and more short-lived
  - Fat tails and extreme co-movements became more pronounced

## Contents
- `findings_and_interpretation.pdf`: Full report with data, models, and interpretation
- `asset_correlation_code.pdf`: R code used for the full analysis


## 🛠 Tools Used

- R and RStudio
- Packages: 'vars', 'tseries', 'rugarch', 'rmgarch', 'FinTS'

## Authors

- Marco Giovanni Barbero  
- Ettore Davide Brignoli  
- Agata Venturi  

*Politecnico di Milano*  
*Project Date: June 15, 2025*
