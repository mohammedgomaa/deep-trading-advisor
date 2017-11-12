# Deep Trading Advisor

An attempt to implement a trading system from scratch based only on deep learning approaches.

## Project Overview

The project comprises of several chunks of functionality that need to be build. These are:
- Initial data collection: Since the Yahoo and Google API's have restricted the amount of historical data that can be requested, initial datasets are needed for a fixed number of stocks
- Monthly data collection: Request and append new data monthly
- Deep learning to predict future stock prices using Keras
- Hyperparameter optimization
- Backtesting using zipline
- Deep Trading Advisor dashboard using Dash and Plotly

## Problem Definition

We will consider our problem as a:
- Regression problem: forecast the close price or return for the next day
- Binary classification problem: the price will go up [1; 0] or down [0; 1]

The initial MVP will consist of regression models only. We want to predict t+1 value based on N previous days information. For example, having close prices from past 30 days on the market we want to predict, what price will be tomorrow, on the 31st day.

### Deep learning: Regression

The following types of neural networks are considered:
- MLP
- CNN
- RNN (+LSTM)

## TODO
- [All] Go through Keras scripts and gather relevant literature
- [Chef] Select initial portfolio of stocks and collect initial datasets
- [Timo] Build zipline pipeline for backtesting
- [Simon] Setup server and including monthly data collection cronjobs
- [Job] Cherry-pick the most relevant deep learning stock prediction scripts. Adjust to new Keras functionality including port to Python 3

## Miscellaneous
- Use minute data instead of daily? (Deep Learning profits from more data)
