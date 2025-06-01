

# Binance Futures Trading Bot

A modular, plug-and-play Python trading bot for Binance USD-M Futures, featuring technical indicators, multi-source sentiment analysis (Reddit & Telegram), trailing stops, risk management, and backtesting capabilities — all wrapped in a Flask-based web UI.

---

## Features

* **Modular Architecture**: Clean separation of concerns for easy maintenance and scalability.
* **Technical Indicators**: RSI, MACD, ADX, ATR, EMA, and more.
* **Sentiment Analysis**: Integrate Reddit and Telegram sentiment to refine trading signals.
* **Trailing Stop Loss**: Dynamic trailing stops for better risk control.
* **Risk Management**: Position sizing, max drawdown, daily loss limits, and circuit breakers.
* **Backtesting Framework**: Validate strategies on historical Binance futures data.
* **Flask UI**: User-friendly interface for live monitoring, strategy control, and reporting.
* **Logging & Performance Metrics**: Trade journaling, win rate, Sharpe ratio, and real-time dashboards.
* **Robust Error Handling**: Retry logic and circuit breakers for API stability.

---

## Repo Structure

```
binance_futures_bot/
├── config/                 # Configuration and credentials
├── core/                   # Main bot logic, risk management, performance
├── data/                   # Data fetching and sentiment analysis modules
├── indicators/             # Technical indicator calculations
├── execution/              # Binance API interaction and order management
├── backtesting/            # Backtesting framework and strategies
├── ui/                     # Flask web app for UI
├── utils/                  # Helper utilities and common functions
├── tests/                  # Unit tests for components
└── main.py                 # Entry point to run the bot
```

---

## Installation

1. Clone the repo:

```bash
git clone https://github.com/yourusername/binance_futures_bot.git
cd binance_futures_bot
```

2. Create and activate a virtual environment:

```bash
python3 -m venv venv
source venv/bin/activate    # Linux/macOS
venv\Scripts\activate       # Windows
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Configure your API keys and settings:

* Add your Binance API keys to `config/credentials.py`.
* Adjust trading parameters in `config/settings.py`.

---

## Usage

### Running the Bot

```bash
python main.py
```

This starts the bot with live data fetching, signal generation, order execution, and risk management.

### Running the Flask UI

```bash
python ui/app.py
```

Access the dashboard at [http://localhost:5000](http://localhost:5000) to monitor performance, view trade history, and control strategies.

### Backtesting

Run backtests with your preferred strategy and historical data:

```bash
python backtesting/backtest.py
```

---

## Configuration

Modify `config/settings.py` to customize:

* Risk parameters (e.g., risk percent, max drawdown)
* Indicator thresholds
* Sentiment weighting
* API endpoints and timeframes
* Logging preferences

---

## Contributing

Contributions are welcome! Please open issues or submit pull requests for improvements or bug fixes.

---

## Disclaimer

This bot is for educational and research purposes only. Trading cryptocurrencies involves risk and you should trade responsibly. The authors are not responsible for any losses incurred.

---

## Contact

For questions or collaborations, reach out at \[[your.email@example.com](mailto:your.email@example.com)].

---

Would you like me to add this README file to the repo directly?
