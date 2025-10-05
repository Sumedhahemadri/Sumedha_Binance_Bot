Overview

This project is a CLI-based trading bot for Binance USDT-M Futures.
It supports multiple order types, input validation, and structured logging.
All orders are executed in simulation mode for safe testing.

Features

Core Orders

Market Orders – place_market_order(symbol, side, quantity)
Limit Orders – place_limit_order(symbol, side, quantity, price)
Validates inputs: symbol, side, quantity, price
Logs all actions to bot.log

Advanced Orders

Stop-Limit Orders – place_stop_limit(symbol, side, quantity, stop_price, limit_price)
OCO Orders – place_oco(symbol, side, quantity, take_profit, stop_loss)
TWAP Orders – twap_order(symbol, side, total_qty, parts, interval_sec)
Grid Orders – create_grid(symbol, base_price, lower, upper, levels, qty_per_level)
All advanced orders are simulated and logged.


Installation


Clone the repo or extract ZIP:
git clone <your_repo_url>
cd sumedha-binance-bot
