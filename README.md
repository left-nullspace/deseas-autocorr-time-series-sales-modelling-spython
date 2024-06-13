# time-series-modelling-python
Analyzing and forecasting retail sales using time series modeling techniques.

## Description
This project focuses on analyzing and forecasting retail sales data using time series modeling techniques. The primary goal is to develop a model that accurately predicts sales patterns by leveraging seasonal, cyclic, and serial dependence features.

## Project Overview
The analysis begins with the creation of a baseline model that utilizes seasonal and cyclic features derived from Fourier series and calendar effects. The performance of the baseline model is then evaluated using Root Mean Squared Logarithmic Error (RMSLE).

To improve the model, we investigate the serial dependence in the deseasonalized sales data by plotting the seven-day moving average, lag plots, and partial autocorrelation plots. These analyses help identify significant lag features that are incorporated into the improved model to enhance predictive accuracy.

## Key Features
- **Baseline Model:** Uses seasonal and cyclic features to capture sales patterns.
- **Improved Model:** Incorporates significant lag features identified through serial dependence analysis.
- **Visualization:** Includes plots for moving averages, lag plots, and partial autocorrelation to provide insights into the data.

## Results
The improved model demonstrates a significant reduction in RMSLE, indicating better predictive performance compared to the baseline model.
