# Comparing `tmp/quantnb-0.2.9.tar.gz` & `tmp/quantnb-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantnb-0.2.9.tar", max compression
+gzip compressed data, was "quantnb-0.3.1.tar", max compression
```

## Comparing `quantnb-0.2.9.tar` & `quantnb-0.3.1.tar`

### file list

```diff
@@ -1,42 +1,73 @@
--rw-r--r--   0        0        0      112 2023-06-07 12:08:16.607057 quantnb-0.2.9/README.md
--rw-r--r--   0        0        0      615 2023-07-18 12:51:30.631981 quantnb-0.2.9/pyproject.toml
--rw-r--r--   0        0        0      280 2023-06-08 09:33:29.937029 quantnb-0.2.9/quantnb/__init__.py
--rw-r--r--   0        0        0     8567 2023-07-18 12:51:02.298676 quantnb-0.2.9/quantnb/core/backtester.py
--rw-r--r--   0        0        0     8199 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/core/backtester_old.py
--rw-r--r--   0        0        0       80 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/core/enums.py
--rw-r--r--   0        0        0     2900 2023-07-18 12:51:02.288676 quantnb-0.2.9/quantnb/helpers/H_ticks_to_ranges.py
--rw-r--r--   0        0        0     1337 2023-06-30 23:07:30.161852 quantnb-0.2.9/quantnb/helpers/S_calculate_metrics.py
--rw-r--r--   0        0        0      357 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/helpers/S_print_orders.py
--rw-r--r--   0        0        0      728 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/helpers/S_print_trades.py
--rw-r--r--   0        0        0      300 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/helpers/__init__.py
--rw-r--r--   0        0        0      793 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/helpers/analyze_trade_duration.py
--rw-r--r--   0        0        0      380 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/helpers/calculate_average_freq.py
--rw-r--r--   0        0        0     1038 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/helpers/calculate_pf_stats.py
--rw-r--r--   0        0        0      390 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/helpers/calculate_risk_free.py
--rw-r--r--   0        0        0      213 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/helpers/get_average_trade_duration.py
--rw-r--r--   0        0        0      672 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/helpers/get_realized_pf_value.py
--rw-r--r--   0        0        0      325 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/helpers/plot_lines.py
--rw-r--r--   0        0        0      731 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/helpers/save_to_csv.py
--rw-r--r--   0        0        0      109 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/indicators/EMA.py
--rw-r--r--   0        0        0      351 2023-07-14 18:13:59.469996 quantnb-0.2.9/quantnb/indicators/HMA.py
--rw-r--r--   0        0        0      109 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/indicators/SMA.py
--rw-r--r--   0        0        0       79 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/indicators/__init__.py
--rw-r--r--   0        0        0      160 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/indicators/cross_below.py
--rw-r--r--   0        0        0     1502 2023-07-14 18:18:10.994171 quantnb-0.2.9/quantnb/indicators/random_data.py
--rw-r--r--   0        0        0     1253 2023-07-14 18:07:37.591031 quantnb-0.2.9/quantnb/indicators/supertrend.py
--rw-r--r--   0        0        0      391 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/lib/__init__.py
--rw-r--r--   0        0        0     1143 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/lib/create_binance_dataframe.py
--rw-r--r--   0        0        0      905 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/lib/fetch_binance_data.py
--rw-r--r--   0        0        0      359 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/lib/find_files.py
--rw-r--r--   0        0        0     1131 2023-07-05 11:15:06.173263 quantnb-0.2.9/quantnb/lib/multiprocess.py
--rw-r--r--   0        0        0      889 2023-07-13 14:40:24.770094 quantnb-0.2.9/quantnb/lib/optimize.py
--rw-r--r--   0        0        0      241 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/lib/resample.py
--rw-r--r--   0        0        0     3666 2023-07-01 00:15:50.699650 quantnb-0.2.9/quantnb/strategies/S_MACD.py
--rw-r--r--   0        0        0     3088 2023-07-18 12:51:02.298676 quantnb-0.2.9/quantnb/strategies/S_base.py
--rw-r--r--   0        0        0     1776 2023-07-18 12:51:02.298676 quantnb-0.2.9/quantnb/strategies/S_bid_ask.py
--rw-r--r--   0        0        0     2245 2023-07-17 17:01:19.633674 quantnb-0.2.9/quantnb/strategies/S_test.py
--rw-r--r--   0        0        0       29 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/strategies/__init__.py
--rw-r--r--   0        0        0      678 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/tests/benchmark_multiple_assets.py
--rw-r--r--   0        0        0      698 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/tests/optimisation_combine_files.py
--rw-r--r--   0        0        0      682 2023-07-14 18:18:30.134596 quantnb-0.2.9/quantnb/tests/supertrend_test.py
--rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 quantnb-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0      276 2023-08-05 09:14:09.397106 quantnb-0.3.1/README.md
+-rw-r--r--   0        0        0     1095 2023-08-05 09:14:09.829109 quantnb-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      282 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/__init__.py
+-rw-r--r--   0        0        0     1901 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/core/PNL.py
+-rw-r--r--   0        0        0      246 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/core/__init__.py
+-rw-r--r--   0        0        0    12236 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/core/backtester.old.py
+-rw-r--r--   0        0        0     4250 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/core/backtester.py
+-rw-r--r--   0        0        0     2236 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/core/base.py
+-rw-r--r--   0        0        0      341 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/core/calculate_commission.py
+-rw-r--r--   0        0        0      517 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/core/calculate_entry_price.py
+-rw-r--r--   0        0        0      516 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/core/calculate_exit_price.py
+-rw-r--r--   0        0        0     3001 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/core/data_module.py
+-rw-r--r--   0        0        0      847 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/core/enums.py
+-rw-r--r--   0        0        0      473 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/core/helpers.py
+-rw-r--r--   0        0        0     2377 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/core/place_orders_on_ohlc.py
+-rw-r--r--   0        0        0      909 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/core/specs_nb.py
+-rw-r--r--   0        0        0       94 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/core/test.py
+-rw-r--r--   0        0        0      515 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/core/trade_add_trade_to_active_trades.py
+-rw-r--r--   0        0        0      974 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/core/trade_close_trade.py
+-rw-r--r--   0        0        0     1183 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/core/trade_create_new_trade.py
+-rw-r--r--   0        0        0     5060 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/core/trade_module.py
+-rw-r--r--   0        0        0      696 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/core/trade_remove_from_active_trades.py
+-rw-r--r--   0        0        0      647 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/core/trade_should_trade_close.py
+-rw-r--r--   0        0        0      558 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/core/update_trades_pnl.py
+-rw-r--r--   0        0        0     2900 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/helpers/H_ticks_to_ranges.py
+-rw-r--r--   0        0        0     1337 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/helpers/S_calculate_metrics.py
+-rw-r--r--   0        0        0      357 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/helpers/S_print_orders.py
+-rw-r--r--   0        0        0      754 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/helpers/S_print_trades.py
+-rw-r--r--   0        0        0      300 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/helpers/__init__.py
+-rw-r--r--   0        0        0      793 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/helpers/analyze_trade_duration.py
+-rw-r--r--   0        0        0      380 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/helpers/calculate_average_freq.py
+-rw-r--r--   0        0        0     1038 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/helpers/calculate_pf_stats.py
+-rw-r--r--   0        0        0      390 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/helpers/calculate_risk_free.py
+-rw-r--r--   0        0        0      213 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/helpers/get_average_trade_duration.py
+-rw-r--r--   0        0        0      672 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/helpers/get_realized_pf_value.py
+-rw-r--r--   0        0        0      325 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/helpers/plot_lines.py
+-rw-r--r--   0        0        0      731 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/helpers/save_to_csv.py
+-rw-r--r--   0        0        0      109 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/indicators/EMA.py
+-rw-r--r--   0        0        0      351 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/indicators/HMA.py
+-rw-r--r--   0        0        0     1233 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/indicators/I_donchian.py
+-rw-r--r--   0        0        0      109 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/indicators/SMA.py
+-rw-r--r--   0        0        0      198 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/indicators/__init__.py
+-rw-r--r--   0        0        0      221 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/indicators/cross_above.py
+-rw-r--r--   0        0        0      222 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/indicators/cross_below.py
+-rw-r--r--   0        0        0     1732 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/indicators/random_data.py
+-rw-r--r--   0        0        0     1253 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/indicators/supertrend.py
+-rw-r--r--   0        0        0      505 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/lib/__init__.py
+-rw-r--r--   0        0        0     3145 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/lib/calculate_stats.py
+-rw-r--r--   0        0        0      147 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/lib/convert_signal_to_markers.py
+-rw-r--r--   0        0        0     1143 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/lib/create_binance_dataframe.py
+-rw-r--r--   0        0        0     1044 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/lib/fetch_binance_data.py
+-rw-r--r--   0        0        0      466 2023-08-05 09:14:09.829109 quantnb-0.3.1/quantnb/lib/find_files.py
+-rw-r--r--   0        0        0     3828 2023-08-05 09:14:09.833109 quantnb-0.3.1/quantnb/lib/helpers.py
+-rw-r--r--   0        0        0     1131 2023-08-05 09:14:09.833109 quantnb-0.3.1/quantnb/lib/multiprocess.py
+-rw-r--r--   0        0        0     1305 2023-08-05 09:14:09.833109 quantnb-0.3.1/quantnb/lib/optimize.py
+-rw-r--r--   0        0        0      685 2023-08-05 09:14:09.833109 quantnb-0.3.1/quantnb/lib/output_trades.py
+-rw-r--r--   0        0        0     4591 2023-08-05 09:14:09.833109 quantnb-0.3.1/quantnb/lib/plotting.py
+-rw-r--r--   0        0        0     2058 2023-08-05 09:14:09.833109 quantnb-0.3.1/quantnb/lib/qs.py
+-rw-r--r--   0        0        0      241 2023-08-05 09:14:09.833109 quantnb-0.3.1/quantnb/lib/resample.py
+-rw-r--r--   0        0        0      881 2023-08-05 09:14:09.833109 quantnb-0.3.1/quantnb/lib/time_manip.py
+-rw-r--r--   0        0        0     3666 2023-08-05 09:14:09.833109 quantnb-0.3.1/quantnb/strategies/S_MACD.py
+-rw-r--r--   0        0        0     3592 2023-08-05 09:14:09.833109 quantnb-0.3.1/quantnb/strategies/S_base.py
+-rw-r--r--   0        0        0     1776 2023-08-05 09:14:09.833109 quantnb-0.3.1/quantnb/strategies/S_bid_ask.py
+-rw-r--r--   0        0        0       29 2023-08-05 09:14:09.833109 quantnb-0.3.1/quantnb/strategies/__init__.py
+-rw-r--r--   0        0        0     2245 2023-08-05 09:14:09.833109 quantnb-0.3.1/quantnb/strategies/s_temp.py
+-rw-r--r--   0        0        0      678 2023-08-05 09:14:09.833109 quantnb-0.3.1/quantnb/tests/benchmark_multiple_assets.py
+-rw-r--r--   0        0        0        0 2023-08-05 09:14:09.833109 quantnb-0.3.1/quantnb/tests/core_calculate_trade_price.py
+-rw-r--r--   0        0        0      698 2023-08-05 09:14:09.833109 quantnb-0.3.1/quantnb/tests/optimisation_combine_files.py
+-rw-r--r--   0        0        0      742 2023-08-05 09:14:09.833109 quantnb-0.3.1/quantnb/tests/supertrend.py
+-rw-r--r--   0        0        0      635 2023-08-05 09:14:09.833109 quantnb-0.3.1/quantnb/tests/test_calculate_commission.py
+-rw-r--r--   0        0        0     2993 2023-08-05 09:14:09.833109 quantnb-0.3.1/quantnb/tests/test_calculate_entry_exit_price.py
+-rw-r--r--   0        0        0     5531 2023-08-05 09:14:09.833109 quantnb-0.3.1/quantnb/tests/test_trade.py
+-rw-r--r--   0        0        0     1428 1970-01-01 00:00:00.000000 quantnb-0.3.1/PKG-INFO
```

### Comparing `quantnb-0.2.9/pyproject.toml` & `quantnb-0.3.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,49 @@
 [tool.poetry]
 name = "quantnb"
