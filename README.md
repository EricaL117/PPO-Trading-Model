# PPO Trading Strategy Project

A reinforcement learning project that trains a PPO (Proximal Policy Optimization) agent to trade stocks using historical price data, implemented with Stable-Baselines3 and Gym AnyTrading.


## Table of Contents
- [Overview](#overview)
- [Repository-Structure](#repository-structure)
- [Running-This-Project](#running-this-project)


## Overview
This project applies the PPO reinforcement learning algorithm to stock trading using daily historical prices.  
The notebook includes:

- Loading and preprocessing price data  
- Creating a trading environment using Gym AnyTrading (`stocks-v0`)  
- Training a PPO agent on historical price movements  
- Simulating buy/sell/hold decisions  
- Tracking balance, shares, and trade history  
- Visualizing model actions and balance over time  

The model starts with an initial cash balance and executes actions predicted by the PPO policy to maximize returns.


## Repository Structure
```bash
├── data/
│   └── Ticker.csv           
├── Code.ipynb                
├── requirements.txt         
├── .gitignore           
└── README.md
```

## Running This Project
1. Clone the repository
2. Install dependencies
```bash
pip install -r requirements.txt
```
3. Load the dataset from the data folder
```bash
data = pd.read_csv("data/Ticker.csv", parse_dates=True, index_col="Date")
```
