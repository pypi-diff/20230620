# Comparing `tmp/martin-binance-1.3.0b23.tar.gz` & `tmp/martin-binance-1.3.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martin-binance-1.3.0b23.tar", last modified: Thu Jun  8 07:35:21 2023, max compression
+gzip compressed data, was "martin-binance-1.3.1b0.tar", last modified: Tue Jun 20 13:24:50 2023, max compression
```

## Comparing `martin-binance-1.3.0b23.tar` & `martin-binance-1.3.1b0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      154 2022-06-16 20:42:55.292826 martin-binance-1.3.0b23/.deepsource.toml
--rw-r--r--   0        0        0       79 2022-09-29 14:39:58.264847 martin-binance-1.3.0b23/.dockerignore
--rw-r--r--   0        0        0       68 2022-06-16 20:42:55.292826 martin-binance-1.3.0b23/.github/FUNDING.yml
--rw-r--r--   0        0        0      665 2022-09-29 14:39:58.268851 martin-binance-1.3.0b23/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      604 2022-09-29 14:39:58.268851 martin-binance-1.3.0b23/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      837 2023-01-08 14:15:30.514225 martin-binance-1.3.0b23/.github/workflows/codeql.yml
--rw-r--r--   0        0        0       45 2022-09-29 14:39:58.268851 martin-binance-1.3.0b23/.gitignore
--rwxr-xr-x   0        0        0    17766 2023-06-08 07:01:31.585733 martin-binance-1.3.0b23/CHANGELOG.md
--rw-r--r--   0        0        0      601 2022-11-24 16:46:07.400338 martin-binance-1.3.0b23/Dockerfile
--rw-r--r--   0        0        0     1079 2022-06-16 20:37:23.392898 martin-binance-1.3.0b23/LICENSE
--rwxr-xr-x   0        0        0    35437 2023-05-30 12:20:07.843798 martin-binance-1.3.0b23/README.md
--rwxr-xr-x   0        0        0    89295 2021-12-09 10:16:46.764494 martin-binance-1.3.0b23/doc/Create_strategy.png
--rwxr-xr-x   0        0        0    26452 2021-12-09 10:16:46.764494 martin-binance-1.3.0b23/doc/Model of logarithmic grid.ods
--rw-r--r--   0        0        0  5309091 2021-12-09 10:16:46.820491 martin-binance-1.3.0b23/doc/Modified martingale.svg
--rwxr-xr-x   0        0        0    79517 2021-12-09 10:16:46.824491 martin-binance-1.3.0b23/doc/graf1.png
--rwxr-xr-x   0        0        0    10318 2021-12-09 10:16:46.824491 martin-binance-1.3.0b23/doc/tlg_notify.png
--rwxr-xr-x   0        0        0     9332 2021-12-09 10:16:46.824491 martin-binance-1.3.0b23/doc/tmux.png
--rw-r--r--   0        0        0     2050 2023-06-07 08:37:58.500647 martin-binance-1.3.0b23/martin_binance/__init__.py
--rw-r--r--   0        0        0     2218 2023-06-05 19:37:24.375292 martin-binance-1.3.0b23/martin_binance/backtest/OoTSP.py
--rw-r--r--   0        0        0     2949 2023-06-03 09:17:19.879857 martin-binance-1.3.0b23/martin_binance/backtest/VCoSEL.py
--rw-r--r--   0        0        0        0 2023-06-01 20:26:31.871396 martin-binance-1.3.0b23/martin_binance/backtest/__init__.py
--rw-r--r--   0        0        0    12323 2023-06-04 14:26:32.096258 martin-binance-1.3.0b23/martin_binance/backtest/exchange_simulator.py
--rw-r--r--   0        0        0     6474 2023-06-01 20:26:31.871396 martin-binance-1.3.0b23/martin_binance/cli_0_BTCUSDT.py.template
--rw-r--r--   0        0        0     6469 2023-06-01 20:26:31.871396 martin-binance-1.3.0b23/martin_binance/cli_1_BTCUSDT.py.template
--rw-r--r--   0        0        0     6475 2023-06-01 20:26:31.871396 martin-binance-1.3.0b23/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
--rw-r--r--   0        0        0     4710 2023-06-01 20:26:31.871396 martin-binance-1.3.0b23/martin_binance/client.py
--rw-r--r--   0        0        0   181684 2023-06-07 16:41:03.333036 martin-binance-1.3.0b23/martin_binance/executor.py
--rw-r--r--   0        0        0   237568 2022-09-29 14:39:58.276860 martin-binance-1.3.0b23/martin_binance/funds_rate.db.template
--rwxr-xr-x   0        0        0   337272 2022-09-29 14:39:58.276860 martin-binance-1.3.0b23/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
--rw-r--r--   0        0        0      376 2022-12-19 14:10:45.443888 martin-binance-1.3.0b23/martin_binance/margin/margin_req.txt
--rw-r--r--   0        0        0      348 2023-01-08 14:15:30.514225 martin-binance-1.3.0b23/martin_binance/margin/margin_req_win.txt
--rw-r--r--   0        0        0    79598 2023-06-06 16:41:38.089871 martin-binance-1.3.0b23/martin_binance/margin_wrapper.py
--rw-r--r--   0        0        0     1472 2023-01-19 11:11:07.967695 martin-binance-1.3.0b23/martin_binance/ms_cfg.toml.template
--rw-r--r--   0        0        0      485 2021-12-09 09:06:56.984779 martin-binance-1.3.0b23/martin_binance/service/.tmux.conf
--rwxr-xr-x   0        0        0      319 2022-09-29 14:39:58.280864 martin-binance-1.3.0b23/martin_binance/service/funds_export.service
--rwxr-xr-x   0        0        0    16185 2023-05-30 12:20:07.847793 martin-binance-1.3.0b23/martin_binance/service/funds_rate_exporter.py
--rwxr-xr-x   0        0        0    75764 2023-05-30 12:20:07.847793 martin-binance-1.3.0b23/martin_binance/service/grafana.json
--rwxr-xr-x   0        0        0     1276 2022-09-29 14:39:58.280864 martin-binance-1.3.0b23/martin_binance/service/relaunch.py
--rwxr-xr-x   0        0        0      271 2022-09-29 14:39:58.284868 martin-binance-1.3.0b23/martin_binance/service/relaunch.service
--rwxr-xr-x   0        0        0      372 2021-12-09 09:06:56.984779 martin-binance-1.3.0b23/martin_binance/service/tmux.service
--rw-r--r--   0        0        0     1203 2023-06-03 20:53:44.166165 martin-binance-1.3.0b23/pyproject.toml
--rw-r--r--   0        0        0      320 2023-06-03 20:53:44.162164 martin-binance-1.3.0b23/requirements.txt
--rw-r--r--   0        0        0     2390 2023-01-19 11:11:07.971695 martin-binance-1.3.0b23/uml/architecture.puml
--rw-r--r--   0        0        0    36614 1970-01-01 00:00:00.000000 martin-binance-1.3.0b23/PKG-INFO
+-rw-r--r--   0        0        0      154 2022-06-16 20:42:55.292826 martin-binance-1.3.1b0/.deepsource.toml
+-rw-r--r--   0        0        0       79 2022-09-29 14:39:58.264847 martin-binance-1.3.1b0/.dockerignore
+-rw-r--r--   0        0        0       68 2022-06-16 20:42:55.292826 martin-binance-1.3.1b0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      665 2022-09-29 14:39:58.268851 martin-binance-1.3.1b0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      604 2022-09-29 14:39:58.268851 martin-binance-1.3.1b0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      837 2023-01-08 14:15:30.514225 martin-binance-1.3.1b0/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0       45 2022-09-29 14:39:58.268851 martin-binance-1.3.1b0/.gitignore
+-rwxr-xr-x   0        0        0    18795 2023-06-20 11:01:32.418813 martin-binance-1.3.1b0/CHANGELOG.md
+-rw-r--r--   0        0        0      601 2022-11-24 16:46:07.400338 martin-binance-1.3.1b0/Dockerfile
+-rw-r--r--   0        0        0     1079 2022-06-16 20:37:23.392898 martin-binance-1.3.1b0/LICENSE
+-rwxr-xr-x   0        0        0     3944 2023-06-19 19:17:03.912066 martin-binance-1.3.1b0/README.md
+-rwxr-xr-x   0        0        0    89295 2021-12-09 10:16:46.764494 martin-binance-1.3.1b0/doc/Create_strategy.png
+-rwxr-xr-x   0        0        0    26452 2021-12-09 10:16:46.764494 martin-binance-1.3.1b0/doc/Model of logarithmic grid.ods
+-rw-r--r--   0        0        0  5309091 2021-12-09 10:16:46.820491 martin-binance-1.3.1b0/doc/Modified martingale.svg
+-rwxr-xr-x   0        0        0    79517 2021-12-09 10:16:46.824491 martin-binance-1.3.1b0/doc/graf1.png
+-rwxr-xr-x   0        0        0    10318 2021-12-09 10:16:46.824491 martin-binance-1.3.1b0/doc/tlg_notify.png
+-rwxr-xr-x   0        0        0     9332 2021-12-09 10:16:46.824491 martin-binance-1.3.1b0/doc/tmux.png
+-rw-r--r--   0        0        0     1947 2023-06-20 13:24:47.109110 martin-binance-1.3.1b0/martin_binance/__init__.py
+-rw-r--r--   0        0        0     3882 2023-06-19 19:16:08.328313 martin-binance-1.3.1b0/martin_binance/backtest/OoTSP.py
+-rw-r--r--   0        0        0     2946 2023-06-10 10:09:47.513439 martin-binance-1.3.1b0/martin_binance/backtest/VCoSEL.py
+-rw-r--r--   0        0        0        0 2023-06-10 10:09:47.513439 martin-binance-1.3.1b0/martin_binance/backtest/__init__.py
+-rw-r--r--   0        0        0    14050 2023-06-19 19:16:08.304258 martin-binance-1.3.1b0/martin_binance/backtest/exchange_simulator.py
+-rw-r--r--   0        0        0     6721 2023-06-19 17:47:04.745501 martin-binance-1.3.1b0/martin_binance/cli_0_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6716 2023-06-19 17:47:04.745501 martin-binance-1.3.1b0/martin_binance/cli_1_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6722 2023-06-19 17:47:04.745501 martin-binance-1.3.1b0/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
+-rw-r--r--   0        0        0     4707 2023-06-10 10:09:47.517442 martin-binance-1.3.1b0/martin_binance/client.py
+-rw-r--r--   0        0        0   185525 2023-06-20 10:20:51.033666 martin-binance-1.3.1b0/martin_binance/executor.py
+-rw-r--r--   0        0        0   237568 2022-09-29 14:39:58.276860 martin-binance-1.3.1b0/martin_binance/funds_rate.db.template
+-rwxr-xr-x   0        0        0   337272 2022-09-29 14:39:58.276860 martin-binance-1.3.1b0/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0      376 2022-12-19 14:10:45.443888 martin-binance-1.3.1b0/martin_binance/margin/margin_req.txt
+-rw-r--r--   0        0        0      348 2023-01-08 14:15:30.514225 martin-binance-1.3.1b0/martin_binance/margin/margin_req_win.txt
+-rw-r--r--   0        0        0    85764 2023-06-19 21:29:05.366900 martin-binance-1.3.1b0/martin_binance/margin_wrapper.py
+-rw-r--r--   0        0        0     1472 2023-01-19 11:11:07.967695 martin-binance-1.3.1b0/martin_binance/ms_cfg.toml.template
+-rw-r--r--   0        0        0      485 2021-12-09 09:06:56.984779 martin-binance-1.3.1b0/martin_binance/service/.tmux.conf
+-rwxr-xr-x   0        0        0      319 2022-09-29 14:39:58.280864 martin-binance-1.3.1b0/martin_binance/service/funds_export.service
+-rwxr-xr-x   0        0        0    16369 2023-06-19 17:47:04.749497 martin-binance-1.3.1b0/martin_binance/service/funds_rate_exporter.py
+-rwxr-xr-x   0        0        0    75764 2023-06-10 10:09:47.517442 martin-binance-1.3.1b0/martin_binance/service/grafana.json
+-rwxr-xr-x   0        0        0     1274 2023-06-20 08:42:34.849378 martin-binance-1.3.1b0/martin_binance/service/relaunch.py
+-rwxr-xr-x   0        0        0      271 2022-09-29 14:39:58.284868 martin-binance-1.3.1b0/martin_binance/service/relaunch.service
+-rwxr-xr-x   0        0        0      372 2021-12-09 09:06:56.984779 martin-binance-1.3.1b0/martin_binance/service/tmux.service
+-rw-r--r--   0        0        0     1277 2023-06-20 13:24:01.170244 martin-binance-1.3.1b0/pyproject.toml
+-rw-r--r--   0        0        0      335 2023-06-19 19:16:08.288221 martin-binance-1.3.1b0/requirements.txt
+-rw-r--r--   0        0        0     2390 2023-01-19 11:11:07.971695 martin-binance-1.3.1b0/uml/architecture.puml
+-rw-r--r--   0        0        0     5151 1970-01-01 00:00:00.000000 martin-binance-1.3.1b0/PKG-INFO
```

### Comparing `martin-binance-1.3.0b23/.github/ISSUE_TEMPLATE/bug_report.md` & `martin-binance-1.3.1b0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b23/.github/ISSUE_TEMPLATE/feature_request.md` & `martin-binance-1.3.1b0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b23/.github/workflows/codeql.yml` & `martin-binance-1.3.1b0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b23/CHANGELOG.md` & `martin-binance-1.3.1b0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,48 @@
+## v1.3.0-4 2023-06-20
+### Fix
+* ```get_free_assets(mode='free', backtest=True)``` return incorrect value for backtest Reverse cycle 
+
+### Update
+* Sometimes Tmux terminal after reboot not restore work path to ```/exch_srv.py```
+For working case: in relaunch.py was changed './exch_srv.py' to 'exch_srv.py' and
+path ```~/.local/lib/python3.10/site-packages/exchanges_wrapper``` must be added to system PATH
+
+For Ubuntu at end of ```~/.bashrc``` add the string
+
+```
+export PATH=$PATH:~/.local/lib/python3.10/site-packages/exchanges_wrapper
+```
+and refresh bash ```source ~/.bashrc```
+
+## v1.3.0-3 2023-06-10
+### Fix
+* Change ast.literal_eval() to eval() for trusted source
+
+## v1.3.0-2 2023-06-19
+### Added for new features
+* Ability to start backtesting from saved state, including in Reverse mode
+
+### Update
+* Monitoring memory usage including swap
+* up requirements for exchanges-wrapper to 1.3.0-2
+
+## v1.3.0-1 2023-06-10
+### Fix
+* Some minor improvements
+
+## v1.3.0 2023-06-09
+### Added for new features
+* Backtesting capabilities
+* Based on [optuna framework](https://optuna.org) search for optimal trading parameters
+* Visual comparison of the results of the initial and trial trading sessions
+
+### Update
+* Doc migrate from readme to wiki 
+
 ## v1.3.0b22-23 2023-06-08
 ### Fix
 * correct funding check in start()
 
 ## v1.3.0b18-21 2023-06-06
 ### Fix
 * #59
@@ -22,19 +63,14 @@
 * Bitfinex: rename test pair from AAABBB to TESTBTCTESTUSDT, update template
 
 ### Update
 * protobuf format for CreateLimitOrder() method. **Not compatible with earlier versions**
 * for some situation (shift grid, cancel grid after filled TP and so on) changed cancel order method from "one by one"
 to bulk mode
 
-### Added for new features
-* Backtesting capabilities
-* Based on [optuna framework](https://optuna.org) search for optimal trading parameters
-* Visual comparison of the results of the initial and trial trading sessions
-
 ## v1.2.18-8 2023-06-xx not released
 ### Fix
 * collect_assets() incorrect convert small decimal.Decimal values to str
 
 ### Update
 * For STANDALONE mode refactoring call environment for place_limit_order(), avoid unnecessary Decimal -> float
 conversions
```

### Comparing `martin-binance-1.3.0b23/Dockerfile` & `martin-binance-1.3.1b0/Dockerfile`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b23/LICENSE` & `martin-binance-1.3.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b23/doc/Create_strategy.png` & `martin-binance-1.3.1b0/doc/Create_strategy.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b23/doc/Model of logarithmic grid.ods` & `martin-binance-1.3.1b0/doc/Model of logarithmic grid.ods`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b23/doc/Modified martingale.svg` & `martin-binance-1.3.1b0/doc/Modified martingale.svg`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b23/doc/graf1.png` & `martin-binance-1.3.1b0/doc/graf1.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b23/doc/tlg_notify.png` & `martin-binance-1.3.1b0/doc/tlg_notify.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b23/doc/tmux.png` & `martin-binance-1.3.1b0/doc/tmux.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b23/martin_binance/__init__.py` & `martin-binance-1.3.1b0/martin_binance/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Free trading system for Binance SPOT API
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0b23"
+__version__ = "1.3.1b0"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from pathlib import Path
 from shutil import copy
 #
 import platform
@@ -30,15 +30,15 @@
     LAST_STATE_PATH = Path(WORK_PATH, "last_state")
     BACKTEST_PATH = Path(WORK_PATH, "back_test")
 else:
     LOG_PATH = None
     LAST_STATE_PATH = None
     BACKTEST_PATH = None
 if CONFIG_FILE.exists():
-    print(f"Config found at {CONFIG_FILE}")
+    print(f"Client config found at {CONFIG_FILE}")
 else:
     print("Can't find config file! Creating it...")
     CONFIG_PATH.mkdir(parents=True, exist_ok=True)
     if STANDALONE:
         LOG_PATH.mkdir(parents=True, exist_ok=True)
         LAST_STATE_PATH.mkdir(parents=True, exist_ok=True)
     copy(Path(Path(__file__).parent.absolute(), "ms_cfg.toml.template"), CONFIG_FILE)
@@ -47,10 +47,7 @@
     copy(Path(Path(__file__).parent.absolute(), "cli_1_BTCUSDT.py.template"), Path(WORK_PATH, "cli_1_BTCUSDT.py"))
     copy(Path(Path(__file__).parent.absolute(), "cli_2_TESTBTCTESTUSDT.py.template"),
          Path(WORK_PATH, "cli_2_TESTBTCTESTUSDT.py"))
     print(f"Before the first run, set the parameters in {CONFIG_FILE}")
     if STANDALONE:
         raise SystemExit(1)
     raise UserWarning()
-
-# TODO GRID_ONLY mode: after depositing asset refresh balance
-# TODO 'S' mode - use last_state for start ???
```

### Comparing `martin-binance-1.3.0b23/martin_binance/backtest/VCoSEL.py` & `martin-binance-1.3.1b0/martin_binance/backtest/VCoSEL.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Visual Comparison of Session Extended Log
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0b14"
+__version__ = "1.3.0"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from dash import Dash, html, dcc
 import plotly.graph_objects as go
 import pandas as pd
```

### Comparing `martin-binance-1.3.0b23/martin_binance/backtest/exchange_simulator.py` & `martin-binance-1.3.1b0/martin_binance/backtest/exchange_simulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 # -*- coding: utf-8 -*-
 """
 Simple exchange simulator for backtest purpose
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0b59"
+__version__ = "1.3.0-2"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from decimal import Decimal
 import pandas as pd
 
 
 class Funds:
+    __slots__ = ("base", "quote")
+
     def __init__(self):
         # {'asset': 'BTC', 'free': '0.0', 'locked': '0.0'}
         self.base = {}
         self.quote = {}
 
     def get_funds(self):
         return [self.base, self.quote]
@@ -58,14 +60,41 @@
             base_locked -= _amount
             quote_free += _amount * _price - fee * (_amount * _price) / 100
             self.base['locked'] = str(base_locked)
             self.quote['free'] = str(quote_free)
 
 
 class Order:
+    __slots__ = (
+        "symbol",
+        "order_id",
+        "order_list_id",
+        "client_order_id",
+        "transact_time",
+        "price",
+        "orig_qty",
+        "executed_qty",
+        "cummulative_quote_qty",
+        "status",
+        "time_in_force",
+        "type",
+        "side",
+        "working_time",
+        "self_trade_prevention_mode",
+        "event_time",
+        "last_executed_quantity",
+        "cumulative_filled_quantity",
+        "last_executed_price",
+        "trade_id",
+        "order_creation_time",
+        "quote_asset_transacted",
+        "last_quote_asset_transacted",
+        "quote_order_quantity",
+    )
+
     def __init__(self, symbol: str, order_id: int, client_order_id: str, buy: bool, amount: str, price: str, lt: int):
         self.symbol = symbol
         self.order_id = order_id
         self.order_list_id = -1
         self.client_order_id = client_order_id
         self.transact_time = lt  # local time
         self.price = price
@@ -87,39 +116,64 @@
         self.order_creation_time = lt
         self.quote_asset_transacted: str
         self.last_quote_asset_transacted: str
         self.quote_order_quantity: str
 
 
 class Account:
+    __slots__ = (
+        "save_ds",
+        "funds",
+        "fee_maker",
+        "fee_taker",
+        "orders",
+        "orders_buy",
+        "orders_sell",
+        "trade_id",
+        "ticker",
+        "grid_buy",
+        "grid_sell",
+        "ticker_last",
+    )
+
     def __init__(self, save_ds: bool):
         self.save_ds = save_ds
         self.funds = Funds()
         self.fee_maker = Decimal('0')
         self.fee_taker = Decimal('0')
         self.orders = []
         self.orders_buy = pd.Series()
         self.orders_sell = pd.Series()
         self.trade_id = 0
         self.ticker = {}
         self.grid_buy = {}
         self.grid_sell = {}
         self.ticker_last = Decimal('0')
 
-    def create_order(self, symbol: str, client_order_id: str, buy: bool, amount: str, price: str, lt: int) -> {}:
-        order_id = len(self.orders)
+    def create_order(
+            self,
+            symbol: str,
+            client_order_id: str,
+            buy: bool,
+            amount: str,
+            price: str,
+            lt: int,
+            order_id=None) -> {}:
+
+        order_id = order_id or len(self.orders)
         order = Order(symbol=symbol,
                       order_id=order_id,
                       client_order_id=client_order_id,
                       buy=buy,
                       amount=amount,
                       price=price,
                       lt=lt)
 
-        if (buy and Decimal(price) >= self.ticker_last) or (not buy and Decimal(price) <= self.ticker_last):
+        if self.ticker_last and ((buy and Decimal(price) >= self.ticker_last) or
+                                 (not buy and Decimal(price) <= self.ticker_last)):
             # Market event
             order.transact_time = lt
             order.executed_qty = order.orig_qty
             order.cummulative_quote_qty = str(Decimal(order.orig_qty) * Decimal(order.price))
             order.status = 'FILLED'
             order.event_time = order.transact_time
             order.last_executed_quantity = order.orig_qty
@@ -160,29 +214,35 @@
                 'timeInForce': order.time_in_force,
                 'type': order.type,
                 'side': order.side,
                 'workingTime': order.working_time,
                 'selfTradePreventionMode': order.self_trade_prevention_mode}
 
     def cancel_order(self, order_id: int, ts: int):
-        order = self.orders[order_id]
+        try:
+            order = next(x for x in self.orders if x.order_id == order_id)
+        except StopIteration:
+            raise UserWarning(f"Error on Cancel order, can't find {order_id} anymore")
+        _order_id = self.orders.index(order)
         order.status = 'CANCELED'
         try:
             if order.side == 'BUY':
                 self.orders_buy = self.orders_buy.drop(order_id)
                 if self.save_ds and self.orders_buy.values.size:
                     self.grid_buy[ts] = self.orders_buy
             else:
                 self.orders_sell = self.orders_sell.drop(order_id)
                 if self.save_ds and self.orders_sell.values.size:
                     self.grid_sell[ts] = self.orders_sell
         except Exception as ex:
             raise UserWarning(f"Order {order_id} not active: {ex}")
         else:
-            self.orders[order_id] = order
+
+            self.orders[_order_id] = order
+
             self.funds.on_order_canceled(order.side, order.orig_qty, order.price)
             return {'symbol': order.symbol,
                     'origClientOrderId': order.client_order_id,
                     'orderId': order.order_id,
                     'orderListId': order.order_list_id,
                     'clientOrderId': 'qwert',
                     'price': order.price,
@@ -277,7 +337,19 @@
                        'last_quote_asset_transacted': order.last_quote_asset_transacted,
                        'quote_order_quantity': order.quote_order_quantity}
                 #
                 orders_filled.append(res)
                 self.funds.on_order_filled(order.side, order.orig_qty, order.last_executed_price, self.fee_maker)
             #
         return orders_filled
+
+    def restore_state(self, symbol: str, lt: int, orders: []):
+        for order in orders:
+            self.create_order(
+                symbol=symbol,
+                client_order_id='',
+                buy=order['buy'],
+                amount=order['amount'],
+                price=order['price'],
+                lt=lt,
+                order_id=order['id']
+            )
```

### Comparing `martin-binance-1.3.0b23/martin_binance/cli_0_BTCUSDT.py.template` & `martin-binance-1.3.1b0/martin_binance/cli_1_BTCUSDT.py.template`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ####################################################################
 # Cyclic grid strategy based on martingale
 # See README.md for detail
 ####################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0"
+__version__ = "1.3.0-2"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 """
 ##################################################################
 Disclaimer
 
 All risks and possible losses associated with use of this strategy lie with you.
@@ -31,28 +31,28 @@
 from martin_binance.executor import *  # lgtm [py/polluting-import]
 ################################################################
 # Exchange setup and parameter settings
 ################################################################
 # Set trading pair for STANDALONE mode, for margin mode takes from terminal
 ex.SYMBOL = 'BTCUSDT'
 # Exchange setup, see list of exchange in ms_cfg.toml
-ex.ID_EXCHANGE = 0  # See ms_cfg.toml Use for collection of statistics *and get client connection*
+ex.ID_EXCHANGE = 1  # See ms_cfg.toml Use for collection of statistics *and get client connection*
 ex.FEE_IN_PAIR = True  # Fee pays in pair
-ex.FEE_MAKER = Decimal('0.0751')  # standard exchange Fee for maker
-ex.FEE_TAKER = Decimal('0.0751')  # standard exchange Fee for taker
+ex.FEE_MAKER = Decimal('0.08')  # standard exchange Fee for maker
+ex.FEE_TAKER = Decimal('0.1')  # standard exchange Fee for taker
 ex.FEE_SECOND = False  # On KRAKEN fee always in second coin
 ex.FEE_BNB_IN_PAIR = False  # Binance fee in BNB and BNB is base asset
 ex.GRID_MAX_COUNT = 5  # Maximum counts for placed grid orders
 ex.EXTRA_CHECK_ORDER_STATE = False  # Additional check for filled order(s), for (OKEX, )
 # Trade parameter
 ex.START_ON_BUY = True  # First cycle direction
 ex.AMOUNT_FIRST = Decimal('0.05')  # Deposit for Sale cycle in first currency
 ex.USE_ALL_FUND = False  # Use all available fund for initial cycle or alltime for GRID_ONLY
 ex.AMOUNT_SECOND = Decimal('1000.0')  # Deposit for Buy cycle in second currency
-ex.PRICE_SHIFT = 0.05  # 'No market' shift price in % from current bid/ask price
+ex.PRICE_SHIFT = 0.01  # 'No market' shift price in % from current bid/ask price
 # Round pattern, set pattern 1.0123456789 or if not set used exchange settings
 ex.ROUND_BASE = str()
 ex.ROUND_QUOTE = str()
 ex.PROFIT = Decimal('0.1')  # 0.1 - 0.85
 ex.PROFIT_MAX = Decimal('0.85')  # If set it is maximum adapted cycle profit
 ex.OVER_PRICE = Decimal('0.6')  # Overlap price in one direction
 ex.ORDER_Q = 12  # Target grid orders quantity in moment
@@ -82,14 +82,17 @@
 # Start first as Reverse cycle, also set appropriate AMOUNT
 ex.REVERSE = False
 ex.REVERSE_TARGET_AMOUNT = Decimal('0')
 ex.REVERSE_INIT_AMOUNT = Decimal('0')
 ex.REVERSE_STOP = False  # Stop after ending reverse cycle
 # Backtest mode parameters
 ex.MODE = 'T'  # 'T' - Trade, 'TC' - Trade and Collect, 'S' - Simulate
+ex.SAVE_DS = True  # Save session result data (ticker, orders) for compare
+ex.SAVE_PERIOD = 24 * 60 * 60  # sec, timetable for save data portion, but memory limitation consider also matter
+ex.SAVED_STATE = True  # Use saved state for backtesing
 ################################################################
 #                 DO NOT EDIT UNDER THIS LINE                ###
 ################################################################
 config = None
 ex.PARAMS = Path(__file__).absolute()
 if ex.CONFIG_FILE.exists():
     config = toml.load(str(ex.CONFIG_FILE))
```

### Comparing `martin-binance-1.3.0b23/martin_binance/cli_1_BTCUSDT.py.template` & `martin-binance-1.3.1b0/martin_binance/cli_0_BTCUSDT.py.template`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ####################################################################
 # Cyclic grid strategy based on martingale
 # See README.md for detail
 ####################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0"
+__version__ = "1.3.0-2"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 """
 ##################################################################
 Disclaimer
 
 All risks and possible losses associated with use of this strategy lie with you.
@@ -31,28 +31,28 @@
 from martin_binance.executor import *  # lgtm [py/polluting-import]
 ################################################################
 # Exchange setup and parameter settings
 ################################################################
 # Set trading pair for STANDALONE mode, for margin mode takes from terminal
 ex.SYMBOL = 'BTCUSDT'
 # Exchange setup, see list of exchange in ms_cfg.toml
-ex.ID_EXCHANGE = 1  # See ms_cfg.toml Use for collection of statistics *and get client connection*
+ex.ID_EXCHANGE = 0  # See ms_cfg.toml Use for collection of statistics *and get client connection*
 ex.FEE_IN_PAIR = True  # Fee pays in pair
-ex.FEE_MAKER = Decimal('0.08')  # standard exchange Fee for maker
-ex.FEE_TAKER = Decimal('0.1')  # standard exchange Fee for taker
+ex.FEE_MAKER = Decimal('0.0751')  # standard exchange Fee for maker
+ex.FEE_TAKER = Decimal('0.0751')  # standard exchange Fee for taker
 ex.FEE_SECOND = False  # On KRAKEN fee always in second coin
 ex.FEE_BNB_IN_PAIR = False  # Binance fee in BNB and BNB is base asset
 ex.GRID_MAX_COUNT = 5  # Maximum counts for placed grid orders
 ex.EXTRA_CHECK_ORDER_STATE = False  # Additional check for filled order(s), for (OKEX, )
 # Trade parameter
 ex.START_ON_BUY = True  # First cycle direction
 ex.AMOUNT_FIRST = Decimal('0.05')  # Deposit for Sale cycle in first currency
 ex.USE_ALL_FUND = False  # Use all available fund for initial cycle or alltime for GRID_ONLY
 ex.AMOUNT_SECOND = Decimal('1000.0')  # Deposit for Buy cycle in second currency
-ex.PRICE_SHIFT = 0.01  # 'No market' shift price in % from current bid/ask price
+ex.PRICE_SHIFT = 0.05  # 'No market' shift price in % from current bid/ask price
 # Round pattern, set pattern 1.0123456789 or if not set used exchange settings
 ex.ROUND_BASE = str()
 ex.ROUND_QUOTE = str()
 ex.PROFIT = Decimal('0.1')  # 0.1 - 0.85
 ex.PROFIT_MAX = Decimal('0.85')  # If set it is maximum adapted cycle profit
 ex.OVER_PRICE = Decimal('0.6')  # Overlap price in one direction
 ex.ORDER_Q = 12  # Target grid orders quantity in moment
@@ -82,14 +82,17 @@
 # Start first as Reverse cycle, also set appropriate AMOUNT
 ex.REVERSE = False
 ex.REVERSE_TARGET_AMOUNT = Decimal('0')
 ex.REVERSE_INIT_AMOUNT = Decimal('0')
 ex.REVERSE_STOP = False  # Stop after ending reverse cycle
 # Backtest mode parameters
 ex.MODE = 'T'  # 'T' - Trade, 'TC' - Trade and Collect, 'S' - Simulate
+ex.SAVE_DS = True  # Save session result data (ticker, orders) for compare
+ex.SAVE_PERIOD = 24 * 60 * 60  # sec, timetable for save data portion, but memory limitation consider also matter
+ex.SAVED_STATE = True  # Use saved state for backtesing
 ################################################################
 #                 DO NOT EDIT UNDER THIS LINE                ###
 ################################################################
 config = None
 ex.PARAMS = Path(__file__).absolute()
 if ex.CONFIG_FILE.exists():
     config = toml.load(str(ex.CONFIG_FILE))
```

### Comparing `martin-binance-1.3.0b23/martin_binance/cli_2_TESTBTCTESTUSDT.py.template` & `martin-binance-1.3.1b0/martin_binance/cli_2_TESTBTCTESTUSDT.py.template`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ####################################################################
 # Cyclic grid strategy based on martingale
 # See README.md for detail
 ####################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0"
+__version__ = "1.3.0-2"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 """
 ##################################################################
 Disclaimer
 
 All risks and possible losses associated with use of this strategy lie with you.
@@ -82,14 +82,17 @@
 # Start first as Reverse cycle, also set appropriate AMOUNT
 ex.REVERSE = False
 ex.REVERSE_TARGET_AMOUNT = Decimal('0')
 ex.REVERSE_INIT_AMOUNT = Decimal('0')
 ex.REVERSE_STOP = False  # Stop after ending reverse cycle
 # Backtest mode parameters
 ex.MODE = 'T'  # 'T' - Trade, 'TC' - Trade and Collect, 'S' - Simulate
+ex.SAVE_DS = True  # Save session result data (ticker, orders) for compare
+ex.SAVE_PERIOD = 24 * 60 * 60  # sec, timetable for save data portion, but memory limitation consider also matter
+ex.SAVED_STATE = True  # Use saved state for backtesing
 ################################################################
 #                 DO NOT EDIT UNDER THIS LINE                ###
 ################################################################
 config = None
 ex.PARAMS = Path(__file__).absolute()
 if ex.CONFIG_FILE.exists():
     config = toml.load(str(ex.CONFIG_FILE))
```

### Comparing `martin-binance-1.3.0b23/martin_binance/client.py` & `martin-binance-1.3.1b0/martin_binance/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 gRPC async client for exchanges-wrapper
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.2.17b1"
+__version__ = "1.3.0"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 import asyncio
 # noinspection PyPackageRequirements
 import grpc
 import random
```

### Comparing `martin-binance-1.3.0b23/martin_binance/executor.py` & `martin-binance-1.3.1b0/martin_binance/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ####################################################################
 # Cyclic grid strategy based on martingale
 ##################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0b23"
+__version__ = "1.3.0-4"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = 'https://github.com/DogsTailFarmer'
 ##################################################################
 import sys
 import gc
 import statistics
 from decimal import Decimal, ROUND_FLOOR, ROUND_CEILING
@@ -104,18 +104,21 @@
 STOP_TLG = 'stop_signal_QWE#@!'
 INLINE_BOT = True
 # Backtesting
 MODE = 'T'  # 'T' - Trade, 'TC' - Trade and Collect, 'S' - Simulate
 XTIME = 500  # Time accelerator
 SAVE_DS = True  # Save session result data (ticker, orders) for compare
 SAVE_PERIOD = 1 * 60 * 60  # sec, timetable for save data portion, but memory limitation consider also matter
+SAVED_STATE = False  # Use saved state for backtesing
 # endregion
 
 
 class Style:
+    __slots__ = ()
+
     BLACK: str = '\033[30m'
     RED: str = '\033[31m'
     B_RED: str = '\033[1;31m'
     GREEN: str = '\033[32m'
     YELLOW: str = '\033[33m'
     B_YELLOW: str = "\033[33;1m"
     BLUE: str = '\033[34m'
@@ -519,14 +522,16 @@
         _err.append(err)
     print('Oops. No solution found')
     print("\n".join(f"delta: {k}\tresult: {v}" for k, v in solves))
     return f2d(0)
 
 
 class Orders:
+    __slots__ = ("orders_list",)
+
     def __init__(self):
         self.orders_list = []
 
     def __iter__(self):
         for i in self.orders_list:
             yield i
 
@@ -620,14 +625,108 @@
         return _sum
 
 
 class Strategy(StrategyBase):
     ##############################################################
     # strategy control methods
     ##############################################################
+    __slots__ = (
+        "cycle_buy",
+        "orders_grid",
+        "orders_init",
+        "orders_hold",
+        # Take profit variables
+        "tp_order_id",
+        "tp_wait_id",
+        "tp_order",
+        "tp_error",
+        "tp_order_hold",
+        "tp_hold",
+        "tp_cancel",
+        "tp_cancel_from_grid_handler",
+        "tp_hold_additional",
+        "tp_target",
+        "tp_amount",
+        "part_profit_first",
+        "part_profit_second",
+        "tp_was_filled",
+        "tp_part_amount_first",
+        "tp_part_amount_second",
+        "tp_init",
+        #
+        "sum_amount_first",
+        "sum_amount_second",
+        #
+        "correction_amount_first",
+        "correction_amount_second",
+        #
+        "deposit_first",
+        "deposit_second",
+        "sum_profit_first",
+        "sum_profit_second",
+        "cycle_buy_count",
+        "cycle_sell_count",
+        "shift_grid_threshold",
+        "f_currency",
+        "s_currency",
+        "connection_analytic",
+        "tlg_header",
+        "last_shift_time",
+        "avg_rate",
+        #
+        "grid_hold",
+        "start_hold",
+        "initial_first",
+        "initial_second",
+        "initial_reverse_first",
+        "initial_reverse_second",
+        "wait_refunding_for_start",
+        #
+        "cancel_order_id",
+        "over_price",
+        "grid_place_flag",
+        "part_amount",
+        "command",
+        "start_after_shift",
+        "queue_to_db",
+        "pr_db",
+        "queue_to_tlg",
+        "pr_tlg",
+        "pr_tlg_control",
+        "restart",
+        "profit_first",
+        "profit_second",
+        "status_time",
+        "cycle_time",
+        "cycle_time_reverse",
+        "reverse",
+        "reverse_target_amount",
+        "reverse_init_amount",
+        "reverse_hold",
+        "reverse_price",
+        "round_base",
+        "round_quote",
+        "order_q",
+        "order_q_placed",
+        "martin",
+        "orders_save",
+        "first_run",
+        "grid_remove",
+        "heartbeat_counter",
+        "grid_order_canceled",
+        "cycle_status",
+        "grid_update_started",
+        "start_reverse_time",
+        "last_ticker_update",
+        "grid_only_restart",
+        "local_time",
+        "wait_wss_refresh",
+        "start_collect",
+    )
+
     def __init__(self):
         super().__init__()
         print(f"Init Strategy, ver: {HEAD_VERSION} + {__version__} + {msb_ver}")
         self.cycle_buy = not START_ON_BUY if REVERSE else START_ON_BUY  # + Direction (Buy/Sell) for current cycle
         self.orders_grid = Orders()  # + List of grid orders
         self.orders_init = Orders()  # - List of initial grid orders
         self.orders_hold = Orders()  # + List of grid orders for later place
@@ -748,15 +847,16 @@
         self.martin = (MARTIN + 100) / 100
         if not check_funds:
             self.first_run = False
         if GRID_ONLY:
             self.message_log(f"Mode for {'buy' if self.cycle_buy else 'sell'} {self.f_currency} by grid orders"
                              f" placement ON",
                              color=Style.B_WHITE)
-        self.message_log(f"Mode is {'Trade' if MODE == 'T' else ('Trade & Collect' if MODE == 'TC' else 'Simulate')}",
+        self.message_log(f"This is {'Trade' if MODE == 'T' else ('Trade & Collect' if MODE == 'TC' else 'Simulate')}"
+                         f" mode",
                          color=Style.B_WHITE if MODE == 'T' else (Style.B_RED if MODE == 'TC' else Style.GREEN))
         # Calculate round float multiplier
         self.round_base = ROUND_BASE or str(tcm.round_amount(1.123456789, RoundingType.FLOOR))
         self.round_quote = ROUND_QUOTE or str(Decimal(self.round_base) *
                                               Decimal(str(tcm.round_price(1.123456789, RoundingType.FLOOR))))
         self.message_log(f"Round pattern, for base: {self.round_base}, quote: {self.round_quote}")
         last_price = self.get_buffered_ticker().last_price
@@ -794,228 +894,229 @@
         s = StrategyConfig()
         s.required_data_updates = {StrategyConfig.ORDER_BOOK,
                                    StrategyConfig.FUNDS,
                                    StrategyConfig.TICKER}
         s.normalize_exchange_buy_amounts = True
         return s
 
-    def save_strategy_state(self) -> Dict[str, str]:
-        # region SaveOperationalStatus
-        # Skip when transition processes or GRID_ONLY mode
-        stable_state = (self.shift_grid_threshold is None
-                        and self.grid_remove is None
-                        and not self.reverse_hold
-                        and not GRID_ONLY
-                        and not self.grid_update_started
-                        and not self.start_after_shift
-                        and not self.tp_hold
-                        and not self.tp_was_filled
-                        and not self.orders_init)
-        if MODE in ('T', 'TC') and stable_state:
-            orders = self.get_buffered_open_orders()
-            order_buy = len([i for i in orders if i.buy is True])
-            order_sell = len([i for i in orders if i.buy is False])
-            order_hold = len(self.orders_hold)
-            cycle_status = (self.cycle_buy, order_buy, order_sell, order_hold)
-            if self.cycle_status != cycle_status:
-                self.cycle_status = cycle_status
-                data_to_db = {'f_currency': self.f_currency,
-                              's_currency': self.s_currency,
-                              'cycle_buy': self.cycle_buy,
-                              'order_buy': order_buy,
-                              'order_sell': order_sell,
-                              'order_hold': order_hold,
-                              'destination': 't_orders'}
-                if self.queue_to_db:
-                    # print('Send data to t_orders')
-                    self.queue_to_db.put(data_to_db)
-        else:
-            self.cycle_status = ()
-        # endregion
-        # region ReportStatus
-        # Get command from Telegram
-        command = None
-        if MODE in ('T', 'TC') and self.connection_analytic and self.heartbeat_counter % 5 == 0:
-            cursor_analytic = self.connection_analytic.cursor()
-            bot_id = self.tlg_header.split('.')[0]
-            try:
-                cursor_analytic.execute('SELECT max(message_id), text_in, bot_id\
-                                        FROM t_control WHERE bot_id=:bot_id', {'bot_id': bot_id})
-                row = cursor_analytic.fetchone()
-                cursor_analytic.close()
-            except sqlite3.Error as err:
-                cursor_analytic.close()
-                row = None
-                print(f"SELECT from t_control: {err}")
-            if row and row[0]:
-                # Analyse and execute received command
-                command = row[1]
-                if command != 'status':
-                    self.command = command
-                    command = None
-                # Remove applied command from .db
+    def save_strategy_state(self, return_only=False) -> Dict[str, str]:
+        if not return_only:
+            # region SaveOperationalStatus
+            # Skip when transition processes or GRID_ONLY mode
+            stable_state = (self.shift_grid_threshold is None
+                            and self.grid_remove is None
+                            and not self.reverse_hold
+                            and not GRID_ONLY
+                            and not self.grid_update_started
+                            and not self.start_after_shift
+                            and not self.tp_hold
+                            and not self.tp_was_filled
+                            and not self.orders_init)
+            if MODE in ('T', 'TC') and stable_state:
+                orders = self.get_buffered_open_orders()
+                order_buy = len([i for i in orders if i.buy is True])
+                order_sell = len([i for i in orders if i.buy is False])
+                order_hold = len(self.orders_hold)
+                cycle_status = (self.cycle_buy, order_buy, order_sell, order_hold)
+                if self.cycle_status != cycle_status:
+                    self.cycle_status = cycle_status
+                    data_to_db = {'f_currency': self.f_currency,
+                                  's_currency': self.s_currency,
+                                  'cycle_buy': self.cycle_buy,
+                                  'order_buy': order_buy,
+                                  'order_sell': order_sell,
+                                  'order_hold': order_hold,
+                                  'destination': 't_orders'}
+                    if self.queue_to_db:
+                        # print('Send data to t_orders')
+                        self.queue_to_db.put(data_to_db)
+            else:
+                self.cycle_status = ()
+            # endregion
+            # region ReportStatus
+            # Get command from Telegram
+            command = None
+            if MODE in ('T', 'TC') and self.connection_analytic and self.heartbeat_counter % 5 == 0:
+                cursor_analytic = self.connection_analytic.cursor()
+                bot_id = self.tlg_header.split('.')[0]
                 try:
-                    self.connection_analytic.execute('UPDATE t_control SET apply = 1 WHERE message_id=:message_id',
-                                                     {'message_id': row[0]})
-                    self.connection_analytic.commit()
+                    cursor_analytic.execute('SELECT max(message_id), text_in, bot_id\
+                                            FROM t_control WHERE bot_id=:bot_id', {'bot_id': bot_id})
+                    row = cursor_analytic.fetchone()
+                    cursor_analytic.close()
                 except sqlite3.Error as err:
-                    print(f"UPDATE t_control: {err}")
-            # self.message_log(f"save_strategy_state.command: {self.command}", log_level=LogLevel.DEBUG)
-        if self.command == 'stopped':
-            if isinstance(self.start_collect, int):
-                if self.start_collect < 5:
-                    self.start_collect += 1
-                else:
-                    self.start_collect = False
-        elif self.command == 'restart':
-            self.stop()
-            os.execv(sys.executable, [sys.executable] + [sys.argv[0]] + ['1'])
-        if (MODE in ('T', 'TC') and
-                (command or (STATUS_DELAY and (self.local_time() - self.status_time) / 60 > STATUS_DELAY))):
-            # Report current status
-            last_price = self.get_buffered_ticker().last_price
-            ticker_update = int(self.local_time()) - self.last_ticker_update
-            if self.cycle_time:
-                ct = str(datetime.utcnow() - self.cycle_time).rsplit('.')[0]
-            else:
-                self.message_log("save_strategy_state: cycle_time is None!", log_level=LogLevel.DEBUG)
-                ct = str(datetime.utcnow()).rsplit('.')[0]
+                    cursor_analytic.close()
+                    row = None
+                    print(f"SELECT from t_control: {err}")
+                if row and row[0]:
+                    # Analyse and execute received command
+                    command = row[1]
+                    if command != 'status':
+                        self.command = command
+                        command = None
+                    # Remove applied command from .db
+                    try:
+                        self.connection_analytic.execute('UPDATE t_control SET apply = 1 WHERE message_id=:message_id',
+                                                         {'message_id': row[0]})
+                        self.connection_analytic.commit()
+                    except sqlite3.Error as err:
+                        print(f"UPDATE t_control: {err}")
+                # self.message_log(f"save_strategy_state.command: {self.command}", log_level=LogLevel.DEBUG)
             if self.command == 'stopped':
-                self.message_log("Strategy stopped. Need manual action", tlg=True)
-            elif self.grid_hold or self.tp_order_hold:
-                funds = self.get_buffered_funds()
-                fund_f = funds.get(self.f_currency, 0)
-                fund_f = fund_f.available if fund_f else 0
-                fund_s = funds.get(self.s_currency, 0)
-                fund_s = fund_s.available if fund_s else 0
-                if self.grid_hold.get('timestamp'):
-                    time_diff = int(self.local_time() - self.grid_hold['timestamp'])
-                    self.message_log(f"Exist unreleased grid orders for\n"
-                                     f"{'Buy' if self.cycle_buy else 'Sell'} cycle with"
-                                     f" {self.grid_hold['depo']}"
-                                     f" {self.s_currency if self.cycle_buy else self.f_currency} depo.\n"
-                                     f"Available first: {fund_f} {self.f_currency}\n"
-                                     f"Available second: {fund_s} {self.s_currency}\n"
-                                     f"Last ticker price: {last_price}\n"
-                                     f"WSS status: {ticker_update}s\n"
-                                     f"From start {ct}\n"
-                                     f"Delay: {time_diff} sec", tlg=True)
-                elif self.tp_order_hold['timestamp']:
-                    time_diff = int(self.local_time() - self.tp_order_hold['timestamp'])
-                    if time_diff > HOLD_TP_ORDER_TIMEOUT:
-                        self.message_log(f"Exist hold TP order for"
-                                         f" {'Sell' if self.cycle_buy else 'Buy'} {self.tp_order_hold['amount']}"
-                                         f" {self.f_currency if self.cycle_buy else self.s_currency}\n"
-                                         f"Available first:{fund_f} {self.f_currency}\n"
-                                         f"Available second:{fund_s} {self.s_currency}\n"
+                if isinstance(self.start_collect, int):
+                    if self.start_collect < 5:
+                        self.start_collect += 1
+                    else:
+                        self.start_collect = False
+            elif self.command == 'restart':
+                self.stop()
+                os.execv(sys.executable, [sys.executable] + [sys.argv[0]] + ['1'])
+            if (MODE in ('T', 'TC') and
+                    (command or (STATUS_DELAY and (self.local_time() - self.status_time) / 60 > STATUS_DELAY))):
+                # Report current status
+                last_price = self.get_buffered_ticker().last_price
+                ticker_update = int(self.local_time()) - self.last_ticker_update
+                if self.cycle_time:
+                    ct = str(datetime.utcnow() - self.cycle_time).rsplit('.')[0]
+                else:
+                    self.message_log("save_strategy_state: cycle_time is None!", log_level=LogLevel.DEBUG)
+                    ct = str(datetime.utcnow()).rsplit('.')[0]
+                if self.command == 'stopped':
+                    self.message_log("Strategy stopped. Need manual action", tlg=True)
+                elif self.grid_hold or self.tp_order_hold:
+                    funds = self.get_buffered_funds()
+                    fund_f = funds.get(self.f_currency, 0)
+                    fund_f = fund_f.available if fund_f else 0
+                    fund_s = funds.get(self.s_currency, 0)
+                    fund_s = fund_s.available if fund_s else 0
+                    if self.grid_hold.get('timestamp'):
+                        time_diff = int(self.local_time() - self.grid_hold['timestamp'])
+                        self.message_log(f"Exist unreleased grid orders for\n"
+                                         f"{'Buy' if self.cycle_buy else 'Sell'} cycle with"
+                                         f" {self.grid_hold['depo']}"
+                                         f" {self.s_currency if self.cycle_buy else self.f_currency} depo.\n"
+                                         f"Available first: {fund_f} {self.f_currency}\n"
+                                         f"Available second: {fund_s} {self.s_currency}\n"
                                          f"Last ticker price: {last_price}\n"
                                          f"WSS status: {ticker_update}s\n"
                                          f"From start {ct}\n"
                                          f"Delay: {time_diff} sec", tlg=True)
-            else:
-                if self.cycle_status:
-                    order_buy = self.cycle_status[1]
-                    order_sell = self.cycle_status[2]
-                    order_hold = self.cycle_status[3]
-                else:
-                    orders = self.get_buffered_open_orders()
-                    order_buy = len([i for i in orders if i.buy is True])
-                    order_sell = len([i for i in orders if i.buy is False])
-                    order_hold = len(self.orders_hold)
-                sum_profit = self.round_truncate(self.sum_profit_first * self.avg_rate + self.sum_profit_second,
-                                                 base=False)
-                command = bool(self.command in ('end', 'stop'))
-                if GRID_ONLY:
-                    header = (f"{'Buy' if self.cycle_buy else 'Sell'} assets Grid only mode\n"
-                              f"{('Waiting funding for convert'+chr(10)) if self.grid_only_restart else ''}"
-                              f"{self.get_free_assets()[3]}"
-                              )
+                    elif self.tp_order_hold['timestamp']:
+                        time_diff = int(self.local_time() - self.tp_order_hold['timestamp'])
+                        if time_diff > HOLD_TP_ORDER_TIMEOUT:
+                            self.message_log(f"Exist hold TP order for"
+                                             f" {'Sell' if self.cycle_buy else 'Buy'} {self.tp_order_hold['amount']}"
+                                             f" {self.f_currency if self.cycle_buy else self.s_currency}\n"
+                                             f"Available first:{fund_f} {self.f_currency}\n"
+                                             f"Available second:{fund_s} {self.s_currency}\n"
+                                             f"Last ticker price: {last_price}\n"
+                                             f"WSS status: {ticker_update}s\n"
+                                             f"From start {ct}\n"
+                                             f"Delay: {time_diff} sec", tlg=True)
                 else:
-                    header = (f"Complete {self.cycle_buy_count} buy cycle and {self.cycle_sell_count} sell cycle\n"
-                              f"For all cycles profit:\n"
-                              f"First: {self.sum_profit_first}\n"
-                              f"Second: {self.sum_profit_second}\n"
-                              f"Summary: {sum_profit}\n"
-                              f"{self.get_free_assets(mode='free')[3]}"
-                              )
-                self.message_log(f"{header}\n"
-                                 f"{'*** Shift grid mode ***' if self.shift_grid_threshold else '* ***  ***  *** *'}\n"
-                                 f"{'Buy' if self.cycle_buy else 'Sell'}{' Reverse' if self.reverse else ''}"
-                                 f"{' Hold reverse' if self.reverse_hold else ''} cycle with"
-                                 f" {order_buy} buy and {order_sell} sell active orders.\n"
-                                 f"{order_hold if order_hold else 'No'} hold grid orders\n"
-                                 f"Over price: {self.over_price:.2f}%\n"
-                                 f"Last ticker price: {last_price}\n"
-                                 f"ver: {HEAD_VERSION}+{__version__}+{msb_ver}\n"
-                                 f"From start {ct}\n"
-                                 f"WSS status: {ticker_update}s\n"
-                                 f"{'-   ***   ***   ***   -' if self.command == 'stop' else ''}\n"
-                                 f"{'Waiting for end of cycle for manual action' if command else ''}",
-                                 tlg=True)
-        # endregion
-        # region ProcessingEvent
-        if self.wait_wss_refresh and self.local_time() - self.wait_wss_refresh['timestamp'] > SHIFT_GRID_DELAY:
-            self.place_grid(self.wait_wss_refresh['buy_side'],
-                            self.wait_wss_refresh['depo'],
-                            self.reverse_target_amount,
-                            self.wait_wss_refresh['allow_grid_shift'],
-                            self.wait_wss_refresh['additional_grid'],
-                            self.wait_wss_refresh['grid_update'])
-        self.heartbeat_counter += 1
-        if self.heartbeat_counter % 5 == 0 and not STANDALONE and EXTRA_CHECK_ORDER_STATE:
-            self.check_order_status()
-        if (stable_state
-                and ADAPTIVE_TRADE_CONDITION
-                and not self.reverse
-                and not self.part_amount
-                and self.command not in ('stopped', 'stop', 'end')
-                and (self.orders_grid or self.orders_hold)):
-            if self.heartbeat_counter % 150 == 0:
-                self.grid_update(frequency='low')
-            elif self.heartbeat_counter % 30 == 0:
-                self.grid_update(frequency='mid')
-            else:
-                self.grid_update(frequency='hi')
-        if self.heartbeat_counter > 150:
-            self.heartbeat_counter = 0
-            if MODE in ('T', 'TC') and not GRID_ONLY:
-                # Update t_funds.active set True
-                data_to_db = {'f_currency': self.f_currency,
-                              's_currency': self.s_currency,
-                              'destination': 't_funds.active update'}
-                if self.queue_to_db:
-                    self.queue_to_db.put(data_to_db)
-        if self.wait_refunding_for_start or self.tp_order_hold or self.grid_hold:
-            self.get_buffered_funds()
-        if self.tp_error:
-            self.tp_error = False
-            self.place_profit_order()
-        if self.reverse_hold:
-            if self.start_reverse_time:
-                if self.local_time() - self.start_reverse_time > 2 * SHIFT_GRID_DELAY:
-                    last_price = self.get_buffered_ticker().last_price
-                    if self.cycle_buy:
-                        price_diff = 100 * (self.reverse_price - last_price) / self.reverse_price
+                    if self.cycle_status:
+                        order_buy = self.cycle_status[1]
+                        order_sell = self.cycle_status[2]
+                        order_hold = self.cycle_status[3]
                     else:
-                        price_diff = 100 * (last_price - self.reverse_price) / self.reverse_price
-                    if price_diff > ADX_PRICE_THRESHOLD:
-                        # Reverse
-                        self.cycle_buy = not self.cycle_buy
-                        self.command = 'stop' if REVERSE_STOP else None
-                        self.reverse = True
-                        self.reverse_hold = False
-                        self.sum_amount_first = self.tp_part_amount_first
-                        self.sum_amount_second = self.tp_part_amount_second
-                        self.tp_part_amount_first = Decimal('0')
-                        self.tp_part_amount_second = Decimal('0')
-                        self.message_log('Release Hold reverse cycle', color=Style.B_WHITE)
-                        self.start()
-            else:
-                self.start_reverse_time = self.local_time()
-        # endregion
+                        orders = self.get_buffered_open_orders()
+                        order_buy = len([i for i in orders if i.buy is True])
+                        order_sell = len([i for i in orders if i.buy is False])
+                        order_hold = len(self.orders_hold)
+                    sum_profit = self.round_truncate(self.sum_profit_first * self.avg_rate + self.sum_profit_second,
+                                                     base=False)
+                    command = bool(self.command in ('end', 'stop'))
+                    if GRID_ONLY:
+                        header = (f"{'Buy' if self.cycle_buy else 'Sell'} assets Grid only mode\n"
+                                  f"{('Waiting funding for convert'+chr(10)) if self.grid_only_restart else ''}"
+                                  f"{self.get_free_assets()[3]}"
+                                  )
+                    else:
+                        header = (f"Complete {self.cycle_buy_count} buy cycle and {self.cycle_sell_count} sell cycle\n"
+                                  f"For all cycles profit:\n"
+                                  f"First: {self.sum_profit_first}\n"
+                                  f"Second: {self.sum_profit_second}\n"
+                                  f"Summary: {sum_profit}\n"
+                                  f"{self.get_free_assets(mode='free')[3]}"
+                                  )
+                    self.message_log(f"{header}\n"
+                                     f"{'*** Shift grid mode ***' if self.shift_grid_threshold else '* **  **  ** *'}\n"
+                                     f"{'Buy' if self.cycle_buy else 'Sell'}{' Reverse' if self.reverse else ''}"
+                                     f"{' Hold reverse' if self.reverse_hold else ''} cycle with"
+                                     f" {order_buy} buy and {order_sell} sell active orders.\n"
+                                     f"{order_hold if order_hold else 'No'} hold grid orders\n"
+                                     f"Over price: {self.over_price:.2f}%\n"
+                                     f"Last ticker price: {last_price}\n"
+                                     f"ver: {HEAD_VERSION}+{__version__}+{msb_ver}\n"
+                                     f"From start {ct}\n"
+                                     f"WSS status: {ticker_update}s\n"
+                                     f"{'-   ***   ***   ***   -' if self.command == 'stop' else ''}\n"
+                                     f"{'Waiting for end of cycle for manual action' if command else ''}",
+                                     tlg=True)
+            # endregion
+            # region ProcessingEvent
+            if self.wait_wss_refresh and self.local_time() - self.wait_wss_refresh['timestamp'] > SHIFT_GRID_DELAY:
+                self.place_grid(self.wait_wss_refresh['buy_side'],
+                                self.wait_wss_refresh['depo'],
+                                self.reverse_target_amount,
+                                self.wait_wss_refresh['allow_grid_shift'],
+                                self.wait_wss_refresh['additional_grid'],
+                                self.wait_wss_refresh['grid_update'])
+            self.heartbeat_counter += 1
+            if self.heartbeat_counter % 5 == 0 and not STANDALONE and EXTRA_CHECK_ORDER_STATE:
+                self.check_order_status()
+            if (stable_state
+                    and ADAPTIVE_TRADE_CONDITION
+                    and not self.reverse
+                    and not self.part_amount
+                    and self.command not in ('stopped', 'stop', 'end')
+                    and (self.orders_grid or self.orders_hold)):
+                if self.heartbeat_counter % 150 == 0:
+                    self.grid_update(frequency='low')
+                elif self.heartbeat_counter % 30 == 0:
+                    self.grid_update(frequency='mid')
+                else:
+                    self.grid_update(frequency='hi')
+            if self.heartbeat_counter > 150:
+                self.heartbeat_counter = 0
+                if MODE in ('T', 'TC') and not GRID_ONLY:
+                    # Update t_funds.active set True
+                    data_to_db = {'f_currency': self.f_currency,
+                                  's_currency': self.s_currency,
+                                  'destination': 't_funds.active update'}
+                    if self.queue_to_db:
+                        self.queue_to_db.put(data_to_db)
+            if self.wait_refunding_for_start or self.tp_order_hold or self.grid_hold:
+                self.get_buffered_funds()
+            if self.tp_error:
+                self.tp_error = False
+                self.place_profit_order()
+            if self.reverse_hold:
+                if self.start_reverse_time:
+                    if self.local_time() - self.start_reverse_time > 2 * SHIFT_GRID_DELAY:
+                        last_price = self.get_buffered_ticker().last_price
+                        if self.cycle_buy:
+                            price_diff = 100 * (self.reverse_price - last_price) / self.reverse_price
+                        else:
+                            price_diff = 100 * (last_price - self.reverse_price) / self.reverse_price
+                        if price_diff > ADX_PRICE_THRESHOLD:
+                            # Reverse
+                            self.cycle_buy = not self.cycle_buy
+                            self.command = 'stop' if REVERSE_STOP else None
+                            self.reverse = True
+                            self.reverse_hold = False
+                            self.sum_amount_first = self.tp_part_amount_first
+                            self.sum_amount_second = self.tp_part_amount_second
+                            self.tp_part_amount_first = Decimal('0')
+                            self.tp_part_amount_second = Decimal('0')
+                            self.message_log('Release Hold reverse cycle', color=Style.B_WHITE)
+                            self.start()
+                else:
+                    self.start_reverse_time = self.local_time()
+            # endregion
         if MODE in ('T', 'TC'):
             return {'command': json.dumps(self.command),
                     'cycle_buy': json.dumps(self.cycle_buy),
                     'cycle_buy_count': json.dumps(self.cycle_buy_count),
                     'cycle_sell_count': json.dumps(self.cycle_sell_count),
                     'cycle_time': json.dumps(self.cycle_time, default=str),
                     'cycle_time_reverse': json.dumps(self.cycle_time_reverse, default=str),
@@ -1429,19 +1530,24 @@
             self.message_log(f"Complete {self.cycle_buy_count} buy cycle and {self.cycle_sell_count} sell cycle\n"
                              f"For all cycles profit:\n"
                              f"First: {self.sum_profit_first}\n"
                              f"Second: {self.sum_profit_second}\n"
                              f"Summary: {self.sum_profit_first * self.avg_rate + self.sum_profit_second:f}\n")
         if self.first_run or MODE in ('T', 'TC'):
             self.cycle_time = datetime.utcnow()
-        mem = psutil.virtual_memory().percent if psutil else 0
-        if mem > 85:
+        if psutil:
+            memory = psutil.virtual_memory()
+            swap = psutil.swap_memory()
+            total_used_percent = 100 * float(swap.used + memory.used) / (swap.total + memory.total)
+        else:
+            total_used_percent = 0
+        if total_used_percent > 85:
             self.message_log(f"For {VPS_NAME} critical memory availability, end", tlg=True)
             self.command = 'end'
-        elif mem > 75:
+        elif total_used_percent > 75:
             self.message_log(f"For {VPS_NAME} low memory availability, stop after end of cycle", tlg=True)
             self.command = 'stop'
         if self.command == 'end' or (self.command == 'stop' and
                                      (not self.reverse or (self.reverse and REVERSE_STOP))):
             self.command = 'stopped'
             self.start_collect = 1
             self.message_log('Stop, waiting manual action', tlg=True)
@@ -1608,18 +1714,19 @@
                                                   include_current_building_candle=True)
         for i in candle:
             high.append(i.high)
             low.append(i.low)
             close.append(i.close)
         n = 1
         while n <= len(high) - 1:
-            tr_arr.append(max(high[n] - low[n], abs(high[n] - close[n - 1]), abs(low[n] - close[n - 1])))
+            i = max(high[n] - low[n], abs(high[n] - close[n - 1]), abs(low[n] - close[n - 1]))
+            if i:
+                tr_arr.append(i)
             n += 1
-        _atr = statistics.geometric_mean(tr_arr)
-        return _atr
+        return statistics.geometric_mean(tr_arr)
 
     def adx(self, adx_candle_size_in_minutes: int, adx_number_of_candles: int, adx_period: int) -> Dict[str, float]:
         """
         Average Directional Index
         Math from https://blog.quantinsti.com/adx-indicator-python/
         Test data
         high = [90, 95, 105, 120, 140, 165, 195, 230, 270, 315, 365]
@@ -1729,20 +1836,21 @@
                          f" part_profit_second: {self.part_profit_second}\n"
                          f"! deposit_first: {self.deposit_first}, deposit_second: {self.deposit_second}\n"
                          f"! command: {self.command}\n"
                          f"! reverse: {self.reverse}\n"
                          f"! Profit: {self.get_sum_profit()}\n"
                          f"! ======================================")
 
-    def get_free_assets(self, ff: Decimal = None, fs: Decimal = None, mode: str = 'total') -> ():
+    def get_free_assets(self, ff: Decimal = None, fs: Decimal = None, mode: str = 'total', backtest=False) -> ():
         """
         Get free asset for current trade pair
         :param fs:
         :param ff:
         :param mode: 'total', 'free', 'reserved'
+        :param backtest: bool
         :return: (ff, fs, ft, free_asset: str)
         """
         if ff is None or fs is None:
             funds = self.get_buffered_funds()
             _ff = funds.get(self.f_currency, 0)
             _fs = funds.get(self.s_currency, 0)
             ff = Decimal('0')
@@ -1756,17 +1864,21 @@
                     fs = f2d(_fs.available)
                 elif mode == 'reserved':
                     ff = f2d(_ff.reserved)
                     fs = f2d(_fs.reserved)
         #
         if mode == 'free':
             if self.cycle_buy:
+                if backtest:
+                    ff = self.initial_reverse_first if self.reverse else self.initial_first
                 fs = (self.initial_reverse_second if self.reverse else self.initial_second) - self.deposit_second
             else:
                 ff = (self.initial_reverse_first if self.reverse else self.initial_first) - self.deposit_first
+                if backtest:
+                    fs = self.initial_reverse_second if self.reverse else self.initial_second
         ff = self.round_truncate(ff, base=True)
         fs = self.round_truncate(fs, base=False)
         ft = ff * self.avg_rate + fs
         assets = f"{mode.capitalize()}: First: {ff}, Second: {fs}"
         return ff, fs, ft, assets
 
     def round_truncate(self, _x: Decimal, base: bool, fee: bool = False, _rounding=ROUND_FLOOR) -> Decimal:
```

### Comparing `martin-binance-1.3.0b23/martin_binance/funds_rate.db.template` & `martin-binance-1.3.1b0/martin_binance/funds_rate.db.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b23/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so` & `martin-binance-1.3.1b0/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b23/martin_binance/margin_wrapper.py` & `martin-binance-1.3.1b0/martin_binance/margin_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 margin.de <-> Python strategy <-> <margin_wrapper> <-> exchanges-wrapper <-> Exchanges API/WSS
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0b21"
+__version__ = "1.3.0-3"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 import ast
 import asyncio
 import simplejson as json
 import logging
@@ -126,14 +126,16 @@
     for _trade in StrategyBase.trades:
         if _trade.order_id == _order_id:
             saved_filled_quantity += Decimal(str(_trade.amount))
     return saved_filled_quantity
 
 
 class PrivateTrade:
+    __slots__ = ("amount", "buy", "id", "order_id", "price", "timestamp")
+
     def __init__(self, _trade: {}) -> None:
         # Amount of the trade.
         self.amount = float(_trade["qty"])
         # True, if the trade was a buy.
         self.buy = _trade.get('isBuyer', False)
         # id of the trade.
         self.id = _trade["id"]
@@ -146,18 +148,22 @@
 
     def __call__(self):
         return self
 
 
 # noinspection PyRedeclaration
 class OrderUpdate(OrderUpdate):
+    __slots__ = ("original_order", "resulting_trades", "status", "timestamp", "updated_order")
+
     def __init__(self, event: {}) -> None:
         super().__init__()
 
         class OriginalOrder:
+            __slots__ = ("id",)
+
             def __init__(self, _event: {}):
                 self.id = _event['order_id']
 
         # Original order previous to this update.
         self.original_order = OriginalOrder(event)
         # Trades that belong to the order, if any exist so far.
         self.resulting_trades = []
@@ -179,14 +185,16 @@
         self.updated_order = None
 
     def __call__(self):
         return self
 
 
 class Order:
+    __slots__ = ("amount", "buy", "id", "order_type", "price", "received_amount", "remaining_amount", "timestamp")
+
     def __init__(self, order: {}) -> None:
         # Overall amount of the order.
         self.amount = float(order['origQty'])
         # True if the order is a buy order.
         self.buy = bool(order['side'] == 'BUY')
         # id of the order.
         self.id = int(order['orderId'])
@@ -202,14 +210,16 @@
         self.timestamp = int(order.get('transactTime', order.get('time', time.time())))
 
     def __call__(self):
         return self
 
 
 class Candle:
+    __slots__ = ("min_time", "open", "high", "low", "close", "volume", "max_time", "trade_number", "vwap")
+
     def __init__(self, _candle: []) -> None:
         # Start time of the candle.
         self.min_time = int(_candle[0])
         # Price of the first trade in the candle.
         self.open = float(_candle[1])
         # Highest traded price in the candle.
         self.high = float(_candle[2])
@@ -227,14 +237,24 @@
         self.vwap = (float(_candle[7]) / self.volume) if self.volume else self.close
 
     def __call__(self):
         return self
 
 
 class TradingCapabilityManager:
+    __slots__ = ("base_asset_precision",
+                 "quote_asset_precision",
+                 "min_qty",
+                 "max_qty",
+                 "step_size",
+                 "min_notional",
+                 "tick_size",
+                 "multiplier_up",
+                 "multiplier_down")
+
     def __init__(self, _exchange_info_symbol):
         self.base_asset_precision = int(_exchange_info_symbol.get('baseAssetPrecision'))
         self.quote_asset_precision = int(_exchange_info_symbol.get('quoteAssetPrecision'))
         self.min_qty = float(_exchange_info_symbol['filters']['lotSize']['minQty'])
         self.max_qty = float(_exchange_info_symbol['filters']['lotSize']['maxQty'])
         self.step_size = float(_exchange_info_symbol['filters']['lotSize']['stepSize'])
         self.min_notional = float(_exchange_info_symbol['filters'].get('notional', {}).get('minNotional', 0))
@@ -307,65 +327,87 @@
         return self.round_price(avg_price * self.multiplier_up, RoundingType.FLOOR)
 
     def get_min_buy_price(self, avg_price: float) -> float:
         return self.round_price(avg_price * self.multiplier_down, RoundingType.CEIL)
 
 
 class Ticker:
+    __slots__ = ("last_day_price", "last_price", "timestamp")
+
     def __init__(self, _ticker):
         # Price of the currency pair one day ago.
         self.last_day_price = float(_ticker.get('openPrice', 0))
         # Last traded price of the currency pair.
         self.last_price = float(_ticker.get('lastPrice', 0))
         # Timestamp of the ticker data.
         self.timestamp = int(_ticker.get('closeTime', 0))
         # print(f"self.last_price: {self.last_price}")
 
     def __call__(self):
         return self
 
 
 class FundsEntry:
+    __slots__ = ("available", "reserved", "total_for_currency")
+
     def __init__(self, _funds):
         # The available amount for a currency.
         self.available = float(_funds.get('free'))
         # The reserved amount for a currency.
         self.reserved = float(_funds.get('locked'))
         # Total amount of a currency in the account.
         self.total_for_currency = float(Decimal(_funds.get('free')) + Decimal(_funds.get('locked')))
         # print(f"self.total_for_currency: {self.total_for_currency}")
 
     def __call__(self):
         return self
 
 
 class OrderBook:
+    __slots__ = ("asks", "bids")
+
     """
     order_book.bids[0].price
     order_book.asks[0].amount
     """
     def __init__(self, _order_book) -> None:
+
         class _OrderBookRow:
+            __slots__ = ("price", "amount")
+
             def __init__(self, _order) -> None:
                 self.price = float(_order[0])
                 self.amount = float(_order[1])
+
         self.asks = []
         # List of asks ordered by price in ascending order.
         self.bids = []
         # List of bids ordered by price in descending order.
         for _, v in enumerate(_order_book['asks']):
             self.asks.append(_OrderBookRow(v))
         for _, v in enumerate(_order_book['bids']):
             self.bids.append(_OrderBookRow(v))
 
     def __call__(self):
         return self
 
 
 class StrategyBase:
+    __slots__ = (
+        "time_operational",
+        "s_ticker",
+        "s_order_book",
+        "klines",
+        "candles",
+        "account",
+        "grid_buy",
+        "grid_sell",
+        "get_buffered_funds_last_time",
+    )
+
     session = None
     client: api_pb2.OpenClientConnectionId = None
     exchange = str()
     symbol = str()
     channel: grpc.Channel = None
     stub = api_pb2_grpc.MartinStub
     client_id = int()
@@ -381,24 +423,39 @@
     canceled_order_id = []  # List canceled orders  for time-out detect
     all_trades = []  # List of all (limit = ALL_TRADES_LIST_LIMIT) trades for a specific account and symbol
     trades = []  # List of trades associated with strategy (limit = TRADES_LIST_LIMIT)
     all_orders = []  # List of all open orders for symbol
     orders = []  # List orders associated with strategy
     tcm = None  # TradingCapabilityManager
     last_state = None
-    get_buffered_funds_last_time = time.time()
     rate_limiter = RATE_LIMITER
     start_time_ms = int(time.time() * 1000)
     send_request = None
     for_request = None
     wss_fire_up = False
     backtest = {}
     delay_ordering_s = 0.5
     bulk_orders_cancel = {}
+    session_root: Path
+    state_file: Path
+
+    def __init__(self):
+        print("Init StrategyBase")
+        self.time_operational = {'start': 0.0, 'ts': 0.0, 'new': 0.0}  # - See get_time()
+        self.s_ticker = {}
+        self.s_order_book = {}
+        self.klines = {}  # KLines snapshot
+        self.candles = {}  # Candles stream
+        self.account = backTestAccount(ms.SAVE_DS) if ms.MODE == 'S' else None
+        self.grid_buy = {}
+        self.grid_sell = {}
+        self.get_buffered_funds_last_time = self.get_time()
 
+    def __call__(self):
+        return self
 
     class Klines:
         klines_series = {}
         klines_lim = int()
 
         def __init__(self, _interval):
             self.interval = _interval
@@ -419,29 +476,14 @@
                         del self.kline[0]
                 self.klines_series[self.interval] = self.kline
 
         @classmethod
         def get_kline(cls, _interval) -> []:
             return cls.klines_series.get(_interval, [])
 
-
-    def __init__(self):
-        print("Init StrategyBase")
-        self.time_operational = {'start': 0.0, 'ts': 0.0, 'new': 0.0}  # - See get_time()
-        self.s_ticker = {}
-        self.s_order_book = {}
-        self.klines = {}  # KLines snapshot
-        self.candles = {}  # Candles stream
-        self.account = backTestAccount(ms.SAVE_DS) if ms.MODE == 'S' else None
-        self.grid_buy = {}
-        self.grid_sell = {}
-
-    def __call__(self):
-        return self
-
     def reset_var(self):
         self.s_ticker = {}
         self.s_order_book = {}
         self.klines = {}  # KLines snapshot
         self.candles = {}  # Candles stream
         self.grid_buy = {}
         self.grid_sell = {}
@@ -455,31 +497,30 @@
         cls.order_id = int(datetime.now().strftime("%S%M")) * 1000
         cls.wait_order_id = []  # List of placed orders for time-out detect
         cls.canceled_order_id = []  # List canceled orders  for time-out detect
         cls.all_trades = []  # List of all (limit = ALL_TRADES_LIST_LIMIT) trades for a specific account and symbol
         cls.trades = []  # List of trades associated with strategy (limit = TRADES_LIST_LIMIT)
         cls.all_orders = []  # List of all open orders for symbol
         cls.orders = []  # List orders associated with strategy
-        cls.get_buffered_funds_last_time = time.time()
+        cls.strategy.get_buffered_funds_last_time = cls.strategy.get_time()
         cls.rate_limiter = RATE_LIMITER
         cls.start_time_ms = int(time.time() * 1000)
         cls.backtest = {}
         cls.bulk_orders_cancel = {}
 
-    def message_log(self,*args, **kwargs):
-        pass
+    def message_log(self, *args, **kwargs):
+        pass  # meant to be overridden in a subclass
 
     def order_exist(self, _id) -> bool:
         return any(i.id == _id for i in self.orders)
 
     def all_order_exist(self, _id) -> bool:
         return any(i.id == _id for i in self.all_orders)
 
     def get_trading_capability_manager(self) -> TradingCapabilityManager:
-        # print(f"get_trading_capability_manager.tcm: {vars(StrategyBase.tcm)}")
         return self.tcm
 
     def get_first_currency(self) -> str:
         return self.info_symbol.get('baseAsset')
 
     def get_second_currency(self) -> str:
         return self.info_symbol.get('quoteAsset')
@@ -487,30 +528,29 @@
     def get_buffered_ticker(self) -> Ticker:
         # print(f"get_buffered_ticker.ticker: {self.ticker}")
         return Ticker(self.ticker)
 
     def get_buffered_funds(self) -> Dict[str, FundsEntry]:
         # print(f"get_buffered_funds.funds: {self.funds}")
         if self.strategy.local_time() - self.get_buffered_funds_last_time > self.rate_limiter:
-            # noinspection PyTypeChecker
             loop.create_task(buffered_funds(print_info=False))
-            self.get_buffered_funds_last_time = self.strategy.local_time()
+            self.get_buffered_funds_last_time = self.get_time()
         return {self.base_asset: FundsEntry(self.funds[self.base_asset]),
                 self.quote_asset: FundsEntry(self.funds[self.quote_asset])}
 
     def get_buffered_order_book(self) -> OrderBook:
         # print(f"get_buffered_order_book.order_book: {self.order_book}")
         return OrderBook(self.order_book)
 
     def place_limit_order(self, buy: bool, amount: Decimal, price: Decimal) -> int:
         cls = StrategyBase
         cls.order_id += 1
         self.message_log(f"Send order id:{cls.order_id} for {'BUY' if buy else 'SELL'}"
-                                          f" {any2str(amount)} by {any2str(price)} = {any2str(amount * price)}",
-                                          color=ms.Style.B_YELLOW)
+                         f" {any2str(amount)} by {any2str(price)} = {any2str(amount * price)}",
+                         color=ms.Style.B_YELLOW)
         loop.create_task(place_limit_order_timeout(cls.order_id))
         loop.create_task(create_limit_order(cls.order_id, buy, any2str(amount), any2str(price)))
         if cls.exchange == 'huobi':
             time.sleep(0.02)
         elif cls.exchange == 'okx':
             time.sleep(0.035)
         return cls.order_id
