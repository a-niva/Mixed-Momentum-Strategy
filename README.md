# Trading Strategy Backtesting Framework

This repository provides a robust framework for backtesting trading strategies, specifically focusing on momentum-based approaches. It allows traders, analysts, and developers to download market data, preprocess it, calculate technical indicators, and evaluate strategy performance across different time intervals.
![image](https://github.com/user-attachments/assets/7bedbaa6-061b-41c7-8137-e8597d20495a)

## Features

- **Market Data Download**: Retrieves historical market data for hundreds of global tickers using Yahoo Finance.
- **Technical Indicator Calculation**: Computes key indicators such as RSI, stochastic oscillators, moving averages (SMA, EMA), mean reversion channels, and momentum metrics.
- **Backtesting Functionality**: Enables strategy testing with custom parameters, including transaction costs, random starting points, and various data intervals.
- **Automated Data Cleaning**: Filters out datasets with insufficient data to ensure reliability.
- **Interval-Based Analysis**: Supports multiple intervals (e.g., 1h, 1d, 15m) for granular backtesting.

## Folder Structure

- `datasets/`: Raw market data downloaded for different intervals.
- `datasets_enough_data/`: Filtered datasets that meet the minimum data quality thresholds.
- `datasets_technicals/`: Preprocessed datasets with computed technical indicators.

## How to Use

### Prerequisites

- Python 3.10 or higher
- Install required dependencies:
  ```bash
  pip install -r requirements.txt

## Configuration

    Set Tickers: Define the list of tickers you want to analyze in the script (e.g., CAC40, S&P500, custom lists).
    Adjust Parameters: Configure settings such as intervals, random backtest iterations, and transaction costs in the script.
    Run the Framework: Execute the main script to download data, process it, and run backtests.

## Execution

Run the main script:

python main.py

## Results

    Filtered datasets will be saved in datasets_enough_data/.
    Datasets with technical indicators will be saved in datasets_technicals/.
    Backtest summaries and results will be printed in the console or saved to a log file.

## Customization

    Add Indicators: Extend the indicator computation section in the script to include custom formulas.
    Integrate with Other APIs: Replace or enhance the Yahoo Finance integration with APIs such as Tiingo or Stooq.
    Enhance Backtesting Logic: Modify the backtesting logic to test advanced strategies.

## Key Dependencies

    yfinance: For market data retrieval.
    pandas: For data manipulation.
    matplotlib: For visualizations.
    tqdm: For progress tracking.
    joblib: For parallel processing.

## Example Outputs

    Data Visualization: Automatically generates plots for indicator distributions and file length thresholds.
    Filtered Tickers: Logs removed tickers due to insufficient data, ensuring data quality.

## Contributing

Feel free to contribute by opening issues or submitting pull requests. Suggestions for new features, optimizations, and bug fixes are welcome!

## License

This project is licensed under the MIT License. See the LICENSE file for details.

Happy backtesting! 🚀