-version = "0.2.9"
+version = "0.3.1"
 description = ""
 authors = ["Alpha <piotr@piotryordanov.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 numba = "^0.57.0"
 numpy = "^1.24.3"
 pandas = "^2.0.1"
 ta-lib = "^0.4.26"
-quantstats = "^0.0.59"
 matplotlib = "^3.7.1"
 pyarrow = "^12.0.0"
 mplfinance = "^0.12.9b7"
 tqdm = "^4.65.0"
-python-binance = "^1.0.17"
-seaborn = {extras = ["stats"], version = "^0.12.2"}
-ipython = "^8.14.0"
-polars = "^0.18.4"
+prettytable = "^3.8.0"
+
+python-binance = {version = "^1.0.17", optional = true}
+quantstats = {version = "^0.0.59", optional = true}
+seaborn = {version = "^0.12.2", extras = ["stats"], optional = true}
+ipython = {version = "^8.14.0", optional = true}
 pandas-ta = {version = "^0.3.14b0", optional = true}
+pytest = "^7.4.0"
+pytest-watcher = "^0.3.4"
+pyright = "^1.1.320"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.extras]
+dev_tools = ["python-binance", "quantstats", "seaborn", "ipython", "pandas-ta"]
+
+[tool.pytest-watcher]
+now = true
+runner = "pytest"
+runner_args = []
+patterns = ["*.py"]
+ignore_patterns = []
+
+[tool.pytest.ini_options]
+pythonpath = "quantnb"
+addopts = "-s"
+testpaths = [
+    "tests",
+]
```

### Comparing `quantnb-0.2.9/quantnb/helpers/H_ticks_to_ranges.py` & `quantnb-0.3.1/quantnb/helpers/H_ticks_to_ranges.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.9/quantnb/helpers/S_calculate_metrics.py` & `quantnb-0.3.1/quantnb/helpers/S_calculate_metrics.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.9/quantnb/helpers/S_print_trades.py` & `quantnb-0.3.1/quantnb/helpers/S_print_trades.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
         trades_arr,
         columns=[
             "entry_time",
             "exit_time",
             "entry_price",
             "exit_price",
             "pnl",
+            "commission",
             "size",
             "direction",
         ],
     )
     # Mapping dictionary for column renaming
     rename_dict = {1: "LONG", 0: "SHORT"}
