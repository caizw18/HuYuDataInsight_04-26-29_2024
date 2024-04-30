# HuYuDataInsight_04-26-29_2024
This is the workload for our company HuYuDataInsight LLC from Apr 26, 2024 to Apr 29, 2024.

We model the stock price of Apple (AAPL). The data file is AAPL2.csv:
1. We identify if there is a drift or a trend in the log return. 
2. We identify if there is any seasonality in the log return. 
3. We remove any drift/trend/seasonality identified in Questions 1 and 2 above, from the log return, and 
obtain the residual.
4. For the residual, we fit the best ARIMA-model using the BIC criterion.
5. For the residual above, we fit the best ARIMA-GARCH model using the BIC criterion.
6. We build the best model for the log closing price directly, and use one-day ahead forecast to predict the 
closing price of March 25, 2022. We also report the corresponding 95% prediction interval. The fun fact is 
that the true closing price for that day was $174.72.

We model the stock price of Apple (AAPL) and QQQ jointly. The data files are AAPL2.csv and QQQ2.csv:
1. We build an ARDL(1,1) model using the log closing price of QQQ to predict the log closing price of AAPL.
2. We convert this ARDL(1,1) model above into an error correction model (ECM).
3. We build a bivariate VAR(1) model using the log closing price of AAPL and QQQ as the two variables. 
4. We use your VAR(1) model to perform the one-day ahead forecast for the closing price of AAPL and QQQ 
on March 25, 2022. The fun fact is that the true closing price on that day for AAPL and QQQ was $174.72,
and $359.35 respectively.
5. We compare the forecast results for AAPL above and make comments.
