# Crypto DCA Backtesting Tool

This repository explores potential improvements to dollar-cost averaging (DCA) strategies in cryptocurrency markets by analyzing how technical indicators and market sentiment affect Bitcoin price movements. Specifically, it investigates the relationship between MACD signals and the Fear & Greed Index to identify opportunities for optimizing long-term DCA accumulation strategies.

## Overview

The goal of this project is to backtest various DCA strategies with MACD and Fear & Greed Index integration to find potential edges that could improve returns over traditional DCA approaches.

## Tech Stack

- **Python 3.x** - Core programming language
- **Jupyter Lab** - Interactive notebooks for analysis and visualization
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Backtrader** - Backtesting framework for strategy evaluation
- **CCXT** - Cryptocurrency exchange integration for real market data
- **TA-Lib** - Technical analysis indicators (MACD, moving averages, etc.)

## Installation

### Prerequisites
- Python 3.8 or higher installed on your system
- Git

### Setup Steps

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/dca_backtest.git
   cd dca_backtest
   ```

2. **Create a virtual environment:**
   ```bash
   python -m venv backtest_env
   ```

3. **Activate the virtual environment:**
   
   **Windows:**
   ```bash
   backtest_env\Scripts\activate
   ```
   
   **macOS/Linux:**
   ```bash
   source backtest_env/bin/activate
   ```

4. **Install dependencies:**
   ```bash
   pip install jupyterlab pandas numpy backtrader ccxt ta-lib
   ```

   *Note: If `ta-lib` installation fails, you can use `pandas-ta` as an alternative.*

5. **Launch Jupyter Lab:**
   ```bash
   jupyter lab
   ```

## Project Structure

```
dca_backtest/
├── notebooks/          # Jupyter notebooks for analysis
├── data/              # Historical price data and indicators
├── strategies/        # Custom backtrading strategy files
├── results/           # Backtest results and visualizations
└── README.md          # This file
```

## Usage

1. Open Jupyter Lab (see Installation step 5)
2. Navigate to the notebooks folder and open an analysis notebook
3. Load historical Bitcoin data using CCXT
4. Define your DCA strategy with MACD and Fear & Greed Index parameters
5. Run the backtest using Backtrader
6. Analyze results and visualizations

## Key Metrics to Evaluate

- **Total Return** - Overall profit/loss from the strategy
- **Sharpe Ratio** - Risk-adjusted returns
- **Maximum Drawdown** - Largest peak-to-trough decline
- **Win Rate** - Percentage of profitable trades
- **MACD Signal Quality** - Effectiveness of MACD crossovers
- **Fear Index Correlation** - How Fear & Greed Index impacts entry points

## Contributing

Feel free to fork this project and submit pull requests with improvements, additional indicators, or optimizations.

## License

This project is open source and available under the MIT License.

## Disclaimer

This backtesting tool is for educational purposes only. Past performance does not guarantee future results. Always conduct your own research before making investment decisions. Cryptocurrency markets are highly volatile and risky.