```

### Comparing `quantnb-0.2.9/quantnb/helpers/analyze_trade_duration.py` & `quantnb-0.3.1/quantnb/helpers/analyze_trade_duration.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.9/quantnb/helpers/calculate_pf_stats.py` & `quantnb-0.3.1/quantnb/helpers/calculate_pf_stats.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.9/quantnb/helpers/get_realized_pf_value.py` & `quantnb-0.3.1/quantnb/helpers/get_realized_pf_value.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.9/quantnb/helpers/save_to_csv.py` & `quantnb-0.3.1/quantnb/helpers/save_to_csv.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.9/quantnb/indicators/random_data.py` & `quantnb-0.3.1/quantnb/indicators/random_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 # from quantnb.indicators.supertrend import supertrend
 # from quantnb.indicators.SMA import SMA
 # import mplfinance as mpf
 # import random
 import pandas as pd
 import numpy as np
+from quantnb.lib.time_manip import time_manip
 
 
 def random_data(seed=None):
     if seed:
         np.random.seed(seed)
 
     # Define parameters
@@ -38,14 +39,18 @@
             "open": open_prices,
             "high": high_prices,
             "low": low_prices,
             "close": close_prices,
         }
     )
     ohlc_data.set_index("date", inplace=True)
+    ohlc_data.dtype = np.float32
+
+    date = time_manip.convert_datetime_to_s(ohlc_data.index).values
     return (
-        ohlc_data["open"].values,
-        ohlc_data["high"].values,
-        ohlc_data["low"].values,
-        ohlc_data["close"].values,
+        date,
+        ohlc_data.open.to_numpy(dtype=np.float32),
+        ohlc_data.high.to_numpy(dtype=np.float32),
+        ohlc_data.low.to_numpy(dtype=np.float32),
+        ohlc_data.close.to_numpy(dtype=np.float32),
         ohlc_data,
     )
