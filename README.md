
Abstract:

This project explores stock price forecasting using both deep learning and statistical models. 
Historical stock data for Apple, Microsoft, and Google is retrieved using the yfinance library and preprocessed with exploratory data analysis (EDA) to prepare it for modeling.
Five recurrent neural network (RNN) architectures—Basic RNN, LSTM, GRU, Bi-directional LSTM, and a custom RNN model—are implemented to capture temporal dependencies in stock price trends. 
Additionally, statistical models such as ARMA and GARCH are applied to analyze stock volatility.
Model performance is evaluated using RMSE, MSE, and MAE metrics, providing a comprehensive comparison between neural and statistical approaches. 
The findings offer insights into model suitability for financial time series forecasting, helping refine predictive accuracy in stock market applications.

About Dataset:

The dataset used for this analysis includes historical stock data for Apple (AAPL), Microsoft (MSFT), and Google (GOOGL), spanning from November 1, 2008, to November 1, 2024.
The data was fetched using the yfinance library, which provides access to comprehensive historical market data, including stock prices, adjusted close prices, trading volume, and other essential metrics.
Each stock's dataset contains multiple features, such as the open, high, low, close, adjusted close prices, and volume for each trading day.
In total, each stock dataset comprises 3,774 rows, corresponding to daily trading data, and 6 columns representing the key financial indicators mentioned above. 
This extensive dataset provides a robust foundation for analyzing long-term trends and patterns in stock prices over a 16-year period. 
The large number of data points allows for a detailed analysis of price movements and market behaviors across different time frames, supporting insights into stock performance and volatility over the years.

Statistical Model Implementation:

ARMA Model: The Autoregressive Moving Average (ARMA) model is used for analyzing and forecasting stationary time series data by combining two components: the autoregressive (AR) part, which regresses the current value on its previous values, and the moving average (MA) part, which models the error term as a linear combination of past error terms. 
ARMA is effective for capturing short-term dependencies in a time series.
GARCH Model: The Generalized Autoregressive Conditional Heteroskedasticity (GARCH) model extends the ARMA approach by accounting for time-varying volatility, commonly observed in financial time series. GARCH captures conditional heteroskedasticity by modeling current volatility as a function of past variances and errors, making it valuable for assessing and forecasting volatility and risk in data prone to sudden fluctuations.

RNN Model Implementation:

RNNs are particularly well-suited for time series data like stock prices due to their ability to capture temporal dependencies. 
Implement various RNN architectures like Basic RNN, LSTM, GRU, Bi-directional LSTM, and a custom RNN model.
