# Times-Series-Analyses
In this repository a generic time series is analyzed in depth.

Initially the TS is analyzed graphically in order to understand its trend and possible patterns.

Later we study the **stationarity** of the time series through two statistical tests. The first test used is the Augmented Dickey-Fuller test which confirms the hypothesis that the TS is stationary. The KPSS test also confirmed the stationarity hypothesis.

It follows that the time series is **stationary** and does not require differentiation.

## Forecast
We analyzed three different approaches to forecast a time series:
- ARIMA (and SARIMA),
- UCM,
- Machine Learning.

In particolar for the ML approaches we explored different architectures: vanilla LSTM, stacked LSTM, bidirectional LSTM and GRU. We discovered the last NN was the most efficient.

## Result

The performance were compared with the MAPE metric.
The ML approach was the most efficient for the task.
| Model    | MAPE  |
|----------|-------|
| Arima    | 10,68 |
| UCM      | 12,19 |
| ML (GRU) | 1,8   |