@@ -584,24 +624,21 @@
     @staticmethod
     def transfer_to_master(symbol: str, amount: str):
         loop.create_task(transfer2master(symbol, amount))
 
 
 async def heartbeat(_session):
     cls = StrategyBase
-    # print(f"tik-tak ', {int(time.time() * 1000)}, _client_id: {_client_id}")
+    # print(f"tik-tak:' {int(time.time() * 1000)}")
     last_exec_time = time.time()
     while cls.strategy:
         try:
             last_state = cls.strategy.save_strategy_state()
             if ms.MODE in ('T', 'TC'):
-                last_state[ms_order_id] = json.dumps(cls.order_id)
-                last_state['ms_start_time_ms'] = json.dumps(cls.start_time_ms)
-                last_state[ms_orders] = jsonpickle.encode(cls.orders)
-                last_state['ms_trades'] = jsonpickle.encode(cls.trades)
+                last_state_update(cls, last_state)
                 # print(f"heartbeat.last_state: {last_state}")
                 if ms.LAST_STATE_FILE.exists():
                     ms.LAST_STATE_FILE.replace(ms.LAST_STATE_FILE.with_suffix('.prev'))
                 with ms.LAST_STATE_FILE.open(mode='w') as outfile:
                     json.dump(last_state, outfile, sort_keys=True, indent=4, ensure_ascii=False)
                 #
                 update_max_queue_size = False
