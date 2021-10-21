# SecondCapstone
Wrangling data for a stock prediction model.
Data retrieved from polygon.io. Each archive contains a subset of end of day data for
Open, High, Low, Close, Daily Volume and Symbol going back to the year 2000.
This is the data that will be used to predict the returns over time.

Current thinking is that a supervised model(possibly linear regression) that utilizes simple moving averages and cross overs as well as volume may be used here.
The data will be augmnented from the same source with implied volatility based on the underlying Options Chains and may use some underlying fundamentals such as P/e ratio. Some open questions are listed below

# Open Questions
#=================
1. Can we use a sliding window of length (~ 250 trading days in a year)
2. Is the relative infrequency of positive data points ie a sliding window that indicates a 1000% (x10) increase in the closing price of the security 
   a factor in this model? Basically 90%+ of the data should be negative outcomes.
3. Is classification a better model?
4. Is there a way to get sentiment data on each of these stocks to augment this model?