```

### Comparing `quantnb-0.2.9/quantnb/indicators/supertrend.py` & `quantnb-0.3.1/quantnb/indicators/supertrend.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.9/quantnb/lib/create_binance_dataframe.py` & `quantnb-0.3.1/quantnb/lib/create_binance_dataframe.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.9/quantnb/lib/fetch_binance_data.py` & `quantnb-0.3.1/quantnb/lib/fetch_binance_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,39 +2,46 @@
 import pandas as pd
 import mplfinance as mpf
 from .multiprocess import multiprocess
 from .create_binance_dataframe import create_binance_dataframe
 
 
 def get_data(asset, tf=Client.KLINE_INTERVAL_1HOUR, days="3000 day ago UTC"):
-    asset = asset[0]
+    # asset = asset[0]
     print(f"Getting data for {asset} on {tf}")
     client = Client()
     klines = client.get_historical_klines(asset, tf, days)
 
     df = create_binance_dataframe(klines)
-    df.to_parquet(f"data/binance-{asset}-1h.parquet")
+    df.to_parquet(f"data/binance-{asset}-{tf}.parquet")
 
 
 assets = [
-    "BTCUSDT",
     "ETHUSDT",
+    "BTCUSDT",
     "DOGEUSDT",
     "BNBUSDT",
     "ATOMUSDT",
     "NEOUSDT",
     "NEOUSDT",
     "XRPUSDT",
     "LTCUSDT",
     "TRXUSDT",
     "AVAXUSDT",
     "SHIBUSDT",
     "ATOMUSDT",
     "LINKUSDT",
     "UNIUSDT",
+    "ADAUSDT",
+    "DOTUSDT",
+    "SOLUSDT",
+    "MATICUSDT",
+    "XLMUSDT",
 ]
 
 
 def fetch_binance_data(
-    assets=assets, tf=Client.KLINE_INTERVAL_15MINUTE, days="3000 day ago UTC"
+    assets=assets, tf=Client.KLINE_INTERVAL_1HOUR, days="3000 day ago UTC"
 ):
