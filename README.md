# NetflixStockPricePrediction

- Generated Netflix stock dataset from Yahoo finance, which contains stock data for the past ten years (5082 rows, and 7
columns); the “open” column represents the opening price for the stock at that given “date”, and the “close” column is
the closing price for that day. The “High” column represents the highest price reached that day, and similarly, the “Low”
column represents the lowest price. The rest are ”closing” prices, and ”adjusted closing” prices; For simplicity, only one
variable i.e. the “open” price is used for analysis.
- Performed a train-test split of 80-20, where the features contain prices appended from the last 75 days, and the price for
the next day is chosen as the dependent variable.
- Implemented an LSTM architecture, with mean-squared-error is set as the loss function, and the rmsprop optimizer to
find the optimal weights. )
- A Root mean squared error of 33.97 is achieved, which is ideal in this case because as we know that stock price value
depends on multiple variables such as a change in top management, seasonal inflation rates, etc for which data is hard to
collect.
- Python libraries used: Keras, Pandas, Numpy, and Matplotlib.
