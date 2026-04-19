# 🤖 RL-Based EMA Crypto Trading Bot

An automated cryptocurrency trading bot that leverages Reinforcement Learning (RL) and Exponential Moving Average (EMA) strategies to make intelligent trading decisions. Built within a Jupyter/Google Colab Notebook, it draws market data using the **Alpaca API** and executes simulated trades in a **Paper Trading Account** (Alpaca/Delta).

## 🌟 Features
- **Reinforcement Learning Core:** Uses an RL agent (trained to maximize profit) to decide the optimal trading actions (Buy, Sell, Hold) based on state representation.
- **EMA Crossover Strategy:** Integrates Exponential Moving Averages into the state environment to capture momentum and market trends.
- **Live Data Fetching:** Connects to the Alpaca API to pull real-time or historical cryptocurrency data.
- **Risk-Free Execution:** Fully integrated with paper trading so the bot can trade automatically using simulated funds without risking real capital.

## 🛠 Prerequisites 

To run this project, make sure you have the following setup:
1. **Google Colab** or a local **Jupyter Notebook** environment.
2. **Alpaca Developer Account:** You will need API keys for paper trading. 
   - [Sign up for an Alpaca Account](https://app.alpaca.markets/signup)
   - Generate your `API_KEY` and `SECRET_KEY` in the paper trading dashboard.

### Required Python Libraries
If running locally, you will need to ensure the following are installed (most are pre-installed on Colab):
- `alpaca-trade-api` (or `alpaca-py`)
- `pandas`
- `numpy`
- `torch` (for the Reinforcement Learning model)
- `matplotlib` (for performance visualizations)

## 🚀 How to Run the Bot

This project is designed to be executed linearly in a notebook environment. No complex terminal commands or Docker setups are required.

1. **Clone the Repository / Open the File:**
   Upload the `.ipynb` notebook file to Google Colab or open it locally in Jupyter Notebook.

2. **Set your API Keys:**
   Locate the configuration cell in the notebook and insert your personal API keys:
   ```python
   API_KEY = "your_alpaca_api_key_here"
   API_SECRET = "your_alpaca_secret_key_here"
   BASE_URL = "https://paper-api.alpaca.markets" 
