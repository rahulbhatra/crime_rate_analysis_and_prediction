# Crime Rate Analysis and Prediction

## Models Used:
* Convolutional Neural Network
  * Forecasts monthly crime counts as a univariate time series using a 1D CNN over sliding windows (look-back → next month prediction)
* Recurrent Neural Network
  * Same forecasting setup as above, but with an RNN (e.g., LSTM/GRU) on the single monthly series.
* Multi Layer Perceptron
  * Uses an MLP (fully connected network) on tabular/time-window features to predict future crime counts (regression) or levels.
* Prophet
  * Fits Meta Prophet to the monthly crime series to model trend/seasonality/holidays and generate forward forecasts with confidence intervals.
* Random Forest
  * Tree-based baseline on engineered features (lags, rolling stats, calendar flags) for predicting future counts; includes feature importance and error metrics.
