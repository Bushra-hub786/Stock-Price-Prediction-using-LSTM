📈 Stock Price Prediction using LSTM
📌 Overview

This project predicts future stock prices based on historical data using a Long Short-Term Memory (LSTM) neural network. LSTM models are highly effective for time series forecasting as they can capture long-term dependencies in sequential data.

🎯 Objective

To forecast stock prices for Apple Inc. (AAPL) using deep learning techniques, enabling better decision-making for traders and analysts.

📂 Dataset

Source: Yahoo Finance via yfinance Python library

Timeframe: 2010-01-01 to 2024-12-31

Features Used: Open, High, Low, Close, Adj Close, Volume

Target Variable: Close price

🔄 Workflow

Data Collection – Downloaded historical AAPL stock prices using yfinance.

Data Preprocessing

Normalized closing prices using MinMaxScaler.

Created sequences of past 60 days to predict the next day's closing price.

Model Building – Implemented a stacked LSTM model with dropout layers to prevent overfitting.

Training & Testing – Trained on 80% data, tested on 20% data.

Evaluation & Visualization – Compared actual prices vs predicted prices using line charts.

🧠 Model Architecture

Layer 1: LSTM with 50 units + Dropout (0.2)

Layer 2: LSTM with 50 units + Dropout (0.2)

Output Layer: Dense (1 unit for predicted price)

Loss Function: Mean Squared Error (MSE)

Optimizer: Adam

📊 Results

Predicted price trend closely follows the actual market price.

Visualization:

🛠 Tech Stack

Languages: Python

Libraries:

yfinance

numpy, pandas

matplotlib, seaborn

scikit-learn

tensorflow.keras

🚀 How to Run
# Install dependencies
pip install yfinance pandas numpy matplotlib scikit-learn tensorflow

# Run the script
python stock_prediction.py

💡 Business Use Case

Helps traders make data-driven decisions.

Can be adapted for real-time market prediction.

Useful for risk assessment and portfolio optimization.
