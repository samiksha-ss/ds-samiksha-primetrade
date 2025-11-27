# Project Overview

This project analyzes how trader behavior changes based on overall market sentiment.
The analysis combines two datasets:

*A daily Fear and Greed Index dataset.*

*A trade-level dataset containing execution details, PnL, timestamps and account activity.*

The goal is to understand whether traders behave differently during fearful markets compared to greedy markets and to identify patterns that could be useful for developing better trading strategies in Web3 environments.

### Repository Structure
ds_samiksha/
│
├── notebook_1.ipynb              # Main Colab notebook containing all code
├── csv_files/
│   ├── trader_raw.csv
│   ├── fear_greed_raw.csv
│   ├── trader_daily_aggregated.csv
│   └── merged_daily.csv
│
├── outputs/
│   ├── volume_vs_sentiment.png
│   ├── pnl_vs_sentiment.png
│   ├── winrate_vs_sentiment.png
│   └── unique_traders_vs_sentiment.png
│
├── ds_report.pdf                 # Final written report
└── README.md                     # This file

### How to Run the Notebook
1. Open notebook_1.ipynb directly in Google Colab.
2. Upload the two datasets when prompted:
    Trader dataset from Kaggle
    Fear and Greed Index CSV
3. Run all cells from top to bottom.
4. The notebook will:
    Clean and process both datasets
    Aggregate trader data by day
    Merge it with the sentiment dataset
    Produce and save all visualizations
    Export all cleaned CSV files into the csv_files directory
    All plots will automatically be saved in the outputs folder.

**Key Steps Performed in the Analysis**
Parsing timestamps and cleaning the raw datasets
Creating derived metrics such as trade value and win rate
Aggregating trade data into daily summaries
Merging trader activity with the Fear and Greed Index
Producing visualizations to compare behavior across sentiment categories
Interpreting patterns in volume, profitability and participation

### Main Findings
Trading activity increases significantly on days labeled as Greed.
Profitability often decreases during Greed periods, suggesting emotional or impulsive trading.
Win rates are higher during Fear and Neutral sentiment.
The number of active traders also increases during Greed phases.
A detailed explanation of these observations is included in the final report.

### Requirements
The analysis was performed in Google Colab and uses standard Python libraries:

pandas
numpy
seaborn
matplotlib
No additional setup is required.

Google Collab Link: https://colab.research.google.com/drive/1jjNHUZxZQdMIG7CC9zAT5aj52zY1nJ7Y?usp=sharing

Author
Samiksha Sharma
Data Science Candidate
