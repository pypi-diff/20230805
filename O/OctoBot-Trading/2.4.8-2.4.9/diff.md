# Comparing `tmp/OctoBot-Trading-2.4.8.tar.gz` & `tmp/OctoBot-Trading-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OctoBot-Trading-2.4.8.tar", last modified: Sat Jul  8 14:45:53 2023, max compression
+gzip compressed data, was "OctoBot-Trading-2.4.9.tar", last modified: Sun Jul 23 14:16:07 2023, max compression
```

## Comparing `OctoBot-Trading-2.4.8.tar` & `OctoBot-Trading-2.4.9.tar`

### file list

```diff
@@ -1,574 +1,576 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.260610 OctoBot-Trading-2.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)    33345 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.220610 OctoBot-Trading-2.4.8/OctoBot_Trading.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-08 14:45:53.000000 OctoBot-Trading-2.4.8/OctoBot_Trading.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24373 2023-07-08 14:45:53.000000 OctoBot-Trading-2.4.8/OctoBot_Trading.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 14:45:53.000000 OctoBot-Trading-2.4.8/OctoBot_Trading.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 14:45:53.000000 OctoBot-Trading-2.4.8/OctoBot_Trading.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-08 14:45:53.000000 OctoBot-Trading-2.4.8/OctoBot_Trading.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-08 14:45:53.000000 OctoBot-Trading-2.4.8/OctoBot_Trading.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-08 14:45:53.260610 OctoBot-Trading-2.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.220610 OctoBot-Trading-2.4.8/octobot_trading/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.220610 OctoBot-Trading-2.4.8/octobot_trading/api/
--rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/api/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/api/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/api/exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/api/modes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/api/orders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/api/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/api/positions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/api/profitability.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/api/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/api/symbol_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/api/trader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/api/trades.py
--rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.220610 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/
--rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.220610 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/contracts/contract_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/contracts/future_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/contracts/margin_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/exchange_symbol_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/exchange_symbols_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.220610 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/funding/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/funding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.224610 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/funding/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/funding/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/funding/channel/funding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/funding/channel/funding_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/funding/funding_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.224610 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/kline/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/kline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.224610 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/kline/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/kline/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/kline/channel/kline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/kline/channel/kline_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/kline/kline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.224610 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ohlcv/
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ohlcv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ohlcv/candles_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ohlcv/candles_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.224610 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ohlcv/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ohlcv/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ohlcv/channel/ohlcv.py
--rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.224610 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/order_book/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/order_book/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.224610 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/order_book/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/order_book/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/order_book/channel/order_book.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/order_book/channel/order_book_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/order_book/order_book_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.224610 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/prices/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/prices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.224610 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/prices/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/prices/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/prices/channel/price.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/prices/channel/prices_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/prices/price_events_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/prices/prices_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.224610 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/recent_trades/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/recent_trades/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.224610 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/recent_trades/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/recent_trades/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/recent_trades/channel/recent_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/recent_trades/recent_trades_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.224610 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ticker/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ticker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.224610 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ticker/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ticker/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ticker/channel/ticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ticker/channel/ticker_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ticker/ticker_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.228610 OctoBot-Trading-2.4.8/octobot_trading/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27517 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/abstract_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/abstract_websocket_exchange.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.228610 OctoBot-Trading-2.4.8/octobot_trading/exchanges/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/adapters/abstract_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.228610 OctoBot-Trading-2.4.8/octobot_trading/exchanges/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/config/backtesting_exchange_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/config/exchange_config_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.228610 OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.228610 OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/ccxt/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/ccxt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/ccxt/ccxt_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/ccxt/ccxt_client_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    36637 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/ccxt/ccxt_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    44886 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/ccxt/ccxt_websocket_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/ccxt/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/ccxt/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.228610 OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/simulator/exchange_simulator_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/simulator/exchange_simulator_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/exchange_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/exchange_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/exchange_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/exchange_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/exchange_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/exchange_websocket_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/exchanges.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.228610 OctoBot-Trading-2.4.8/octobot_trading/exchanges/implementations/
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/implementations/default_rest_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/implementations/default_websocket_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/implementations/exchange_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.228610 OctoBot-Trading-2.4.8/octobot_trading/exchanges/traders/
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/traders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42964 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/traders/trader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/traders/trader_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.228610 OctoBot-Trading-2.4.8/octobot_trading/exchanges/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45451 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/types/rest_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/types/websocket_exchange.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.228610 OctoBot-Trading-2.4.8/octobot_trading/exchanges/util/
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/util/exchange_market_status_fixer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/util/exchange_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/exchanges/util/websockets_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.232610 OctoBot-Trading-2.4.8/octobot_trading/modes/
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/modes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16571 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/modes/abstract_trading_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.232610 OctoBot-Trading-2.4.8/octobot_trading/modes/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/modes/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11155 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/modes/channel/abstract_mode_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)    23028 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/modes/channel/abstract_mode_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/modes/channel/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/modes/mode_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/modes/modes_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/modes/modes_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.232610 OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.232610 OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/basic_keywords/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/basic_keywords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/basic_keywords/account_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/basic_keywords/amount.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/basic_keywords/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/basic_keywords/run_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/basic_keywords/trading_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/basic_keywords/user_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25931 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/context_management.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.232610 OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/dsl/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/dsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/dsl/quantity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/dsl/values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.232610 OctoBot-Trading-2.4.8/octobot_trading/modes/scripted_trading_mode/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/modes/scripted_trading_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16335 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/modes/scripted_trading_mode/abstract_scripted_trading_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/octobot_channel_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.232610 OctoBot-Trading-2.4.8/octobot_trading/personal_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19668 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/exchange_personal_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.232610 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/
--rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.232610 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14382 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/channel/orders.py
--rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/channel/orders_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/channel/orders_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/decimal_order_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.232610 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/groups/group_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    41049 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/order.py
--rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/order_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/order_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/order_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    22239 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/order_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/orders_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/orders_storage_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.236610 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/states/
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/states/cancel_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/states/close_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/states/fill_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/states/open_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/states/order_state_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/states/pending_creation_chained_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/states/pending_creation_order_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.236610 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.236610 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/limit/
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/limit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/limit/buy_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/limit/limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/limit/sell_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/limit/stop_loss_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/limit/take_profit_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.236610 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/market/
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/market/buy_market_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/market/market_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/market/sell_market_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.236610 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/trailing/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/trailing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/unknown_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/unsupported_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.236610 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.236610 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/assets/future_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/assets/margin_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/assets/spot_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.236610 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/channel/balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/channel/balance_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.236610 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/history/
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/history/historical_asset_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    17826 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14495 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/portfolio_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/portfolio_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/portfolio_profitability.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/portfolio_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/portfolio_value_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/sub_portfolio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.236610 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/types/future_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/types/margin_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/types/spot_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)    17489 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/value_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.240610 OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.240610 OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/channel/positions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/channel/positions_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/channel/positions_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    39334 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/position_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/position_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/position_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/positions_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.240610 OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/states/
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/states/active_position_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/states/idle_position_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/states/liquidate_position_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/states/position_state_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.240610 OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/types/inverse_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/types/linear_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.240610 OctoBot-Trading-2.4.8/octobot_trading/personal_data/trades/
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/trades/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.240610 OctoBot-Trading-2.4.8/octobot_trading/personal_data/trades/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/trades/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/trades/channel/trades.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/trades/channel/trades_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/trades/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/trades/trade_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/trades/trade_pnl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/trades/trades_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/trades/trades_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.240610 OctoBot-Trading-2.4.8/octobot_trading/personal_data/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/transactions/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/transactions/transaction_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/transactions/transactions_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.240610 OctoBot-Trading-2.4.8/octobot_trading/personal_data/transactions/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/transactions/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/transactions/types/blockchain_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/transactions/types/fee_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/transactions/types/realised_pnl_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/personal_data/transactions/types/transfer_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.240610 OctoBot-Trading-2.4.8/octobot_trading/signals/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/signals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.240610 OctoBot-Trading-2.4.8/octobot_trading/signals/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/signals/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/signals/channel/remote_trading_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/signals/channel/remote_trading_signal_channel_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/signals/channel/signal_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/signals/signal_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/signals/trading_signal_bundle_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/signals/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.244610 OctoBot-Trading-2.4.8/octobot_trading/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/storage/abstract_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/storage/candles_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/storage/orders_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/storage/portfolio_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/storage/storage_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/storage/trades_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/storage/transactions_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/storage/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.244610 OctoBot-Trading-2.4.8/octobot_trading/supervisors/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/supervisors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/supervisors/abstract_portfolio_supervisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/supervisors/abstract_supervisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.244610 OctoBot-Trading-2.4.8/octobot_trading/util/
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/util/config_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/util/initializable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/util/initialization_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/util/simulator_updater_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.244610 OctoBot-Trading-2.4.8/octobot_trading/util/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/util/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/util/test_tools/exchanges_test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/util/test_tools/spot_rest_exchange_test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/octobot_trading/util/test_tools/websocket_test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 14:45:53.260610 OctoBot-Trading-2.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.220610 OctoBot-Trading-2.4.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.244610 OctoBot-Trading-2.4.8/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/api/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/api/test_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/api/test_modes.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/api/test_orders.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/api/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/api/test_profitability.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/api/test_symbol_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/api/test_trader.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/api/test_trades.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.244610 OctoBot-Trading-2.4.8/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.244610 OctoBot-Trading-2.4.8/tests/exchange_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchange_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.244610 OctoBot-Trading-2.4.8/tests/exchange_data/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchange_data/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchange_data/contracts/test_future_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchange_data/contracts/test_margin_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.244610 OctoBot-Trading-2.4.8/tests/exchange_data/funding/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchange_data/funding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchange_data/funding/test_funding_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.244610 OctoBot-Trading-2.4.8/tests/exchange_data/kline/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchange_data/kline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchange_data/kline/test_kline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.244610 OctoBot-Trading-2.4.8/tests/exchange_data/ohlcv/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchange_data/ohlcv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchange_data/ohlcv/test_candles_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchange_data/ohlcv/test_candles_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.244610 OctoBot-Trading-2.4.8/tests/exchange_data/order_book/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchange_data/order_book/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchange_data/order_book/test_order_book_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.244610 OctoBot-Trading-2.4.8/tests/exchange_data/prices/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchange_data/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchange_data/prices/test_price_events_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchange_data/prices/test_prices_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.244610 OctoBot-Trading-2.4.8/tests/exchange_data/recent_trades/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchange_data/recent_trades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchange_data/recent_trades/test_recent_trades_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchange_data/test_exchange_symbols_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.244610 OctoBot-Trading-2.4.8/tests/exchange_data/ticker/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchange_data/ticker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchange_data/ticker/test_ticker_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.248610 OctoBot-Trading-2.4.8/tests/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchanges/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.248610 OctoBot-Trading-2.4.8/tests/exchanges/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchanges/connectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.248610 OctoBot-Trading-2.4.8/tests/exchanges/connectors/ccxt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchanges/connectors/ccxt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchanges/connectors/ccxt/test_ccxt_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.248610 OctoBot-Trading-2.4.8/tests/exchanges/implementations/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchanges/implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchanges/implementations/test_default_rest_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchanges/implementations/test_default_websocket_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchanges/test_abstract_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchanges/test_abstract_websocket_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchanges/test_exchange_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchanges/test_exchange_config_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchanges/test_exchange_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchanges/test_exchange_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchanges/test_exchange_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchanges/test_exchanges.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.248610 OctoBot-Trading-2.4.8/tests/exchanges/traders/
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchanges/traders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50875 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchanges/traders/test_trader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.248610 OctoBot-Trading-2.4.8/tests/exchanges/types/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchanges/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchanges/types/test_websocket_exchange.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.248610 OctoBot-Trading-2.4.8/tests/exchanges/util/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchanges/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchanges/util/test_exchange_market_status_fixer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/exchanges/util/test_exchange_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.248610 OctoBot-Trading-2.4.8/tests/modes/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/modes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.248610 OctoBot-Trading-2.4.8/tests/modes/script_keywords/
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/modes/script_keywords/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.248610 OctoBot-Trading-2.4.8/tests/modes/script_keywords/basic_keywords/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/modes/script_keywords/basic_keywords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/modes/script_keywords/basic_keywords/test_account_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/modes/script_keywords/basic_keywords/test_amount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.248610 OctoBot-Trading-2.4.8/tests/modes/script_keywords/dsl/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/modes/script_keywords/dsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/modes/script_keywords/dsl/test_quantity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/modes/test_abstract_mode_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/modes/test_abstract_trading_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.248610 OctoBot-Trading-2.4.8/tests/personal_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.248610 OctoBot-Trading-2.4.8/tests/personal_data/orders/
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.248610 OctoBot-Trading-2.4.8/tests/personal_data/orders/groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19148 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/groups/test_balanced_take_profit_and_stop_order_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/groups/test_group_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/groups/test_one_cancels_the_other_order_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.252610 OctoBot-Trading-2.4.8/tests/personal_data/orders/states/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/states/test_cancel_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/states/test_close_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/states/test_fill_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/states/test_open_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/states/test_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/states/test_order_state_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/states/test_pending_creation_chained_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/states/test_pending_creation_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/test_decimal_order_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/test_double_filled_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    19279 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/test_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    20330 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/test_order_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/test_order_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    27711 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/test_order_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/test_orders_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/test_orders_storage_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.252610 OctoBot-Trading-2.4.8/tests/personal_data/orders/types/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.252610 OctoBot-Trading-2.4.8/tests/personal_data/orders/types/limit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/types/limit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/types/limit/test_buy_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/types/limit/test_sell_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/types/limit/test_stop_loss_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/types/limit/test_stop_loss_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/types/limit/test_take_profit_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/types/limit/test_take_profit_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.252610 OctoBot-Trading-2.4.8/tests/personal_data/orders/types/market/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/types/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/types/market/test_buy_market_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/types/market/test_sell_market_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/types/test_unknown_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.252610 OctoBot-Trading-2.4.8/tests/personal_data/orders/types/trailing/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/types/trailing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/types/trailing/test_trailing_stop_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/orders/types/trailing/test_trailing_stop_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.252610 OctoBot-Trading-2.4.8/tests/personal_data/portfolios/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/portfolios/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.252610 OctoBot-Trading-2.4.8/tests/personal_data/portfolios/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/portfolios/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/portfolios/assets/test_future_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/portfolios/assets/test_margin_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/portfolios/assets/test_spot_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.252610 OctoBot-Trading-2.4.8/tests/personal_data/portfolios/history/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/portfolios/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/portfolios/history/test_historical_asset_value_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    31055 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/portfolios/history/test_historical_portfolio_value_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/portfolios/test_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    52120 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/portfolios/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/portfolios/test_portfolio_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/portfolios/test_portfolio_profitability.py
--rw-r--r--   0 runner    (1001) docker     (123)    11149 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/portfolios/test_portfolio_value_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/portfolios/test_value_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.252610 OctoBot-Trading-2.4.8/tests/personal_data/portfolios/types/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/portfolios/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85551 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/portfolios/types/test_future_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/portfolios/types/test_margin_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/portfolios/types/test_spot_portfolio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.252610 OctoBot-Trading-2.4.8/tests/personal_data/positions/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/positions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.252610 OctoBot-Trading-2.4.8/tests/personal_data/positions/channel/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/positions/channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.256610 OctoBot-Trading-2.4.8/tests/personal_data/positions/states/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/positions/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67901 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/positions/test_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/positions/test_position_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/positions/test_positions_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.256610 OctoBot-Trading-2.4.8/tests/personal_data/positions/types/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/positions/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37450 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/positions/types/test_inverse_position.py
--rw-r--r--   0 runner    (1001) docker     (123)    45257 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/positions/types/test_linear_position.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.256610 OctoBot-Trading-2.4.8/tests/personal_data/trades/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/trades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/trades/test_trade_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/trades/test_trade_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/trades/test_trade_pnl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.256610 OctoBot-Trading-2.4.8/tests/personal_data/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/transactions/test_transaction_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/personal_data/transactions/test_transactions_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.256610 OctoBot-Trading-2.4.8/tests/signals/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29924 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/signals/test_trading_signal_bundle_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/signals/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.256610 OctoBot-Trading-2.4.8/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/test_utils/order_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/test_utils/random_numbers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.256610 OctoBot-Trading-2.4.8/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests/util/test_config_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.256610 OctoBot-Trading-2.4.8/tests_additional/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:45:53.260610 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/real_exchange_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/real_futures_exchange_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_ascendex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_binance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_binance_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_bitfinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_bitget.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_bithumb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_bitso.py
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_bitstamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_bittrex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_bybit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_bybit_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_coinbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_coinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_cryptocom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_gateio.py
--rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_hitbtc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_hollaex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_huobi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_huobipro.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_kraken.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_kucoin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_kucoin_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_mexc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_ndax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_okcoin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_okx.py
--rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_okx_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_phemex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_poloniex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_upbit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-07-08 14:45:00.000000 OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_wavesexchange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.708534 OctoBot-Trading-2.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    33500 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.624534 OctoBot-Trading-2.4.9/OctoBot_Trading.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-23 14:16:07.000000 OctoBot-Trading-2.4.9/OctoBot_Trading.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24477 2023-07-23 14:16:07.000000 OctoBot-Trading-2.4.9/OctoBot_Trading.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 14:16:07.000000 OctoBot-Trading-2.4.9/OctoBot_Trading.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 14:16:07.000000 OctoBot-Trading-2.4.9/OctoBot_Trading.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-23 14:16:07.000000 OctoBot-Trading-2.4.9/OctoBot_Trading.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-23 14:16:07.000000 OctoBot-Trading-2.4.9/OctoBot_Trading.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-23 14:16:07.708534 OctoBot-Trading-2.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.624534 OctoBot-Trading-2.4.9/octobot_trading/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.624534 OctoBot-Trading-2.4.9/octobot_trading/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/api/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/api/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/api/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/api/modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/api/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/api/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/api/positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/api/profitability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/api/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/api/symbol_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/api/trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/api/trades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.628534 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.628534 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/contracts/contract_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/contracts/future_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/contracts/margin_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/exchange_symbol_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/exchange_symbols_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.628534 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/funding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/funding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.628534 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/funding/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/funding/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/funding/channel/funding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/funding/channel/funding_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/funding/funding_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.628534 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/kline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/kline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.628534 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/kline/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/kline/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/kline/channel/kline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/kline/channel/kline_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/kline/kline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.628534 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ohlcv/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ohlcv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ohlcv/candles_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ohlcv/candles_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.632534 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ohlcv/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ohlcv/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ohlcv/channel/ohlcv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.632534 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/order_book/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/order_book/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.632534 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/order_book/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/order_book/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/order_book/channel/order_book.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/order_book/channel/order_book_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/order_book/order_book_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.632534 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/prices/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/prices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.632534 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/prices/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/prices/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/prices/channel/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/prices/channel/prices_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/prices/price_events_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/prices/prices_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.632534 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/recent_trades/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/recent_trades/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.636534 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/recent_trades/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/recent_trades/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/recent_trades/channel/recent_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/recent_trades/recent_trades_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.636534 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ticker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ticker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.636534 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ticker/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ticker/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ticker/channel/ticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ticker/channel/ticker_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ticker/ticker_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.636534 OctoBot-Trading-2.4.9/octobot_trading/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27517 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/abstract_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/abstract_websocket_exchange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.636534 OctoBot-Trading-2.4.9/octobot_trading/exchanges/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/adapters/abstract_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.636534 OctoBot-Trading-2.4.9/octobot_trading/exchanges/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/config/backtesting_exchange_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/config/exchange_config_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.636534 OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.640534 OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/ccxt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/ccxt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/ccxt/ccxt_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/ccxt/ccxt_client_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37015 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/ccxt/ccxt_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45448 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/ccxt/ccxt_websocket_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/ccxt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/ccxt/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.640534 OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/simulator/exchange_simulator_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/simulator/exchange_simulator_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/exchange_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/exchange_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/exchange_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/exchange_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13982 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/exchange_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/exchange_websocket_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/exchanges.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.640534 OctoBot-Trading-2.4.9/octobot_trading/exchanges/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/implementations/default_rest_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/implementations/default_websocket_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/implementations/exchange_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.640534 OctoBot-Trading-2.4.9/octobot_trading/exchanges/traders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/traders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42964 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/traders/trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/traders/trader_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.640534 OctoBot-Trading-2.4.9/octobot_trading/exchanges/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45451 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/types/rest_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/types/websocket_exchange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.640534 OctoBot-Trading-2.4.9/octobot_trading/exchanges/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/util/exchange_market_status_fixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17636 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/util/exchange_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/exchanges/util/websockets_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.644534 OctoBot-Trading-2.4.9/octobot_trading/modes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/modes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16710 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/modes/abstract_trading_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.644534 OctoBot-Trading-2.4.9/octobot_trading/modes/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/modes/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/modes/channel/abstract_mode_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23458 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/modes/channel/abstract_mode_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/modes/channel/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/modes/mode_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/modes/modes_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/modes/modes_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.644534 OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.644534 OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/basic_keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/basic_keywords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/basic_keywords/account_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/basic_keywords/amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/basic_keywords/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/basic_keywords/run_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/basic_keywords/trading_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/basic_keywords/user_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25931 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/context_management.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.648534 OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/dsl/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/dsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/dsl/quantity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/dsl/values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.648534 OctoBot-Trading-2.4.9/octobot_trading/modes/scripted_trading_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/modes/scripted_trading_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16335 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/modes/scripted_trading_mode/abstract_scripted_trading_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/octobot_channel_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.648534 OctoBot-Trading-2.4.9/octobot_trading/personal_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19668 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/exchange_personal_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.648534 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.652534 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14381 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/channel/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/channel/orders_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/channel/orders_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/decimal_order_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.652534 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/groups/group_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40970 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/order_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/order_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/order_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22239 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/order_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/orders_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/orders_storage_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.652534 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/states/
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/states/cancel_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/states/close_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/states/fill_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/states/open_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/states/order_state_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/states/pending_creation_chained_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/states/pending_creation_order_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.656534 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.656534 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/limit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/limit/buy_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/limit/limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/limit/sell_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/limit/stop_loss_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/limit/take_profit_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.656534 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/market/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/market/buy_market_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/market/market_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/market/sell_market_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.656534 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/trailing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/trailing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/unknown_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/unsupported_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.660534 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.660534 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/assets/future_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/assets/margin_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/assets/spot_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.660534 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/channel/balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/channel/balance_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.660534 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/history/
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/history/historical_asset_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17826 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14685 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/portfolio_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15012 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/portfolio_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/portfolio_profitability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/portfolio_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/portfolio_value_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/sub_portfolio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.660534 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/types/future_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/types/margin_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/types/spot_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17489 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/value_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.664534 OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.664534 OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/channel/positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/channel/positions_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/channel/positions_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39331 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/position_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/position_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/position_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/positions_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.664534 OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/states/
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/states/active_position_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/states/idle_position_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/states/liquidate_position_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/states/position_state_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.664534 OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/types/inverse_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/types/linear_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.668534 OctoBot-Trading-2.4.9/octobot_trading/personal_data/trades/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/trades/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.668534 OctoBot-Trading-2.4.9/octobot_trading/personal_data/trades/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/trades/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/trades/channel/trades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/trades/channel/trades_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/trades/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/trades/trade_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/trades/trade_pnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/trades/trades_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/trades/trades_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.668534 OctoBot-Trading-2.4.9/octobot_trading/personal_data/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/transactions/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/transactions/transaction_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/transactions/transactions_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.668534 OctoBot-Trading-2.4.9/octobot_trading/personal_data/transactions/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/transactions/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/transactions/types/blockchain_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/transactions/types/fee_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/transactions/types/realised_pnl_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/personal_data/transactions/types/transfer_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.668534 OctoBot-Trading-2.4.9/octobot_trading/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/signals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.672534 OctoBot-Trading-2.4.9/octobot_trading/signals/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/signals/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/signals/channel/remote_trading_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/signals/channel/remote_trading_signal_channel_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/signals/channel/signal_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/signals/signal_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/signals/trading_signal_bundle_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/signals/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.672534 OctoBot-Trading-2.4.9/octobot_trading/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/storage/abstract_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/storage/candles_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/storage/orders_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/storage/portfolio_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/storage/storage_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/storage/trades_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/storage/transactions_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/storage/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.672534 OctoBot-Trading-2.4.9/octobot_trading/supervisors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/supervisors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/supervisors/abstract_portfolio_supervisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/supervisors/abstract_supervisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.672534 OctoBot-Trading-2.4.9/octobot_trading/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/util/config_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/util/initializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/util/initialization_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/util/simulator_updater_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.676534 OctoBot-Trading-2.4.9/octobot_trading/util/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/util/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/util/test_tools/exchange_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/util/test_tools/exchanges_test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/util/test_tools/spot_rest_exchange_test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/octobot_trading/util/test_tools/websocket_test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 14:16:07.708534 OctoBot-Trading-2.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.620535 OctoBot-Trading-2.4.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.676534 OctoBot-Trading-2.4.9/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/api/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/api/test_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/api/test_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/api/test_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/api/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/api/test_profitability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/api/test_symbol_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/api/test_trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/api/test_trades.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.676534 OctoBot-Trading-2.4.9/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.676534 OctoBot-Trading-2.4.9/tests/exchange_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchange_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.676534 OctoBot-Trading-2.4.9/tests/exchange_data/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchange_data/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchange_data/contracts/test_future_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchange_data/contracts/test_margin_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.680534 OctoBot-Trading-2.4.9/tests/exchange_data/funding/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchange_data/funding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchange_data/funding/test_funding_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.680534 OctoBot-Trading-2.4.9/tests/exchange_data/kline/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchange_data/kline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchange_data/kline/test_kline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.680534 OctoBot-Trading-2.4.9/tests/exchange_data/ohlcv/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchange_data/ohlcv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchange_data/ohlcv/test_candles_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchange_data/ohlcv/test_candles_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.680534 OctoBot-Trading-2.4.9/tests/exchange_data/order_book/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchange_data/order_book/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchange_data/order_book/test_order_book_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.680534 OctoBot-Trading-2.4.9/tests/exchange_data/prices/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchange_data/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchange_data/prices/test_price_events_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchange_data/prices/test_prices_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.680534 OctoBot-Trading-2.4.9/tests/exchange_data/recent_trades/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchange_data/recent_trades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchange_data/recent_trades/test_recent_trades_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchange_data/test_exchange_symbols_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.680534 OctoBot-Trading-2.4.9/tests/exchange_data/ticker/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchange_data/ticker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchange_data/ticker/test_ticker_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.684534 OctoBot-Trading-2.4.9/tests/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchanges/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.684534 OctoBot-Trading-2.4.9/tests/exchanges/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchanges/connectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.684534 OctoBot-Trading-2.4.9/tests/exchanges/connectors/ccxt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchanges/connectors/ccxt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90633 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchanges/connectors/ccxt/mock_exchanges_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchanges/connectors/ccxt/test_ccxt_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.684534 OctoBot-Trading-2.4.9/tests/exchanges/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchanges/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchanges/implementations/test_default_rest_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchanges/implementations/test_default_websocket_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchanges/test_abstract_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchanges/test_abstract_websocket_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchanges/test_exchange_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchanges/test_exchange_config_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchanges/test_exchange_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchanges/test_exchange_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchanges/test_exchange_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchanges/test_exchanges.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.684534 OctoBot-Trading-2.4.9/tests/exchanges/traders/
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchanges/traders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50875 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchanges/traders/test_trader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.684534 OctoBot-Trading-2.4.9/tests/exchanges/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchanges/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchanges/types/test_websocket_exchange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.684534 OctoBot-Trading-2.4.9/tests/exchanges/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchanges/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchanges/util/test_exchange_market_status_fixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/exchanges/util/test_exchange_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.684534 OctoBot-Trading-2.4.9/tests/modes/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/modes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.684534 OctoBot-Trading-2.4.9/tests/modes/script_keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/modes/script_keywords/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.688534 OctoBot-Trading-2.4.9/tests/modes/script_keywords/basic_keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/modes/script_keywords/basic_keywords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/modes/script_keywords/basic_keywords/test_account_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/modes/script_keywords/basic_keywords/test_amount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.688534 OctoBot-Trading-2.4.9/tests/modes/script_keywords/dsl/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/modes/script_keywords/dsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/modes/script_keywords/dsl/test_quantity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/modes/test_abstract_mode_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/modes/test_abstract_trading_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.688534 OctoBot-Trading-2.4.9/tests/personal_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.688534 OctoBot-Trading-2.4.9/tests/personal_data/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.688534 OctoBot-Trading-2.4.9/tests/personal_data/orders/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19148 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/groups/test_balanced_take_profit_and_stop_order_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/groups/test_group_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/groups/test_one_cancels_the_other_order_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.692534 OctoBot-Trading-2.4.9/tests/personal_data/orders/states/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/states/test_cancel_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/states/test_close_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/states/test_fill_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/states/test_open_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/states/test_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/states/test_order_state_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/states/test_pending_creation_chained_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/states/test_pending_creation_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/test_decimal_order_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/test_double_filled_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19264 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/test_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20330 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/test_order_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/test_order_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27711 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/test_order_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/test_orders_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/test_orders_storage_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.692534 OctoBot-Trading-2.4.9/tests/personal_data/orders/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.692534 OctoBot-Trading-2.4.9/tests/personal_data/orders/types/limit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/types/limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/types/limit/test_buy_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/types/limit/test_sell_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/types/limit/test_stop_loss_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/types/limit/test_stop_loss_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/types/limit/test_take_profit_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/types/limit/test_take_profit_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.692534 OctoBot-Trading-2.4.9/tests/personal_data/orders/types/market/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/types/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/types/market/test_buy_market_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/types/market/test_sell_market_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/types/test_unknown_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.696534 OctoBot-Trading-2.4.9/tests/personal_data/orders/types/trailing/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/types/trailing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/types/trailing/test_trailing_stop_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/orders/types/trailing/test_trailing_stop_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.696534 OctoBot-Trading-2.4.9/tests/personal_data/portfolios/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/portfolios/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.696534 OctoBot-Trading-2.4.9/tests/personal_data/portfolios/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/portfolios/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/portfolios/assets/test_future_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/portfolios/assets/test_margin_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/portfolios/assets/test_spot_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.696534 OctoBot-Trading-2.4.9/tests/personal_data/portfolios/history/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/portfolios/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/portfolios/history/test_historical_asset_value_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31055 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/portfolios/history/test_historical_portfolio_value_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/portfolios/test_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53074 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/portfolios/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/portfolios/test_portfolio_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/portfolios/test_portfolio_profitability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11149 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/portfolios/test_portfolio_value_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/portfolios/test_value_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.696534 OctoBot-Trading-2.4.9/tests/personal_data/portfolios/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/portfolios/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85551 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/portfolios/types/test_future_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/portfolios/types/test_margin_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/portfolios/types/test_spot_portfolio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.700534 OctoBot-Trading-2.4.9/tests/personal_data/positions/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/positions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.700534 OctoBot-Trading-2.4.9/tests/personal_data/positions/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/positions/channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.700534 OctoBot-Trading-2.4.9/tests/personal_data/positions/states/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/positions/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67901 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/positions/test_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/positions/test_position_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/positions/test_positions_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.700534 OctoBot-Trading-2.4.9/tests/personal_data/positions/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/positions/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37450 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/positions/types/test_inverse_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45257 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/positions/types/test_linear_position.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.700534 OctoBot-Trading-2.4.9/tests/personal_data/trades/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/trades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/trades/test_trade_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/trades/test_trade_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/trades/test_trade_pnl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.700534 OctoBot-Trading-2.4.9/tests/personal_data/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/transactions/test_transaction_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/personal_data/transactions/test_transactions_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.700534 OctoBot-Trading-2.4.9/tests/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29924 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/signals/test_trading_signal_bundle_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/signals/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.704534 OctoBot-Trading-2.4.9/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/test_utils/order_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/test_utils/random_numbers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.704534 OctoBot-Trading-2.4.9/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests/util/test_config_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.704534 OctoBot-Trading-2.4.9/tests_additional/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:16:07.708534 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/real_exchange_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/real_futures_exchange_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_ascendex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_binance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_binance_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_bitfinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_bitget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_bithumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_bitso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_bitstamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_bittrex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_bybit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_bybit_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_coinbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_coinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_cryptocom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_gateio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_hitbtc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_hollaex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_huobi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_huobipro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_kraken.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_kucoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_kucoin_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_mexc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_ndax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_okcoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_okx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_okx_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_phemex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_poloniex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_upbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-07-23 14:14:57.000000 OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_wavesexchange.py
```

### Comparing `OctoBot-Trading-2.4.8/CHANGELOG.md` & `OctoBot-Trading-2.4.9/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.4.9] - 2023-07-23
+### Updated
+- [Tests] testing tools
+- [TradingModes] logs on minimum trading volumes
+### Fixed
+- [Websockets] Reconnection issues
+
 ## [2.4.8] - 2023-07-08
 ### Fixed
 - [Positions] Contracts live update
 
 ## [2.4.7] - 2023-07-07
 ### Added
 - [Positions] Log error on hedged positions
