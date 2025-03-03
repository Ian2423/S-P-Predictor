# S-P-Predictor
How does it work?

1. Get the Data: The code fetches historical S&P 500 data (like stock prices and trading volume) using the yfinance library.

2. Prepare the Data: It cleans up the data, adds a column for the next day's price, and creates a target column that indicates whether the price went up (1) or down (0).

3. Train the Model: A Random Forest Classifier is trained on the data to learn patterns.

4. Make Predictions: The model predicts whether the price will rise or fall the next day.

5. Check Accuracy: The model's predictions are tested on the last 100 days of data, and it achieves about 65% precision (meaning it’s correct 65% of the time when it predicts a price increase).
