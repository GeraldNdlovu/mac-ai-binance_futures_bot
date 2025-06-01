---

````markdown
# Binance Futures Trading Bot 🐍📈

A smart algorithmic trading bot for **BTC/USDT Binance USD-M Futures**, combining **technical indicators (RSI, MACD, ADX, ATR)** with **Twitter sentiment analysis** for smarter entry/exit decisions. Built with risk management in mind and designed to run on the **Binance Testnet** for safe testing.

---

## 🚀 Features

- 📊 **Indicators Used**: RSI, MACD, ADX (trend strength), ATR (volatility)
- 🧠 **Sentiment Analysis**: Real-time Twitter sentiment via VADER NLP
- 🧮 **Risk Management**: Dynamic position sizing (1% risk rule), bracket orders (SL/TP)
- 🔄 **Automated Trading Loop**: Monitors the market and places trades every cycle
- 🧪 **Runs on Binance Testnet** for safe and cost-free testing
- 🪵 **Logging**: Logs all activities in `trading_bot.log`

---

## 🛠️ Requirements

- Python 3.8+
- Binance API key and secret (testnet)
- Twitter developer credentials
- `.env` file for API keys
- Dependencies (see below)

---

## 📦 Installation

```bash
git clone https://github.com/yourusername/binance-futures-bot.git
cd binance-futures-bot
pip install -r requirements.txt
````

---

## 🔐 Environment Variables

Create a `.env` file in the root directory and add the following:

```env
BINANCE_API_KEY=your_binance_api_key
BINANCE_API_SECRET=your_binance_api_secret

TWITTER_API_KEY=your_twitter_api_key
TWITTER_API_SECRET=your_twitter_api_secret
TWITTER_ACCESS_TOKEN=your_access_token
TWITTER_ACCESS_TOKEN_SECRET=your_access_token_secret
```

---

## 📈 How It Works

1. Fetches latest market data (`1h` OHLCV) from Binance.
2. Calculates key indicators (RSI, MACD, ADX, ATR).
3. Fetches and scores Twitter sentiment.
4. Generates buy/sell signals only when:

   * Technical indicators align
   * Sentiment is supportive
   * ADX confirms strong trend
5. Dynamically sizes the position and places bracket orders:

   * Market entry
   * Stop-loss
   * Take-profit

---

## 🔁 Running the Bot

```bash
python3 main.py
```

> ⚠️ The bot runs on an infinite loop with a configurable sleep interval. It trades only when all signal conditions are met.

---

## 📋 To-Do / Coming Soon

* [ ] Flask web dashboard
* [ ] Telegram/Reddit sentiment integration
* [ ] Live PnL and equity tracking
* [ ] Backtesting module
* [ ] Trailing stop-loss support

---

## 🧠 Disclaimer

This project is for educational and testing purposes only. **Use at your own risk.** Trading cryptocurrencies involves significant financial risk. Never trade real funds without proper testing and due diligence.

---

## 👨‍💻 Author

**Gerald Nqobile Ndlovu**
🧠 Quant enthusiast | 🐍 Python dev | 📍 Philippines
Feel free to reach out or contribute!

---

## ⭐️ Star this repo if you find it helpful!

```

---

Let me know your GitHub username so I can plug it into the repo URL. Want a `requirements.txt` file next?
```