@@ -628,14 +665,21 @@
                         logger.warning(f"Exception on fire up WSS: {ex}")
                         cls.wss_fire_up = True
             await asyncio.sleep(HEARTBEAT)
         except (KeyboardInterrupt, asyncio.CancelledError):
             break
 
 
+def last_state_update(cls, last_state):
+    last_state[ms_order_id] = json.dumps(cls.order_id)
+    last_state['ms_start_time_ms'] = json.dumps(cls.start_time_ms)
+    last_state[ms_orders] = jsonpickle.encode(cls.orders)
+    last_state['ms_trades'] = jsonpickle.encode(cls.trades)
+
+
 async def save_asset():
     """
     Update account asset list and value in t_asset
     """
     cls = StrategyBase
     connection_analytic = None
     while connection_analytic is None:
@@ -753,20 +797,19 @@
 
 
 async def ask_exit():
     cls = StrategyBase
     if cls.strategy:
         cls.strategy.message_log("Got signal for exit", color=ms.Style.MAGENTA)
 
-        if ms.MODE == 'TC':
-            # Save stream data for backtesting
-            session_data_handler(cls.strategy)
-
         if ms.MODE in ('T', 'TC'):
             await cls.send_request(cls.stub.StopStream, api_pb2.MarketRequest, symbol=cls.symbol)
