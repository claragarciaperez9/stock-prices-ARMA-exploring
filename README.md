## Project Overview

This notebook contains a comprehensive analysis of stock price time series data.
Trend removal and stationarity transformation (log returns)

Statistical and distributional analysis of returns

Time series modeling (ARMA models)

Volatility analysis and explanation of volatility clustering

Autocorrelation analysis of transformed returns

## Key sections

### Data Preparation
How we get to 100* ( log(pt) - log(Pt-1) )

### Statistical and Distributional Analysis of returns

Fat tails, non normality and not uncorrelated returns

### Model decision based on correlograms

Compare Normality tests (Jarque-Bera, Shapiro-Wilk), tail behavior analysis, Diebold-Mariano tests for forecast comparisons.

### Diebold confidence bounds --> estimate variance

Since there is heteroskedasticity, the asymptotic variance under H₀ is no longer 1/T, but larger. We plot the ACF with corrected confidence bands.

### Volatility clustering visualization with ACF of transformed returns

Since the expectation is zero, the squared and absolute returns are related to the dispersion/risk/variance. 
Thus, a positive correlation of these transformations means that volatility exhibits temporal dependence and will therefore appear clustered.

## Conclusions

A linear model is not sufficient for a series with such volatility clustering.
The model that will explain the dependence of returns must be nonlinear and capable of explaining the 3 stylized facts.

