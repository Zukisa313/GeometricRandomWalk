# Geometric Random Walk Simulation for Stock Prices

## Overview

This repository contains a Python script in a Jupyter Notebook that models stock price movements using a **Geometric Random Walk (GRW)**. The simulation is based on historical stock data for Apple Inc. (AAPL) fetched using the `yfinance` library.

The primary goal is to use the statistical properties (mean and standard deviation of log returns) from the first half of a given historical dataset to forecast the price movements for the second half. This is achieved through a Monte Carlo simulation of multiple GRW paths.

## Concepts Demonstrated

* **Geometric Random Walk (GRW)**: A stochastic process often used in financial modeling, where the logarithmic returns of the asset price are assumed to follow a normal distribution. The price at the next time step is the current price multiplied by an exponential factor involving a drift (mean) and a random shock (volatility). * **Logarithmic Returns**: Used to normalize the price series and is a key component in financial time series analysis.
* **Monte Carlo Simulation**: A computational technique that uses repeated random sampling to obtain numerical results. In this case, we simulate thousands of possible future price paths.
* **Parameter Estimation**: The drift ($\mu$) and volatility ($\sigma$) for the GRW model are estimated from a historical "training" period (the first half of the data).
* **Financial Data Analysis**: The script demonstrates fetching, processing, and analyzing real-world stock market data using Python libraries.

## Repository Contents

* `Geometric_Random_Walk.ipynb`: The Jupyter Notebook containing the Python code, visualizations, and detailed explanations of each step.
* `README.md`: This file.

## Requirements

To run the notebook, you'll need the following Python libraries:
* `yfinance`: For fetching stock market data.
* `numpy`: For numerical operations.
* `matplotlib`: For plotting the results.

You can install them using pip:
```bash
pip install yfinance numpy matplotlib