+            if ms.MODE == 'TC':
+                # Save stream data for backtesting
+                session_data_handler(cls.strategy)
 
         tasks = [t for t in asyncio.all_tasks() if t is not asyncio.current_task()]
         [task.cancel() for task in tasks]
         print(f"Cancelling {len(tasks)} outstanding tasks")
         await asyncio.gather(*tasks, return_exceptions=True)
         try:
             cls.strategy.stop()
@@ -821,31 +864,33 @@
     #
     ds_ticker.to_pickle(Path(session_data, "ticker.pkl"))
     df_grid_sell.to_pickle(Path(session_data, "sell.pkl"))
     df_grid_buy.to_pickle(Path(session_data, "buy.pkl"))
     #
     copy(ms.PARAMS, Path(session_root, Path(ms.PARAMS).name))
 
-    shutil.make_archive(str(Path(BACKTEST_PATH,f"{session_root}_{datetime.now().strftime('%m%d-%H:%M')}")),
+    shutil.make_archive(str(Path(BACKTEST_PATH, f"{session_root}_{datetime.now().strftime('%m%d-%H:%M')}")),
                         'zip',
                         session_root)
 
     print(f"Stream data for backtesting saved to {session_root}")
 
 
 async def backtest_data_control():
     """
     Control memory usage and safe saving by predefined timetable
     """
     cls = StrategyBase.strategy
     delay = HEARTBEAT * 300  # 10 min
     ts = time.time()
-    while True:
-        mem = psutil.virtual_memory().percent
-        if time.time() - ts > ms.SAVE_PERIOD or mem > 70:
+    while 1:
+        memory = psutil.virtual_memory()
+        swap = psutil.swap_memory()
+        total_used_percent = 100 * float(swap.used + memory.used) / (swap.total + memory.total)
+        if time.time() - ts > ms.SAVE_PERIOD or total_used_percent > 70:
             sc = cls.start_collect
             if sc:
                 cls.start_collect = False
                 session_data_handler(cls)
                 cls.reset_var()
                 cls.start_collect = sc
                 ts = time.time()
@@ -1060,14 +1105,20 @@
                     diff_id = list(set(ms_orders_id).difference(exch_orders_id))
                     if diff_id:
                         cls.strategy.message_log(f"Executed order(s) is: {diff_id}", log_level=LogLevel.INFO)
                         for _id in diff_id:
                             await fetch_order(_id, _filled_update_call=True)
                     if not restore:
                         cls.strategy.restore_strategy_state(last_state)
+                        if ms.MODE == 'TC':
+                            last_state = cls.strategy.save_strategy_state(return_only=True)
+                            last_state_update(cls, last_state)
+                            with cls.state_file.open(mode='w') as outfile:
+                                json.dump(last_state, outfile, sort_keys=True, indent=4, ensure_ascii=False)
+                            cls.strategy.start_collect = True
                 except Exception as _ex:
                     cls.last_state = None
                     cls.strategy.message_log(f"Exception restore_strategy_state: {_ex}\n{traceback.format_exc()}",
                                              log_level=LogLevel.WARNING)
                 else:
                     restore = False
                     cls.strategy.message_log("Restored successfully", color=ms.Style.GREEN)
@@ -1121,15 +1172,15 @@
 
 
 def on_funds_update_handler(cls, funds):
     cls.funds.update(funds)
     funds = {cls.base_asset: FundsEntry(cls.funds[cls.base_asset]),
              cls.quote_asset: FundsEntry(cls.funds[cls.quote_asset])}
     cls.strategy.on_new_funds(funds)
-    cls.get_buffered_funds_last_time = cls.strategy.local_time()
+    cls.strategy.get_buffered_funds_last_time = cls.strategy.get_time()
 
 
 async def on_balance_update():
     cls = StrategyBase
     try:
         async for res in cls.for_request(cls.stub.OnBalanceUpdate, api_pb2.MarketRequest, symbol=cls.symbol):
             cls.strategy.on_balance_update(json.loads(res.balance))
@@ -1143,15 +1194,15 @@
     try:
         async for event in cls.for_request(cls.stub.OnOrderUpdate, api_pb2.MarketRequest, symbol=cls.symbol):
             # Only for registered orders on own pair
             ed = ast.literal_eval(json.loads(event.result))
             # print(f"on_order_update.ed: {ed}")
             on_order_update_handler(cls, ed)
     except Exception as ex:
-        logger.warning(f"Exception on WSS, on_order_update loop closed: {ex}")
+        logger.warning(f"Exception on WSS, on_order_update loop closed: {ex}\n{traceback.format_exc()}")
         cls.wss_fire_up = True
 
 
 def on_order_update_handler(cls, ed):
     if (cls.symbol == ed['symbol']
             and cls.strategy.order_exist(ed['order_id'])
             and ed['order_status'] in ('FILLED', 'PARTIALLY_FILLED')):
@@ -1478,15 +1529,15 @@
         ds_ticker.to_pickle(Path(session_path, "ticker.pkl"))
         df_grid_sell.to_pickle(Path(session_path, "sell.pkl"))
         df_grid_buy.to_pickle(Path(session_path, "buy.pkl"))
         copy(ms.PARAMS, Path(session_path, Path(ms.PARAMS).name))
         print(f"Session data saved to: {session_path}")
         #
     s_profit = session_result['profit'] = f"{cls.strategy.get_sum_profit()}"
-    s_free = session_result['free'] = f"{cls.strategy.get_free_assets(mode='free')[2]}"
+    s_free = session_result['free'] = f"{cls.strategy.get_free_assets(mode='free', backtest=True)[2]}"
     print(f"Session profit: {s_profit}, free: {s_free}, total: {float(s_profit) + float(s_free)}")
     loop.stop()
 
 
 def order_book_prepare(_order_book: {}) -> {}:
     order_book = json_format.MessageToDict(_order_book)
     order_book_bids = order_book.pop('bids', [])
@@ -1520,28 +1571,29 @@
     else:
         async for row in loop_ds(cls.backtest['order_book']):
             cls.order_book = row
             cls.strategy.on_new_order_book(OrderBook(cls.order_book))
         print("Backtest *** order_book *** timeSeries ended")
 
 
-def load_last_state() -> {}:
-    def load_file(name: Path) -> {}:
-        _res = {}
-        if name.exists():
-            try:
-                with name.open() as state_file:
-                    _last_state = json.load(state_file)
-            except json.JSONDecodeError as er:
-                print(f"Exception on decode last state file: {er}")
-            else:
-                if _last_state.get('ms_start_time_ms', None):
-                    _res = _last_state
-        return _res
+def load_file(name: Path) -> {}:
+    _res = {}
+    if name.exists():
+        try:
+            with name.open() as state_file:
+                _last_state = json.load(state_file)
+        except json.JSONDecodeError as er:
+            print(f"Exception on decode last state file: {er}")
+        else:
+            if _last_state.get('ms_start_time_ms', None):
+                _res = _last_state
+    return _res
 
+
+def load_last_state() -> {}:
     res = {}
     if ms.LAST_STATE_FILE.exists():
         res = load_file(ms.LAST_STATE_FILE)
         if not res:
             print("Can't load last state, try load previous saved state")
             res = load_file(ms.LAST_STATE_FILE.with_suffix('.prev'))
         if res:
@@ -1556,15 +1608,15 @@
     await buffered_candle()
     loop.create_task(on_order_book_update())
     if ms.MODE in ('T', 'TC'):
         # User Stream
         loop.create_task(on_funds_update())
         loop.create_task(on_order_update())
         loop.create_task(on_balance_update())
-        if ms.MODE =='TC':
+        if ms.MODE == 'TC':
             loop.create_task(backtest_data_control())
 
 
 async def wss_init(update_max_queue_size=False):
     cls = StrategyBase
     cls.strategy.message_log(f"Init WSS, client_id: {cls.client_id}")
     if cls.client_id:
@@ -1597,14 +1649,65 @@
     cls.channel = _session.channel
     cls.client_id = _session.client.client_id if _session.client else None
     cls.exchange = _session.client.exchange if _session.client else None
     cls.send_request = _session.send_request
     cls.for_request = _session.for_request
 
 
+def restore_state_before_backtesting(cls):
+    saved_state = load_file(cls.state_file)
+    cls.order_id = json.loads(saved_state.pop(ms_order_id, "0"))
+    cls.trades = jsonpickle.decode(saved_state.pop('ms_trades', '[]'))
+    cls.orders = jsonpickle.decode(saved_state.pop(ms_orders, '[]'))
+    orders = json.loads(saved_state.get('orders'))
+    # Restore initial state
+    cls.strategy.cycle_buy = json.loads(saved_state.get('cycle_buy'))
+    cls.strategy.reverse = json.loads(saved_state.get('reverse'))
+    cls.strategy.deposit_first = ms.f2d(json.loads(saved_state.get('deposit_first')))
+    cls.strategy.deposit_second = ms.f2d(json.loads(saved_state.get('deposit_second')))
+    if cls.strategy.reverse:
+        cls.strategy.initial_reverse_first = ms.f2d(json.loads(saved_state.get('initial_reverse_first')))
+        cls.strategy.initial_reverse_second = ms.f2d(json.loads(saved_state.get('initial_reverse_second')))
+        cls.strategy.account.funds.base = {'asset': cls.base_asset,
+                                           'free': cls.strategy.initial_reverse_first,
+                                           'locked': '0.0'}
+        cls.strategy.account.funds.quote = {'asset': cls.quote_asset,
+                                            'free': cls.strategy.initial_reverse_second,
+                                            'locked': '0.0'}
+    else:
+        if cls.strategy.cycle_buy:
+            cls.strategy.initial_second = cls.strategy.deposit_second
+        else:
+            cls.strategy.initial_first = cls.strategy.deposit_first
+    cls.strategy.account.restore_state(cls.symbol, cls.start_time_ms, orders)
+    cls.strategy.last_shift_time = json.loads(saved_state.get('last_shift_time')) or cls.strategy.local_time()
+    cls.strategy.order_q = json.loads(saved_state.get('order_q'))
+    cls.strategy.orders_grid.restore(json.loads(saved_state.get('orders')))
+    cls.strategy.orders_hold.restore(json.loads(saved_state.get('orders_hold')))
+    cls.strategy.orders_save.restore(json.loads(saved_state.get('orders_save')))
+    cls.strategy.over_price = json.loads(saved_state.get('over_price'))
+    cls.strategy.part_amount = eval(json.loads(saved_state.get('part_amount')))
+    cls.strategy.reverse_hold = json.loads(saved_state.get('reverse_hold'))
+    cls.strategy.reverse_init_amount = ms.f2d(json.loads(saved_state.get('reverse_init_amount')))
+    cls.strategy.reverse_price = json.loads(saved_state.get('reverse_price'))
+    cls.strategy.reverse_target_amount = ms.f2d(json.loads(saved_state.get('reverse_target_amount')))
+    cls.strategy.shift_grid_threshold = json.loads(saved_state.get('shift_grid_threshold'))
+    cls.strategy.sum_amount_first = ms.f2d(json.loads(saved_state.get('sum_amount_first')))
+    cls.strategy.sum_amount_second = ms.f2d(json.loads(saved_state.get('sum_amount_second')))
+    cls.strategy.tp_amount = ms.f2d(json.loads(saved_state.get('tp_amount')))
+    cls.strategy.tp_init = eval(json.loads(saved_state.get('tp_init')))
+    cls.strategy.tp_order_id = json.loads(saved_state.get('tp_order_id'))
+    cls.strategy.tp_part_amount_first = ms.f2d(json.loads(saved_state.get('tp_part_amount_first')))
+    cls.strategy.tp_part_amount_second = ms.f2d(json.loads(saved_state.get('tp_part_amount_second')))
+    cls.strategy.tp_target = ms.f2d(json.loads(saved_state.get('tp_target')))
+    cls.strategy.tp_order = eval(json.loads(saved_state.get('tp_order')))
+    cls.strategy.tp_wait_id = json.loads(saved_state.get('tp_wait_id'))
+    cls.strategy.start_collect = True
+
+
 async def main(_symbol):
     cls = StrategyBase
     cls.strategy = ms.Strategy()
     restore_state = None
     last_state = {}
     try:
         if cls.session is None:
@@ -1655,32 +1758,28 @@
                                       f" amount:{i['origQty']}, price:{i['price']}, status:{i['status']}")
                             print('================================================================')
                         except asyncio.CancelledError:
                             pass  # Task cancellation should not be logged as an error.
                         except grpc.RpcError as ex:
                             status_code = ex.code()
                             print(f"Exception on cancel All order: {status_code.name}, {ex.details()}")