```

### Comparing `OctoBot-Trading-2.4.8/LICENSE` & `OctoBot-Trading-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/OctoBot_Trading.egg-info/PKG-INFO` & `OctoBot-Trading-2.4.9/OctoBot_Trading.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot-Trading
-Version: 2.4.8
+Version: 2.4.9
 Summary: OctoBot project trading package
 Home-page: https://github.com/Drakkar-Software/OctoBot-Trading
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# OctoBot-Trading [2.4.8](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
+# OctoBot-Trading [2.4.9](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/903b6b22bceb4661b608a86fea655f69)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Trading?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Trading&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Trading.svg)](https://pypi.python.org/pypi/OctoBot-Trading/)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Trading/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Trading?branch=master)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Trading/workflows/OctoBot-Trading-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Trading/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Trading/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Trading)
 
 OctoBot trading package.
```

### Comparing `OctoBot-Trading-2.4.8/OctoBot_Trading.egg-info/SOURCES.txt` & `OctoBot-Trading-2.4.9/OctoBot_Trading.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -275,14 +275,15 @@
 octobot_trading/supervisors/abstract_supervisor.py
 octobot_trading/util/__init__.py
 octobot_trading/util/config_util.py
 octobot_trading/util/initializable.py
 octobot_trading/util/initialization_util.py
 octobot_trading/util/simulator_updater_utils.py
 octobot_trading/util/test_tools/__init__.py
