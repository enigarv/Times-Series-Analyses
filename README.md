# Times Series Analysis
The data refer to hourly measurements of CO covering the period from 10-03-2004 to 28-02-2005.
The aim of the project, given a univariate time series relating to hourly measurements of Oxide of Carbon (CO), is to predict the values of CO in the period between 2005-03-01 and 31-03-2005.

Initially the TS is analyzed graphically in order to understand its trend and possible patterns.

Later we study the **stationarity** of the time series through two statistical tests. The first test used is the **Augmented Dickey-Fuller** test which confirms the hypothesis that the TS is stationary. The **KPSS** test also confirmed this hypothesis.
It follows that the time series is **stationary** and does not require differentiation.

## Forecast
We explored three different approaches to forecast the time series:
- ARIMA (and SARIMA),
- UCM,
- Machine Learning.

In particolar for the ML approaches we explored different architectures: vanilla LSTM, stacked LSTM, bidirectional LSTM and GRU. We discovered that the last NN was the most efficient.

## Result

The performance were compared through the **MAPE** metric which will be used as a reference to evaluate the performance of the models.
The ML model was found to be the best:

| Model    | MAPE  |
|----------|-------|
| Arima    | 10,68 |
| UCM      | 12,19 |
| ML (GRU) | 1,8   |