-    multiprocess(assets, get_data, tf, days)
+    # multiprocess(assets, get_data, tf, days)
+    for asset in assets:
+        get_data(asset, tf, days)
```

### Comparing `quantnb-0.2.9/quantnb/lib/multiprocess.py` & `quantnb-0.3.1/quantnb/lib/multiprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def worker(method, items, NUMBER_OF_CPU, iteration, args, queue):
     result = method(items, NUMBER_OF_CPU, iteration, *args)
     queue.put(result)
 
 
 def multiprocess(items, method, *args):
-    NUMBER_OF_CPU = multiprocessing.cpu_count() - 1
+    NUMBER_OF_CPU = multiprocessing.cpu_count() - 2
 
     # Calculate the length of each part
     part_length = math.ceil(len(items) / NUMBER_OF_CPU)
     divided_list = [
         items[i : i + part_length] for i in range(0, len(items), part_length)
     ]
```

### Comparing `quantnb-0.2.9/quantnb/lib/optimize.py` & `quantnb-0.3.1/quantnb/lib/optimize.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 import pandas as pd
 import itertools
 from tqdm import tqdm
 from . import find_files, multiprocess
 
 
-def optimize(data, strategy, **kwargs):
+# def optimize(data, strategy, strategy_params=None, **kwargs):
+def optimize(data, strategy, INITIAL_CAPITAL, **kwargs):
     kwargs = list(kwargs.values())
     total_combinations = list(itertools.product(*kwargs))
     print("Total combinations to test: ", len(total_combinations))
 
     def execution(params, NUMBER_OF_CPU, iteration, *args):
         df = pd.DataFrame()
 
         # we use pbar to display progress bar
         pbar = tqdm(total=len(params * NUMBER_OF_CPU), ncols=40)
 
         for param in params:
-            bt = strategy(data)
+            # bt = strategy(data, *strategy_params)
+
+            bt = strategy(
+                data,
+                commission_type="fixed",
+                initial_capital=INITIAL_CAPITAL,
+                # commission=0.6,
+                # multiplier=2,
+                commission=1.2,
+                multiplier=20,
+                default_size=1,
+            )
             bt.backtest(param)
 
             bt.stats.index = [param]
             df = pd.concat([df, bt.stats])
             if iteration == 0:
                 pbar.update(NUMBER_OF_CPU)
         pbar.close()
```

### Comparing `quantnb-0.2.9/quantnb/strategies/S_MACD.py` & `quantnb-0.3.1/quantnb/strategies/S_MACD.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.9/quantnb/strategies/S_base.py` & `quantnb-0.3.1/quantnb/strategies/S_base.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,56 +4,76 @@
 import matplotlib.pyplot as plt
 
 from quantnb.helpers import save_to_csv, print_orders, print_trades, calculate_metrics
 
 
 class S_base:
     def __init__(
-        self, data, offset=0, commission=0.0002, initial_capital=10000, use_sl=False
+        self,
+        data,
+        offset=0,
+        commission=0.0002,
+        commission_type="percentage",
+        initial_capital=10000,
+        multiplier=1,
+        default_size=None,
+        use_sl=False,
     ):
         data = data[offset:]
 
         data.rename(
             columns={"close": "Close", "high": "High", "low": "Low", "open": "Open"},
             inplace=True,
         )
         data.index = data.index.astype(int) // 10**9
         self.data = data
         self.commmision = commission
