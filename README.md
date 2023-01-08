
# StockSentimentAnalysis

The StockSentimentAnalysis class is a tool for analyzing stock sentiment based on news headlines. It allows users to get the top N news articles for a given stock and date, calculate the sentiment of the articles, and get the stock return over the next 3 days. 

To use the class, you must create an instance with your API keys for newsapi.org and OpenAI. You also need to provide a list of stocks you wish to analyze, a start date, and the number of articles to return. 

Example:

ssa = StockSentimentAnalysis()

ssa.apiKey = 'YOUR_API_KEY'

ssa.openai_apiKey = 'YOUR_OPENAI_API_KEY'

ssa.stocks = ['AAPL', 'MSFT']

ssa.start_date = '2020-01-01'

ssa.end_date = '2020-05-01'

ssa.N = 10

This will create an instance of the StockSentimentAnalysis class with the given parameters. 

To get the sentiment dataset, you can then call the get_stock_sentiment_dataset() method:

ssa.get_stock_sentiment_dataset()

This will return a dataset of stock sentiment data for the given stocks and date range. 

The get_sentiment_summary() method can then be used to get a summary of the sentiment data:

ssa.get_sentiment_summary()

Finally, the get_final_dataframe() method can be used to generate the final dataframe with stock ROI data:

ssa.get_final_dataframe()

This will return a dataframe with the sentiment summary and stock ROI data.