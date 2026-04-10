# Stock-Price-Forecasting-Project-Using-Hybrid-ARIMA-LSTM-and-Sentiment-Analysis
improve daily stock price predictions by combining historical price data and financial news sentiment.
Project Overview:
The goal of this project was to forecast stock prices by combining historical stock data with financial news sentiment. The approach integrates traditional time series models with modern deep learning techniques, augmented by sentiment signals from news headlines.


ARIMA was used to capture linear trends in stock prices.

LSTM, a deep learning model, captured non-linear temporal patterns.

News sentiment scores were extracted using NLP techniques (VADER and TextBlob) and incorporated into predictions to account for market reactions.

as a Hybrid Forecast, ARIMA and LSTM predictions were combined using weighted averaging based on model performance, with sentiment signals further adjusting the forecast.

Results:

The hybrid approach improved prediction accuracy compared to individual models. The performance metrics were RMSE and MAPE.

Visual dashboards were created to clearly communicate predicted vs. actual stock movements.

Impact:
This project demonstrates the integration of quantitative models with unstructured data (news sentiment) to improve financial forecasting. The workflow can be adapted for other financial instruments or applied to real-time prediction pipelines for investment and risk management decisions.

#Interpretation of Results:
<img width="1507" height="751" alt="download" src="https://github.com/user-attachments/assets/74a9b3d3-c6fd-4ec5-8a05-5d3e31bc4638" />



in the last plot that we have blue line for training data, red line for validation set, and yellow line for hybrid model of LSTM ans ARIMA+ sentiment adjustment), the predicted values closely follow the validation set trends, capturing both upward and downward movements. This indicates that the hybrid model effectively learned the underlying price patterns and market behavior.
also in results using RMSE and MAPE, RMSE with the value of 307.80, shows that on average, the predicted price deviates from the actual price by roughly 308 points, which is relatively small given that DJIA values are in the range of 16,000–18,000.

This indicates high predictive accuracy for daily price forecasting.and MAPE with 1.56% is very low for stock market prediction, demonstrating that the hybrid model produces predictions very close to the real prices.
Overall, the hybrid approach combining ARIMA, LSTM, and sentiment analysis successfully captures both linear and non-linear patterns, as well as market sentiment effects.
 Low RMSE and MAPE indicate the model is reliable and suitable for short-term stock forecasting or decision support.

The alignment of predicted and actual values in the plot confirms the model’s robustness across the validation period.
This level of accuracy is strong, especially in financial time series forecasting where volatility is high.


This project implements a multi-stage ensemble pipeline designed to overcome the limitations of single-model forecasting. By decomposing stock price series into linear and non-linear components, the framework leverages ARIMA for structural trend capturing and LSTM for residual pattern recognition