+        self.multiplier = multiplier
+        self.default_size = default_size
+        self.commmision_type = commission_type
         self.initial_capital = initial_capital
         self.use_sl = use_sl
 
-    def simulation(self, mode, use_sl):
-        close = self.data.Close
-        size = np.full_like(close, 1)
-        multiplier = 1
-        size = size * multiplier
+        self.set_bt_data()
 
+    def set_bt_data(self):
         df = self.data
         open = df.Open.to_numpy(dtype=np.float32)
         high = df.High.to_numpy(dtype=np.float32)
         low = df.Low.to_numpy(dtype=np.float32)
         close = df.Close.to_numpy(dtype=np.float32)
-        index = df.index.to_numpy(dtype=np.int32)
+        index = df.index.to_numpy(dtype=np.int64)
 
-        bt = Backtester(
-            commissions=self.commmision, initial_capital=self.initial_capital
+        self.bt = Backtester(
+            initial_capital=self.initial_capital,
+            commission=self.commmision,
+            commission_type=self.commmision_type,
+            default_size=self.default_size,
+            multiplier=self.multiplier,
         )
-        bt.set_data(open, high, low, close, index)
+        self.bt.set_data(open, high, low, close, index)
+
+    def simulation(self, mode, use_sl):
+        close = self.data.Close
+
         sl = None
         if self.use_sl:
             sl = self.sl.values
 
-        bt.backtest(self.entries.values, self.exits.values, sl, use_sl)
+        # size = np.full_like(close, 1)
+        # multiplier = 1
+        # size = size * multiplier
+
+        self.bt.from_signals(self.entries, self.exits, sl, use_sl)
 
         return (
-            bt.final_value,
-            bt.equity,
-            bt.orders[: bt.order_idx, :],
-            bt.trades[: bt.trade_idx, :],
+            self.bt.final_value,
+            self.bt.equity,
+            self.bt.orders[: self.bt.order_idx, :],
+            self.bt.trades[: self.bt.trade_idx, :],
         )
 
     def backtest_bid_ask(self, params):
         pass
 
     def backtest(self, params):
         self.get_signals(params)
@@ -79,15 +99,15 @@
 
         self.trades_arr = trades_arr
         self.equity = equity
         # print(self.stats)
 
     # HELPERS
     def print_trades(self):
-        print_trades(self.trades_arr)
+        return print_trades(self.trades_arr)
 
     def save_to_csv(self):
         data = self.data.copy()
         data.reset_index(inplace=True)
         data.rename(columns={"timestamp": "Date"}, inplace=True)
         data.set_index("Date", inplace=True)
```

### Comparing `quantnb-0.2.9/quantnb/strategies/S_bid_ask.py` & `quantnb-0.3.1/quantnb/strategies/S_bid_ask.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.9/quantnb/strategies/S_test.py` & `quantnb-0.3.1/quantnb/strategies/s_temp.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.9/quantnb/tests/benchmark_multiple_assets.py` & `quantnb-0.3.1/quantnb/tests/benchmark_multiple_assets.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.9/quantnb/tests/optimisation_combine_files.py` & `quantnb-0.3.1/quantnb/tests/optimisation_combine_files.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.9/quantnb/tests/supertrend_test.py` & `quantnb-0.3.1/quantnb/tests/supertrend.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,12 +23,13 @@
 # Create MPF plot
 mpf.plot(
     ohlc_data,
     type="candle",
     volume=False,
     ylabel="Price",
     addplot=[
-        mpf.make_addplot(supers, color="red", panel=0),
-        mpf.make_addplot(superl, color="teal", panel=0),
+        mpf.make_addplot(supert, color="red", panel=0),
+        # mpf.make_addplot(supers, color="red", panel=0),
+        # mpf.make_addplot(superl, color="teal", panel=0),
     ],
     title="Supertrend Indicator",
 )
```