-            #
-            if ms.MODE == 'TC':
-                BACKTEST_PATH.mkdir(parents=True, exist_ok=True)
             # Init section
             _exchange_info_symbol = await send_request(cls.stub.FetchExchangeInfoSymbol,
                                                        api_pb2.MarketRequest,
                                                        symbol=_symbol)
             exchange_info_symbol = json_format.MessageToDict(_exchange_info_symbol)
             # print("\n".join(f"{k}\t{v}" for k, v in exchange_info_symbol.items()))
             filters = exchange_info_symbol.get('filters')
             for _filter in filters:
                 print(f"{filters.get(_filter).pop('filterType')}: {filters.get(_filter)}")
             # init Strategy class var
             cls.info_symbol = exchange_info_symbol
             cls.tcm = TradingCapabilityManager(exchange_info_symbol)
             cls.base_asset = exchange_info_symbol.get('baseAsset')
             cls.quote_asset = exchange_info_symbol.get('quoteAsset')
-
             if ms.MODE in ('T', 'TC'):
                 # region Get and processing Order book
                 _order_book = await cls.send_request(cls.stub.FetchOrderBook, api_pb2.MarketRequest, symbol=_symbol)
                 order_book = order_book_prepare(_order_book)
                 if not order_book['bids'] or not order_book['asks']:
                     _price = await cls.send_request(cls.stub.FetchSymbolPriceTicker, api_pb2.MarketRequest,
                                                     symbol=_symbol)
