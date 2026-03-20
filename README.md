#🔹 Overview:

SMA Crossover Trading Strategy Backtester is a comprehensive quantitative analysis tool that simulates and evaluates a simple moving average (SMA) crossover trading strategy on historical stock data. The application fetches real market data, simulated trades based on predefined rules, calculates performance metrics, and generates professional-grade visual reports. This tool allows traders and investors to quantitatively assess the viability of a momentum-based trading strategy before risking actual capital.


#🔹 Primary Objectives:

1. Strategy Validation: Evaluate whether a basic SMA crossover strategy generates alpha (excess returns) compared to a simple buy-and-hold approach

2. Risk Assessment: Quantify key risk metrics including maximum drawdown, Sharpe ratio, and win rate to understand the strategy's risk-adjusted performance

3. Parameter Optimization: Provide a flexible framework to test different SMA window combinations ( 50/200, 20/50) to identify optimal parameters for specific stocks

4. Educational Tool: Demonstrate core concepts of algorithmic trading including signal generation, position management, and performance measurement.

5. Decision Support: Enable informed investment decisions by providing quantitative evidence of strategy effectiveness across different market conditions.


#🔹 Detailed Library Functions:

1. yfinance (yf): Retrieves Open, High, Low, Close, volume data supports multi-stock downloads, handles automatic date parsing.
2. pandas(pd) : Handling missing data with dropna() , rolling window calculations for technical indicators, time series indexing for date-based operations.
3. numpy(np): Efficient array operations for signal generation, mathematical computations for performance metrics.
4. matplotlib : for plotting charts


#📈 Technical Architecture


##Data Flow:

Input Collection → User provides stock symbol, date range, capital, and SMA parameters

Data Acquisition → yfinance fetches historical price data

Indicator Calculation → pandas calculates short and long SMAs

Signal Generation → numpy creates binary signals based on crossover logic

Backtest Execution → Loop iterates through dates executing trades

Performance Analysis → Calculate returns, risk metrics, and statistics

Visualization → matplotlib generates comprehensive 4-panel dashboard

Export → Save results and charts for review


###SAMPLE OUTPUT METRICS :

Total Return:             +47.32%

Buy & Hold Return:        +32.15%

Annualised Return:        +15.67%

Sharpe Ratio:             1.43

Max Drawdown:            -12.45%

Total Trades:             24

Wins / Losses:            15 / 9

Win Rate:                 62.5%

Final Portfolio:          $14,732.00
