# Raise The Stakes 

## Team Members
- **Chinmay Agarwal** - 23BCE0715  
- **Veeksha Anne** - 24BCE0628  
- **Mahalakshmi Manikandan** - 24BEE0093  

---

## Problem Statement
Investing in the stock market is risky due to its unpredictable nature. Our project leverages Machine Learning to assist users in making better stock decisions by analyzing the last 10 minutes of market data.

---

## Goal
Help investors and stock market enthusiasts make **smarter, more informed trading decisions** using real-time ML predictions.

---


### 1. **LSTM**
- **LSTM** for short-term trend analysis predictions:
    - RaiseTheStakes_LSTM: Using LSTM for price prediction:
        - For the dataset :0941.HKHKD_Candlestick_1_s_BID_16.06.2025-16.06.2025.csv
        - Which can be downloaded from https://www.dukascopy.com/trading-tools/widgets/quotes/historical_data_feed
        - ![image](https://github.com/user-attachments/assets/6615a922-c1f8-4202-b06c-e8bad2296c5d)

    - LSTM2: Adding droupout layer in LSTM & training on a bigger dataset
        - ![image](https://github.com/user-attachments/assets/5104f22d-aa6a-4bbc-9430-ed9c05f9f5e7)
        - Test.csv for testing with the RaiseTheStakes.keras


### 2. **Reinforcement Learning(DQN) + LSTM hybrid**
- For the dataset :0941.HKHKD_Candlestick_1_s_BID_16.06.2025-16.06.2025.csv
- Model acts as an agent that:
  - **-1** = Short (predicts price fall)
  - **0** = Hold
  - **1** = Long (predicts price rise)
- Agent receives rewards based on prediction accuracy.
- ![image](https://github.com/user-attachments/assets/ecf2f027-c95e-4eba-923b-7cb329e72c98)


### 3. **Multi Head Axial Attention**
  - CNN
  - RNN
  - GRU
  - Multi head Attention
  - Axial attention -Unlike lstm this converts the Data to single dimensional format(not actually but traverses the data in 1-D format) which helps to grab the long range dependencies
  - Dataset - FI-2010 dataset-https://etsin.fairdata.fi/dataset/73eb48d7-4dbc-4a10-a52a-da745b47a649
        - This dataset has 144 features(eg Tick level data,Spread,Cumulative Volume)
  - ![image](https://github.com/user-attachments/assets/5050febb-0b68-4080-b42a-3e1b53d7cd1a)
  - ![image](https://github.com/user-attachments/assets/49e7f2d3-cbd1-4af0-a1fb-e1bcb2fd70e3)

---

## 🔍 Similar Projects
- [pskrunner14/trading-bot](https://github.com/pskrunner14/trading-bot)

## Papers Used
- https://www.cis.upenn.edu/~mkearns/papers/KearnsNevmyvakaHFTRiskBooks.pdf
---
