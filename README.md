# Load-Forecasting-with-ARIMA 

## INTRODUCTION
ARIMA Model: The ARIMA model is a time series forecasting technique that combines
autoregression (AR), differencing (I), and moving averages (MA). The three components of the
model work together to capture different patterns and trends in time series data.

1. AutoRegressive (AR): This component accounts for the relationship between the current value
and its past values. It assumes that the future value of a variable depends on its previous values.
2. Integrated (I): This component involves differencing the time series data to make it stationary.
Stationarity is important for ARIMA models as they work better with time series data that
exhibit constant statistical properties over time.
3. Moving Average (MA): This component considers the relationship between the current value
and a residual error from a moving average of past values. It helps capture short-term
fluctuations in the time series data.

The ARIMA process is written with the notation ARIMA(p,d,q), where (p) denotes the number
of autoregressive orders in the model. Autoregressive orders specify the previous values from the
series which are used to predict current values; difference (d) specifies the order of differencing
applied to the series before estimating models; and moving average (q) specifies how deviations
from the series mean for previous values are used to predict current values.


## METHODOLOGY
This methodology combines the strengths of the ARIMA model for time series forecasting
with the ability of clustering algorithms to identify groups of similar data points. Here's a
breakdown of the key steps:

1. Data Preprocessing:
Collect historical load data: This could be hourly, daily, or even monthly data
depending on your desired forecast horizon.
Cleaning and filtering: Check for missing values, outliers, and inconsistencies in the
data.
2. Clustering:
Cluster historical data: Group similar load patterns together based on their features.
Identify the cluster of the forecasting day: This cluster will be used for training the
ARIMA model.
3. ARIMA Model Training:
Select the appropriate ARIMA order (p,d,q): Analyze the autocorrelation and partial
autocorrelation plots to identify the order of the autoregressive (p), integrated (d), and
moving average (q) components.
Train the ARIMA model: Use the historical data within the forecasting day's cluster to train
the ARIMA model.
4. Validate the model:
Evaluate the performance of the model using metrics like Mean Absolute Error (MAE) and
Root Mean Squared Error (RMSE).
5. Forecasting:
Input the features of the forecasting day into the trained ARIMA model.
Obtain the forecast load value for the desired horizon.
Repeat steps 3 and 4 for each forecasting period.


## OUTPUT
1. The comparison between
forecasting result of ARIMA
model and proposed method in
comparison to actual data on
July 27, 2018.
2. The graph of proposed model
is more closer to graph of
actual value as compared to
ARIMA model.
3. This shows that the proposed
model has more accuracy as
compared to ARIMA model.

<img width="443" alt="Screenshot 2024-01-03 at 1 03 16 PM" src="https://github.com/divykantsharma/Load-Forecasting-with-ARIMA/assets/89973756/569ca596-dcdb-47f0-85fa-c5aeccda17d5">
