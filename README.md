# Binance Futures Trading Bot

## Features
- Place **Market Orders**
- Place **Limit Orders**
- Advanced Orders: **OCO**, **TWAP**
- Input validation & error handling
- Structured logging to `bot.log`

## Setup
1. Clone the repo
2. Install dependencies:
   ```bash
   pip install python-binance
   ```
3. Export API credentials as environment variables:
   ```bash
   export BINANCE_API_KEY="your_key"
   export BINANCE_API_SECRET="your_secret"
   ```
4. Run orders:
   - Market: `python src/market_orders.py BTCUSDT BUY 0.01`
   - Limit: `python src/limit_orders.py BTCUSDT SELL 0.01 27000`
   - OCO: `python src/advanced/oco.py BTCUSDT SELL 0.01 28000 27000 26950`
   - TWAP: `python src/advanced/twap.py BTCUSDT BUY 0.05 5 10`