+octobot_trading/util/test_tools/exchange_data.py
 octobot_trading/util/test_tools/exchanges_test_tools.py
 octobot_trading/util/test_tools/spot_rest_exchange_test_tools.py
 octobot_trading/util/test_tools/websocket_test_tools.py
 tests/api/__init__.py
 tests/api/test_channels.py
 tests/api/test_exchange.py
 tests/api/test_modes.py
@@ -321,14 +322,15 @@
 tests/exchanges/test_exchange_config_data.py
 tests/exchanges/test_exchange_factory.py
 tests/exchanges/test_exchange_manager.py
 tests/exchanges/test_exchange_simulator.py
 tests/exchanges/test_exchanges.py
 tests/exchanges/connectors/__init__.py
 tests/exchanges/connectors/ccxt/__init__.py
+tests/exchanges/connectors/ccxt/mock_exchanges_data.py
 tests/exchanges/connectors/ccxt/test_ccxt_connector.py
 tests/exchanges/implementations/__init__.py
 tests/exchanges/implementations/test_default_rest_exchange.py
 tests/exchanges/implementations/test_default_websocket_exchange.py
 tests/exchanges/traders/__init__.py
 tests/exchanges/traders/test_trader.py
 tests/exchanges/types/__init__.py
```

### Comparing `OctoBot-Trading-2.4.8/PKG-INFO` & `OctoBot-Trading-2.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot-Trading
-Version: 2.4.8
+Version: 2.4.9
 Summary: OctoBot project trading package
 Home-page: https://github.com/Drakkar-Software/OctoBot-Trading
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# OctoBot-Trading [2.4.8](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
+# OctoBot-Trading [2.4.9](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/903b6b22bceb4661b608a86fea655f69)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Trading?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Trading&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Trading.svg)](https://pypi.python.org/pypi/OctoBot-Trading/)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Trading/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Trading?branch=master)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Trading/workflows/OctoBot-Trading-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Trading/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Trading/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Trading)
 
 OctoBot trading package.
```

### Comparing `OctoBot-Trading-2.4.8/README.md` & `OctoBot-Trading-2.4.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# OctoBot-Trading [2.4.8](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
+# OctoBot-Trading [2.4.9](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/903b6b22bceb4661b608a86fea655f69)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Trading?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Trading&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Trading.svg)](https://pypi.python.org/pypi/OctoBot-Trading/)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Trading/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Trading?branch=master)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Trading/workflows/OctoBot-Trading-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Trading/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Trading/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Trading)
 
 OctoBot trading package.
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
 PROJECT_NAME = "OctoBot-Trading"
-VERSION = "2.4.8"  # major.minor.revision
+VERSION = "2.4.9"  # major.minor.revision
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/api/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/api/channels.py` & `OctoBot-Trading-2.4.9/octobot_trading/api/channels.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/api/contracts.py` & `OctoBot-Trading-2.4.9/octobot_trading/api/contracts.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/api/exchange.py` & `OctoBot-Trading-2.4.9/octobot_trading/api/exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/api/modes.py` & `OctoBot-Trading-2.4.9/octobot_trading/api/modes.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/api/orders.py` & `OctoBot-Trading-2.4.9/octobot_trading/api/orders.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/api/portfolio.py` & `OctoBot-Trading-2.4.9/octobot_trading/api/portfolio.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         exchange_manager.exchange_personal_data.portfolio_manager.portfolio_value_holder.origin_portfolio.portfolio,
         as_decimal
     )
 
 
 def set_simulated_portfolio_initial_config(exchange_manager, portfolio_content):
     if exchange_manager.exchange_personal_data.portfolio_manager:
-        exchange_manager.exchange_personal_data.portfolio_manager.set_simulated_portfolio_initial_config(
+        exchange_manager.exchange_personal_data.portfolio_manager.set_forced_portfolio_initial_config(
             portfolio_content
         )
 
 
 def format_portfolio(portfolio, as_decimal) -> dict:
     if as_decimal:
         return portfolio
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/api/positions.py` & `OctoBot-Trading-2.4.9/octobot_trading/api/positions.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/api/profitability.py` & `OctoBot-Trading-2.4.9/octobot_trading/api/profitability.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/api/storage.py` & `OctoBot-Trading-2.4.9/octobot_trading/api/storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/api/symbol_data.py` & `OctoBot-Trading-2.4.9/octobot_trading/api/symbol_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/api/trader.py` & `OctoBot-Trading-2.4.9/octobot_trading/api/trader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/api/trades.py` & `OctoBot-Trading-2.4.9/octobot_trading/api/trades.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/constants.py` & `OctoBot-Trading-2.4.9/octobot_trading/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 ENABLE_EXCHANGE_HTTP_PROXY_FROM_ENV = os_util.parse_boolean_environment_var(
     "ENABLE_EXCHANGE_HTTP_PROXY_FROM_ENV", "True")
 ENABLE_CCXT_VERBOSE = os_util.parse_boolean_environment_var("ENABLE_CCXT_VERBOSE", "False")
 ENABLE_CCXT_RATE_LIMIT = os_util.parse_boolean_environment_var("ENABLE_CCXT_RATE_LIMIT", "True")
 THROTTLED_WS_UPDATES = float(os.getenv("THROTTLED_WS_UPDATES", "0.1"))  # avoid spamming CPU
 ENABLE_LIVE_CANDLES_STORAGE = os_util.parse_boolean_environment_var("ENABLE_LIVE_CANDLES_STORAGE", "False")
 ENABLE_HISTORICAL_ORDERS_UPDATES_STORAGE = os_util.parse_boolean_environment_var("ENABLE_HISTORICAL_ORDERS_UPDATES_STORAGE", "False")
+STORAGE_ORIGIN_VALUE = "origin_value"
 DISPLAY_TIME_FRAME = commons_enums.TimeFrames.ONE_HOUR
 
 # Decimal default values (decimals are immutable, can be stored as constant)
 ZERO = decimal.Decimal(0)
 ONE = decimal.Decimal(1)
 ONE_HUNDRED = decimal.Decimal(100)
 NaN = decimal.Decimal("nan")
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/enums.py` & `OctoBot-Trading-2.4.9/octobot_trading/enums.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/errors.py` & `OctoBot-Trading-2.4.9/octobot_trading/errors.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_channel.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_channel.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/contracts/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/contracts/contract_factory.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/contracts/contract_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/contracts/future_contract.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/contracts/future_contract.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/contracts/margin_contract.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/contracts/margin_contract.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/exchange_symbol_data.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/exchange_symbol_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/exchange_symbols_data.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/exchange_symbols_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/funding/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/funding/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/funding/channel/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/funding/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/funding/channel/funding.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/funding/channel/funding.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/funding/channel/funding_updater.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/funding/channel/funding_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/funding/funding_manager.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/funding/funding_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/kline/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/kline/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/kline/channel/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/kline/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/kline/channel/kline.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/kline/channel/kline.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/kline/channel/kline_updater.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/kline/channel/kline_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/kline/kline_manager.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/kline/kline_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ohlcv/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ohlcv/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ohlcv/candles_adapter.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ohlcv/candles_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ohlcv/candles_manager.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ohlcv/candles_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ohlcv/channel/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ohlcv/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ohlcv/channel/ohlcv.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ohlcv/channel/ohlcv.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/order_book/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/order_book/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/order_book/channel/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/order_book/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/order_book/channel/order_book.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/order_book/channel/order_book.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/order_book/channel/order_book_updater.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/order_book/channel/order_book_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/order_book/order_book_manager.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/order_book/order_book_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/prices/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/prices/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/prices/channel/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/prices/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/prices/channel/price.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/prices/channel/price.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/prices/channel/prices_updater.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/prices/channel/prices_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/prices/price_events_manager.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/prices/price_events_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/prices/prices_manager.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/prices/prices_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/recent_trades/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/recent_trades/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/recent_trades/channel/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/recent_trades/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/recent_trades/channel/recent_trade.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/recent_trades/channel/recent_trade.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/recent_trades/recent_trades_manager.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/recent_trades/recent_trades_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ticker/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ticker/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ticker/channel/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ticker/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ticker/channel/ticker.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ticker/channel/ticker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ticker/channel/ticker_updater.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ticker/channel/ticker_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchange_data/ticker/ticker_manager.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchange_data/ticker/ticker_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/abstract_exchange.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/abstract_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/abstract_websocket_exchange.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/abstract_websocket_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/adapters/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/adapters/abstract_adapter.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/adapters/abstract_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/config/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/config/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/config/backtesting_exchange_config.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/config/backtesting_exchange_config.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/config/exchange_config_data.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/config/exchange_config_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/ccxt/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/ccxt/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/ccxt/ccxt_adapter.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/ccxt/ccxt_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/ccxt/ccxt_client_util.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/ccxt/ccxt_client_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/ccxt/ccxt_connector.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/ccxt/ccxt_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,17 +86,16 @@
                 )
                 
             if self.force_authentication or (
                 self._should_authenticate() and not self.exchange_manager.exchange_only
             ):
                 await self._ensure_auth()
 
-            if self.exchange_manager.is_loading_markets:
-                with self.error_describer():
-                    await self.load_symbol_markets()
+            with self.error_describer():
+                await self.load_symbol_markets(forced_markets=self.exchange_manager.forced_markets)
 
             # initialize symbols and timeframes
             self.symbols = self.get_client_symbols()
             self.time_frames = self.get_client_time_frames()
 
         except (ccxt.ExchangeNotAvailable, ccxt.RequestTimeout) as e:
             raise octobot_trading.errors.UnreachableExchange() from e
@@ -107,16 +106,24 @@
         return adapter_class or ccxt_adapter.CCXTAdapter
 
     @classmethod
     def load_user_inputs_from_class(cls, tentacles_setup_config, tentacle_config):
         # no user input in connector
         pass
 
-    async def load_symbol_markets(self, reload=False):
-        await self.client.load_markets(reload=reload)
+    async def load_symbol_markets(self, reload=False, forced_markets=None):
+        if forced_markets is not None:
+            if forced_markets:
+                # only set markets if there are markets to be set
+                self.client.set_markets([
+                    self.client.parse_market(market) if hasattr(self.client, "parse_market") else market
+                    for market in forced_markets
+                ])
+        else:
+            await self.client.load_markets(reload=reload)
 
     def get_client_symbols(self):
         return ccxt_client_util.get_symbols(self.client)
 
     def get_client_time_frames(self):
         return ccxt_client_util.get_time_frames(self.client)
 
@@ -629,17 +636,17 @@
     def get_exchange_current_time(self):
         return self.get_uniform_timestamp(self.client.milliseconds())
 
     def get_uniform_timestamp(self, timestamp):
         return self.adapter.get_uniformized_timestamp(timestamp)
 
     async def stop(self) -> None:
-        self.logger.info(f"Closing connection.")
+        self.logger.debug(f"Closing connection.")
         await ccxt_client_util.close_client(self.client)
-        self.logger.info(f"Connection closed.")
+        self.logger.debug(f"Connection closed.")
         self.client = None
         self.exchange_manager = None
 
     def get_pair_from_exchange(self, pair) -> typing.Optional[str]:
         try:
             return self.client.market(pair)["symbol"]
         except ccxt.BadSymbol:
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/ccxt/ccxt_websocket_connector.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/ccxt/ccxt_websocket_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,16 @@
 
 class CCXTWebsocketConnector(abstract_websocket_exchange.AbstractWebsocketExchange):
     INIT_REQUIRING_EXCHANGE_FEEDS = [Feeds.CANDLE]
     SUPPORTS_LIVE_PAIR_ADDITION = True
     FEED_INITIALIZATION_TIMEOUT = 15 * commons_constants.MINUTE_TO_SECONDS
     MIN_CONNECTION_CLOSE_INTERVAL = 2 * commons_constants.MINUTE_TO_SECONDS
     NO_MESSAGE_DISCONNECTED_TIMEOUT = 4 * commons_constants.MINUTE_TO_SECONDS
