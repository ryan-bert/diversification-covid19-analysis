# Is Diversification Effective in the Face of a Black Swan Event? A Case Study of COVID-19

## Overview

This project examines the effectiveness of portfolio diversification before and after the onset of the COVID-19 pandemic. By analyzing historical data across various asset classes—including equities, commodities, property, and fixed income—the study investigates how these assets correlate with the S&P 500 under different market conditions. The goal is to understand the role of diversification during significant market upheavals and provide insights for investors and portfolio managers on risk management and asset allocation.

## Motivation

In an era marked by unforeseen events and global disruptions, traditional investment strategies like diversification are put to the test. The COVID-19 pandemic serves as a prime example of a black swan event that challenged conventional financial wisdom. This project aims to dissect the role of diversification during such periods, helping investors make informed decisions in the face of uncertainty.

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

## Usage

1. **Clone the Repository:**
```bash
git clone <repository-url>
cd diversification-project
```

2. **Install Dependencies:**
```bash
pip install -r requirements.txt
```

3. **Run the Analysis:**
```bash
python main.py
```

## Analysis Methodology

The analysis involves the following steps:

1. Data Preparation: Reads and processes the data from bloomberg_data.xlsx, calculating weekly returns and handling missing values.
2. Data Segmentation: Splits the data into pre-COVID and post-COVID periods, using March 6, 2020, as the cutoff date.
3. Conditional Correlation Calculation: Computes the conditional correlations of each asset with the S&P 500 across various return thresholds. This involves calculating correlations for subsets of data where the S&P 500 returns are above or below certain thresholds.
4. Visualization: Generates line graphs showing how the correlation between each asset and the S&P 500 changes across different return thresholds in both periods. Also, creates bar graphs comparing average upside and downside correlations for each asset.
5. Ranking Assets: Ranks the assets based on the difference in their correlations during positive and negative S&P 500 returns to identify the most effective diversification tools.

## Key Findings

- Gold and Bonds: Post-COVID, gold and bonds stood out as effective diversification assets, showing low or negative correlations with the S&P 500 during market downturns. Gold, in particular, capitalized on market upswings and exhibited resilience during declines.
- Commodities: Brent Crude Oil and Corn had varying correlations but were generally less effective for diversification during the pandemic. Their correlation profiles remained relatively consistent, suggesting limited protective benefits during extreme market conditions.
- Property and Equities: Real estate (via REITs) and equities like Walmart showed significant changes in correlation profiles before and after COVID-19, emphasizing the need for dynamic portfolio management. REITs, for instance, exhibited high correlations with the S&P 500 post-COVID, reducing their diversification effectiveness.
- Tech Stocks: Apple and Tesla, representing the tech sector, exhibited high correlations with the S&P 500, offering less diversification benefit during market downturns. Their volatility could enhance a portfolio’s beta, requiring careful consideration in risk management strategies.


## Author

Ryan Bertschinger
