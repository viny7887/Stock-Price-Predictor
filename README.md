# Stock-Price-Predictor using LSTM

This project uses Long Short-Term Memory (LSTM), a type of Recurrent Neural Network (RNN), to predict stock prices based on historical data. The model is trained using historical stock prices, and the primary goal is to predict the next day's closing price. This project uses RELIANCE.NS as the stock ticker, but the model can be easily modified to work with other stocks.

Features
Data Downloading: The project fetches historical stock price data using the yfinance API.
Data Preprocessing: The data is preprocessed by normalizing it and splitting it into sequences to feed into the LSTM model.
LSTM Model: The stock price prediction model is built using LSTM layers to predict the future stock price based on the previous days' data.
Evaluation: The model's performance is evaluated using the Root Mean Squared Error (RMSE), and the results are visualized.
Installation
Prerequisites
Ensure you have Python 3.x installed and the following packages:

numpy
pandas
yfinance
sklearn
tensorflow
matplotlib
You can install these dependencies using pip:

View the Results
The code will display:

RMSE (Root Mean Squared Error): This metric measures the difference between the predicted and actual stock prices.
Prediction vs Actual Graph: A graph showing the actual vs. predicted stock prices.

Model Architecture
The LSTM model is built using Keras, and the architecture is as follows:

LSTM Layer 1: 50 units with dropout for regularization.
LSTM Layer 2: 50 units with dropout.
Dense Layer: 25 units.
Output Layer: 1 unit to predict the next day's closing price.
Evaluation
The model uses the Root Mean Squared Error (RMSE) to evaluate performance. Lower RMSE values indicate better model accuracy.

Conclusion
This project demonstrates how to use LSTM to predict stock prices, providing a basis for more advanced time-series forecasting models. You can further improve the model by using additional features like trading volume, high/low prices, or even external factors like market news.