-    EXCHANGE_RECONNECT_INTERVAL = None
+    RECREATE_CLIENT_ON_DISCONNECT = False   # when True, a new ccxt websocket client will replace the previous
+    # one when the exchange is disconnected
 
     IGNORED_FEED_PAIRS = {
         # When ticker or future index is available : no need to calculate mark price from recent trades
         Feeds.TRADES: [Feeds.TICKER, Feeds.FUTURES_INDEX],
         # When candles are available : use min timeframe kline to push ticker
         Feeds.TICKER: [Feeds.KLINE],
         # When funding can be found in websocket ticker
@@ -282,18 +283,20 @@
             self.logger.exception(e, True, f"Failed to subscribe when creating websocket feed : {e}")
         finally:
             self.initialized_event.set()
 
     async def _close_exchange_to_force_reconnect(self):
         if time.time() - self._last_close_time > self.MIN_CONNECTION_CLOSE_INTERVAL and not self.should_stop:
             # Close client to force connections re-open. The next watch_xyz will recreate the connection
+            self._last_close_time = time.time()
             self.logger.debug(f"Closing exchange connection.")
             await self.client.close()
+            if self.RECREATE_CLIENT_ON_DISCONNECT:
+                self._create_client()
             self.logger.debug("Exchange connection closed. The next watch-xyz will re-open it.")
-            self._last_close_time = time.time()
             return True
         return False
 
     def _subscribe_feeds(self):
         """
         Prepares the subscription of unauthenticated and authenticated feeds and subscribe all
         """
@@ -561,33 +564,37 @@
                     else self.LONG_RECONNECT_DELAY
                 self.logger.debug(f"Can't connect to exchange {ws_des} websocket: {err}. "
                                   f"Retrying in {reconnect_delay} seconds")
                 if await self._close_exchange_to_force_reconnect():
                     message = f"Closed exchange connection to force reconnect. Error: {err}"
                     if subsequent_disconnections > 1 and subsequent_disconnections % 5 == 0:
                         self.logger.error(
-                            f"Multiple disconnections if a row [{subsequent_disconnections}] for {ws_des}. {message}"
+                            f"Multiple disconnections in a row [{subsequent_disconnections}] for {ws_des}. {message}"
                         )
                     else:
                         self.logger.debug(message)
                 await asyncio.sleep(reconnect_delay)
                 self.logger.debug(f"Reconnecting to {ws_des}")
+                # self.client might have changed
+                watch_func = self._get_feed_generator_by_feed()[feed]
                 subsequent_disconnections += 1  # wait for a longer time before the next reconnect
             except ccxt.BadRequest as err:
                 message = f"Impossible to start {ws_des} feed due to exchange refusing the connection request: {err}."
                 self.logger.exception(
                     err,
                     True,
                     f"{message} {'Will retry once' if not already_got_feed_stopping_error else 'Now stopping'}."
                 )
                 if already_got_feed_stopping_error:
                     # there is a real issue when connecting to the feed. Don't loop
                     return
                 already_got_feed_stopping_error = True
                 await asyncio.sleep(self.LONG_RECONNECT_DELAY)  # avoid spamming
+                # self.client might have changed
+                watch_func = self._get_feed_generator_by_feed()[feed]
             except ccxt.NotSupported as err:
                 self.logger.exception(
                     err,
                     True,
                     f"Impossible to start {ws_des} feed: {err}. "
                     f"Stopping it. Please report to the OctoBot team if you see this error"
                 )
@@ -600,14 +607,16 @@
                     self.logger.exception(err, True, error_message)
                 elif error_count % spamming_logs_warning_interval == 0:
                     self.logger.warning(error_message)
                 elif error_count % spamming_logs_debug_interval == 0:
                     self.logger.debug(error_message)
                 await asyncio.sleep(self.LONG_RECONNECT_DELAY)  # avoid spamming
                 subsequent_disconnections += 1  # wait for a longer time before the next reconnect
+                # self.client might have changed
+                watch_func = self._get_feed_generator_by_feed()[feed]
 
     def _create_task_if_necessary(self, feed, feed_callback, feed_generator, **kwargs):
         identifier = self._get_feed_identifier(feed_generator, kwargs)
         if identifier not in self.feed_tasks:
             self.logger.debug(f"Subscribing to {feed.value} with {kwargs}")
             self.feed_tasks[identifier] = asyncio.create_task(
                 self._feed_task(feed, feed_callback, feed_generator, **kwargs)
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/ccxt/constants.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/ccxt/constants.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/ccxt/enums.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/ccxt/enums.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/simulator/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/simulator/exchange_simulator_adapter.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/simulator/exchange_simulator_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/connectors/simulator/exchange_simulator_connector.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/connectors/simulator/exchange_simulator_connector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/exchange_builder.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/exchange_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,21 +111,24 @@
                     self.logger.warning(f"There wont be any order created on {self.exchange_name}: neither "
                                         f"simulated nor real trader has been activated.")
                 else:
                     self.exchange_manager.trading_modes = await self._build_trading_modes(trading_mode_class)
             else:
                 self.logger.info(f"{self.exchange_name} exchange is online and won't be trading")
 
-    async def _build_trading_modes(self, trading_mode_class):
+    async def _build_trading_modes(self, trading_mode_class, trading_config_by_trading_mode=None):
         try:
             self._ensure_trading_mode_compatibility(trading_mode_class)
-            return await modes.create_trading_modes(self.config,
-                                                    self.exchange_manager,
-                                                    trading_mode_class,
-                                                    self.exchange_manager.bot_id)
+            return await modes.create_trading_modes(
+                self.config,
+                self.exchange_manager,
+                trading_mode_class,
+                self.exchange_manager.bot_id,
+                trading_config_by_trading_mode=trading_config_by_trading_mode
+            )
         except errors.TradingModeIncompatibility as e:
             raise e
         except Exception as e:
             self.logger.error(f"An error occurred when initializing trading mode : {e}")
             raise e
 
     def _ensure_exchange_compatibility(self):
@@ -207,16 +210,16 @@
         self.exchange_manager.rest_only = True
         return self
 
     def is_exchange_only(self):
         self.exchange_manager.exchange_only = True
         return self
 
-    def is_loading_markets(self, is_loading_markets):
-        self.exchange_manager.is_loading_markets = is_loading_markets
+    def has_forced_markets(self, forced_markets: dict):
+        self.exchange_manager.forced_markets = forced_markets
         return self
 
     def is_ignoring_config(self, ignore_config=True):
         self.exchange_manager.ignore_config = ignore_config
         return self
 
     def is_without_auth(self):
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/exchange_channels.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/exchange_channels.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,18 +30,19 @@
     """
     for exchange_channel_class_type in [exchange_channel.ExchangeChannel, exchange_channel.TimeFrameExchangeChannel]:
         await channel_util.create_all_subclasses_channel(exchange_channel_class_type, exchange_channel.set_chan,
                                                          is_synchronized=exchange_manager.is_backtesting,
                                                          exchange_manager=exchange_manager)
 
 
-async def create_exchange_producers(exchange_manager) -> None:
+async def create_exchange_producers(exchange_manager, forced_producers=None) -> None:
     """
     Create exchange channels producers according to exchange manager context (backtesting, simulator, real)
     :param exchange_manager: the related exchange manager
+    :param forced_producers: producers to create no anyway
     """
     import octobot_trading.personal_data as personal_data
 
     # Always init exchange user data first on real trading
     if _should_create_authenticated_producers(exchange_manager):
         await _create_producers(exchange_manager, personal_data.AUTHENTICATED_UPDATER_PRODUCERS)
 
@@ -50,14 +51,17 @@
         import octobot_trading.exchange_data as exchange_data
         await _create_producers(exchange_manager, exchange_data.UNAUTHENTICATED_UPDATER_PRODUCERS)
 
     # Simulated producers
     if _should_create_simulated_producers(exchange_manager):
         await _create_producers(exchange_manager, personal_data.AUTHENTICATED_UPDATER_SIMULATOR_PRODUCERS)
 
+    if forced_producers:
+        await _create_producers(exchange_manager, forced_producers)
+
 
 def _should_create_authenticated_producers(exchange_manager):
     """
     :param exchange_manager: the related exchange manager
     :return: True if should create authenticated producers
     """
     return exchange_manager.exchange.authenticated() \
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/exchange_details.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/exchange_details.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/exchange_factory.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/exchange_factory.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -51,17 +51,17 @@
     """
     Create and initialize real REST exchange
     :param exchange_manager: the related exchange manager
     """
     await _create_rest_exchange(exchange_manager)
     try:
         await exchange_manager.exchange.initialize()
+        _create_exchange_backend(exchange_manager)
         if exchange_manager.exchange_only:
             return
-        _create_exchange_backend(exchange_manager)
         await _initialize_exchange_backend(exchange_manager)
         _ensure_exchange_validity(exchange_manager)
     except errors.AuthenticationError:
         exchange_manager.logger.error("Authentication error, retrying without authentication...")
         exchange_manager.without_auth = True
         await create_real_exchange(exchange_manager)
         return
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/exchange_manager.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/exchange_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         self.logger = logging.get_logger(self.__class__.__name__)
 
         self.is_ready = False
         self.is_simulated: bool = False
         self.is_backtesting: bool = False
         self.rest_only: bool = False
         self.ignore_config: bool = False
-        self.is_loading_markets: bool = True
+        self.forced_markets: dict = None
         self.is_spot_only: bool = False
         self.is_margin: bool = False
         self.is_future: bool = False
         self.is_sandboxed: bool = False
         self.is_trading: bool = True
         self.without_auth: bool = False
         self.check_credentials: bool = True
@@ -116,16 +116,20 @@
         if enable_logs:
             self.logger.debug("Stopped trading modes")
 
         # stop exchange channels
         if enable_logs:
             self.logger.debug(f"Stopping exchange channels for exchange_id: {self.id} ...")
         if self.exchange is not None:
-            if not self.exchange_only:
+            try:
+                exchange_channel.get_exchange_channels(self.id)
                 await exchange_channel.stop_exchange_channels(self, should_warn=warning_on_missing_elements)
+            except KeyError:
+                # no exchange channel to stop
+                pass
             await self.exchange.stop()
             exchanges.Exchanges.instance().del_exchange(
                 self.exchange.name, self.id, should_warn=warning_on_missing_elements
             )
             self.exchange.exchange_manager = None
             self.exchange = None
         if self.exchange_personal_data is not None:
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/exchange_websocket_factory.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/exchange_websocket_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/exchanges.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/exchanges.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,16 +36,17 @@
     def __init__(self):
         self.exchanges = {}
 
     def add_exchange(self, exchange_manager, matrix_id) -> None:
         if exchange_manager.exchange_name not in self.exchanges:
             self.exchanges[exchange_manager.exchange_name] = {}
 
-        self.exchanges[exchange_manager.exchange_name][exchange_manager.id] = ExchangeConfiguration(exchange_manager,
-                                                                                                    matrix_id)
+        self.exchanges[exchange_manager.exchange_name][exchange_manager.id] = ExchangeConfiguration(
+            exchange_manager, matrix_id
+        )
 
     def get_exchange(self, exchange_name, exchange_manager_id) -> ExchangeConfiguration:
         return self.exchanges[exchange_name][exchange_manager_id]
 
     def get_all_exchanges(self):
         exchanges_list: list = []
         for exchange_name in self.exchanges.keys():
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/implementations/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/implementations/default_rest_exchange.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/implementations/default_rest_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/implementations/default_websocket_exchange.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/implementations/default_websocket_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/implementations/exchange_simulator.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/implementations/exchange_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/traders/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/traders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/traders/trader.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/traders/trader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/traders/trader_simulator.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/traders/trader_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/types/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/types/rest_exchange.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/types/rest_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/types/websocket_exchange.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/types/websocket_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/util/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/util/exchange_market_status_fixer.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/util/exchange_market_status_fixer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/util/exchange_util.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/util/exchange_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,28 +198,29 @@
                 common_constants.CONFIG_ENABLED_OPTION, True
         )
     ]
 
 
 @contextlib.asynccontextmanager
 async def get_local_exchange_manager(
-    exchange_name: str, exchange_config: dict, tentacles_setup_config, is_sandboxed: bool, ignore_config=False
+    exchange_name: str, exchange_config: dict, tentacles_setup_config,
+    is_sandboxed: bool, ignore_config=False, builder=None, forced_markets=None,
 ):
     exchange_type = exchange_config.get(common_constants.CONFIG_EXCHANGE_TYPE, get_default_exchange_type(exchange_name))
-    builder = exchange_builder.ExchangeBuilder(
+    builder = builder or exchange_builder.ExchangeBuilder(
         _get_minimal_exchange_config(exchange_name, exchange_config),
         exchange_name
     )
     exchange_manager = await builder.use_tentacles_setup_config(tentacles_setup_config) \
         .is_checking_credentials(False) \
         .is_sandboxed(is_sandboxed) \
         .is_using_exchange_type(exchange_type) \
         .is_exchange_only() \
         .is_rest_only() \
-        .is_loading_markets(False) \
+        .has_forced_markets(forced_markets or {}) \
         .is_ignoring_config(ignore_config) \
         .disable_trading_mode() \
         .build()
     try:
         yield exchange_manager
     finally:
         # do not log stopping message
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/exchanges/util/websockets_util.py` & `OctoBot-Trading-2.4.9/octobot_trading/exchanges/util/websockets_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/modes/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/modes/abstract_trading_mode.py` & `OctoBot-Trading-2.4.9/octobot_trading/modes/abstract_trading_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     ALLOW_CUSTOM_TRIGGER_SOURCE = False
     HISTORIZE_USER_INPUT_CONFIG = True
 
     MODE_PRODUCER_CLASSES = []
     MODE_CONSUMER_CLASSES = []
     # maximum seconds before sending a trading signal if orders are slow to create on exchange
     TRADING_SIGNAL_TIMEOUT = 10
+    REQUIRE_TRADES_HISTORY = False   # set True when this trading mode needs the trade history to operate
 
     def __init__(self, config, exchange_manager):
         super().__init__()
         self.logger = logging.get_logger(self.get_name())
 
         # Global OctoBot configuration
         self.config: dict = config
@@ -173,19 +174,19 @@
     def is_backtestable() -> bool:
         """
         Should be overwritten
         :return: True if the TradingMode can be used in a backtesting else False
         """
         return True
 
-    async def initialize(self) -> None:
+    async def initialize(self, trading_config=None) -> None:
         """
         Triggers producers and consumers creation
         """
-        await self.reload_config(self.exchange_manager.bot_id)
+        await self.reload_config(self.exchange_manager.bot_id, trading_config=trading_config)
         self.producers = await self.create_producers()
         self.consumers = await self.create_consumers()
 
     async def stop(self) -> None:
         """
         Stops all producers and consumers
         """
@@ -278,21 +279,21 @@
             consumer_instance=mode_consumer,
             trading_mode_name=self.get_name(),
             cryptocurrency=self.cryptocurrency if self.cryptocurrency else channel_constants.CHANNEL_WILDCARD,
             symbol=self.symbol if self.symbol else channel_constants.CHANNEL_WILDCARD,
             time_frame=self.time_frame if self.time_frame else channel_constants.CHANNEL_WILDCARD)
         return mode_consumer
 
-    async def reload_config(self, bot_id: str) -> None:
+    async def reload_config(self, bot_id: str, trading_config=None) -> None:
         """
         Try to load TradingMode tentacle config.
         Calls set_default_config() if the tentacle config is empty
         """
-        self.trading_config = tentacles_manager_api.get_tentacle_config(self.exchange_manager.tentacles_setup_config,
-                                                                        self.__class__)
+        self.trading_config = trading_config or \
+            tentacles_manager_api.get_tentacle_config(self.exchange_manager.tentacles_setup_config, self.__class__)
         # set default config if nothing found
         if not self.trading_config:
             self.set_default_config()
         await self.load_and_save_user_inputs(bot_id)
         for element in self.consumers + self.producers:
             if isinstance(element, (abstract_mode_consumer.AbstractTradingModeConsumer,
                                     abstract_mode_producer.AbstractTradingModeProducer)):
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/modes/channel/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/modes/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/modes/channel/abstract_mode_consumer.py` & `OctoBot-Trading-2.4.9/octobot_trading/modes/channel/abstract_mode_consumer.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,35 +127,41 @@
                                                        portfolio_type=commons_constants.PORTFOLIO_AVAILABLE)
             side = enums.TradeOrderSide.SELL \
                 if state == enums.EvaluatorStates.VERY_SHORT.value or state == enums.EvaluatorStates.SHORT.value \
                 else enums.TradeOrderSide.BUY
             max_order_size, _ = personal_data.get_futures_max_order_size(
                 self.exchange_manager, symbol, side, current_price, False, current_symbol_holding, market_quantity
             )
+            can_create_order = max_order_size > symbol_min_amount
             self.logger.debug(
-                f"can_create_order: max_order_size > symbol_min_amount: {max_order_size} > {symbol_min_amount}"
+                f"can_create_order: {can_create_order} = "
+                f"max_order_size > symbol_min_amount = {max_order_size} > {symbol_min_amount}"
             )
-            return max_order_size > symbol_min_amount
+            return can_create_order
 
         # spot, trade asset directly
         # short cases => sell => need this currency
         if state == enums.EvaluatorStates.VERY_SHORT.value or state == enums.EvaluatorStates.SHORT.value:
+            can_create_order = portfolio.get_currency_portfolio(currency).available > symbol_min_amount
             self.logger.debug(
-                f"can_create_order: portfolio.get_currency_portfolio(currency).available > symbol_min_amount: "
+                f"can_create_order: {can_create_order} = "
+                f"portfolio.get_currency_portfolio(currency).available > symbol_min_amount = "
                 f"{portfolio.get_currency_portfolio(currency).available} > {symbol_min_amount}"
             )
-            return portfolio.get_currency_portfolio(currency).available > symbol_min_amount
+            return can_create_order
 
         # long cases => buy => need money(aka other currency in the pair) to buy this currency
         elif state == enums.EvaluatorStates.LONG.value or state == enums.EvaluatorStates.VERY_LONG.value:
+            can_create_order = portfolio.get_currency_portfolio(market).available > order_min_amount
             self.logger.debug(
-                f"can_create_order: portfolio.get_currency_portfolio(market).available > order_min_amount: "
+                f"can_create_order: {can_create_order} = "
+                f"portfolio.get_currency_portfolio(market).available > order_min_amount = "
                 f"{portfolio.get_currency_portfolio(market).available} > {order_min_amount}"
             )
-            return portfolio.get_currency_portfolio(market).available > order_min_amount
+            return can_create_order
 
         # other cases like neutral state or unfulfilled previous conditions
         self.logger.debug("can_create_order: return False")
         return False
 
     def get_holdings_ratio(self, currency):
         return self.exchange_manager.exchange_personal_data.portfolio_manager.portfolio_value_holder \
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/modes/channel/abstract_mode_producer.py` & `OctoBot-Trading-2.4.9/octobot_trading/modes/channel/abstract_mode_producer.py`

 * *Files 2% similar despite different names*

```diff
@@ -406,18 +406,27 @@
             return True
         except (asyncio.TimeoutError, concurrent.futures.TimeoutError):
             self.logger.error(f"Initialization took more than {timeout} seconds")
         return False
 
     async def _wait_for_bot_init(self, timeout) -> bool:
         try:
-            self.logger.debug("Trading mode start complete. Now waiting for orders full initialisation.")
-            await util.wait_for_topic_init(self.exchange_manager, timeout,
-                                           common_enums.InitializationEventExchangeTopics.ORDERS.value)
-            self.logger.debug("Trading mode start complete. Orders initialisation completed.")
+            topics = [
+                common_enums.InitializationEventExchangeTopics.BALANCE.value,
+                common_enums.InitializationEventExchangeTopics.ORDERS.value
+            ]
+            if self.trading_mode.REQUIRE_TRADES_HISTORY:
+                topics.append(common_enums.InitializationEventExchangeTopics.TRADES.value)
+            for topic in topics:
+                self.logger.debug(f"Trading mode [{self.exchange_manager.exchange_name}] start complete. "
+                                  f"Now waiting for {topic} full initialisation.")
+                await util.wait_for_topic_init(self.exchange_manager, timeout, topic)
+            self.logger.debug(
+                f"Trading mode requirements init complete: {', '.join(t for t in topics)} initialisation completed."
+            )
             return True
         except (asyncio.TimeoutError, concurrent.futures.TimeoutError):
             self.logger.error(f"Initialization took more than {timeout} seconds")
         return False
 
     async def init_user_inputs(self, should_clear_inputs):
         if should_clear_inputs:
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/modes/channel/mode.py` & `OctoBot-Trading-2.4.9/octobot_trading/modes/channel/mode.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/modes/mode_config.py` & `OctoBot-Trading-2.4.9/octobot_trading/modes/mode_config.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/modes/modes_factory.py` & `OctoBot-Trading-2.4.9/octobot_trading/modes/modes_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,69 +17,85 @@
 import octobot_commons.logging as logging
 
 import octobot_trading.errors as errors
 
 LOGGER_TAG = "TradingModeFactory"
 
 
-async def create_trading_modes(config: dict,
-                               exchange_manager,
-                               trading_mode_class,
-                               bot_id: str) -> list:
+async def create_trading_modes(
+    config: dict,
+    exchange_manager,
+    trading_mode_class,
+    bot_id: str,
+    trading_config_by_trading_mode: dict = None
+) -> list:
     is_symbol_wildcard = trading_mode_class.get_is_symbol_wildcard()
     if is_symbol_wildcard or (not is_symbol_wildcard and exchange_manager.exchange_config.traded_symbol_pairs):
-        return await _create_trading_modes(trading_mode_class=trading_mode_class,
-                                           config=config,
-                                           exchange_manager=exchange_manager,
-                                           cryptocurrencies=exchange_manager.exchange_config.traded_cryptocurrencies,
-                                           symbols=exchange_manager.exchange_config.traded_symbol_pairs,
-                                           time_frames=exchange_manager.exchange_config.traded_time_frames,
-                                           bot_id=bot_id)
+        return await _create_trading_modes(
+            trading_mode_class=trading_mode_class,
+            config=config,
+            exchange_manager=exchange_manager,
+            cryptocurrencies=exchange_manager.exchange_config.traded_cryptocurrencies,
+            symbols=exchange_manager.exchange_config.traded_symbol_pairs,
+            time_frames=exchange_manager.exchange_config.traded_time_frames,
+            bot_id=bot_id,
+            trading_config_by_trading_mode=trading_config_by_trading_mode
+        )
     # Do not create no symbol wildcard trading mode if no trading pair is available
     raise errors.TradingModeIncompatibility(
         f"As non symbol-wildcard trading mode, {trading_mode_class.get_name()} requires "
         f"at least one exchange trading pair to be initialized. "
         f"None of the required pairs are available on {exchange_manager.exchange_name}.")
 
 
-async def _create_trading_modes(trading_mode_class,
-                                config: dict,
-                                exchange_manager,
-                                cryptocurrencies: dict = None,
-                                symbols: list = None,
-                                time_frames: list = None,
-                                bot_id: str = None) -> list:
+async def _create_trading_modes(
+    trading_mode_class,
+    config: dict,
+    exchange_manager,
+    cryptocurrencies: dict = None,
+    symbols: list = None,
+    time_frames: list = None,
+    bot_id: str = None,
+    trading_config_by_trading_mode: dict = None
+) -> list:
+    trading_config_by_trading_mode = trading_config_by_trading_mode or {}
     return [
-        await create_trading_mode(trading_mode_class=trading_mode_class,
-                                  config=config,
-                                  exchange_manager=exchange_manager,
-                                  cryptocurrency=cryptocurrency,
-                                  symbol=symbol,
-                                  time_frame=time_frame,
-                                  bot_id=bot_id)
+        await create_trading_mode(
+            trading_mode_class=trading_mode_class,
+            config=config,
+            exchange_manager=exchange_manager,
+            cryptocurrency=cryptocurrency,
+            symbol=symbol,
+            time_frame=time_frame,
+            bot_id=bot_id,
+            trading_config=trading_config_by_trading_mode.get(trading_mode_class.get_name())
+        )
         for cryptocurrency in _get_cryptocurrencies_to_create(trading_mode_class, cryptocurrencies)
         for symbol in _get_symbols_to_create(trading_mode_class, cryptocurrencies, cryptocurrency, symbols)
         for time_frame in _get_time_frames_to_create(trading_mode_class, time_frames)
     ]
 
 
-async def create_trading_mode(trading_mode_class,
-                              config: dict,
-                              exchange_manager,
-                              cryptocurrency: str = None,
-                              symbol: str = None,
-                              time_frame: object = None,
-                              bot_id: str = None):
+async def create_trading_mode(
+    trading_mode_class,
+    config: dict,
+    exchange_manager,
+    cryptocurrency: str = None,
+    symbol: str = None,
+    time_frame: object = None,
+    bot_id: str = None,
+    trading_config: dict = None
+):
     try:
         trading_mode = trading_mode_class(config, exchange_manager)
         trading_mode.cryptocurrency = cryptocurrency
         trading_mode.symbol = symbol
         trading_mode.time_frame = time_frame
         trading_mode.bot_id = bot_id
-        await trading_mode.initialize()
+        await trading_mode.initialize(trading_config=trading_config)
         logging.get_logger(f"{LOGGER_TAG}[{exchange_manager.exchange_name}]") \
             .debug(f"{trading_mode.get_name()} started for "
                    f"[cryptocurrency={cryptocurrency if cryptocurrency else constants.CONFIG_WILDCARD},"
                    f" symbol={symbol if symbol else constants.CONFIG_WILDCARD},"
                    f" time_frame={time_frame if time_frame else constants.CONFIG_WILDCARD}]")
         return trading_mode
     except RuntimeError as e:
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/modes/modes_util.py` & `OctoBot-Trading-2.4.9/octobot_trading/modes/modes_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/basic_keywords/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/basic_keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/basic_keywords/account_balance.py` & `OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/basic_keywords/account_balance.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/basic_keywords/amount.py` & `OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/basic_keywords/amount.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/basic_keywords/configuration.py` & `OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/basic_keywords/configuration.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/basic_keywords/run_persistence.py` & `OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/basic_keywords/run_persistence.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/basic_keywords/trading_signals.py` & `OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/basic_keywords/trading_signals.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/basic_keywords/user_inputs.py` & `OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/basic_keywords/user_inputs.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/context_management.py` & `OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/context_management.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/dsl/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/dsl/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/dsl/quantity.py` & `OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/dsl/quantity.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/modes/script_keywords/dsl/values.py` & `OctoBot-Trading-2.4.9/octobot_trading/modes/script_keywords/dsl/values.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/modes/scripted_trading_mode/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/modes/scripted_trading_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/modes/scripted_trading_mode/abstract_scripted_trading_mode.py` & `OctoBot-Trading-2.4.9/octobot_trading/modes/scripted_trading_mode/abstract_scripted_trading_mode.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/octobot_channel_consumer.py` & `OctoBot-Trading-2.4.9/octobot_trading/octobot_channel_consumer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/exchange_personal_data.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/exchange_personal_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/channel/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/channel/orders.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/channel/orders.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         :param raw_order: the order dict
         """
         await self.channel.exchange_manager.exchange_personal_data.handle_closed_order_update(
             exchange_order_id, raw_order
         )
 
     async def handle_post_open_orders_update(
-            self, symbols, orders, waiting_complete_init_orders, has_new_order, is_from_bot
+        self, symbols, orders, waiting_complete_init_orders, has_new_order, is_from_bot
     ):
         """
         Perform post open Order update actions :
         - 1. Check if some previously known open order has not been found during update
         - 2. Force portfolio refresh if a new order has been loaded or waiting a init order exists
         - 3. Complete order init process when necessary
         :param symbols: the updated orders symbols
@@ -239,16 +239,18 @@
                         synchronize_tasks.append(order_to_update.state.synchronize(force_synchronization=True,
                                                                                    catch_exception=True))
                 except KeyError:
                     self.logger.error(f"Order with id {missing_order_id} could not be synchronized: "
                                       f"missing from order manager")
             await asyncio.gather(*synchronize_tasks)
 
-    async def send(self, cryptocurrency, symbol, order, is_from_bot=True,
-                   update_type=enums.OrderUpdateType.STATE_CHANGE, is_closed=False):
+    async def send(
+        self, cryptocurrency, symbol, order, is_from_bot=True,
+        update_type=enums.OrderUpdateType.STATE_CHANGE, is_closed=False
+    ):
         if is_closed or update_type is enums.OrderUpdateType.CLOSED:
             # do not push closed orders
             return
         for consumer in self.channel.get_filtered_consumers(symbol=symbol):
             await consumer.queue.put({
                 "exchange": self.channel.exchange_manager.exchange_name,
                 "exchange_id": self.channel.exchange_manager.id,
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/channel/orders_updater.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/channel/orders_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/channel/orders_updater_simulator.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/channel/orders_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/decimal_order_adapter.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/decimal_order_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/groups/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/groups/group_util.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/groups/group_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/order.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/order.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 import octobot_trading.constants as constants
 import octobot_trading.enums as enums
 import octobot_trading.errors as errors
 import octobot_trading.personal_data.orders.states as orders_states
 import octobot_trading.personal_data.orders.order_util as order_util
 import octobot_trading.util as util
-import octobot_trading.storage.orders_storage as orders_storage
 
 
 class Order(util.Initializable):
     """
     Order class will represent an open order in the specified exchange
     In simulation it will also define rules to be filled / canceled
     It is also use to store creation & fill values of the order
@@ -628,15 +627,15 @@
         self.is_waiting_for_chained_trigger = other_order.is_waiting_for_chained_trigger
 
         if other_order.state is not None:
             await other_order.state.replace_order(self)
 
     def update_from_storage_order_details(self, order_details):
         # rebind order attributes that are not stored on exchange
-        order_dict = order_details.get(orders_storage.OrdersStorage.ORIGIN_VALUE_KEY, {})
+        order_dict = order_details.get(constants.STORAGE_ORIGIN_VALUE, {})
         self.tag = order_dict.get(enums.ExchangeConstantsOrderColumns.TAG.value, self.tag)
         self.order_id = order_dict.get(enums.ExchangeConstantsOrderColumns.ID.value, self.order_id)
         self.exchange_order_id = order_dict.get(enums.ExchangeConstantsOrderColumns.EXCHANGE_ID.value,
                                                 self.exchange_order_id)
         self.trader_creation_kwargs = order_details.get(enums.StoredOrdersAttr.TRADER_CREATION_KWARGS.value,
                                                         self.trader_creation_kwargs)
         self.exchange_creation_params = order_details.get(enums.StoredOrdersAttr.EXCHANGE_CREATION_PARAMS.value,
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/order_adapter.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/order_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/order_factory.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/order_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import octobot_trading.personal_data as personal_data
 import octobot_trading.enums as enums
 import octobot_trading.constants as constants
-import octobot_trading.storage.orders_storage as orders_storage
 
 
 def create_order_from_raw(trader, raw_order):
     _, order_type = personal_data.parse_order_type(raw_order)
     return create_order_from_type(trader, order_type)
 
 
@@ -116,18 +115,18 @@
         timestamp=order_dict[enums.ExchangeConstantsOrderColumns.TIMESTAMP.value],
         side=enums.TradeOrderSide(order_dict[enums.ExchangeConstantsOrderColumns.SIDE.value]),
         tag=order_dict[enums.ExchangeConstantsOrderColumns.TAG.value],
         reduce_only=order_dict[enums.ExchangeConstantsOrderColumns.REDUCE_ONLY.value],
     )
 
 
-async def create_order_from_order_storage_details(order_storage_details, exchange_manager, pending_groups):
+async def create_order_from_order_storage_details(order_storage_details, exchange_manager, pending_groups: dict):
     order = create_order_from_dict(
         exchange_manager.trader,
-        order_storage_details[orders_storage.OrdersStorage.ORIGIN_VALUE_KEY]
+        order_storage_details[constants.STORAGE_ORIGIN_VALUE]
     )
     order.update_from_storage_order_details(order_storage_details)
     await personal_data.create_orders_storage_related_elements(
         order, order_storage_details, exchange_manager, pending_groups
     )
     return order
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/order_group.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/order_state.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/order_util.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/order_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/orders_manager.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/orders_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/orders_storage_operations.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/orders_storage_operations.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/states/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/states/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/states/cancel_order_state.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/states/cancel_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/states/close_order_state.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/states/close_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/states/fill_order_state.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/states/fill_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/states/open_order_state.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/states/open_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/states/order_state_factory.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/states/order_state_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/states/pending_creation_chained_order_state.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/states/pending_creation_chained_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/states/pending_creation_order_state.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/states/pending_creation_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/limit/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/limit/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/limit/buy_limit_order.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/limit/buy_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/limit/limit_order.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/limit/limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/limit/sell_limit_order.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/limit/sell_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/limit/stop_loss_order.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/limit/stop_loss_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/limit/take_profit_order.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/limit/take_profit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/market/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/market/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/market/buy_market_order.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/market/buy_market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/market/market_order.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/market/market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/market/sell_market_order.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/market/sell_market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/trailing/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/trailing/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/unknown_order.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/unknown_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/orders/types/unsupported_order.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/orders/types/unsupported_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/asset.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,10 +127,10 @@
         """
         Ensure update complete without raising PortfolioNegativeValueError else restore Asset instance's attributes
         """
         previous_asset = copy.copy(self)
         try:
             yield
         except errors.PortfolioNegativeValueError:
-            logging.get_logger(self.__class__.__name__).warning("Restoring after PortfolioNegativeValueError...")
+            logging.get_logger(self.__class__.__name__).info("Restoring after PortfolioNegativeValueError...")
             self.restore(previous_asset)
             raise
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/assets/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/assets/future_asset.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/assets/future_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/assets/margin_asset.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/assets/margin_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/assets/spot_asset.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/assets/spot_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/channel/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/channel/balance.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/channel/balance.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/channel/balance_updater.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/channel/balance_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/history/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/history/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/history/historical_asset_value.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/history/historical_asset_value.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/portfolio.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/portfolio.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,18 +179,24 @@
 
     def get_portfolio_from_amount_dict(self, amount_dict):
         """
         Create a portfolio from an amount dictionary
         :param amount_dict:
         :return: the portfolio dictionary
         """
-        if not all(isinstance(i, decimal.Decimal) for i in amount_dict.values()):
+        if not all(all(isinstance(v, decimal.Decimal) for v in values.values()) for values in amount_dict.values()):
             raise RuntimeError("Portfolio has to be initialized using decimal.Decimal")
-        return {currency: self.create_currency_asset(currency=currency, available=total, total=total).to_dict()
-                for currency, total in amount_dict.items()}
+        return {
+            currency: self.create_currency_asset(
+                currency=currency,
+                available=values[common_constants.PORTFOLIO_AVAILABLE],
+                total=values[common_constants.PORTFOLIO_TOTAL]
+            ).to_dict()
+            for currency, values in amount_dict.items()
+        }
 
     def _update_portfolio_data(self, currency, total_value=constants.ZERO, available_value=constants.ZERO,
                                replace_value=False):
         """
         Set new currency quantity in the portfolio
         :param currency: the currency to update
         :param total_value: the total update value
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/portfolio_factory.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/portfolio_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/portfolio_manager.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/portfolio_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,25 +41,25 @@
 
         self.portfolio = None
         self.portfolio_profitability = None
         self.portfolio_value_holder = None
         self.historical_portfolio_value_manager = None
         self.reference_market = None
         self._is_initialized_event_set = False
-        self._simulated_portfolio_initial_config = None
+        self._forced_portfolio = None
 
     async def initialize_impl(self):
         """
         Reset the portfolio instance
         """
 
         if self.exchange_manager.is_storage_enabled() and self.historical_portfolio_value_manager is None:
             self.historical_portfolio_value_manager = personal_data.HistoricalPortfolioValueManager(self)
             await self.historical_portfolio_value_manager.initialize()
-        self.set_simulated_portfolio_initial_config(
+        self.set_forced_portfolio_initial_config(
             self.config[commons_constants.CONFIG_SIMULATOR][commons_constants.CONFIG_STARTING_PORTFOLIO]
         )
         self._reset_portfolio()
 
     def handle_balance_update(self, balance, is_diff_update=False):
         """
         Handle a balance update request
@@ -266,37 +266,44 @@
         Load simulated portfolio from config if required
         """
         if self.trader.is_enabled:
             if self.trader.simulate:
                 if reset_from_config \
                         or self.historical_portfolio_value_manager is None \
                         or not self.historical_portfolio_value_manager.has_previous_session_portfolio():
-                    self._apply_starting_simulated_portfolio()
+                    self.apply_forced_portfolio()
                 else:
                     self._load_simulated_portfolio_from_history()
-            self.logger.info(f"{constants.CURRENT_PORTFOLIO_STRING} {self.portfolio.portfolio}")
+            self.logger.debug(f"{constants.CURRENT_PORTFOLIO_STRING} {self.portfolio.portfolio}")
 
     def _load_simulated_portfolio_from_history(self):
-        #  todo also load available amounts when loading simulated orders
         portfolio_amount_dict = personal_data.parse_decimal_config_portfolio(
             {
-                symbol: value[commons_constants.PORTFOLIO_TOTAL]
+                symbol: value
                 for symbol, value in self.historical_portfolio_value_manager.historical_ending_portfolio.items()
             }
         )
         self.handle_balance_update(self.portfolio.get_portfolio_from_amount_dict(portfolio_amount_dict))
 
-    def set_simulated_portfolio_initial_config(self, portfolio_config):
-        self._simulated_portfolio_initial_config = copy.deepcopy(portfolio_config)
+    def set_forced_portfolio_initial_config(self, portfolio_config):
+        forced_portfolio_initial_config = copy.deepcopy(portfolio_config)
+        # ensure free and total amounts are present
+        for key in list(forced_portfolio_initial_config):
+            if not isinstance(forced_portfolio_initial_config[key], dict):
+                forced_portfolio_initial_config[key] = {
+                    commons_constants.PORTFOLIO_AVAILABLE: forced_portfolio_initial_config[key],
+                    commons_constants.PORTFOLIO_TOTAL: forced_portfolio_initial_config[key],
+                }
+        self._forced_portfolio = forced_portfolio_initial_config
 
-    def _apply_starting_simulated_portfolio(self):
+    def apply_forced_portfolio(self):
         """
         Load new portfolio from config settings
         """
-        portfolio_amount_dict = personal_data.parse_decimal_config_portfolio(self._simulated_portfolio_initial_config)
+        portfolio_amount_dict = personal_data.parse_decimal_config_portfolio(self._forced_portfolio)
         self.handle_balance_update(self.portfolio.get_portfolio_from_amount_dict(portfolio_amount_dict))
 
     def _set_initialized_event(self):
         commons_tree.EventProvider.instance().trigger_event(
             self.exchange_manager.bot_id, commons_tree.get_exchange_path(
                 self.exchange_manager.exchange_name,
                 commons_enums.InitializationEventExchangeTopics.BALANCE.value
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/portfolio_profitability.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/portfolio_profitability.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/portfolio_util.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/portfolio_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,16 @@
                 if isinstance(balance_val, (int, float, decimal.Decimal)):
                     portfolio_to_fill[balance_type] = decimal.Decimal(str(balance_val))
     return decimal_portfolio
 
 
 def parse_decimal_config_portfolio(portfolio):
     return {
-        symbol: decimal.Decimal(str(symbol_balance))
+        symbol: {k: decimal.Decimal(str(v)) for k, v in symbol_balance.items()} if isinstance(symbol_balance, dict)
+        else decimal.Decimal(str(symbol_balance))
         for symbol, symbol_balance in portfolio.items()
     }
 
 
 def filter_empty_values(portfolio):
     return {
         symbol: value
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/portfolio_value_holder.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/portfolio_value_holder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/sub_portfolio.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/sub_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/types/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/types/future_portfolio.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/types/future_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/types/margin_portfolio.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/types/margin_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/types/spot_portfolio.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/types/spot_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/portfolios/value_converter.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/portfolios/value_converter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/channel/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/channel/positions.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/channel/positions.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/channel/positions_updater.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/channel/positions_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/channel/positions_updater_simulator.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/channel/positions_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/position.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/position.py`

 * *Files 1% similar despite different names*

```diff
@@ -893,10 +893,10 @@
         """
         Ensure update complete without raising PortfolioNegativeValueError else restore Position instance's attributes
         """
         previous_position = copy.copy(self)
         try:
             yield
         except errors.PortfolioNegativeValueError:
-            logging.get_logger(self.get_logger_name()).warning("Restoring after PortfolioNegativeValueError...")
+            logging.get_logger(self.get_logger_name()).info("Restoring after PortfolioNegativeValueError...")
             self.restore(previous_position)
             raise
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/position_factory.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/position_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/position_state.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/position_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/position_util.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/position_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/positions_manager.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/positions_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/states/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/states/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/states/active_position_state.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/states/active_position_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/states/idle_position_state.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/states/idle_position_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/states/liquidate_position_state.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/states/liquidate_position_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/states/position_state_factory.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/states/position_state_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/types/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/types/inverse_position.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/types/inverse_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/positions/types/linear_position.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/positions/types/linear_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/state.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/trades/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/trades/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/trades/channel/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/trades/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/trades/channel/trades.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/trades/channel/trades.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/trades/channel/trades_updater.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/trades/channel/trades_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/trades/trade.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/trades/trade.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/trades/trade_factory.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/trades/trade_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/trades/trade_pnl.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/trades/trade_pnl.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/trades/trades_manager.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/trades/trades_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/trades/trades_util.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/trades/trades_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/transactions/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/transactions/transaction.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/transactions/transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/transactions/transaction_factory.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/transactions/transaction_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/transactions/transactions_manager.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/transactions/transactions_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/transactions/types/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/transactions/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/transactions/types/blockchain_transaction.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/transactions/types/blockchain_transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/transactions/types/fee_transaction.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/transactions/types/fee_transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/transactions/types/realised_pnl_transaction.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/transactions/types/realised_pnl_transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/personal_data/transactions/types/transfer_transaction.py` & `OctoBot-Trading-2.4.9/octobot_trading/personal_data/transactions/types/transfer_transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/signals/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/signals/channel/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/signals/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/signals/channel/remote_trading_signal.py` & `OctoBot-Trading-2.4.9/octobot_trading/signals/channel/remote_trading_signal.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/signals/channel/remote_trading_signal_channel_factory.py` & `OctoBot-Trading-2.4.9/octobot_trading/signals/channel/remote_trading_signal_channel_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/signals/channel/signal_producer.py` & `OctoBot-Trading-2.4.9/octobot_trading/signals/channel/signal_producer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/signals/signal_creation.py` & `OctoBot-Trading-2.4.9/octobot_trading/signals/signal_creation.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             for chained_order in order.chained_orders
         ]
     created_order = await exchange_manager.trader.create_order(
         order, loaded=loaded, params=params,
         wait_for_creation=wait_for_creation, creation_timeout=creation_timeout
     )
     if created_order is not None and should_emit_signal:
-        builder = signals.SignalPublisher.instance().get_signal_bundle_builder(order.symbol)
+        builder = signals.SignalPublisher.instance().get_signal_bundle_builder(created_order.symbol)
         builder.add_created_order(
             created_order, exchange_manager, target_amount=order_pf_percent
         )
         for chained_order, chained_order_pf_percent in chained_orders_pf_percent:
             builder.add_created_order(
                 chained_order, exchange_manager, target_amount=chained_order_pf_percent
             )
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/signals/trading_signal_bundle_builder.py` & `OctoBot-Trading-2.4.9/octobot_trading/signals/trading_signal_bundle_builder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/signals/util.py` & `OctoBot-Trading-2.4.9/octobot_trading/signals/util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/storage/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/storage/abstract_storage.py` & `OctoBot-Trading-2.4.9/octobot_trading/storage/abstract_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,25 +18,25 @@
 import decimal
 import types
 
 import octobot_commons.display as commons_display
 import octobot_commons.logging as logging
 
 import octobot_trading.exchange_channel as exchanges_channel
+import octobot_trading.constants as trading_constants
 
 
 class AbstractStorage:
     IS_LIVE_CONSUMER = True
     USE_LIVE_CONSUMER_IN_BACKTESTING = False
     LIVE_CHANNEL = None
     IS_HISTORICAL = True
     HISTORY_TABLE = None
     AUTH_UPDATE_DEBOUNCE_DURATION = 1
     FLUSH_DEBOUNCE_DURATION = 0.5   # avoid disc spam on multiple quick live updated
-    ORIGIN_VALUE_KEY = "origin_value"
 
     def __init__(self, exchange_manager, plot_settings: commons_display.PlotSettings,
                  use_live_consumer_in_backtesting=None, is_historical=None):
         self.exchange_manager = exchange_manager
         self.plot_settings: commons_display.PlotSettings = plot_settings
         self.consumer = None
         self.use_live_consumer_in_backtesting = use_live_consumer_in_backtesting \
@@ -112,17 +112,17 @@
         if self._flush_task is not None and not self._flush_task.done():
             self._flush_task.cancel()
         self._flush_task = asyncio.create_task(self._waiting_flush())
 
     async def get_history(self):
         # override if necessary
         return [
-            copy.copy(document[self.ORIGIN_VALUE_KEY])
+            copy.copy(document[trading_constants.STORAGE_ORIGIN_VALUE])
             for document in await self._get_db().all(self.HISTORY_TABLE)
-            if self.ORIGIN_VALUE_KEY in document
+            if trading_constants.STORAGE_ORIGIN_VALUE in document
         ]
 
     async def _waiting_update_auth_data(self, reset):
         try:
             await asyncio.sleep(self.AUTH_UPDATE_DEBOUNCE_DURATION)
             await self._update_auth_data(reset)
         except Exception as err:
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/storage/candles_storage.py` & `OctoBot-Trading-2.4.9/octobot_trading/storage/candles_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/storage/orders_storage.py` & `OctoBot-Trading-2.4.9/octobot_trading/storage/orders_storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,55 +100,31 @@
 
     async def get_startup_order_details(self, order_exchange__id):
         return self.startup_orders.get(order_exchange__id, None)
 
     async def _load_startup_orders(self):
         if self.should_store_date():
             self.startup_orders = {
-                _get_startup_order_key(order): self._from_order_document(order)
+                _get_startup_order_key(order): _from_order_document(order)
                 for order in copy.deepcopy(await self._get_db().all(self.HISTORY_TABLE))
                 if order    # skip empty order details (error when serializing)
             }
         else:
             self.startup_orders = {}
 
     def get_startup_self_managed_orders_details_from_group(self, group_id):
         return [
             order
             for order in self.startup_orders.values()
             if order.get(enums.StoredOrdersAttr.GROUP.value, {}).get(enums.StoredOrdersAttr.GROUP_ID.value, None)
             == group_id
-            and order.get(OrdersStorage.ORIGIN_VALUE_KEY, {})
+            and order.get(constants.STORAGE_ORIGIN_VALUE, {})
             .get(enums.ExchangeConstantsOrderColumns.SELF_MANAGED.value, False)
         ]
 
-    def _from_order_document(self, order_document):
-        order_dict = dict(order_document)
-        try:
-            origin_val = order_dict[OrdersStorage.ORIGIN_VALUE_KEY]
-            origin_val[enums.ExchangeConstantsOrderColumns.AMOUNT.value] = \
-                decimal.Decimal(str(origin_val[enums.ExchangeConstantsOrderColumns.AMOUNT.value]))
-            origin_val[enums.ExchangeConstantsOrderColumns.COST.value] = \
-                decimal.Decimal(str(origin_val[enums.ExchangeConstantsOrderColumns.COST.value]))
-            origin_val[enums.ExchangeConstantsOrderColumns.FILLED.value] = \
-                decimal.Decimal(str(origin_val[enums.ExchangeConstantsOrderColumns.FILLED.value]))
-            origin_val[enums.ExchangeConstantsOrderColumns.PRICE.value] = \
-                decimal.Decimal(str(origin_val[enums.ExchangeConstantsOrderColumns.PRICE.value]))
-            if origin_val[enums.ExchangeConstantsOrderColumns.FEE.value] and \
-                    enums.FeePropertyColumns.COST.value in origin_val[enums.ExchangeConstantsOrderColumns.FEE.value]:
-                origin_val[enums.ExchangeConstantsOrderColumns.FEE.value][enums.FeePropertyColumns.COST.value] = \
-                    decimal.Decimal(str(
-                        origin_val[enums.ExchangeConstantsOrderColumns.FEE.value][enums.FeePropertyColumns.COST.value]
-                    ))
-        except Exception as err:
-            commons_logging.get_logger(OrdersStorage.__name__).exception(
-                err, True, f"Error when reading: {err} order: {order_document}"
-            )
-        return order_dict
-
     @classmethod
     async def clear_database_history(cls, database, flush=True):
         await super().clear_database_history(database, flush=False)
         if cls.ENABLE_HISTORICAL_ORDER_UPDATES_STORAGE:
             await database.delete(cls.HISTORICAL_OPEN_ORDERS_TABLE, None)
         if flush:
             await database.flush()
@@ -174,15 +150,15 @@
         for chained_order in order.chained_orders
     ]
 
 
 def _format_order(order, exchange_manager):
     try:
         return {
-            OrdersStorage.ORIGIN_VALUE_KEY: OrdersStorage.sanitize_for_storage(order.to_dict()),
+            constants.STORAGE_ORIGIN_VALUE: OrdersStorage.sanitize_for_storage(order.to_dict()),
             enums.StoredOrdersAttr.EXCHANGE_CREATION_PARAMS.value:
                 OrdersStorage.sanitize_for_storage(order.exchange_creation_params),
             enums.StoredOrdersAttr.TRADER_CREATION_KWARGS.value:
                 OrdersStorage.sanitize_for_storage(order.trader_creation_kwargs),
             enums.StoredOrdersAttr.HAS_BEEN_BUNDLED.value: order.has_been_bundled,
             enums.StoredOrdersAttr.ENTRIES.value: order.associated_entry_ids,
             enums.StoredOrdersAttr.GROUP.value: _get_group_dict(order),
@@ -211,17 +187,41 @@
             exchange_manager.exchange_personal_data.orders_manager.get_order(order_id),
             exchange_manager
         )
     except KeyError:
         if status == enums.OrderStatus.OPEN.value:
             # ensure order details are present in open orders
             details = {
-                OrdersStorage.ORIGIN_VALUE_KEY: OrdersStorage.sanitize_for_storage(order_dict),
+                constants.STORAGE_ORIGIN_VALUE: OrdersStorage.sanitize_for_storage(order_dict),
             }
     order_update[enums.StoredOrdersAttr.ORDER_DETAILS.value] = details
     return order_update
 
 
+def _from_order_document(order_document):
+    order_dict = dict(order_document)
+    try:
+        origin_val = order_dict[constants.STORAGE_ORIGIN_VALUE]
+        origin_val[enums.ExchangeConstantsOrderColumns.AMOUNT.value] = \
+            decimal.Decimal(str(origin_val[enums.ExchangeConstantsOrderColumns.AMOUNT.value]))
+        origin_val[enums.ExchangeConstantsOrderColumns.COST.value] = \
+            decimal.Decimal(str(origin_val[enums.ExchangeConstantsOrderColumns.COST.value]))
+        origin_val[enums.ExchangeConstantsOrderColumns.FILLED.value] = \
+            decimal.Decimal(str(origin_val[enums.ExchangeConstantsOrderColumns.FILLED.value]))
+        origin_val[enums.ExchangeConstantsOrderColumns.PRICE.value] = \
+            decimal.Decimal(str(origin_val[enums.ExchangeConstantsOrderColumns.PRICE.value]))
+        if origin_val[enums.ExchangeConstantsOrderColumns.FEE.value] and \
+                enums.FeePropertyColumns.COST.value in origin_val[enums.ExchangeConstantsOrderColumns.FEE.value]:
+            origin_val[enums.ExchangeConstantsOrderColumns.FEE.value][enums.FeePropertyColumns.COST.value] = \
+                decimal.Decimal(str(
+                    origin_val[enums.ExchangeConstantsOrderColumns.FEE.value][enums.FeePropertyColumns.COST.value]
+                ))
+    except Exception as err:
+        commons_logging.get_logger(OrdersStorage.__name__).exception(
+            err, True, f"Error when reading: {err} order: {order_document}"
+        )
+    return order_dict
+
 def _get_startup_order_key(order_dict):
     # use exchange id if available, fallback to order_id (for self managed orders)
-    return order_dict[OrdersStorage.ORIGIN_VALUE_KEY][enums.ExchangeConstantsOrderColumns.EXCHANGE_ID.value] or \
-        order_dict[OrdersStorage.ORIGIN_VALUE_KEY][enums.ExchangeConstantsOrderColumns.ID.value]
+    return order_dict[constants.STORAGE_ORIGIN_VALUE][enums.ExchangeConstantsOrderColumns.EXCHANGE_ID.value] or \
+        order_dict[constants.STORAGE_ORIGIN_VALUE][enums.ExchangeConstantsOrderColumns.ID.value]
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/storage/portfolio_storage.py` & `OctoBot-Trading-2.4.9/octobot_trading/storage/portfolio_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/storage/storage_manager.py` & `OctoBot-Trading-2.4.9/octobot_trading/storage/storage_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/storage/trades_storage.py` & `OctoBot-Trading-2.4.9/octobot_trading/storage/trades_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #  License along with this library
 import octobot_commons.channels_name as channels_name
 import octobot_commons.enums as commons_enums
 import octobot_commons.authentication as authentication
 import octobot_commons.databases as commons_databases
 
 import octobot_trading.enums as enums
+import octobot_trading.constants as constants
 import octobot_trading.storage.abstract_storage as abstract_storage
 import octobot_trading.storage.util as storage_util
 
 
 class TradesStorage(abstract_storage.AbstractStorage):
     LIVE_CHANNEL = channels_name.OctoBotTradingChannelsName.TRADES_CHANNEL.value
     HISTORY_TABLE = commons_enums.DBTables.TRADES.value
@@ -51,21 +52,21 @@
             await self.trigger_debounced_flush()
             self._to_update_auth_data_ids_buffer.add(trade[enums.ExchangeConstantsOrderColumns.ID.value])
             await self.trigger_debounced_update_auth_data(False)
 
     async def _update_auth_data(self, reset):
         authenticator = authentication.Authenticator.instance()
         history = [
-            trade
+            trade.to_dict()
             for trade in self.exchange_manager.exchange_personal_data.trades_manager.trades.values()
             if trade.status is not enums.OrderStatus.CANCELED and trade.trade_id in self._to_update_auth_data_ids_buffer
         ]
         if (history or reset) and authenticator.is_initialized():
             # also update when history is empty to reset trade history
-            await authenticator.update_trades(history, reset)
+            await authenticator.update_trades(history, self.exchange_manager.exchange_name, reset)
             self._to_update_auth_data_ids_buffer.clear()
 
     async def _store_history(self):
         database = self._get_db()
         await database.replace_all(
             self.HISTORY_TABLE,
             [
@@ -137,15 +138,15 @@
         else:
             color = "magenta"
             shape = "arrow-bar-left"
     fee = trade_dict[enums.ExchangeConstantsOrderColumns.FEE.value]
     fee_cost = float(fee[enums.FeePropertyColumns.COST.value] if
                      fee and fee[enums.FeePropertyColumns.COST.value] else 0)
     return {
-        TradesStorage.ORIGIN_VALUE_KEY: TradesStorage.sanitize_for_storage(trade_dict),
+        constants.STORAGE_ORIGIN_VALUE: TradesStorage.sanitize_for_storage(trade_dict),
         commons_enums.DisplayedElementTypes.CHART.value: chart,
         commons_enums.DBRows.SYMBOL.value: trade_dict[enums.ExchangeConstantsOrderColumns.SYMBOL.value],
         commons_enums.DBRows.FEES_AMOUNT.value: fee_cost,
         commons_enums.DBRows.FEES_CURRENCY.value: fee[enums.FeePropertyColumns.CURRENCY.value]
         if trade_dict[enums.ExchangeConstantsOrderColumns.FEE.value] else "",
         commons_enums.DBRows.ID.value: trade_dict[enums.ExchangeConstantsOrderColumns.ID.value],
         commons_enums.DBRows.TRADING_MODE.value: exchange_manager.trading_modes[0].get_name(),
```

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/storage/transactions_storage.py` & `OctoBot-Trading-2.4.9/octobot_trading/storage/transactions_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/storage/util.py` & `OctoBot-Trading-2.4.9/octobot_trading/storage/util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/supervisors/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/supervisors/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/supervisors/abstract_portfolio_supervisor.py` & `OctoBot-Trading-2.4.9/octobot_trading/supervisors/abstract_portfolio_supervisor.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/supervisors/abstract_supervisor.py` & `OctoBot-Trading-2.4.9/octobot_trading/supervisors/abstract_supervisor.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/util/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/util/config_util.py` & `OctoBot-Trading-2.4.9/octobot_trading/util/config_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/util/initializable.py` & `OctoBot-Trading-2.4.9/octobot_trading/util/initializable.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/util/initialization_util.py` & `OctoBot-Trading-2.4.9/octobot_trading/util/initialization_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/util/simulator_updater_utils.py` & `OctoBot-Trading-2.4.9/octobot_trading/util/simulator_updater_utils.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/util/test_tools/__init__.py` & `OctoBot-Trading-2.4.9/octobot_trading/util/test_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/util/test_tools/spot_rest_exchange_test_tools.py` & `OctoBot-Trading-2.4.9/octobot_trading/util/test_tools/spot_rest_exchange_test_tools.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/octobot_trading/util/test_tools/websocket_test_tools.py` & `OctoBot-Trading-2.4.9/octobot_trading/util/test_tools/websocket_test_tools.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/requirements.txt` & `OctoBot-Trading-2.4.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/setup.py` & `OctoBot-Trading-2.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/api/__init__.py` & `OctoBot-Trading-2.4.9/tests/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/api/test_channels.py` & `OctoBot-Trading-2.4.9/tests/api/test_channels.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/api/test_exchange.py` & `OctoBot-Trading-2.4.9/tests/api/test_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/api/test_modes.py` & `OctoBot-Trading-2.4.9/tests/api/test_modes.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/api/test_orders.py` & `OctoBot-Trading-2.4.9/tests/api/test_orders.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/api/test_portfolio.py` & `OctoBot-Trading-2.4.9/tests/api/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/api/test_profitability.py` & `OctoBot-Trading-2.4.9/tests/api/test_profitability.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/api/test_symbol_data.py` & `OctoBot-Trading-2.4.9/tests/api/test_symbol_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/api/test_trader.py` & `OctoBot-Trading-2.4.9/tests/api/test_trader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/api/test_trades.py` & `OctoBot-Trading-2.4.9/tests/api/test_trades.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/cli/__init__.py` & `OctoBot-Trading-2.4.9/tests/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchange_data/__init__.py` & `OctoBot-Trading-2.4.9/tests/exchange_data/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchange_data/contracts/__init__.py` & `OctoBot-Trading-2.4.9/tests/exchange_data/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchange_data/contracts/test_future_contract.py` & `OctoBot-Trading-2.4.9/tests/exchange_data/contracts/test_future_contract.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchange_data/contracts/test_margin_contract.py` & `OctoBot-Trading-2.4.9/tests/exchange_data/contracts/test_margin_contract.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchange_data/funding/__init__.py` & `OctoBot-Trading-2.4.9/tests/exchange_data/funding/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchange_data/funding/test_funding_manager.py` & `OctoBot-Trading-2.4.9/tests/exchange_data/funding/test_funding_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchange_data/kline/__init__.py` & `OctoBot-Trading-2.4.9/tests/exchange_data/kline/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchange_data/kline/test_kline_manager.py` & `OctoBot-Trading-2.4.9/tests/exchange_data/kline/test_kline_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchange_data/ohlcv/__init__.py` & `OctoBot-Trading-2.4.9/tests/exchange_data/ohlcv/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchange_data/ohlcv/test_candles_adapter.py` & `OctoBot-Trading-2.4.9/tests/exchange_data/ohlcv/test_candles_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchange_data/ohlcv/test_candles_manager.py` & `OctoBot-Trading-2.4.9/tests/exchange_data/ohlcv/test_candles_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchange_data/order_book/__init__.py` & `OctoBot-Trading-2.4.9/tests/exchange_data/order_book/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchange_data/order_book/test_order_book_manager.py` & `OctoBot-Trading-2.4.9/tests/exchange_data/order_book/test_order_book_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchange_data/prices/__init__.py` & `OctoBot-Trading-2.4.9/tests/exchange_data/prices/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchange_data/prices/test_price_events_manager.py` & `OctoBot-Trading-2.4.9/tests/exchange_data/prices/test_price_events_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchange_data/prices/test_prices_manager.py` & `OctoBot-Trading-2.4.9/tests/exchange_data/prices/test_prices_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchange_data/recent_trades/__init__.py` & `OctoBot-Trading-2.4.9/tests/exchange_data/recent_trades/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchange_data/recent_trades/test_recent_trades_manager.py` & `OctoBot-Trading-2.4.9/tests/exchange_data/recent_trades/test_recent_trades_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchange_data/test_exchange_symbols_data.py` & `OctoBot-Trading-2.4.9/tests/exchange_data/test_exchange_symbols_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchange_data/ticker/__init__.py` & `OctoBot-Trading-2.4.9/tests/exchange_data/ticker/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchange_data/ticker/test_ticker_manager.py` & `OctoBot-Trading-2.4.9/tests/exchange_data/ticker/test_ticker_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchanges/__init__.py` & `OctoBot-Trading-2.4.9/tests/exchanges/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,27 +32,40 @@
 from octobot_trading.exchanges.implementations.default_rest_exchange import DefaultRestExchange
 from octobot_trading.exchanges.connectors.ccxt.ccxt_connector import CCXTConnector
 from octobot_trading.exchanges.traders.trader_simulator import TraderSimulator
 import octobot_trading.personal_data as personal_data
 from octobot_trading.enums import FeePropertyColumns, ExchangeConstantsMarketPropertyColumns, \
     ExchangeConstantsMarketPropertyColumns
 
+import tests.exchanges.connectors.ccxt.mock_exchanges_data as mock_exchanges_data
+
 pytestmark = pytest.mark.asyncio
 
 TESTS_FOLDER = "tests"
 TESTS_STATIC_FOLDER = os.path.join(TESTS_FOLDER, "static")
 DEFAULT_EXCHANGE_NAME = "binanceus"
 DEFAULT_FUTURE_EXCHANGE_NAME = "bybit"
 
 
 class MockedCCXTConnector(CCXTConnector):
     @classmethod
     def get_name(cls):
         return DEFAULT_EXCHANGE_NAME
 
+    async def load_symbol_markets(self, reload=False, forced_markets=None):
+        if forced_markets is None:
+            forced_markets = mock_exchanges_data.MOCKED_EXCHANGE_INFO.get(self.exchange_manager.exchange_name, None)
+        await super().load_symbol_markets(
+            reload=reload,
+            forced_markets=forced_markets
+        )
+
+    def _should_authenticate(self):
+        return False
+
 
 class MockedRestExchange(DefaultRestExchange):
     DEFAULT_CONNECTOR_CLASS = MockedCCXTConnector
 
     @classmethod
     def get_exchange_connector_class(cls, exchange_manager):
         return cls.DEFAULT_CONNECTOR_CLASS
```

### Comparing `OctoBot-Trading-2.4.8/tests/exchanges/connectors/__init__.py` & `OctoBot-Trading-2.4.9/tests/exchanges/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchanges/connectors/ccxt/test_ccxt_connector.py` & `OctoBot-Trading-2.4.9/tests/exchanges/connectors/ccxt/test_ccxt_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,23 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import decimal
-import pytest
 
-import ccxt.async_support
-from mock import patch, Mock
+from mock import patch
 
 import octobot_trading.exchanges.connectors as exchange_connectors
 import octobot_trading.enums as enums
 import octobot_trading.exchange_data.contracts as contracts
 import pytest
 
+import tests.exchanges.connectors.ccxt.mock_exchanges_data as mock_exchanges_data
 from tests.exchanges import exchange_manager, future_simulated_exchange_manager, set_future_exchange_fees
 from tests.exchanges.traders import future_trader, future_trader_simulator_with_default_linear, DEFAULT_FUTURE_SYMBOL, \
     DEFAULT_FUTURE_SYMBOL_MARGIN_TYPE, DEFAULT_FUTURE_SYMBOL_LEVERAGE
 
 # All test coroutines will be treated as marked.
 pytestmark = pytest.mark.asyncio
 
@@ -149,15 +148,18 @@
            _get_fees("taker", "BTC", 0.001, decimal.Decimal("0.00045"))
     assert spot_ccxt_exchange.get_trade_fee(spot_symbol, enums.TraderOrderType.SELL_LIMIT, decimal.Decimal("0.45"),
                                             decimal.Decimal(10000), "maker") == \
            _get_fees("maker", "USDT", 0.001, decimal.Decimal("4.5"))
 
     # future trading
     fut_ccxt_exchange.client.options['defaultType'] = enums.ExchangeTypes.FUTURE.value
-    await fut_ccxt_exchange.client.load_markets()
+
+    await fut_ccxt_exchange.load_symbol_markets(
+        forced_markets=mock_exchanges_data.MOCKED_EXCHANGE_INFO.get(fut_exchange_manager_inst.exchange_name, None)
+    )
     # enforce taker and maker values
     set_future_exchange_fees(fut_ccxt_exchange, future_symbol, taker=future_fees_value, maker=future_fees_value)
     assert future_fees_value / 5 <= fut_ccxt_exchange.client.markets[future_symbol]['taker'] <= future_fees_value * 5
     # linear
     assert fut_ccxt_exchange.get_trade_fee(future_symbol, enums.TraderOrderType.BUY_LIMIT, decimal.Decimal("0.45"),
                                            decimal.Decimal(10000), "taker") == \
            _get_fees("taker", "USDT", future_fees_value, decimal.Decimal("1.800000"))
```

### Comparing `OctoBot-Trading-2.4.8/tests/exchanges/implementations/__init__.py` & `OctoBot-Trading-2.4.9/tests/exchanges/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchanges/implementations/test_default_rest_exchange.py` & `OctoBot-Trading-2.4.9/tests/exchanges/implementations/test_default_rest_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchanges/implementations/test_default_websocket_exchange.py` & `OctoBot-Trading-2.4.9/tests/exchanges/implementations/test_default_websocket_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchanges/test_abstract_exchange.py` & `OctoBot-Trading-2.4.9/tests/exchanges/test_abstract_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchanges/test_abstract_websocket_exchange.py` & `OctoBot-Trading-2.4.9/tests/exchanges/test_abstract_websocket_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchanges/test_exchange_builder.py` & `OctoBot-Trading-2.4.9/tests/exchanges/test_exchange_builder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchanges/test_exchange_config_data.py` & `OctoBot-Trading-2.4.9/tests/exchanges/test_exchange_config_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchanges/test_exchange_factory.py` & `OctoBot-Trading-2.4.9/tests/exchanges/test_exchange_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchanges/test_exchange_manager.py` & `OctoBot-Trading-2.4.9/tests/exchanges/test_exchange_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchanges/test_exchange_simulator.py` & `OctoBot-Trading-2.4.9/tests/exchanges/test_exchange_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchanges/test_exchanges.py` & `OctoBot-Trading-2.4.9/tests/exchanges/test_exchanges.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         config = await self.init_default()
 
         exchange_manager_binance = ExchangeManager(config, "binanceus")
         await exchange_manager_binance.initialize()
         Exchanges.instance().add_exchange(exchange_manager_binance, "")
 
         exchange_manager_bybit = ExchangeManager(config, "bybit")
+        exchange_manager_bybit.exchange_only = True
         await exchange_manager_bybit.initialize()
         Exchanges.instance().add_exchange(exchange_manager_bybit, "")
 
         assert "binanceus" in Exchanges.instance().exchanges
         assert "bybit" in Exchanges.instance().exchanges
         assert "test" not in Exchanges.instance().exchanges
```

### Comparing `OctoBot-Trading-2.4.8/tests/exchanges/traders/__init__.py` & `OctoBot-Trading-2.4.9/tests/exchanges/traders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchanges/traders/test_trader.py` & `OctoBot-Trading-2.4.9/tests/exchanges/traders/test_trader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchanges/types/__init__.py` & `OctoBot-Trading-2.4.9/tests/exchanges/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchanges/types/test_websocket_exchange.py` & `OctoBot-Trading-2.4.9/tests/exchanges/types/test_websocket_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchanges/util/__init__.py` & `OctoBot-Trading-2.4.9/tests/exchanges/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchanges/util/test_exchange_market_status_fixer.py` & `OctoBot-Trading-2.4.9/tests/exchanges/util/test_exchange_market_status_fixer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/exchanges/util/test_exchange_util.py` & `OctoBot-Trading-2.4.9/tests/exchanges/util/test_exchange_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/modes/__init__.py` & `OctoBot-Trading-2.4.9/tests/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/modes/script_keywords/__init__.py` & `OctoBot-Trading-2.4.9/tests/modes/script_keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/modes/script_keywords/basic_keywords/test_account_balance.py` & `OctoBot-Trading-2.4.9/tests/modes/script_keywords/basic_keywords/test_account_balance.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/modes/script_keywords/basic_keywords/test_amount.py` & `OctoBot-Trading-2.4.9/tests/modes/script_keywords/basic_keywords/test_amount.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/modes/script_keywords/dsl/__init__.py` & `OctoBot-Trading-2.4.9/tests/modes/script_keywords/dsl/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/modes/script_keywords/dsl/test_quantity.py` & `OctoBot-Trading-2.4.9/tests/modes/script_keywords/dsl/test_quantity.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/modes/test_abstract_mode_consumer.py` & `OctoBot-Trading-2.4.9/tests/modes/test_abstract_mode_consumer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/modes/test_abstract_trading_mode.py` & `OctoBot-Trading-2.4.9/tests/modes/test_abstract_trading_mode.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/__init__.py` & `OctoBot-Trading-2.4.9/tests/personal_data/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/__init__.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/groups/__init__.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/groups/test_balanced_take_profit_and_stop_order_group.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/groups/test_balanced_take_profit_and_stop_order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/groups/test_group_util.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/groups/test_group_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/groups/test_one_cancels_the_other_order_group.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/groups/test_one_cancels_the_other_order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/states/__init__.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/states/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/states/test_cancel_order_state.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/states/test_cancel_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/states/test_close_order_state.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/states/test_close_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/states/test_fill_order_state.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/states/test_fill_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/states/test_open_order_state.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/states/test_open_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/states/test_order_state.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/states/test_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/states/test_order_state_factory.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/states/test_order_state_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,31 +9,35 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import mock
 import octobot_trading.personal_data as personal_data
 from octobot_trading.enums import OrderStatus, OrderStates, States
 from octobot_trading.personal_data.orders import create_order_state
 
 import pytest
 from tests import event_loop
 from tests.exchanges import simulated_trader, simulated_exchange_manager
 from tests.personal_data.orders import buy_limit_order
 
 pytestmark = pytest.mark.asyncio
 
 
 async def test_create_order_state_pending_creation(buy_limit_order):
     buy_limit_order.status = OrderStatus.PENDING_CREATION
-    await create_order_state(buy_limit_order)
-    assert isinstance(buy_limit_order.state, personal_data.PendingCreationOrderState)
-    assert buy_limit_order.state.state is States.PENDING_CREATION
+    with mock.patch.object(personal_data.PendingCreationOrderState, "_synchronize_with_exchange", mock.AsyncMock()) as \
+        _synchronize_with_exchange_mock:
+        await create_order_state(buy_limit_order)
+        _synchronize_with_exchange_mock.assert_called_once()
+        assert isinstance(buy_limit_order.state, personal_data.PendingCreationOrderState)
+        assert buy_limit_order.state.state is States.PENDING_CREATION
 
 
 async def test_create_order_state_pending_chained_creation(buy_limit_order):
     buy_limit_order.status = OrderStatus.PENDING_CREATION
     buy_limit_order.is_waiting_for_chained_trigger = True
     await create_order_state(buy_limit_order)
     assert isinstance(buy_limit_order.state, personal_data.PendingCreationChainedOrderState)
```

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/states/test_pending_creation_chained_order_state.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/states/test_pending_creation_chained_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/states/test_pending_creation_order_state.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/states/test_pending_creation_order_state.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,29 +9,34 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import mock
+
 import octobot_trading.personal_data as personal_data
 from octobot_trading.enums import OrderStatus, OrderStates, States
 from octobot_trading.personal_data.orders.states.order_state_factory import create_order_state
 from tests import event_loop
 from tests.exchanges import simulated_trader, simulated_exchange_manager
 from tests.personal_data.orders import buy_limit_order
 import pytest
 
 pytestmark = pytest.mark.asyncio
 
 
 async def test_on_order_refresh_successful(buy_limit_order):
     buy_limit_order.exchange_manager.is_backtesting = True
     buy_limit_order.status = OrderStatus.PENDING_CREATION
-    await buy_limit_order.initialize()
+    with mock.patch.object(personal_data.PendingCreationOrderState, "_synchronize_with_exchange", mock.AsyncMock()) as \
+        _synchronize_with_exchange_mock:
+        await buy_limit_order.initialize()
+        _synchronize_with_exchange_mock.assert_called_once()
     assert isinstance(buy_limit_order.state, personal_data.PendingCreationOrderState)
     await buy_limit_order.state.on_refresh_successful()
     assert buy_limit_order.state.state is States.PENDING_CREATION
     buy_limit_order.status = OrderStatus.PENDING_CREATION
     await buy_limit_order.state.on_refresh_successful()
     buy_limit_order.status = OrderStatus.PENDING_CREATION
     assert buy_limit_order.is_created() is True
```

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/test_decimal_order_adapter.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/test_decimal_order_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/test_double_filled_order.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/test_double_filled_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/test_order.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/test_order.py`

 * *Files 0% similar despite different names*

```diff
@@ -400,15 +400,15 @@
     assert order.exchange_order_id is origin_exchange_order_id
     assert order.has_been_bundled is origin_has_been_bundled
     assert order.associated_entry_ids is origin_associated_entry_ids
     assert order.update_with_triggering_order_fees is origin_update_with_triggering_order_fees
 
     # full update
     order.update_from_storage_order_details({
-        orders_storage.OrdersStorage.ORIGIN_VALUE_KEY: {
+        constants.STORAGE_ORIGIN_VALUE: {
             enums.ExchangeConstantsOrderColumns.TAG.value: "t1",
             enums.ExchangeConstantsOrderColumns.ID.value: "11a",
             enums.ExchangeConstantsOrderColumns.EXCHANGE_ID.value: "eee1",
         },
         enums.StoredOrdersAttr.TRADER_CREATION_KWARGS.value: {"plop2": 1},
         enums.StoredOrdersAttr.EXCHANGE_CREATION_PARAMS.value: {"ex": 2, "gg": "yesyes"},
         enums.StoredOrdersAttr.HAS_BEEN_BUNDLED.value: True,
```

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/test_order_adapter.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/test_order_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/test_order_factory.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/test_order_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/test_order_util.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/test_order_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/test_orders_manager.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/test_orders_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/test_orders_storage_operations.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/test_orders_storage_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import mock
 import pytest
 import pytest_asyncio
 import decimal
 
 import octobot_trading.enums as enums
 import octobot_trading.personal_data as personal_data
-import octobot_trading.storage as storage
+import octobot_trading.constants as constants
 
 from tests import event_loop
 from tests.exchanges import exchange_manager, simulated_exchange_manager
 from tests.exchanges.traders import trader_simulator
 from tests.exchanges.traders import trader
 
 # All test coroutines will be treated as marked.
@@ -66,15 +66,15 @@
     await personal_data.apply_order_storage_details_if_any(order, exchange_manager_inst, {})
     mocked_order_storage.get_startup_order_details.assert_awaited_once_with("plop exchange_id")
 
     # ensure order update is done
     assert order.order_id != "new id 123"
     assert order.exchange_order_id != "new exchange id 123"
     mocked_order_storage.get_startup_order_details = mock.AsyncMock(return_value={
-        storage.OrdersStorage.ORIGIN_VALUE_KEY: {
+        constants.STORAGE_ORIGIN_VALUE: {
             enums.ExchangeConstantsOrderColumns.ID.value: "new id 123",
             enums.ExchangeConstantsOrderColumns.EXCHANGE_ID.value: "new exchange id 123"
         }
     })
     await personal_data.apply_order_storage_details_if_any(order, exchange_manager_inst, {})
     mocked_order_storage.get_startup_order_details.assert_awaited_once_with("plop exchange_id")
     assert order.order_id == "new id 123"
```

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/types/__init__.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/types/limit/test_buy_limit_order.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/types/limit/test_buy_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/types/limit/test_sell_limit_order.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/types/limit/test_sell_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/types/limit/test_stop_loss_limit_order.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/types/limit/test_stop_loss_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/types/limit/test_stop_loss_order.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/types/limit/test_stop_loss_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/types/limit/test_take_profit_limit_order.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/types/limit/test_take_profit_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/types/limit/test_take_profit_order.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/types/limit/test_take_profit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/types/market/test_buy_market_order.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/types/market/test_buy_market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/types/market/test_sell_market_order.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/types/market/test_sell_market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/types/test_unknown_order.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/types/test_unknown_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/types/trailing/__init__.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/types/trailing/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/types/trailing/test_trailing_stop_limit_order.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/types/trailing/test_trailing_stop_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/orders/types/trailing/test_trailing_stop_order.py` & `OctoBot-Trading-2.4.9/tests/personal_data/orders/types/trailing/test_trailing_stop_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/portfolios/__init__.py` & `OctoBot-Trading-2.4.9/tests/personal_data/portfolios/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/portfolios/assets/__init__.py` & `OctoBot-Trading-2.4.9/tests/personal_data/portfolios/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/portfolios/assets/test_future_asset.py` & `OctoBot-Trading-2.4.9/tests/personal_data/portfolios/assets/test_future_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/portfolios/assets/test_margin_asset.py` & `OctoBot-Trading-2.4.9/tests/personal_data/portfolios/assets/test_margin_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/portfolios/assets/test_spot_asset.py` & `OctoBot-Trading-2.4.9/tests/personal_data/portfolios/assets/test_spot_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/portfolios/history/test_historical_asset_value_factory.py` & `OctoBot-Trading-2.4.9/tests/personal_data/portfolios/history/test_historical_asset_value_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/portfolios/history/test_historical_portfolio_value_manager.py` & `OctoBot-Trading-2.4.9/tests/personal_data/portfolios/history/test_historical_portfolio_value_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/portfolios/test_asset.py` & `OctoBot-Trading-2.4.9/tests/personal_data/portfolios/test_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/portfolios/test_portfolio.py` & `OctoBot-Trading-2.4.9/tests/personal_data/portfolios/test_portfolio.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,23 +63,38 @@
     assert pf1 != pf2
 
 
 async def test_get_portfolio_from_amount_dict(backtesting_trader):
     config, exchange_manager, trader = backtesting_trader
     portfolio_manager = exchange_manager.exchange_personal_data.portfolio_manager
     assert portfolio_manager.portfolio.get_portfolio_from_amount_dict(
-        {"zyx": decimal.Decimal(str(10)), "BTC": decimal.Decimal('1')}) == {
-               'zyx': {'available': decimal.Decimal('10'), 'total': decimal.Decimal('10')},
-               'BTC': {'available': decimal.Decimal('1'), 'total': decimal.Decimal('1')}
+        {"zyx": {commons_constants.PORTFOLIO_AVAILABLE: decimal.Decimal('10'),
+                 commons_constants.PORTFOLIO_TOTAL: decimal.Decimal('24')},
+         "BTC": {commons_constants.PORTFOLIO_AVAILABLE: decimal.Decimal('0.1'),
+                 commons_constants.PORTFOLIO_TOTAL: decimal.Decimal('0.1')}}) == {
+               'zyx': {'available': decimal.Decimal('10'), 'total': decimal.Decimal('24')},
+               'BTC': {'available': decimal.Decimal('0.1'), 'total': decimal.Decimal('0.1')}
            }
     assert portfolio_manager.portfolio.get_portfolio_from_amount_dict({}) == {}
     with pytest.raises(RuntimeError):
-        portfolio_manager.portfolio.get_portfolio_from_amount_dict({"zyx": "10", "BTC": decimal.Decimal('1')})
+        portfolio_manager.portfolio.get_portfolio_from_amount_dict({
+            "zyx":  {commons_constants.PORTFOLIO_AVAILABLE: decimal.Decimal('10'),
+                     commons_constants.PORTFOLIO_TOTAL: '24'},
+            "BTC":  {commons_constants.PORTFOLIO_AVAILABLE: decimal.Decimal('10'),
+                     commons_constants.PORTFOLIO_TOTAL: decimal.Decimal('24')},
+        })
     with pytest.raises(RuntimeError):
-        portfolio_manager.portfolio.get_portfolio_from_amount_dict({"BTC": 1})
+        portfolio_manager.portfolio.get_portfolio_from_amount_dict({
+            "zyx":  {commons_constants.PORTFOLIO_AVAILABLE: decimal.Decimal('10'),
+                     commons_constants.PORTFOLIO_TOTAL: 24},
+            "BTC":  {commons_constants.PORTFOLIO_AVAILABLE: decimal.Decimal('10'),
+                     commons_constants.PORTFOLIO_TOTAL: decimal.Decimal('24')},
+        })
+    with pytest.raises(AttributeError):
+        portfolio_manager.portfolio.get_portfolio_from_amount_dict({"BTC":  '10'})
 
 
 async def test_get_currency_portfolio(backtesting_trader):
     config, exchange_manager, trader = backtesting_trader
     portfolio_manager = exchange_manager.exchange_personal_data.portfolio_manager
     assert portfolio_manager.portfolio.get_currency_portfolio("BTC").available == decimal.Decimal('10')
     assert portfolio_manager.portfolio.get_currency_portfolio("BTC").total == decimal.Decimal('10')
```

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/portfolios/test_portfolio_manager.py` & `OctoBot-Trading-2.4.9/tests/personal_data/portfolios/test_portfolio_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/portfolios/test_portfolio_profitability.py` & `OctoBot-Trading-2.4.9/tests/personal_data/portfolios/test_portfolio_profitability.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/portfolios/test_portfolio_value_holder.py` & `OctoBot-Trading-2.4.9/tests/personal_data/portfolios/test_portfolio_value_holder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/portfolios/test_value_converter.py` & `OctoBot-Trading-2.4.9/tests/personal_data/portfolios/test_value_converter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/portfolios/types/__init__.py` & `OctoBot-Trading-2.4.9/tests/personal_data/portfolios/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/portfolios/types/test_future_portfolio.py` & `OctoBot-Trading-2.4.9/tests/personal_data/portfolios/types/test_future_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/portfolios/types/test_margin_portfolio.py` & `OctoBot-Trading-2.4.9/tests/personal_data/portfolios/types/test_margin_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/portfolios/types/test_spot_portfolio.py` & `OctoBot-Trading-2.4.9/tests/personal_data/portfolios/types/test_spot_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/positions/__init__.py` & `OctoBot-Trading-2.4.9/tests/personal_data/positions/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/positions/channel/__init__.py` & `OctoBot-Trading-2.4.9/tests/personal_data/positions/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/positions/states/__init__.py` & `OctoBot-Trading-2.4.9/tests/personal_data/positions/states/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/positions/test_position.py` & `OctoBot-Trading-2.4.9/tests/personal_data/positions/test_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/positions/test_position_factory.py` & `OctoBot-Trading-2.4.9/tests/personal_data/positions/test_position_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/positions/test_positions_manager.py` & `OctoBot-Trading-2.4.9/tests/personal_data/positions/test_positions_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/positions/types/__init__.py` & `OctoBot-Trading-2.4.9/tests/personal_data/positions/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/positions/types/test_inverse_position.py` & `OctoBot-Trading-2.4.9/tests/personal_data/positions/types/test_inverse_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/positions/types/test_linear_position.py` & `OctoBot-Trading-2.4.9/tests/personal_data/positions/types/test_linear_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/trades/__init__.py` & `OctoBot-Trading-2.4.9/tests/personal_data/trades/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/trades/test_trade_factory.py` & `OctoBot-Trading-2.4.9/tests/personal_data/trades/test_trade_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/trades/test_trade_manager.py` & `OctoBot-Trading-2.4.9/tests/personal_data/trades/test_trade_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/trades/test_trade_pnl.py` & `OctoBot-Trading-2.4.9/tests/personal_data/trades/test_trade_pnl.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/transactions/__init__.py` & `OctoBot-Trading-2.4.9/tests/personal_data/transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/transactions/test_transaction_factory.py` & `OctoBot-Trading-2.4.9/tests/personal_data/transactions/test_transaction_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/personal_data/transactions/test_transactions_manager.py` & `OctoBot-Trading-2.4.9/tests/personal_data/transactions/test_transactions_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/signals/__init__.py` & `OctoBot-Trading-2.4.9/tests/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/signals/test_trading_signal_bundle_builder.py` & `OctoBot-Trading-2.4.9/tests/signals/test_trading_signal_bundle_builder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/signals/test_util.py` & `OctoBot-Trading-2.4.9/tests/signals/test_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/test_utils/order_util.py` & `OctoBot-Trading-2.4.9/tests/test_utils/order_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/test_utils/random_numbers.py` & `OctoBot-Trading-2.4.9/tests/test_utils/random_numbers.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/util/__init__.py` & `OctoBot-Trading-2.4.9/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests/util/test_config_util.py` & `OctoBot-Trading-2.4.9/tests/util/test_config_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/__init__.py` & `OctoBot-Trading-2.4.9/tests_additional/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/__init__.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/real_exchange_tester.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/real_exchange_tester.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/real_futures_exchange_tester.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/real_futures_exchange_tester.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_ascendex.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_ascendex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_binance.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_binance.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_binance_futures.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_binance_futures.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_bitfinex.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_bitfinex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_bitget.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_bitget.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_bithumb.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_bithumb.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_bitso.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_bitso.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_bitstamp.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_bitstamp.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_bittrex.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_bittrex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_bybit.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_bybit.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_bybit_futures.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_bybit_futures.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_coinbase.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_coinbase.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_coinex.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_coinex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_cryptocom.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_cryptocom.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_gateio.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_gateio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_hitbtc.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_hitbtc.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_hollaex.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_hollaex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_huobi.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_huobi.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_huobipro.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_huobipro.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_kraken.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_kraken.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_kucoin.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_kucoin.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_kucoin_futures.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_kucoin_futures.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_mexc.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_mexc.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_ndax.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_ndax.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_okcoin.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_okcoin.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_okx.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_okx.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_okx_futures.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_okx_futures.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_phemex.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_phemex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_poloniex.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_poloniex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_upbit.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_upbit.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.8/tests_additional/real_exchanges/test_wavesexchange.py` & `OctoBot-Trading-2.4.9/tests_additional/real_exchanges/test_wavesexchange.py`

 * *Files identical despite different names*

