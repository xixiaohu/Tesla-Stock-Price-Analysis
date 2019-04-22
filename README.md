# Tesla-Stock-Price-Analysis
An interactive dashboard is created for this analysis using Dash. It generates an online dashboard with 3 tabs. Stock prices and news are web scrapped from Yahoo Finance.

Tab 1: Stock Price Analysis contains
Live-updated graph: According to the time running the script, different results will be generated. If it runs in Saturday, Sunday and Monday morning before stock market open time, this graph will show the stock price fluctuantions in Friday. For other days of a week, if the program runs before open time, the graph will show yesterday's prices. And if it runs after close time, graph will show today's prices. Only if the program runs during the stock market open, the graph will lively updated to display most recent stock price. In this situation, graph will first scrapp and display data from open time of today and up to now. Then, it will be lively updated during running the script.
Histoical Price graph: I provided 4 dropdowns of indicators: close price, moving average, high/low prices and volume. Also, 4 radio items of periods are provided: 1 month, 6 months, 1 year, 3 years. User could see the trends of indicators in different periods through this graph.

Tab 2: Stock News Analysis contains:
Lis of News: A sorted list of news is displayed in this tab. It sorted by tfidf of the key word "Tesla" in its headline and summaries. The title of each news is a hyperlink directing to the news website. A wordcloud picture is displayed with a graph showing sentiment analysis of news.

Tab 3: Stock Price Prediction contains:
Model Performances: 3 SVR models are built and model performances are displayed. Models are trained by last 30 days data. According to the performance, user could choose one model to predict next 5 days price.
Price Prediction: Based on the model chose by the user, prices of next 5 days are plotted.

