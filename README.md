# exchange-rate-time-series-modeling
Time series econometrics project: stationarity analysis, ARMA modeling, impulse responses and forecasting of the CAD/USD exchange rate.
# 📈 CAD/USD Exchange Rate Time Series Analysis

Time series econometrics project implemented in **R**, focusing on the analysis and forecasting of the CAD/USD exchange rate.

---

## Project Overview

This project investigates the dynamics of the monthly CAD/USD exchange rate using classical time series econometric methods.

The objectives are to:

- Study the stationarity properties of the series;
- Estimate AR and ARMA models by maximum likelihood;
- Select the most appropriate model using statistical tests and information criteria;
- Analyze impulse response functions;
- Perform out-of-sample forecasting.

---

## Data

- Monthly CAD/USD exchange rate data.
- Variable analyzed:

\[
z_t=\ln(CADUSD_t)
\]

---

## Methodology

### 1. Stationarity Analysis

- Log transformation
- Quadratic deterministic trend removal
- First differencing
- Autocorrelation function (ACF)

#### Conclusion

The first-differenced series is found to be stationary.

---

### 2. Model Estimation

Eight models are estimated using Maximum Likelihood:

#### AR Models

- AR(1)
- AR(2)
- AR(3)
- AR(4)

#### ARMA Models

- ARMA(1,1)
- ARMA(2,2)
- ARMA(3,3)
- ARMA(4,4)

---

### 3. Model Selection

Models are compared using:

- Wald tests
- Likelihood ratio tests
- AIC
- BIC
- Ljung-Box residual autocorrelation tests

#### Selected Models

- **AR(1)**
- **ARMA(1,1)**

---

### 4. Dynamic Responses

Impulse response functions are studied under:

- A single positive shock
- Three consecutive negative shocks

Both models exhibit stationary behavior and rapidly converge back to equilibrium.

---

### 5. Forecasting

Out-of-sample forecasts are generated using:

- AR(1)
- ARMA(1,1)

The forecasts are compared with the actual series and a naïve benchmark.

---

## Main Results

- The CAD/USD exchange rate exhibits a stochastic trend.
- First differencing successfully achieves stationarity.
- AR(1) and ARMA(1,1) provide parsimonious and adequate representations of the series.
- Impulse responses decay rapidly, confirming stationarity.
- Forecasting performance is evaluated on a validation sample.

---

## Tools and Packages

### Programming Language

- R

### Packages

- forecast
- stats
- tseries
- ggplot2
- MASS
- readxl

---

## Repository Structure

```
.
├── README.md
├── report.pdf
├── econometrics_project.R
├── data/
│   └── EXCAUS.xlsx
└── figures/
```

---

## Skills Demonstrated

- Time Series Analysis
- Stationarity Testing
- AR and ARMA Modeling
- Maximum Likelihood Estimation
- Model Selection
- Residual Diagnostics
- Impulse Response Analysis
- Forecasting
- Data Visualization
- R Programming

---

## Author

**Lijin Gao**

M.Sc. Financial Engineering  
HEC Montréal

GitHub: https://github.com/gaolijinfr

---
