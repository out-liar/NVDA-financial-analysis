# NVDA financial analysis
Basic analysis of stocks and some financial ratios resulting in a CAPM comparison
<p>This project uses Anaconda, NumPy, Pandas DataReader to show:<br>
Portfolios and returns<br>
Volitilty and Risk<br>
Average True Range<br>
Risk and Return<br>
Risk as standard deviation<br>
Sharpe Ratio<br>
Monte Carlo Simulation<br>
Portfolio Optimisation<br>
Correlation of assets<br>
Risk and coherence<br>
Linear regression vs correlation<br>
True Random distribution vs correlated<br>
Visulaisation of linear regression<br>
Market Beta of the S&P500<br>
Capital Wealth pricing model (CAPM)<br>
Beta and CAPM calculations<br>
Expected return on investment</p>

# First, historical stock prices data is extracted from Yahoo! Finance in CSV file format. 
# This will be an analysis on which silicon chip manufacturer to buy, starting with NVIDIA Corp
# The data will be downloaded from the historical data tab on google finance.
# $TSM Taiwan Semiconductor Manufacturing Co. Ltd.
# $INTC Intel Corp.
# $AMD Advanced Micro Devices Ltd.
# $QCOM Qualcomm Inc.
# $AVGO Broadcom Inc.
# $MU Micron Technology Inc.
# $NVDA NVIDIA Corp.
# $AMAT Applied MAterials, Inc.
# $ASX ASE Technology Holding Co. Ltd.
# Secondly,the data is parsed and indexed.

# Tchniques: reading data from CSV files, understanding data types, set dexes, parse dates, use index with
# loc, use indexing with iloc.

import pandas as pd
data = pd.read_csv("NVDA.csv", index_col=0, parse_dates=True)
# Formatting the data:
# Use index_col to remove the automatic indexing and instead use the dates as the index.
# USe parse_dates to convert the date column from an object data type to datetime.
ata.head()
