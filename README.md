# Option Pricing and Hedging Strategies

This repository contains implementations of various option pricing models and hedging strategies as part of the Model Calibration course (TD3).

## Repository Contents

- **Données TD3.xlsx**: Excel file containing the market data (stock prices, option prices, etc.)
- **rules_hedging_project.pdf**: instructions for the assignment
- **notebook_hedging_project.ipynb**: Jupyter notebook containing the implementation of different hedging strategies and models

## Project Overview

This project explores financial derivatives modeling with focus on:

1. **Basic Delta Hedging** (Question 1)
   - Implementation of a dynamic delta hedging strategy for a European call option
   - Comparison of the hedged portfolio value with theoretical option price

2. **Delta-Gamma Hedging** (Question 2)
   - Use of two options to hedge both delta and gamma risk
   - Implementation of a more stable hedging strategy using a second option

3. **Implied Volatility Calculation** (Question 4)
   - Implementation of Newton-Raphson and Bisection methods to extract implied volatility
   - Comparison of implied volatilities across different strike prices

4. **Market Implied Volatility Hedging** (Question 5)
   - Implementation of delta hedging using market implied volatility instead of constant volatility

5. **Advanced Volatility-Sensitive Hedging** (Question 5+)
   - Extension of hedging to account for changes in implied volatility
   - Using multiple options to hedge against both price and volatility risks

## Data

The file `Données TD3.xlsx` contains:
- Daily stock prices
- Option prices at different strike prices (6.0 and 6.5)
- Trading dates
- All data necessary to implement the hedging strategies

## Requirements

The code requires the following Python libraries:
- pandas
- numpy
- scipy
- matplotlib
- datetime

## Results Visualization

The notebook includes multiple visualizations:
- Comparison between theoretical option prices and hedged portfolio values
- Evolution of implied volatility over time for different strike prices
- Sensitivity of option prices to volatility changes

## Mathematical Model

The project implements the Black-Scholes model for European call options:
- Call price calculation
- Delta and gamma computation for hedging
- Vega calculation for volatility sensitivity
- Implied volatility extraction from market prices