@@ -1693,19 +1792,29 @@
                 # endregion
                 _ticker = await cls.send_request(cls.stub.FetchTickerPriceChangeStatistics,
                                                  api_pb2.MarketRequest,
                                                  symbol=_symbol)
                 cls.ticker = json_format.MessageToDict(_ticker)
                 # print(f"main.ticker: {cls.ticker}")
                 loop.create_task(save_asset())
+            #
+            if ms.MODE == 'TC':
+                BACKTEST_PATH.mkdir(parents=True, exist_ok=True)
+            #
+            if ms.MODE in ('TC', 'S') and ms.SAVED_STATE:
+                cls.session_root = Path(BACKTEST_PATH, f"{cls.exchange}_{cls.symbol}")
+                cls.state_file = Path(cls.session_root, "saved_state.json")
+                #
+                if ms.MODE == 'TC':
+                    cls.session_root.mkdir(parents=True, exist_ok=True)
         #
         else:
             # Init class atr for reuse in next backtest cycle
             cls.reset_class_var()
-
+        #
         if ms.MODE == 'S':
             cls.strategy.account.funds.base = {'asset': cls.base_asset,
                                                'free': f"{ms.AMOUNT_FIRST}",
                                                'locked': '0.0'}
             cls.strategy.account.funds.quote = {'asset': cls.quote_asset,
                                                 'free': f"{ms.AMOUNT_SECOND}",
                                                 'locked': '0.0'}
