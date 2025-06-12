# Stock_Price_Prediction

This project aims to predict stock prices using historical data with a deep learning model — **Long Short-Term Memory (LSTM)** networks. It showcases how LSTM can be applied to time-series financial data for forecasting purposes.

## Project Overview

Predicting stock prices is a challenging task due to market volatility and external influences. This project focuses on analyzing historical stock prices of **Tesla Inc. (TSLA)** and predicting future closing prices using a Recurrent Neural Network (RNN) architecture — specifically, LSTM layers.

## Technologies Used

- Python  
- Pandas, NumPy  
- Matplotlib  
- scikit-learn  
- TensorFlow / Keras  
- yfinance  

## Dataset

- The dataset is automatically retrieved using the `yfinance` Python module.  
- **Stock Ticker**: TSLA (Tesla Inc.)  
- Includes historical `Open`, `High`, `Low`, `Close`, `Adj Close`, and `Volume` values.  

## Model Architecture

- **Data Preprocessing**:  
  - Normalized using `MinMaxScaler`  
  - Created sequences of 60 previous days to predict the next day's price  
- **LSTM Network**:  
  - 2 LSTM layers with 50 units each  
  - 1 Dense output layer  
- **Loss Function**: Mean Squared Error (MSE)  
- **Optimizer**: Adam  

## Results

- The LSTM model captures stock price trends effectively.  
- Visual plots show predicted vs actual values.  
- The model performs well in identifying directional changes, though exact short-term values may slightly vary.  

## Output
![image](https://github.com/user-attachments/assets/7880174d-fdba-44c7-baab-7c5825eb2e39)

## Key Learnings

- Using LSTM for time-series prediction  
- Preparing sequential data for RNN input  
- Retrieving and processing financial data using `yfinance`  
- Plotting and interpreting model predictions  

