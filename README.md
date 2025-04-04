# S&P 500 Trading Strategy with RSI

## Project Overview
This repository contains a Python implementation for backtesting a trading strategy based on the Relative Strength Index (RSI) technical indicator using historical S&P 500 stock data. The project demonstrates the complete workflow from data acquisition to strategy evaluation.

## Key Features
- Historical S&P 500 stock price data retrieval and preprocessing
- Calculation of technical indicators (RSI)
- Implementation of a simple RSI-based trading strategy
- Comprehensive backtesting framework with performance metrics
- Evaluation using financial metrics (CAGR, Sharpe Ratio) and classification metrics

## Data Creation and Preparation
The project begins with creating a robust dataset:
1. Downloads historical price data for S&P 500 companies
2. Filters out tickers with insufficient historical data
3. Calculates price returns over different time horizons
4. Computes technical indicators like RSI

## Trading Strategy
The implemented strategy is based on RSI values:
- When RSI < 65: Go long (buy the stock)
- Otherwise: No position (stay out of the market)

This simple rule-based approach demonstrates how technical indicators can be used to make trading decisions.

## Backtesting Framework
The backtesting process includes:
1. Applying the trading strategy to historical data
2. Calculating position performance metrics
3. Comparing strategy returns against a benchmark (equally-weighted S&P 500)
4. Visualizing cumulative and calendar returns

## Performance Evaluation
The strategy is evaluated using:
- Financial metrics:
  - Compound Annual Growth Rate (CAGR)
  - Sharpe Ratio (risk-adjusted returns)
  - Cumulative and calendar year returns
- Classification metrics:
  - Accuracy: Correctness of price movement predictions
  - Precision: Reliability of positive predictions
  - Recall: Ability to identify actual positive movements

## Dependencies
- pandas, numpy, matplotlib
- yfinance (for data retrieval)
- scikit-learn (for evaluation metrics)

## Getting Started
1. Clone this repository
2. Install required packages: `pip install pandas numpy matplotlib yfinance scikit-learn`
3. Run the main notebook to replicate the analysis

## Further Development
This project can be extended by:
- Testing alternative technical indicators
- Implementing more sophisticated trading rules
- Incorporating machine learning models for prediction
- Adding transaction costs and slippage to the backtesting framework
- Optimizing strategy parameters
