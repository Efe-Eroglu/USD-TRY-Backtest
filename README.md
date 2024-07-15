# <p align="center"> Trading Strategy Analysis using Vectorbt</p>

This script performs a comprehensive analysis of different trading strategies using various technical indicators and optimizes the best entry and exit signals for trading the USD/TRY currency pair.


## Requirements

Make sure to install the required libraries before running the script

```bash
pip install yfinance vectorbt ta pandas numpy
```

## Overview
The script downloads historical data for the USD/TRY currency pair, calculates various technical indicators, and evaluates the performance of different trading strategies. It optimizes the strategies by testing different combinations of stop-loss and take-profit values.

## Script Breakdown


## 1. Data Download
The script starts by downloading historical data for the USD/TRY currency pair using the yfinance library.

```python
import yfinance as yf
import pandas as pd

symbol = 'USDTRY=X'
data = yf.download(symbol)
close = data['Close']
```

## 2.Moving Averages
The script calculates several moving averages (MA) with different window sizes.

## 3. Technical Indicators
Various technical indicators are calculated using the ta library:

* Relative Strength Index (RSI)
* Moving Average Convergence Divergence (MACD)
* Bollinger Bands
* Ichimoku Cloud
* Stochastic Oscillator
* Parabolic SAR

## 4. Entry and Exit Conditions
The script defines several entry and exit conditions based on the calculated technical indicators.

## 5. Strategy Optimization
The script tests different combinations of stop-loss and take-profit values to find the best performing strategy.


## Conclusion
This script helps in identifying the best trading strategy for the USD/TRY currency pair by testing various technical indicators and optimizing stop-loss and take-profit values. The final output provides detailed statistics of the best performing strategy.
