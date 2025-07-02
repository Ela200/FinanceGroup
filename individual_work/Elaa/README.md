In this code I attempted to download and clean the dataset by importing it directly from Yahoo Finance (2010 to 2025 Q1) for 20 stocks.
I tried to do some EDA to visualize the evolution of the adjusted closing prices, the trading volume, and the rolling mean for each stock to better understand the trends and volatility.

As a first step, I implemented a baseline model using a simple moving average (window of 20 days), forecasting the next 5 days.
Then I implemented two tree-based models: XGBoost and LightGBM, for the same task of predicting the next 5 days of adjusted closing prices.

Finally, I compared the performance of all three models (Baseline vs XGBoost vs LightGBM) based on RMSE, and plotted the comparison across all stocks.