@@ -1735,23 +1844,35 @@
                     cls.strategy.init(check_funds=False)
                 except Exception as ex:
                     print(f"Strategy init error: {ex}")
                     restored = False
         if ms.MODE in ('T', 'TC'):
             loop.create_task(buffered_orders())
         if not restore_state or (not ms.LOAD_LAST_STATE and answer.lower() != 'y'):
-            cls.strategy.init()
             if ms.MODE in ('T', 'TC'):
+                cls.strategy.init()
                 input('Press Enter for Start or Ctrl-Z for Cancel\n')
                 await wss_init()
+                cls.strategy.start()
             else:
+                if ms.SAVED_STATE and cls.state_file.exists():
+                    cls.strategy.init(check_funds=False)
+                else:
+                    cls.strategy.init()
                 await wss_declare()
                 # Set initial local time from backtest data
                 cls.strategy.time_operational['new'] = cls.backtest['ticker'].index[0] / 1000
-                cls.get_buffered_funds_last_time = cls.strategy.local_time()
+                cls.strategy.get_buffered_funds_last_time = cls.strategy.get_time()
                 cls.start_time_ms = int(cls.strategy.local_time() * 1000)
-            cls.strategy.start()
+                cls.strategy.cycle_time = datetime.utcnow()
+
+                if ms.SAVED_STATE and cls.state_file.exists():
+                    restore_state_before_backtesting(cls)
+                elif not ms.SAVED_STATE:
+                    cls.strategy.start()
+                else:
+                    print("Can't load saved state")
         if restored:
             loop.create_task(heartbeat(cls.session))
     except (KeyboardInterrupt, SystemExit):
         # noinspection PyProtectedMember, PyUnresolvedReferences
         os._exit(1)
