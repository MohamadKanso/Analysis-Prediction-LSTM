# Stock Market Analysis and Prediction Using LSTM

This project focuses on analysing historical stock market data + predicting future stock prices using LSTM) models a type of recurrent neural network optimised for time series predictions.

## Features
- Fetches real-time stock data for companies like (AAPL),  (GOOG),  (MSFT) and  (AMZN) using the `yfinance` library.
- Preprocesses data by scaling and creating input sequences for training.
- Trains an LSTM model to predict future stock closing prices.
- Visualises actual vs. predicted stock prices to evaluate the model's accuracy.

## Project Workflow
1. **Data Collection**:
   - Stock data is fetched from Yahoo Finance.
   - Columns include `Close`, `Open`, `High`, `Low` and `Volume`.

2. **Preprocessing**:
   - Data is scaled using `MinMaxScaler` for better LSTM performance.

3. **Model Architecture**:
   - Two LSTM layers followed by dense layers.
   - Optimised using the Adam optimiser with a mean squared error (MSE) loss function.

4. **Training**:
   - Model is trained on the historical data of a single stock (e.g **AAPL**) with adjustable parameters like batch size and epochs.

5. **Prediction and Visualization**:
   - Predictions are made on unseen test data.
   - Actual vs. predicted prices are visualised for easy interpretation.

## Results
- Outputs a graph showing:
  - **Training data** -- Historical stock prices used for training.
  - **Validation data** -- Actual prices compared against predicted prices.
  - **Predicted data** -- Forecasted stock prices.

## Dependencies
- <img src="https://pandas.pydata.org/static/img/pandas.svg" alt="pandas" width="80"/>  

- <img src="https://upload.wikimedia.org/wikipedia/commons/3/31/NumPy_logo_2020.svg" alt="numpy" width="80"/>  

- <img src="https://github.com/ranaroussi/yfinance/raw/main/resources/logo/yfinance_128.png" alt="yfinance" width="80"/>  

- <img src="https://matplotlib.org/stable/_static/images/logo2.svg" alt="matplotlib" width="80"/>  

- <img src="https://scikit-learn.org/stable/_static/scikit-learn-logo-small.png" alt="scikit-learn" width="80"/>  

- <img src="https://upload.wikimedia.org/wikipedia/commons/a/ab/TensorFlow_logo.svg" alt="tensorflow" width="80"/>  

## Next Steps
- Include additional technical indicators like moving averages or RSI.
- Expand the dataset to include multiple features for better accuracy.
- Test the model with other stocks or indices.

## Disclaimer
This project is for educational purposes only and should not be used for financial or investment advice.
