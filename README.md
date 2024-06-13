# time-series-modelling-python
Analyzing and forecasting retail sales using time series modeling techniques using Kaggles store sales dataset

## Description
This project focuses on analyzing and forecasting retail sales data using time series modeling techniques. The primary goal is to develop a model that accurately predicts sales patterns by leveraging seasonal, cyclic, and serial dependence features.

## Project Overview
The analysis begins with the creation of a baseline model that utilizes seasonal and cyclic features derived from Fourier series and calendar effects. The performance of the baseline model is then evaluated using Root Mean Squared Logarithmic Error (RMSLE). The baseline model demonstrated a moderate ability to capture the overall sales pattern but fell short in predictive accuracy, as evidenced by high RMSLE values on both the training and validation sets (0.88620 and 1.68564, respectively).

To improve the model, we investigated the deseasonalized sales data for serial dependence. The analysis involved plotting the seven-day moving average, which showed a pattern similar to the deseasonalized sales data. This similarity suggested that cyclicality was a prominent characteristic driving the sales patterns, rather than just seasonal trends.

Further analysis using lag plots and partial autocorrelation plots provided deeper insights. The lag plots indicated strong linear relationships between the deseasonalized sales and its past values up to lag 8, with lags 1 and 2 showing the highest correlations. The partial autocorrelation plot confirmed that lags 1 and 8 were statistically significant, implying that these lags should be considered as features to capture the serial dependence effectively.

Based on these findings, we introduced a single lag feature (lag 1) into the model. The inclusion of this lag feature led to a substantial improvement in model performance, highlighting the significance of serial dependence in this time series data. The improved model achieved significantly lower RMSLE values: 0.31966 on the training set and 0.39642 on the validation set.

## Key Features
- **Baseline Model:** Uses seasonal and cyclic features to capture sales patterns. Achieved RMSLE values of 0.88620 (training) and 1.68564 (validation).
- **Improved Model:** Incorporates significant lag features identified through serial dependence analysis. Achieved RMSLE values of 0.31966 (training) and 0.39642 (validation).
- **Visualization:** Includes plots for moving averages, lag plots, and partial autocorrelation to provide insights into the data.

## Results
The improved model demonstrates a significant reduction in RMSLE, indicating better predictive performance compared to the baseline model. The RMSLE for the improved model is reduced to 0.31966 on the training set and 0.39642 on the validation set, highlighting the effectiveness of incorporating lag features to capture serial dependence in the sales data.