```

### Comparing `martin-binance-1.3.0b23/martin_binance/ms_cfg.toml.template` & `martin-binance-1.3.1b0/martin_binance/ms_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b23/martin_binance/service/funds_rate_exporter.py` & `martin-binance-1.3.1b0/martin_binance/service/funds_rate_exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ####################################################################
 # Config for prometheus_client
 # See README.md for detail
 ####################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.2.18-4"
+__version__ = "1.3.0-2"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = 'https://github.com/DogsTailFarmer'
 
 import os
 import time
 import sqlite3
 import psutil
@@ -353,9 +353,14 @@
         print("SQLite error:", error)
     while True:
         try:
             CURRENCY_RATE_LAST_TIME = db_handler(sqlite_connection, currency_rate, CURRENCY_RATE_LAST_TIME)
         except sqlite3.Error as error:
             print("DB operational error:", error)
         VPS_CPU.labels(VPS_NAME).set(psutil.getloadavg()[1])
-        VPS_MEMORY.labels(VPS_NAME).set(psutil.virtual_memory()[2])
+        #
+        memory = psutil.virtual_memory()
+        swap = psutil.swap_memory()
+        total_used_percent = 100 * float(swap.used + memory.used) / (swap.total + memory.total)
+        VPS_MEMORY.labels(VPS_NAME).set(total_used_percent)
+        #
         time.sleep(SLEEP_TIME_S)
```

### Comparing `martin-binance-1.3.0b23/martin_binance/service/grafana.json` & `martin-binance-1.3.1b0/martin_binance/service/grafana.json`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b23/martin_binance/service/relaunch.py` & `martin-binance-1.3.1b0/martin_binance/service/relaunch.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 ####################################################################
 # Restart trade sessions saved in /last_state
 ##################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.2.7b7"
+__version__ = "1.3.0-4"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = 'https://github.com/DogsTailFarmer'
 ##################################################################
 
 import libtmux
 import time
 from martin_binance import Path, WORK_PATH, LAST_STATE_PATH
@@ -22,14 +22,14 @@
 session = server.find_where({"session_name": "Trade"})
 
 if session:
     for window in session.list_windows():
         window_name = window.get('window_name')
         pane = window.attached_pane
         if window_name == 'srv':
-            pane.send_keys('./exch_srv.py', enter=True)
+            pane.send_keys('exch_srv.py', enter=True)
         else:
             last_state = Path(LAST_STATE_PATH, f"{window_name.replace('-', '_').replace('/', '')}.json")
             pair = Path(WORK_PATH, f"cli_{window_name.replace('-', '_').replace('/', '')}.py")
             if pair.exists() and last_state.exists():
                 pane.send_keys(f"{pair} 1", enter=True)
         time.sleep(4)
```

### Comparing `martin-binance-1.3.0b23/pyproject.toml` & `martin-binance-1.3.1b0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -13,32 +13,36 @@
              "Operating System :: Unix",
              "Operating System :: Microsoft :: Windows",
              "Operating System :: MacOS"]
 dynamic = ["version", "description"]
 requires-python = ">=3.8"
 
 dependencies = [
-    "exchanges-wrapper==1.3.0.post1",
+    "exchanges-wrapper==1.3.0.post2",
     "margin-strategy-sdk==0.0.11",
     "aiohttp==3.8.4",
     "grpcio==1.48.1",
     "grpcio-tools==1.48.1",
     "jsonpickle==3.0.1",
     "psutil==5.9.5",
     "requests==2.31.0",
     "simplejson==3.19.1",
     "toml==0.10.2",
     "libtmux==0.22.1",
     "colorama==0.4.6",
     "prometheus-client==0.17.0",
     "optuna==3.2.0",
-    "plotly==5.14.1",
+    "plotly==5.15.0",
     "pandas==2.0.2",
     "dash==2.10.2",
     "future==0.18.3",
+    "inquirer==3.1.3"
 ]
 
 [tool.flit.module]
 name = "martin_binance"
 
 [project.urls]
 Source = "https://github.com/DogsTailFarmer/martin-binance"
+
+[project.scripts]
+init = "martin_binance:__init__"
```

### Comparing `martin-binance-1.3.0b23/uml/architecture.puml` & `martin-binance-1.3.1b0/uml/architecture.puml`

 * *Files identical despite different names*

