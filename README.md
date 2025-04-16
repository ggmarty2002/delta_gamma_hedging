# Option Pricing and Hedging Strategies

This project implements various option pricing models and hedging strategies using the Black-Scholes framework. The project explores delta hedging, implied volatility calculation, and portfolio replication for European call options.

## Overview

This project is structured as a series of exercises (TD3) related to options pricing and hedging:

1. **Basic Delta Hedging**: Implementation of a simple delta hedging strategy for a European call option
2. **Delta-Gamma Hedging**: Enhanced hedging using a second option to control for gamma risk
3. **Implied Volatility Calculation**: Extraction of market implied volatilities using Newton-Raphson and Bisection methods
4. **Dynamic Hedging with Market IV**: Implementation of delta hedging using market-implied volatility
5. **Advanced Hedging with Volatility Risk**: Implementation of a hedging strategy that accounts for changes in implied volatility

## Requirements

- Python 3.x
- Libraries:
  - pandas
  - numpy
  - scipy
  - matplotlib
  - datetime

## Data

The project uses data from 'Données TD3.xlsx' which contains:
- Daily stock prices
- Option prices for different strike prices (6.0 and 6.5)
- Trading dates

## Key Components

### Black-Scholes Model

The project implements the Black-Scholes formula for European call options, calculating:
- Option prices
- Delta (for hedging)
- Gamma (for second-order risk)
- Vega (for volatility sensitivity)

### Implied Volatility Calculation

Two methods are implemented for extracting implied volatility from market prices:
- Newton-Raphson method (faster convergence)
- Bisection method (more stable)

### Hedging Strategies

1. **Delta Hedging**: Dynamically adjusting stock position based on option delta
2. **Delta-Gamma Hedging**: Using two options to hedge against both price changes and convexity
3. **Volatility-Aware Hedging**: Accounting for changes in implied volatility when constructing portfolios

## Usage

1. Load the Jupyter notebook in a compatible environment
2. Ensure 'Données TD3.xlsx' is in the same directory
3. Run the cells sequentially to see the results of each hedging strategy

## Visualization

The project includes visualizations of:
- Option prices vs. portfolio values for different hedging strategies
- Implied volatilities across time for different strike prices
- Option price sensitivity to volatility

## Results

The notebook demonstrates how different hedging strategies perform in replicating option payoffs, with visualizations comparing the theoretical option prices with the hedged portfolio values.
