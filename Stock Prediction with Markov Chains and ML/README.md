# Stock Price Prediction Movements Using Markov Chains and Machine Learning


## Overview

This project demonstrates the use of **Markov Chains and Machine Learning** for **predicting stock price movements**. By analyzing historical stock data, we classify daily price movements into discrete states (Up, Down, Stable) and model the transitions between these states using a Markov Chain. Additionally, we train a machine learning model (logistic regression model) to predict stock price movements using daily returns


## Motivation

**Predicting stock prices is a challenging task due to the inherent stochastic nature of financial markets**. This project explores a hybrid approach, combining probabilistic Markov models with machine learning, to gain insights into the dynamics of stock price movements.

## Why using Markov chains?
Markov chains are useful in finance, for instance, Modeling Stock Prices: 
Markov chains are often used to model stock prices or financial instruments where future states (e.g., price changes) depend only on the present state and not on past states. The idea is to represent different possible price levels or returns as discrete states, and the Markov chain determines the probabilities of transitioning from one state to another.

For example, stock prices can be categorized into states like "Up", "Down", or "Stable". The Markov chain would calculate the probability of the price going from "Up" to "Down", or staying in "Stable", given the current state. **By using these probabilities, analysts can predict future price movements or simulate possible price scenarios, helping in risk management, option pricing, and decision-making**.




## Repository Structure

```plaintext
Stock Price Prediction Using Markov Chains and Machine Learning/
│
├── README.md                # Project description and instructions
│
├── data/                    # Folder for storing raw and processed data
│   ├── stock_data.csv       # Stock data downloaded by fetch_data.py and used for analysis and modeling
│   
├── scripts/                 # Folder for all Python scripts
│   ├── fetch_data.py        # Script to get and download stock data
│   ├── markov_model.py      # Script for Markov chain analysis
│   ├── ml_model.py          # Script to train the ML model
│   ├── visualize.py         # Script to visualize results
│
├── results/                 # Folder for results and outcomes
│   ├── figures/             # Visualizations (plots, graphs, etc.)
│   ├── reports/             # Analysis reports or summaries
```



## Features

  -  Download real-time stock data using Yahoo Finance with the yfinance library.
    
  -  Classify stock price movements into Up, Down, and Stable states.
    
  -  Construct a Markov Chain for modeling state transitions and predicting future states.
    
  -  Train a Logistic Regression model to predict stock price movements using daily returns.
    
  -  Evaluate and compare the performance of Markov Chains and Machine Learning predictions.

## How to Use

In the **scripts** folder:

  1- Run **fetch_data.py** to download stock data.
    
  2- Use **markov_model.py** to analyze states and build the transition matrix.
    
  3- Train a machine learning model using **ml_model.py**.
    
  4- Visualize results using **visualize.py**.
