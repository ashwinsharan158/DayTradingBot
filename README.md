# DayTradingBot
# Comparative Study on Efficient Approaches for Creating a Stock Trading Bot

## Introduction
In this study, we perform a comparative analysis to find an efficient approach for creating a bot that can buy, sell, and hold a stable stock. We utilize a Blotter, PPO reinforcement learning model, and a PPO model with a transformer encoding by conducting an ablation study.

## Libraries and Dataset

### Yahoo Finance API
Python library for accessing market data from Yahoo Finance.

### Provided Dataset
Historical trade data in `trades_EQUITIES.csv`.

## Setup and Environment

1. **Python and Relevant Libraries**
   - Used Python along with libraries such as PyTorch or TensorFlow for the implementation.
   
2. **Installation**
   - Installed the Yahoo Finance library using:
     ```sh
     pip install yfinance
     ```

## Data Preparation

1. **Load Dataset**
   - Loaded the `trades_EQUITIES.csv` dataset.

2. **Fetch Historical Market Data**
   - Used the Yahoo Finance API to fetch historical market data (e.g., stock prices, volumes) relevant to the trades in the dataset.
   
3. **Merge Data**
   - Merged the market data with the trade data to create a comprehensive dataset for model training.

## Model Implementation

1. **Transformer Model**
   - Implemented a transformer model using PyTorch or TensorFlow.
   
2. **Trade and Market Data Processing**
   - Used the Blotter, PPO reinforcement learning model, and PPO model with a transformer to process the trade and market data, aiming to generate trade recommendations.

## Fine-Tuning

- Fine-tuned the models on the provided dataset.
- Utilized the `optuna` library to fine-tune the parameters.

## Evaluation

### PPO Transformer Model
- **Balance:** 9,820,018.905
- **Shares Held:** 935.0
- **Total Shares Traded:** 935.0
- **Total Portfolio Value:** 10,000,997.504999999
- **Cumulative Reward:** -2.2282120732540283
- **Average Reward:** -0.1856843394378357

### PPO Model
- **Balance:** 9,655,819.284999968
- **Shares Held:** 1793.0
- **Total Shares Traded:** 1793.0
- **Total Portfolio Value:** 10,003,750.934999969
- **Cumulative Reward:** -11,589.792624079966
- **Average Reward:** -10.185684

### Trading Blotter
- **Cumulative Reward:** -12,231.775689639546
- **Average Reward:** -0.3688269113990938
- **Total Portfolio Value:** 10,031,043.267704722

