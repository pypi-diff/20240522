# Comparing `tmp/pyschwab-0.0.1a1.tar.gz` & `tmp/pyschwab-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyschwab-0.0.1a1.tar", max compression
+gzip compressed data, was "pyschwab-0.0.1a2.tar", max compression
```

## Comparing `pyschwab-0.0.1a1.tar` & `pyschwab-0.0.1a2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1066 2024-05-18 23:05:22.835825 pyschwab-0.0.1a1/LICENSE
--rw-r--r--   0        0        0     3410 2024-05-19 02:34:36.504672 pyschwab-0.0.1a1/README.md
--rw-r--r--   0        0        0     1023 2024-05-19 02:46:25.243790 pyschwab-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-03 17:04:38.470243 pyschwab-0.0.1a1/pyschwab/__init__.py
--rw-r--r--   0        0        0     5685 2024-05-08 01:21:35.060439 pyschwab-0.0.1a1/pyschwab/auth.py
--rw-r--r--   0        0        0     1049 2024-05-07 01:38:22.801915 pyschwab-0.0.1a1/pyschwab/exceptions.py
--rw-r--r--   0        0        0      372 2024-05-08 01:24:44.285515 pyschwab-0.0.1a1/pyschwab/log.py
--rw-r--r--   0        0        0     5741 2024-05-18 17:08:51.216896 pyschwab-0.0.1a1/pyschwab/market.py
--rw-r--r--   0        0        0    13261 2024-05-17 19:50:29.088317 pyschwab-0.0.1a1/pyschwab/market_models.py
--rw-r--r--   0        0        0     7640 2024-05-18 17:21:37.992167 pyschwab-0.0.1a1/pyschwab/trading.py
--rw-r--r--   0        0        0    17333 2024-05-17 20:22:44.846254 pyschwab-0.0.1a1/pyschwab/trading_models.py
--rw-r--r--   0        0        0     6052 2024-05-18 17:17:09.662636 pyschwab-0.0.1a1/pyschwab/types.py
--rw-r--r--   0        0        0     1013 2024-05-06 01:12:52.452168 pyschwab-0.0.1a1/pyschwab/user_input.py
--rw-r--r--   0        0        0     6161 2024-05-18 17:10:21.691244 pyschwab-0.0.1a1/pyschwab/utils.py
--rw-r--r--   0        0        0     4455 1970-01-01 00:00:00.000000 pyschwab-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-22 03:56:59.206055 pyschwab-0.0.1a2/LICENSE
+-rw-r--r--   0        0        0     3878 2024-05-22 03:56:59.206055 pyschwab-0.0.1a2/README.md
+-rw-r--r--   0        0        0     1033 2024-05-22 03:56:59.210055 pyschwab-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-22 03:56:59.210055 pyschwab-0.0.1a2/pyschwab/__init__.py
+-rw-r--r--   0        0        0     5685 2024-05-22 03:56:59.210055 pyschwab-0.0.1a2/pyschwab/auth.py
+-rw-r--r--   0        0        0     1049 2024-05-22 03:56:59.210055 pyschwab-0.0.1a2/pyschwab/exceptions.py
+-rw-r--r--   0        0        0      372 2024-05-22 03:56:59.210055 pyschwab-0.0.1a2/pyschwab/log.py
+-rw-r--r--   0        0        0     5741 2024-05-22 03:56:59.210055 pyschwab-0.0.1a2/pyschwab/market.py
+-rw-r--r--   0        0        0    13261 2024-05-22 03:56:59.210055 pyschwab-0.0.1a2/pyschwab/market_models.py
+-rw-r--r--   0        0        0     7640 2024-05-22 03:56:59.210055 pyschwab-0.0.1a2/pyschwab/trading.py
+-rw-r--r--   0        0        0    17333 2024-05-22 03:56:59.210055 pyschwab-0.0.1a2/pyschwab/trading_models.py
+-rw-r--r--   0        0        0     6052 2024-05-22 03:56:59.210055 pyschwab-0.0.1a2/pyschwab/types.py
+-rw-r--r--   0        0        0     1013 2024-05-22 03:56:59.210055 pyschwab-0.0.1a2/pyschwab/user_input.py
+-rw-r--r--   0        0        0     6161 2024-05-22 03:56:59.210055 pyschwab-0.0.1a2/pyschwab/utils.py
+-rw-r--r--   0        0        0     4930 1970-01-01 00:00:00.000000 pyschwab-0.0.1a2/PKG-INFO
```

### Comparing `pyschwab-0.0.1a1/LICENSE` & `pyschwab-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyschwab-0.0.1a1/README.md` & `pyschwab-0.0.1a2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,93 +1,101 @@
 
 # Schwab API Python Library
 
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
 
