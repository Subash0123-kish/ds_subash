# Data Science Analysis Project

## Overview
This project analyzes the correlation between cryptocurrency trading behavior and market sentiment using the Fear & Greed Index. It combines historical trading data with sentiment indicators to provide insights into market psychology and trading patterns.

## Project Structure

```
ds_subash/
├── notebook_1.ipynb              # Main Jupyter notebook with analysis
├── csv_files/                    # Data files
│   ├── historical_data.csv       # Trading transaction history
│   └── fear_greed_index.csv      # Market sentiment data
├── outputs/                      # Generated outputs and visualizations
└── README.md                     # This file
```

## Data Files

### historical_data.csv
Contains detailed cryptocurrency trading transaction records with the following columns:
- **Account**: Wallet address
- **Coin**: Token/cryptocurrency identifier
- **Execution Price**: Price at which the trade was executed
- **Size Tokens**: Volume of tokens traded
- **Size USD**: USD value of the trade
- **Side**: BUY or SELL
- **Timestamp IST**: Trade execution time (Indian Standard Time)
- **Start Position**: Initial position size
- **Direction**: Trade direction (Buy/Sell)
- **Closed PnL**: Closed profit and loss
- **Transaction Hash**: Blockchain transaction hash
- **Order ID**: Unique order identifier
- **Crossed**: Whether the order was crossed
- **Fee**: Transaction fee
- **Trade ID**: Unique trade identifier

### fear_greed_index.csv
Market sentiment data indexed from historical records:
- **timestamp**: Unix timestamp
- **value**: Numerical sentiment score (0-100)
- **classification**: Sentiment label (Fear, Extreme Fear, Greed, Extreme Greed, etc.)
- **date**: Calendar date

## Analysis Contents

The notebook performs the following analyses:

1. **Data Loading & Exploration**: Imports and examines both datasets
2. **Data Cleaning**: Normalizes column names and formats timestamps
3. **Time Series Processing**: Converts timestamps to datetime format for time-based analysis
4. **Exploratory Data Analysis**: Statistics and distributions
5. **Sentiment-Trading Correlation**: Analyzes relationship between market sentiment and trading patterns
6. **Visualizations**: Generates charts and plots for insights

## Requirements

### Python Libraries
- pandas
- numpy
- matplotlib
- seaborn

### Environment
- Python 3.x
- Jupyter Notebook

## Usage

1. Ensure all CSV files are in the `csv_files/` directory
2. Open `notebook_1.ipynb` in Jupyter Notebook
3. Run the cells sequentially to perform the analysis
4. Generated outputs will be saved to the `outputs/` directory

## Key Insights

This analysis explores:
- How market sentiment (Fear & Greed Index) correlates with trading volume and behavior
- Trading patterns during different market sentiment periods
- Statistical relationships between sentiment indicators and transaction data

## Notes

- The historical data uses Indian Standard Time (IST) timestamps
- The Fear & Greed Index values range from 0-100, where:
  - 0-25: Extreme Fear
  - 25-45: Fear
  - 45-55: Neutral
  - 55-75: Greed
  - 75-100: Extreme Greed
- All price values are in USD

## Output

Analysis results, visualizations, and processed data are saved to the `outputs/` folder.
