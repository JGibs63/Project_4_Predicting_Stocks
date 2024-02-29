# Project_4_Predicting_Stocks

Starting Out:
We started this Project wanting to predict the stock prices for stocks because it would offer an opportunity for us to delve into the exciting combination of  both finance and machine learning while potentially gaining insights into the dynamics of financial markets.

On Kaggle we found a Stock Dataset that the creator updated and had clean. We then used this data to help train our Machine so that it would learn a capture the trend that we needed it to so it would be able to accurately predict the outcome of the stock prices.

When we trained and created our Machine we also created a graph to see the data and keep track of the test data, training data, and actual data to know if it was successful.

We ran into issues after creating our machine and training it that we did not foresee happening, we had our model not really giving accurate readouts and would stagnant after a few readouts. After some research and conversations we reached the conclusion that the farther from the day you are the less accurate your prediction will become due to multiple factors like social media.

We started looking at all sorts of possible reasons and checking our R^2. After some research and a conversation with Ahmad we reached the conclusion that the farther from the current day. The less accurate your prediction will become due to multiple factors like social media.

Finding out this information led us to a very weird predicament that we didn't know the next steps to go for with our project. However, after some thinking Joshua came up with the idea, that because the data was being updated daily that we could take the data that the creator had added since we started the project and create a model that kept track and compared our models estimate for the next day and then giving it the actual so it could make the guess again. Leading to a better way for us to track if the data trend is being followed correctly.

We tried using the yfinance library. This library contained formulas to add moving averages, strength index, and a couple of ratios.This allowed us to basically add more features for the model to go off of, and enabled the machine to get a more accurate 1-day result for what would be today’s closing price

# Stock Technical Indicators for LSTM Stock Prediction Model
In a LSTM (Long Short-Term Memory) stock prediction model for Keras, incorporating relevant technical indicators can enhance the model's ability to capture patterns and trends in stock price data. The three commonly used technical indicators used in our final model include the following: moving average, relative strength index (RSI), and OHLC (Open, High, Low, Close) Ratios.

1. Moving Average (MA)
Definition: Moving averages are calculated by averaging a specific number of past data points, typically closing prices, over a defined period. This smoothed average is used to identify trends by filtering out short-term fluctuations.
Usage in LSTM Model: Adding moving averages of different time periods (e.g., 50-day, 200-day) as features can help the LSTM model capture trend information and identify potential reversal points.
2. Relative Strength Index (RSI)
Definition: The Relative Strength Index (RSI) is a momentum oscillator that measures the speed and change of price movements. It ranges from 0 to 100 and is typically used to identify overbought or oversold conditions in a stock.
Usage in LSTM Model: RSI can be included as a feature in the LSTM model to detect potential price reversals or confirm trends. Extreme RSI values may indicate that a stock is overbought or oversold, suggesting potential buying or selling opportunities.
3. OHLC Ratios (Open, High, Low, Close)
Definition: OHLC ratios are calculated based on the relationship between the open, high, low, and close prices of a stock within a specific period. These ratios provide insights into the price movement and volatility of the stock.
Usage in LSTM Model: OHLC ratios such as the daily price range (high-low), daily price change (close-open), or the ratio of close to open prices can be used as features in the LSTM model to capture price dynamics and volatility patterns.

# Incorporating Technical Indicators into LSTM Model
Feature Engineering: Before training the LSTM model, preprocess the historical stock price data to compute the selected technical indicators.

Normalization: Scale the feature values to a common range to facilitate model convergence and improve performance.

Model Training: Include the computed technical indicators along with other relevant features as input to the LSTM model for training.

Evaluation: Evaluate the model's performance using appropriate evaluation metrics and validate its predictive accuracy on a separate test dataset.

By incorporating these technical indicators into the LSTM stock prediction model, you can improve its ability to analyze historical price data and make informed predictions about future price movements. Experiment with different combinations of indicators and model architectures to optimize performance and enhance predictive accuracy.

Conclusion:
In the end we tried many different libraries and used a lot of resources and research to look into the problems that we were having. We know that our Machine does not give a 100% readout but it does give a fairly good estimate and we think that if we had more access to more features we could make our estimate more and more accurate for each upcoming day.

Contributors: 
Joshua Gibson (JGibs63)
Andrew Clifft (DarkWolf776)
Morgan Foge (Moisasleep)
Jesse Brents (JBrents100)

Works Cited:
Data: 
- https://www.kaggle.com/datasets/andrewmvd/sp-500-stocks
Reference Material:
- https://data-flair.training/blogs/stock-price-prediction-machine-learning-project-in-python/amp/
- https://theaiquant.medium.com/forecasting-stock-returns-with-deep-learning-a-technical-approach-caccee231051
- https://www.investopedia.com/

AI Help at times from ChatGPT. :)