-A Python library for interacting with the Schwab API. This library provides a simple and convenient way to access Schwab's trading data and market data.
+A Python library for interacting with the Schwab API, providing simple access to trading and market data.
+
+## Prerequisites
+1. You need to have a Schwab brokerage account.
+2. Become an Individual Developer via the [Schwab Developer Portal](https://beta-developer.schwab.com/).
+3. Create an individual developer app and wait until its status is "Ready for use".
 
 ## Installation
 
-You can install the library using pip:
+Install the library using pip:
 
 ```bash
 pip install pyschwab
 ```
 
 ## Preparation
 
-In the root directory, copy https://github.com/hzheng/pyschwab/blob/main/config/pyschwab.yaml to config directory. copy https://github.com/hzheng/pyschwab/blob/main/env_example to .env and replace variables with your settings.
+1. Change directory to your project directory
+2. Copy [pyschwab.yaml](https://github.com/hzheng/pyschwab/blob/main/config/pyschwab.yaml) to your project's `config` directory.
+3. Copy [env_example](https://github.com/hzheng/pyschwab/blob/main/env_example) to `.env` and replace the placeholders with your settings.
 
 ## Usage
 
-Here's a basic example of how to use the library:
+Here are some sample usages:
 
 ```python
+import yaml
+
 from pyschwab.auth import Authorizer
 from pyschwab.trading import TradingApi
 from pyschwab.market import MarketApi
 
-# Configuration
+# Load configuration
 with open("config/pyschwab.yaml", 'r') as file:
     app_config = yaml.safe_load(file)
 
+# Authorization
+# On the first run, this will open a browser for authorization.
+# Follow the instructions. Subsequent runs will auto-refresh the access token.
+# When refresh token expires, it will open browser for authorization again.
 authorizer = Authorizer(app_config['auth'])
+
 access_token = authorizer.get_access_token()
+print(access_token)
 
-# Create trading api client 
+# Example usage of trading APIs
 trading_api = TradingApi(access_token, app_config['trading'])
 
 account_num = 0 # CHANGE this to your actual account number
 trading_data = trading_api.fetch_trading_data(account_num)
-# list positions
+# List positions
 for position in trading_data.positions:
     print("position:", position)
 
-# list transactions 
+# List transactions 
 for transaction in trading_api.get_transactions(account_num):
     print("transaction:", transaction)
 
-# list orders
-for order in trading_api.get_orders(account_num):
-    print("order:", order)
-
-# place order
+# Place order
 order_dict = {
     "orderType": "LIMIT", "session": "NORMAL", "duration": "DAY", "orderStrategyType": "SINGLE", "price": '100.00',
     "orderLegCollection": [
         {"instruction": "BUY", "quantity": 1, "instrument": {"symbol": "TSLA", "assetType": "EQUITY"}}
     ]
     }
 trading_api.place_order(order_dict, account_num)
 
+# List orders
+for order in trading_api.get_orders(account_num):
+    print("order:", order)
 
-# Create market api client 
+# Example usage of market APIs
 market_api = MarketApi(access_token, app_config['market'])
 
-# get quotes
+# Get quotes
 symbols = ['TSLA', 'NVDA']
 quotes = market_api.get_quotes(symbols)
 for symbol in symbols:
-    print("quote for ", symbol, ":", quotes[symbol] )
+    print("quote for ", symbol, ":", quotes[symbol])
 
+# Get option chains
 option_chain = market_api.get_option_chains('TSLA')
 print(option_chain)
- 
+
+# Get price history 
 history = market_api.get_price_history('TSLA')
 print(history)
 ```
 
-## Features
-
-- Retrieve account information
-- Place trades
-- Check order status
-- Access market data
-- And more...
-
 ---
 
 ## License
 
 MIT License
 
 ```
```

### Comparing `pyschwab-0.0.1a1/pyproject.toml` & `pyschwab-0.0.1a2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "pyschwab"
-version = "0.0.1a1"
+version = "0.0.1a2"
 description = "A Python library for the Schwab trading API"
 authors = ["Hui Zheng <xyz.dll@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/hzheng/pyschwab"
 documentation = "https://pyschwab.readthedocs.io"
-keywords = ["schwab", "trading", "api", "finance"]
+keywords = ["finance", "trading", "schwab", "api", "python"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries",
```

### Comparing `pyschwab-0.0.1a1/pyschwab/auth.py` & `pyschwab-0.0.1a2/pyschwab/auth.py`

 * *Files identical despite different names*

### Comparing `pyschwab-0.0.1a1/pyschwab/exceptions.py` & `pyschwab-0.0.1a2/pyschwab/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyschwab-0.0.1a1/pyschwab/market.py` & `pyschwab-0.0.1a2/pyschwab/market.py`

 * *Files identical despite different names*

### Comparing `pyschwab-0.0.1a1/pyschwab/market_models.py` & `pyschwab-0.0.1a2/pyschwab/market_models.py`

 * *Files identical despite different names*

### Comparing `pyschwab-0.0.1a1/pyschwab/trading.py` & `pyschwab-0.0.1a2/pyschwab/trading.py`

 * *Files identical despite different names*

### Comparing `pyschwab-0.0.1a1/pyschwab/trading_models.py` & `pyschwab-0.0.1a2/pyschwab/trading_models.py`

 * *Files identical despite different names*

### Comparing `pyschwab-0.0.1a1/pyschwab/types.py` & `pyschwab-0.0.1a2/pyschwab/types.py`

 * *Files identical despite different names*

### Comparing `pyschwab-0.0.1a1/pyschwab/user_input.py` & `pyschwab-0.0.1a2/pyschwab/user_input.py`

 * *Files identical despite different names*

### Comparing `pyschwab-0.0.1a1/pyschwab/utils.py` & `pyschwab-0.0.1a2/pyschwab/utils.py`

 * *Files identical despite different names*

### Comparing `pyschwab-0.0.1a1/PKG-INFO` & `pyschwab-0.0.1a2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pyschwab
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: A Python library for the Schwab trading API
 Home-page: https://github.com/hzheng/pyschwab
 License: MIT
-Keywords: schwab,trading,api,finance
+Keywords: finance,trading,schwab,api,python
 Author: Hui Zheng
 Author-email: xyz.dll@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -26,95 +26,103 @@
 Description-Content-Type: text/markdown
 
 
 # Schwab API Python Library
 
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
 
-A Python library for interacting with the Schwab API. This library provides a simple and convenient way to access Schwab's trading data and market data.
+A Python library for interacting with the Schwab API, providing simple access to trading and market data.
+
+## Prerequisites
+1. You need to have a Schwab brokerage account.
+2. Become an Individual Developer via the [Schwab Developer Portal](https://beta-developer.schwab.com/).
+3. Create an individual developer app and wait until its status is "Ready for use".
 
 ## Installation
 
-You can install the library using pip:
+Install the library using pip:
 
 ```bash
 pip install pyschwab
 ```
 
 ## Preparation
 
-In the root directory, copy https://github.com/hzheng/pyschwab/blob/main/config/pyschwab.yaml to config directory. copy https://github.com/hzheng/pyschwab/blob/main/env_example to .env and replace variables with your settings.
+1. Change directory to your project directory
+2. Copy [pyschwab.yaml](https://github.com/hzheng/pyschwab/blob/main/config/pyschwab.yaml) to your project's `config` directory.
+3. Copy [env_example](https://github.com/hzheng/pyschwab/blob/main/env_example) to `.env` and replace the placeholders with your settings.
 
 ## Usage
 
-Here's a basic example of how to use the library:
+Here are some sample usages:
 
 ```python
+import yaml
+
 from pyschwab.auth import Authorizer
 from pyschwab.trading import TradingApi
 from pyschwab.market import MarketApi
 
-# Configuration
+# Load configuration
 with open("config/pyschwab.yaml", 'r') as file:
     app_config = yaml.safe_load(file)
 
+# Authorization
+# On the first run, this will open a browser for authorization.
+# Follow the instructions. Subsequent runs will auto-refresh the access token.
+# When refresh token expires, it will open browser for authorization again.
 authorizer = Authorizer(app_config['auth'])
+
 access_token = authorizer.get_access_token()
+print(access_token)
 
-# Create trading api client 
+# Example usage of trading APIs
 trading_api = TradingApi(access_token, app_config['trading'])
 
 account_num = 0 # CHANGE this to your actual account number
 trading_data = trading_api.fetch_trading_data(account_num)
-# list positions
+# List positions
 for position in trading_data.positions:
     print("position:", position)
 
-# list transactions 
+# List transactions 
 for transaction in trading_api.get_transactions(account_num):
     print("transaction:", transaction)
 
-# list orders
-for order in trading_api.get_orders(account_num):
-    print("order:", order)
-
-# place order
+# Place order
 order_dict = {
     "orderType": "LIMIT", "session": "NORMAL", "duration": "DAY", "orderStrategyType": "SINGLE", "price": '100.00',
     "orderLegCollection": [
         {"instruction": "BUY", "quantity": 1, "instrument": {"symbol": "TSLA", "assetType": "EQUITY"}}
     ]
     }
 trading_api.place_order(order_dict, account_num)
 
+# List orders
+for order in trading_api.get_orders(account_num):
+    print("order:", order)
 
-# Create market api client 
+# Example usage of market APIs
 market_api = MarketApi(access_token, app_config['market'])
 
-# get quotes
+# Get quotes
 symbols = ['TSLA', 'NVDA']
 quotes = market_api.get_quotes(symbols)
 for symbol in symbols:
-    print("quote for ", symbol, ":", quotes[symbol] )
+    print("quote for ", symbol, ":", quotes[symbol])
 
+# Get option chains
 option_chain = market_api.get_option_chains('TSLA')
 print(option_chain)
- 
+
+# Get price history 
 history = market_api.get_price_history('TSLA')
 print(history)
 ```
 
-## Features
-
-- Retrieve account information
-- Place trades
-- Check order status
-- Access market data
-- And more...
-
 ---
 
 ## License
 
 MIT License
 
 ```
```

