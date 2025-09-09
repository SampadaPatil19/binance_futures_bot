# Simplified Binance Futures Trading Bot (USDT-M Testnet)

A command-line Python trading bot for Binance Futures Testnet (USDT-M) that supports **MARKET**, **LIMIT**, and **STOP** orders with both **BUY** and **SELL** sides.

---

## Features

- Place MARKET and LIMIT orders on Binance Futures Testnet.
- Input validation via CLI (argparse).
- Logging of API requests, responses, and errors (rotating log file).
- Structured and reusable Python code.

---

## Requirements

- Python 3.8+
- `requests`
- `python-dotenv` (for loading API keys from `.env`)

**Install dependencies:**
```bash
pip install -r requirements.txt
```
Setup
Register and activate a Binance Futures Testnet account.

Generate API Key and Secret.

Create a .env file in the project root:
env
```bash
BINANCE_API_KEY=your_testnet_api_key
BINANCE_API_SECRET=your_testnet_api_secret
```
Do not commit .env to GitHub.

Usage
Ping Testnet
Check if the testnet API is reachable:

```bash
python binance_futures_bot.py ping
```

Place Orders
Market Buy:

```bash
python binance_futures_bot.py place-order --symbol BTCUSDT --side BUY --type MARKET --quantity 0.0
```
