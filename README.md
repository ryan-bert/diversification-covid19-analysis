# Diversification Project

## Overview

This project analyzes the effectiveness of portfolio diversification during pre- and post-COVID-19 periods. Using data from various asset classes, the study investigates their correlation with the S&P 500, offering insights into their performance during different market conditions.

## Project Structure

```bash
.
├── Report.pdf
├── input
│   └── bloomberg_data.xlsx
├── main.py
└── output
    ├── AAPLUS_corr.png
    ├── Bond_corr.png
    ├── BrentCrude_corr.png
    ├── CombinedCorrelation_Post-COVID.png
    ├── CombinedCorrelation_Pre-COVID.png
    ├── Corn_corr.png
    ├── Gold_corr.png
    ├── Post-COVID_correlation_bar_graph.png
    ├── Pre-COVID_correlation_bar_graph.png
    ├── REIT_corr.png
    ├── TSLAUS_corr.png
    └── WMTUS_corr.png
```

## Files

- `Report.pdf`: Detailed report analyzing diversification effectiveness.
- `input/bloomberg_data.xlsx`: Input data file with asset prices.
- `main.py`: Script for data analysis and generating plots.
- `output/`: Directory with generated plots and tables.

## main.py

1. Reads and processes data from bloomberg_data.xlsx.
2. Calculates returns and splits data into pre and post-COVID-19 periods.
3. Computes conditional correlations of assets with the S&P 500.
4. Generates and saves correlation plots and tables.

### Key Parameters

- `INCREMENT`: Step size for return thresholds.
- `MIN_DATA_POINTS`: Minimum data points for correlations.
- `COVID_START_DATE`: Start date for the COVID-19 period.

## Install dependencies

```bash
pip install pandas numpy matplotlib openpyxl
```

## Author

Ryan Bertschinger
