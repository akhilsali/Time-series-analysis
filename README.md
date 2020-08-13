# Forecasting Beer Demand using Seasonal ARIMA model

In this notebook, I will be implementing the Seasonal ARIMA model on a non stationary time series data and forecast the future demand.
The seasonal part of an ARIMA model has the same structure as the non-seasonal part: it may have an AR factor, an MA factor, and/or an order of differencing. 
* A seasonal ARIMA model is classified as an ARIMA(p,d,q)x(P,D,Q) model, where P=number of seasonal autoregressive (SAR) terms, D=number of seasonal differences, Q=number of seasonal moving average (SMA) terms
* In identifying a seasonal model, the first step is to determine whether or not a seasonal difference is needed, in addition to or perhaps instead of a non-seasonal difference. You should look at time series plots and ACF and PACF plots for all possible combinations of 0 or 1 non-seasonal difference and 0 or 1 seasonal difference. Caution: don't EVER use more than ONE seasonal difference, nor more than TWO total differences (seasonal and non-seasonal combined).
* If the seasonal pattern is both strong and stable over time (e.g., high in the Summer and low in the Winter, or vice versa), then you probably should use a seasonal difference regardless of whether you use a non-seasonal difference, since this will prevent the seasonal pattern from "dying out" in the long-term forecasts.
