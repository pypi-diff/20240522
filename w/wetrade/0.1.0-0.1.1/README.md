# Comparing `tmp/wetrade-0.1.0.tar.gz` & `tmp/wetrade-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wetrade-0.1.0.tar", last modified: Fri May 17 19:14:19 2024, max compression
+gzip compressed data, was "wetrade-0.1.1.tar", last modified: Tue May 21 22:10:37 2024, max compression
```

## Comparing `wetrade-0.1.0.tar` & `wetrade-0.1.1.tar`

### file list

```diff
@@ -1,54 +1,58 @@
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-17 19:14:19.036647 wetrade-0.1.0/
--rw-r--r--   0 mason     (1000) mason     (1000)     1089 2024-05-17 18:51:50.000000 wetrade-0.1.0/LICENSE
--rw-r--r--   0 mason     (1000) mason     (1000)       44 2024-05-17 18:51:50.000000 wetrade-0.1.0/MANIFEST.in
--rw-r--r--   0 mason     (1000) mason     (1000)     4384 2024-05-17 19:14:19.036647 wetrade-0.1.0/PKG-INFO
--rw-r--r--   0 mason     (1000) mason     (1000)     3926 2024-05-17 19:14:11.000000 wetrade-0.1.0/README.rst
--rw-r--r--   0 mason     (1000) mason     (1000)       38 2024-05-17 19:14:19.036647 wetrade-0.1.0/setup.cfg
--rw-r--r--   0 mason     (1000) mason     (1000)      607 2024-05-17 19:10:05.000000 wetrade-0.1.0/setup.py
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-17 19:14:19.036647 wetrade-0.1.0/tests/
--rw-r--r--   0 mason     (1000) mason     (1000)        0 2024-05-17 18:51:50.000000 wetrade-0.1.0/tests/__init__.py
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-17 19:14:19.036647 wetrade-0.1.0/tests/mock_api/
--rw-r--r--   0 mason     (1000) mason     (1000)       68 2024-05-17 18:51:50.000000 wetrade-0.1.0/tests/mock_api/__init__.py
--rw-r--r--   0 mason     (1000) mason     (1000)    17447 2024-05-17 18:51:50.000000 wetrade-0.1.0/tests/mock_api/account_responses.py
--rw-r--r--   0 mason     (1000) mason     (1000)     2272 2024-05-17 18:51:50.000000 wetrade-0.1.0/tests/mock_api/mock_api.py
--rw-r--r--   0 mason     (1000) mason     (1000)     6888 2024-05-17 18:51:50.000000 wetrade-0.1.0/tests/mock_api/order_responses.py
--rw-r--r--   0 mason     (1000) mason     (1000)     1786 2024-05-17 18:51:50.000000 wetrade-0.1.0/tests/mock_api/quote_responses.py
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-17 19:14:19.036647 wetrade-0.1.0/tests/order/
--rw-r--r--   0 mason     (1000) mason     (1000)        0 2024-05-17 18:51:50.000000 wetrade-0.1.0/tests/order/__init__.py
--rw-r--r--   0 mason     (1000) mason     (1000)     2034 2024-05-17 18:51:50.000000 wetrade-0.1.0/tests/order/test_base_order.py
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-17 19:14:19.036647 wetrade-0.1.0/tests/quote/
--rw-r--r--   0 mason     (1000) mason     (1000)        0 2024-05-17 18:51:50.000000 wetrade-0.1.0/tests/quote/__init__.py
--rw-r--r--   0 mason     (1000) mason     (1000)      281 2024-05-17 18:51:50.000000 wetrade-0.1.0/tests/quote/test_data_frame_quote.py
--rw-r--r--   0 mason     (1000) mason     (1000)      951 2024-05-17 18:51:50.000000 wetrade-0.1.0/tests/quote/test_quote.py
--rw-r--r--   0 mason     (1000) mason     (1000)      951 2024-05-17 18:51:50.000000 wetrade-0.1.0/tests/test_account.py
--rw-r--r--   0 mason     (1000) mason     (1000)     8211 2024-05-17 18:55:17.000000 wetrade-0.1.0/tests/test_api.py
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-17 19:14:19.036647 wetrade-0.1.0/wetrade/
--rw-r--r--   0 mason     (1000) mason     (1000)      126 2024-05-17 18:51:50.000000 wetrade-0.1.0/wetrade/__init__.py
--rw-r--r--   0 mason     (1000) mason     (1000)      223 2024-05-17 18:51:50.000000 wetrade-0.1.0/wetrade/__main__.py
--rw-r--r--   0 mason     (1000) mason     (1000)     1929 2024-05-17 18:51:50.000000 wetrade-0.1.0/wetrade/account.py
--rw-r--r--   0 mason     (1000) mason     (1000)     5836 2024-05-17 18:51:50.000000 wetrade-0.1.0/wetrade/api.py
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-17 19:14:19.036647 wetrade-0.1.0/wetrade/order/
--rw-r--r--   0 mason     (1000) mason     (1000)      292 2024-05-17 18:51:50.000000 wetrade-0.1.0/wetrade/order/__init__.py
--rw-r--r--   0 mason     (1000) mason     (1000)    10855 2024-05-17 18:51:50.000000 wetrade-0.1.0/wetrade/order/base_order.py
--rw-r--r--   0 mason     (1000) mason     (1000)      624 2024-05-17 18:51:50.000000 wetrade-0.1.0/wetrade/order/basic_order_types.py
--rw-r--r--   0 mason     (1000) mason     (1000)     2827 2024-05-17 18:51:50.000000 wetrade-0.1.0/wetrade/order/converting_stop_order.py
--rw-r--r--   0 mason     (1000) mason     (1000)     2139 2024-05-17 18:51:50.000000 wetrade-0.1.0/wetrade/order/lookup_msg.py
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-17 19:14:19.036647 wetrade-0.1.0/wetrade/project_template/
--rw-r--r--   0 mason     (1000) mason     (1000)      271 2024-05-17 18:51:50.000000 wetrade-0.1.0/wetrade/project_template/Dockerfile
--rw-r--r--   0 mason     (1000) mason     (1000)        0 2024-05-17 18:51:50.000000 wetrade-0.1.0/wetrade/project_template/__init__.py
--rw-r--r--   0 mason     (1000) mason     (1000)      506 2024-05-17 18:51:50.000000 wetrade-0.1.0/wetrade/project_template/main.py
--rw-r--r--   0 mason     (1000) mason     (1000)      315 2024-05-17 18:51:50.000000 wetrade-0.1.0/wetrade/project_template/new_project.py
--rw-r--r--   0 mason     (1000) mason     (1000)        7 2024-05-17 18:51:50.000000 wetrade-0.1.0/wetrade/project_template/requirements.txt
--rw-r--r--   0 mason     (1000) mason     (1000)      824 2024-05-17 18:51:50.000000 wetrade-0.1.0/wetrade/project_template/settings.py
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-17 19:14:19.036647 wetrade-0.1.0/wetrade/quote/
--rw-r--r--   0 mason     (1000) mason     (1000)      113 2024-05-17 18:51:50.000000 wetrade-0.1.0/wetrade/quote/__init__.py
--rw-r--r--   0 mason     (1000) mason     (1000)     3580 2024-05-17 18:51:50.000000 wetrade-0.1.0/wetrade/quote/data_frame_quote.py
--rw-r--r--   0 mason     (1000) mason     (1000)     2712 2024-05-17 18:51:50.000000 wetrade-0.1.0/wetrade/quote/quote.py
--rw-r--r--   0 mason     (1000) mason     (1000)     8136 2024-05-17 18:51:50.000000 wetrade-0.1.0/wetrade/user_session.py
--rw-r--r--   0 mason     (1000) mason     (1000)     3496 2024-05-17 18:51:50.000000 wetrade-0.1.0/wetrade/utils.py
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-17 19:14:19.036647 wetrade-0.1.0/wetrade.egg-info/
--rw-r--r--   0 mason     (1000) mason     (1000)     4384 2024-05-17 19:14:19.000000 wetrade-0.1.0/wetrade.egg-info/PKG-INFO
--rw-r--r--   0 mason     (1000) mason     (1000)     1130 2024-05-17 19:14:19.000000 wetrade-0.1.0/wetrade.egg-info/SOURCES.txt
--rw-r--r--   0 mason     (1000) mason     (1000)        1 2024-05-17 19:14:19.000000 wetrade-0.1.0/wetrade.egg-info/dependency_links.txt
--rw-r--r--   0 mason     (1000) mason     (1000)      123 2024-05-17 19:14:19.000000 wetrade-0.1.0/wetrade.egg-info/requires.txt
--rw-r--r--   0 mason     (1000) mason     (1000)       14 2024-05-17 19:14:19.000000 wetrade-0.1.0/wetrade.egg-info/top_level.txt
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-21 22:10:37.785747 wetrade-0.1.1/
+-rw-r--r--   0 mason     (1000) mason     (1000)     1089 2024-05-17 18:51:50.000000 wetrade-0.1.1/LICENSE
+-rw-r--r--   0 mason     (1000) mason     (1000)       44 2024-05-17 18:51:50.000000 wetrade-0.1.1/MANIFEST.in
+-rw-r--r--   0 mason     (1000) mason     (1000)     5414 2024-05-21 22:10:37.785747 wetrade-0.1.1/PKG-INFO
+-rw-r--r--   0 mason     (1000) mason     (1000)     4956 2024-05-21 22:07:33.000000 wetrade-0.1.1/README.rst
+-rw-r--r--   0 mason     (1000) mason     (1000)       38 2024-05-21 22:10:37.785747 wetrade-0.1.1/setup.cfg
+-rw-r--r--   0 mason     (1000) mason     (1000)      607 2024-05-21 22:10:33.000000 wetrade-0.1.1/setup.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-21 22:10:37.785747 wetrade-0.1.1/tests/
+-rw-r--r--   0 mason     (1000) mason     (1000)        0 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/__init__.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-21 22:10:37.785747 wetrade-0.1.1/tests/mock_api/
+-rw-r--r--   0 mason     (1000) mason     (1000)       68 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/mock_api/__init__.py
+-rw-r--r--   0 mason     (1000) mason     (1000)    17447 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/mock_api/account_responses.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     2272 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/mock_api/mock_api.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     6888 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/mock_api/order_responses.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     1786 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/mock_api/quote_responses.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-21 22:10:37.785747 wetrade-0.1.1/tests/order/
+-rw-r--r--   0 mason     (1000) mason     (1000)        0 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/order/__init__.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     2034 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/order/test_base_order.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-21 22:10:37.785747 wetrade-0.1.1/tests/quote/
+-rw-r--r--   0 mason     (1000) mason     (1000)        0 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/quote/__init__.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      281 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/quote/test_data_frame_quote.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      951 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/quote/test_quote.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      951 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/test_account.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     8049 2024-05-21 22:07:33.000000 wetrade-0.1.1/tests/test_api.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-21 22:10:37.785747 wetrade-0.1.1/wetrade/
+-rw-r--r--   0 mason     (1000) mason     (1000)      126 2024-05-17 18:51:50.000000 wetrade-0.1.1/wetrade/__init__.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      223 2024-05-17 18:51:50.000000 wetrade-0.1.1/wetrade/__main__.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     2303 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/account.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     8927 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/api.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-21 22:10:37.785747 wetrade-0.1.1/wetrade/order/
+-rw-r--r--   0 mason     (1000) mason     (1000)      292 2024-05-17 18:51:50.000000 wetrade-0.1.1/wetrade/order/__init__.py
+-rw-r--r--   0 mason     (1000) mason     (1000)    12601 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/order/base_order.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     1091 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/order/basic_order_types.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     3021 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/order/converting_stop_order.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     2139 2024-05-17 18:51:50.000000 wetrade-0.1.1/wetrade/order/lookup_msg.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-21 22:10:37.785747 wetrade-0.1.1/wetrade/project_template/
+-rw-r--r--   0 mason     (1000) mason     (1000)      271 2024-05-17 18:51:50.000000 wetrade-0.1.1/wetrade/project_template/Dockerfile
+-rw-r--r--   0 mason     (1000) mason     (1000)        0 2024-05-17 18:51:50.000000 wetrade-0.1.1/wetrade/project_template/__init__.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-21 22:10:37.785747 wetrade-0.1.1/wetrade/project_template/__pycache__/
+-rw-r--r--   0 mason     (1000) mason     (1000)      187 2024-05-21 22:10:27.000000 wetrade-0.1.1/wetrade/project_template/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 mason     (1000) mason     (1000)      741 2024-05-21 22:10:27.000000 wetrade-0.1.1/wetrade/project_template/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0 mason     (1000) mason     (1000)     1209 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/project_template/main.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      362 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/project_template/new_project.py
+-rw-r--r--   0 mason     (1000) mason     (1000)        7 2024-05-17 18:51:50.000000 wetrade-0.1.1/wetrade/project_template/requirements.txt
+-rw-r--r--   0 mason     (1000) mason     (1000)      827 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/project_template/settings.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-21 22:10:37.785747 wetrade-0.1.1/wetrade/quote/
+-rw-r--r--   0 mason     (1000) mason     (1000)      165 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/quote/__init__.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     4151 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/quote/data_frame_quote.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     5138 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/quote/multi_quote.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     4682 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/quote/quote.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     8299 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/user_session.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     3689 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/utils.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-21 22:10:37.785747 wetrade-0.1.1/wetrade.egg-info/
+-rw-r--r--   0 mason     (1000) mason     (1000)     5414 2024-05-21 22:10:37.000000 wetrade-0.1.1/wetrade.egg-info/PKG-INFO
+-rw-r--r--   0 mason     (1000) mason     (1000)     1283 2024-05-21 22:10:37.000000 wetrade-0.1.1/wetrade.egg-info/SOURCES.txt
+-rw-r--r--   0 mason     (1000) mason     (1000)        1 2024-05-21 22:10:37.000000 wetrade-0.1.1/wetrade.egg-info/dependency_links.txt
+-rw-r--r--   0 mason     (1000) mason     (1000)      123 2024-05-21 22:10:37.000000 wetrade-0.1.1/wetrade.egg-info/requires.txt
+-rw-r--r--   0 mason     (1000) mason     (1000)       14 2024-05-21 22:10:37.000000 wetrade-0.1.1/wetrade.egg-info/top_level.txt
```

### Comparing `wetrade-0.1.0/LICENSE` & `wetrade-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wetrade-0.1.0/PKG-INFO` & `wetrade-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wetrade
-Version: 0.1.0
+Version: 0.1.1
 Summary: An E-Trade python library built for active stock trading
 Author: Mason Krause
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: authlib
 Requires-Dist: playwright
 Requires-Dist: urllib3==1.26.16
@@ -19,16 +19,16 @@
 ``wetrade``: An E-Trade Python library built for automated stock trading 
 =========================================================================
 
 ``wetrade`` overview
 --------------------
 
 ``wetrade`` is an unofficial `E-Trade API <https://developer.etrade.com/home/>`__ 
-library originally built as part of a headless trading system. It provides a lot 
-of useful built-in functionality, and was designed to be flexible and extensible
+library initially created for use in headless trading systems. It provides a lot 
+of helpful built-in functionality, and was designed to be flexible and extensible
 and to accommodate a wide variety of stock trading needs.
 
 Features include:
 
 * Automated login and authentication supporting 2FA
 * Easy setup and configuration
 * Quotes, account info, and custom ordering
@@ -53,30 +53,32 @@
 `the subscription center <https://us.etrade.com/etx/pxy/my-profile/subscription-center/>`__
 so that you don't receive delayed quotes. 
 
 Install ``wetrade``:
 
 It's a good idea to create a new virtual environment for a new Python project
 
-.. code-block:: console
+.. code-block:: shell
 
   # create venv
   python3 -m venv venv
   # enter venv
   source venv/bin/activate
 
-We can then install ``wetrade`` into our venv
+We can then install ``wetrade`` into our venv. For automatic login, we'll also
+need to install our browser.
 
-.. code-block:: console
+.. code-block:: shell
 
   pip install wetrade
+  playwright install firefox
 
 Next, you'll get going in no time using our automated new project script!
 
-.. code-block:: console
+.. code-block:: shell
 
   python -m wetrade new-project
 
 You'll now see a handful of files in your project directory including a *settings.py*
 file where you'll enter your user and API info and have the option to configure various
 ``wetrade`` settings. In this file, you'll enter your username, password, client_key, 
 and client_secret so ``wetrade`` can log into your account.
@@ -93,37 +95,66 @@
   from wetrade.account import Account
   from wetrade.quote import Quote
   from wetrade.order import LimitOrder
   from wetrade.utils import setup_logging
 
 
   def main():
+    # Setup logging (optional) and APIClient
     setup_logging()
     client = APIClient()
 
+    # Check out your account
     account = Account(client=client)
     print('My Account Key: ', account.account_key)
     print('My Balance: ', account.check_balance())
 
-    quote = Quote(client=client, symbol='AAPL')
-    print('Last Quote Price: ', quote.get_last_price())
-
-
-  if __name__ == '__main__':
-    main()
+    # Get a stock quote
+    quote = Quote(client=client, symbol='IBM')
+    print(f'Last {quote.symbol} Quote Price: ', quote.get_last_price())
+
+    # Place some orders and stuff
+    order1 = LimitOrder(
+        client = client,
+        account_key = account.account_key,
+        symbol = 'NVDA',
+        action = 'BUY',
+        quantity = 1,
+        price = 50.00)
+    order1.place_order()
+    order1.run_when_status(
+        'CANCELLED', 
+        func = print, 
+        func_args = ['Test message'])
+    
+    order2 = LimitOrder(
+        client = client,
+        account_key = account.account_key,
+        symbol = 'NFLX',
+        action = 'BUY',
+        quantity = 1,
+        price = 50.00)
+    order2.place_order()
+    order2.run_when_status(
+        'CANCELLED',
+        order1.cancel_order)
+    
+    order2.cancel_order()
 
 
 Other info
 -------------
 
-``wetrade`` was initially designed to run headlessly and has built-in handling 
-for most expected brokerage, server, and API errors. Our goal is to consistently
-add new functionality to support additional use cases. If you have any comments or 
-suggestions for new features, don't hesitate to create an issue or reach out to 
-`wetrade.inbox@gmail.com <mailto:wetrade.inbox@gmail.com>`__.
+``wetrade`` was initially designed to run headlessly and has built-in handling for 
+most expected brokerage, server, and API errors. This and the majority of other 
+``wetrade`` functionality is entirely optional to use, and our modular structure 
+allows you to utilize as much or as little of the library as you'd like. Our goal 
+is to consistently add new functionality to support additional use cases. If you 
+have any comments or suggestions for new features, don't hesitate to create an 
+issue or reach out to: `wetrade.inbox@gmail.com <mailto:wetrade.inbox@gmail.com>`__.
 
 
 **Disclaimer:** *wetrade is an unofficial API library and comes with no warranty
 of any kind. It is in no way endorsed by or affiliated with E*TRADE Financial 
 or any associated organization. Make sure to read and understand the terms of 
 service of the underlying API before using this package. This authors accept 
 no responsibility for any damage that might stem from use of this package.
```

### Comparing `wetrade-0.1.0/README.rst` & `wetrade-0.1.1/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -11,236 +11,300 @@
 000000a0: 206f 7665 7276 6965 770a 2d2d 2d2d 2d2d   overview.------
 000000b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
 000000c0: 6060 7765 7472 6164 6560 6020 6973 2061  ``wetrade`` is a
 000000d0: 6e20 756e 6f66 6669 6369 616c 2060 452d  n unofficial `E-
 000000e0: 5472 6164 6520 4150 4920 3c68 7474 7073  Trade API <https
 000000f0: 3a2f 2f64 6576 656c 6f70 6572 2e65 7472  ://developer.etr
 00000100: 6164 652e 636f 6d2f 686f 6d65 2f3e 605f  ade.com/home/>`_
-00000110: 5f20 0a6c 6962 7261 7279 206f 7269 6769  _ .library origi
-00000120: 6e61 6c6c 7920 6275 696c 7420 6173 2070  nally built as p
-00000130: 6172 7420 6f66 2061 2068 6561 646c 6573  art of a headles
-00000140: 7320 7472 6164 696e 6720 7379 7374 656d  s trading system
+00000110: 5f20 0a6c 6962 7261 7279 2069 6e69 7469  _ .library initi
+00000120: 616c 6c79 2063 7265 6174 6564 2066 6f72  ally created for
+00000130: 2075 7365 2069 6e20 6865 6164 6c65 7373   use in headless
+00000140: 2074 7261 6469 6e67 2073 7973 7465 6d73   trading systems
 00000150: 2e20 4974 2070 726f 7669 6465 7320 6120  . It provides a 
-00000160: 6c6f 7420 0a6f 6620 7573 6566 756c 2062  lot .of useful b
-00000170: 7569 6c74 2d69 6e20 6675 6e63 7469 6f6e  uilt-in function
-00000180: 616c 6974 792c 2061 6e64 2077 6173 2064  ality, and was d
-00000190: 6573 6967 6e65 6420 746f 2062 6520 666c  esigned to be fl
-000001a0: 6578 6962 6c65 2061 6e64 2065 7874 656e  exible and exten
-000001b0: 7369 626c 650a 616e 6420 746f 2061 6363  sible.and to acc
-000001c0: 6f6d 6d6f 6461 7465 2061 2077 6964 6520  ommodate a wide 
-000001d0: 7661 7269 6574 7920 6f66 2073 746f 636b  variety of stock
-000001e0: 2074 7261 6469 6e67 206e 6565 6473 2e0a   trading needs..
-000001f0: 0a46 6561 7475 7265 7320 696e 636c 7564  .Features includ
-00000200: 653a 0a0a 2a20 4175 746f 6d61 7465 6420  e:..* Automated 
-00000210: 6c6f 6769 6e20 616e 6420 6175 7468 656e  login and authen
-00000220: 7469 6361 7469 6f6e 2073 7570 706f 7274  tication support
-00000230: 696e 6720 3246 410a 2a20 4561 7379 2073  ing 2FA.* Easy s
-00000240: 6574 7570 2061 6e64 2063 6f6e 6669 6775  etup and configu
-00000250: 7261 7469 6f6e 0a2a 2051 756f 7465 732c  ration.* Quotes,
-00000260: 2061 6363 6f75 6e74 2069 6e66 6f2c 2061   account info, a
-00000270: 6e64 2063 7573 746f 6d20 6f72 6465 7269  nd custom orderi
-00000280: 6e67 0a2a 2043 616c 6c62 6163 6b20 6675  ng.* Callback fu
-00000290: 6e63 7469 6f6e 616c 6974 7920 666f 7220  nctionality for 
-000002a0: 6f72 6465 7220 616e 6420 7175 6f74 6520  order and quote 
-000002b0: 7570 6461 7465 7320 0a2a 2041 7574 6f6d  updates .* Autom
-000002c0: 6174 6564 2073 6574 7570 2066 6f72 206e  ated setup for n
-000002d0: 6577 2070 726f 6a65 6374 7320 200a 2a20  ew projects  .* 
-000002e0: 4561 7379 2064 6570 6c6f 796d 656e 7420  Easy deployment 
-000002f0: 7769 7468 2044 6f63 6b65 7220 7465 6d70  with Docker temp
-00000300: 6c61 7465 0a2a 2052 6f62 7573 7420 6c6f  late.* Robust lo
-00000310: 6767 696e 6720 7769 7468 206f 7074 696f  gging with optio
-00000320: 6e61 6c20 476f 6f67 6c65 2043 6c6f 7564  nal Google Cloud
-00000330: 2069 6e74 6567 7261 7469 6f6e 0a0a 6060   integration..``
-00000340: 7765 7472 6164 6560 6020 646f 6375 6d65  wetrade`` docume
-00000350: 6e74 6174 696f 6e0a 2d2d 2d2d 2d2d 2d2d  ntation.--------
+00000160: 6c6f 7420 0a6f 6620 6865 6c70 6675 6c20  lot .of helpful 
+00000170: 6275 696c 742d 696e 2066 756e 6374 696f  built-in functio
+00000180: 6e61 6c69 7479 2c20 616e 6420 7761 7320  nality, and was 
+00000190: 6465 7369 676e 6564 2074 6f20 6265 2066  designed to be f
+000001a0: 6c65 7869 626c 6520 616e 6420 6578 7465  lexible and exte
+000001b0: 6e73 6962 6c65 0a61 6e64 2074 6f20 6163  nsible.and to ac
+000001c0: 636f 6d6d 6f64 6174 6520 6120 7769 6465  commodate a wide
+000001d0: 2076 6172 6965 7479 206f 6620 7374 6f63   variety of stoc
+000001e0: 6b20 7472 6164 696e 6720 6e65 6564 732e  k trading needs.
+000001f0: 0a0a 4665 6174 7572 6573 2069 6e63 6c75  ..Features inclu
+00000200: 6465 3a0a 0a2a 2041 7574 6f6d 6174 6564  de:..* Automated
+00000210: 206c 6f67 696e 2061 6e64 2061 7574 6865   login and authe
+00000220: 6e74 6963 6174 696f 6e20 7375 7070 6f72  ntication suppor
+00000230: 7469 6e67 2032 4641 0a2a 2045 6173 7920  ting 2FA.* Easy 
+00000240: 7365 7475 7020 616e 6420 636f 6e66 6967  setup and config
+00000250: 7572 6174 696f 6e0a 2a20 5175 6f74 6573  uration.* Quotes
+00000260: 2c20 6163 636f 756e 7420 696e 666f 2c20  , account info, 
+00000270: 616e 6420 6375 7374 6f6d 206f 7264 6572  and custom order
+00000280: 696e 670a 2a20 4361 6c6c 6261 636b 2066  ing.* Callback f
+00000290: 756e 6374 696f 6e61 6c69 7479 2066 6f72  unctionality for
+000002a0: 206f 7264 6572 2061 6e64 2071 756f 7465   order and quote
+000002b0: 2075 7064 6174 6573 200a 2a20 4175 746f   updates .* Auto
+000002c0: 6d61 7465 6420 7365 7475 7020 666f 7220  mated setup for 
+000002d0: 6e65 7720 7072 6f6a 6563 7473 2020 0a2a  new projects  .*
+000002e0: 2045 6173 7920 6465 706c 6f79 6d65 6e74   Easy deployment
+000002f0: 2077 6974 6820 446f 636b 6572 2074 656d   with Docker tem
+00000300: 706c 6174 650a 2a20 526f 6275 7374 206c  plate.* Robust l
+00000310: 6f67 6769 6e67 2077 6974 6820 6f70 7469  ogging with opti
+00000320: 6f6e 616c 2047 6f6f 676c 6520 436c 6f75  onal Google Clou
+00000330: 6420 696e 7465 6772 6174 696f 6e0a 0a60  d integration..`
+00000340: 6077 6574 7261 6465 6060 2064 6f63 756d  `wetrade`` docum
+00000350: 656e 7461 7469 6f6e 0a2d 2d2d 2d2d 2d2d  entation.-------
 00000360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000370: 2d0a 0a46 6f72 206f 7572 2066 756c 6c20  -..For our full 
-00000380: 646f 6375 6d65 6e74 6174 696f 6e2c 2063  documentation, c
-00000390: 6865 636b 206f 7574 3a20 0a60 6874 7470  heck out: .`http
-000003a0: 733a 2f2f 7765 7472 6164 652e 7265 6164  s://wetrade.read
-000003b0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-000003c0: 7465 7374 2f20 3c68 7474 7073 3a2f 2f77  test/ <https://w
-000003d0: 6574 7261 6465 2e72 6561 6474 6865 646f  etrade.readthedo
-000003e0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-000003f0: 3e60 5f5f 2e0a 0a47 6574 7469 6e67 2073  >`__...Getting s
-00000400: 7461 7274 6564 2077 6974 6820 6060 7765  tarted with ``we
-00000410: 7472 6164 6560 600a 2d2d 2d2d 2d2d 2d2d  trade``.--------
+00000370: 2d2d 0a0a 466f 7220 6f75 7220 6675 6c6c  --..For our full
+00000380: 2064 6f63 756d 656e 7461 7469 6f6e 2c20   documentation, 
+00000390: 6368 6563 6b20 6f75 743a 200a 6068 7474  check out: .`htt
+000003a0: 7073 3a2f 2f77 6574 7261 6465 2e72 6561  ps://wetrade.rea
+000003b0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+000003c0: 6174 6573 742f 203c 6874 7470 733a 2f2f  atest/ <https://
+000003d0: 7765 7472 6164 652e 7265 6164 7468 6564  wetrade.readthed
+000003e0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+000003f0: 2f3e 605f 5f2e 0a0a 4765 7474 696e 6720  />`__...Getting 
+00000400: 7374 6172 7465 6420 7769 7468 2060 6077  started with ``w
+00000410: 6574 7261 6465 6060 0a2d 2d2d 2d2d 2d2d  etrade``.-------
 00000420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000430: 2d2d 2d2d 2d2d 2d2d 2d0a 0a49 6e20 6f72  ---------..In or
-00000440: 6465 7220 746f 2061 6363 6573 7320 7468  der to access th
-00000450: 6520 452d 5472 6164 6520 4150 492c 2079  e E-Trade API, y
-00000460: 6f75 276c 6c20 6e65 6564 2074 6f20 666f  ou'll need to fo
-00000470: 6c6c 6f77 2074 6865 2034 2073 7465 7073  llow the 4 steps
-00000480: 2064 6574 6169 6c65 6420 6f6e 2074 6865   detailed on the
-00000490: 0a60 452d 5472 6164 6520 6465 7665 6c6f  .`E-Trade develo
-000004a0: 7065 7220 6765 7474 696e 6720 7374 6172  per getting star
-000004b0: 7465 6420 7061 6765 203c 6874 7470 733a  ted page <https:
-000004c0: 2f2f 6465 7665 6c6f 7065 722e 6574 7261  //developer.etra
-000004d0: 6465 2e63 6f6d 2f67 6574 7469 6e67 2d73  de.com/getting-s
-000004e0: 7461 7274 6564 2f3e 605f 5f0a 7468 656e  tarted/>`__.then
-000004f0: 2072 6571 7565 7374 2061 6e20 4150 4920   request an API 
-00000500: 6b65 7920 7468 726f 7567 6820 6074 6865  key through `the
-00000510: 206c 696e 6b65 6420 7061 6765 203c 6874   linked page <ht
-00000520: 7470 733a 2f2f 7573 2e65 7472 6164 652e  tps://us.etrade.
-00000530: 636f 6d2f 6574 782f 7269 732f 6170 696b  com/etx/ris/apik
-00000540: 6579 2f3e 605f 5f2e 0a49 7427 7320 616c  ey/>`__..It's al
-00000550: 736f 2072 6563 6f6d 6d65 6e64 6564 2074  so recommended t
-00000560: 6861 7420 796f 7520 656e 6162 6c65 2072  hat you enable r
-00000570: 6561 6c2d 7469 6d65 2064 6174 6120 696e  eal-time data in
-00000580: 2074 6865 200a 6074 6865 2073 7562 7363   the .`the subsc
-00000590: 7269 7074 696f 6e20 6365 6e74 6572 203c  ription center <
-000005a0: 6874 7470 733a 2f2f 7573 2e65 7472 6164  https://us.etrad
-000005b0: 652e 636f 6d2f 6574 782f 7078 792f 6d79  e.com/etx/pxy/my
-000005c0: 2d70 726f 6669 6c65 2f73 7562 7363 7269  -profile/subscri
-000005d0: 7074 696f 6e2d 6365 6e74 6572 2f3e 605f  ption-center/>`_
-000005e0: 5f0a 736f 2074 6861 7420 796f 7520 646f  _.so that you do
-000005f0: 6e27 7420 7265 6365 6976 6520 6465 6c61  n't receive dela
-00000600: 7965 6420 7175 6f74 6573 2e20 0a0a 496e  yed quotes. ..In
-00000610: 7374 616c 6c20 6060 7765 7472 6164 6560  stall ``wetrade`
-00000620: 603a 0a0a 4974 2773 2061 2067 6f6f 6420  `:..It's a good 
-00000630: 6964 6561 2074 6f20 6372 6561 7465 2061  idea to create a
-00000640: 206e 6577 2076 6972 7475 616c 2065 6e76   new virtual env
-00000650: 6972 6f6e 6d65 6e74 2066 6f72 2061 206e  ironment for a n
-00000660: 6577 2050 7974 686f 6e20 7072 6f6a 6563  ew Python projec
-00000670: 740a 0a2e 2e20 636f 6465 2d62 6c6f 636b  t.... code-block
-00000680: 3a3a 2063 6f6e 736f 6c65 0a0a 2020 2320  :: console..  # 
-00000690: 6372 6561 7465 2076 656e 760a 2020 7079  create venv.  py
-000006a0: 7468 6f6e 3320 2d6d 2076 656e 7620 7665  thon3 -m venv ve
-000006b0: 6e76 0a20 2023 2065 6e74 6572 2076 656e  nv.  # enter ven
-000006c0: 760a 2020 736f 7572 6365 2076 656e 762f  v.  source venv/
-000006d0: 6269 6e2f 6163 7469 7661 7465 0a0a 5765  bin/activate..We
-000006e0: 2063 616e 2074 6865 6e20 696e 7374 616c   can then instal
-000006f0: 6c20 6060 7765 7472 6164 6560 6020 696e  l ``wetrade`` in
-00000700: 746f 206f 7572 2076 656e 760a 0a2e 2e20  to our venv.... 
-00000710: 636f 6465 2d62 6c6f 636b 3a3a 2063 6f6e  code-block:: con
-00000720: 736f 6c65 0a0a 2020 7069 7020 696e 7374  sole..  pip inst
-00000730: 616c 6c20 7765 7472 6164 650a 0a4e 6578  all wetrade..Nex
-00000740: 742c 2079 6f75 276c 6c20 6765 7420 676f  t, you'll get go
-00000750: 696e 6720 696e 206e 6f20 7469 6d65 2075  ing in no time u
-00000760: 7369 6e67 206f 7572 2061 7574 6f6d 6174  sing our automat
-00000770: 6564 206e 6577 2070 726f 6a65 6374 2073  ed new project s
-00000780: 6372 6970 7421 0a0a 2e2e 2063 6f64 652d  cript!.... code-
-00000790: 626c 6f63 6b3a 3a20 636f 6e73 6f6c 650a  block:: console.
-000007a0: 0a20 2070 7974 686f 6e20 2d6d 2077 6574  .  python -m wet
-000007b0: 7261 6465 206e 6577 2d70 726f 6a65 6374  rade new-project
-000007c0: 0a0a 596f 7527 6c6c 206e 6f77 2073 6565  ..You'll now see
-000007d0: 2061 2068 616e 6466 756c 206f 6620 6669   a handful of fi
-000007e0: 6c65 7320 696e 2079 6f75 7220 7072 6f6a  les in your proj
-000007f0: 6563 7420 6469 7265 6374 6f72 7920 696e  ect directory in
-00000800: 636c 7564 696e 6720 6120 2a73 6574 7469  cluding a *setti
-00000810: 6e67 732e 7079 2a0a 6669 6c65 2077 6865  ngs.py*.file whe
-00000820: 7265 2079 6f75 276c 6c20 656e 7465 7220  re you'll enter 
-00000830: 796f 7572 2075 7365 7220 616e 6420 4150  your user and AP
-00000840: 4920 696e 666f 2061 6e64 2068 6176 6520  I info and have 
-00000850: 7468 6520 6f70 7469 6f6e 2074 6f20 636f  the option to co
-00000860: 6e66 6967 7572 6520 7661 7269 6f75 730a  nfigure various.
-00000870: 6060 7765 7472 6164 6560 6020 7365 7474  ``wetrade`` sett
-00000880: 696e 6773 2e20 496e 2074 6869 7320 6669  ings. In this fi
-00000890: 6c65 2c20 796f 7527 6c6c 2065 6e74 6572  le, you'll enter
-000008a0: 2079 6f75 7220 7573 6572 6e61 6d65 2c20   your username, 
-000008b0: 7061 7373 776f 7264 2c20 636c 6965 6e74  password, client
-000008c0: 5f6b 6579 2c20 0a61 6e64 2063 6c69 656e  _key, .and clien
-000008d0: 745f 7365 6372 6574 2073 6f20 6060 7765  t_secret so ``we
-000008e0: 7472 6164 6560 6020 6361 6e20 6c6f 6720  trade`` can log 
-000008f0: 696e 746f 2079 6f75 7220 6163 636f 756e  into your accoun
-00000900: 742e 0a0a 496e 2061 6464 6974 696f 6e20  t...In addition 
-00000910: 746f 202a 7365 7474 696e 6773 2e70 792a  to *settings.py*
-00000920: 2c20 7765 2776 6520 616c 736f 2063 7265  , we've also cre
-00000930: 6174 6564 2061 202a 446f 636b 6572 6669  ated a *Dockerfi
-00000940: 6c65 2a20 666f 7220 6561 7379 2064 6570  le* for easy dep
-00000950: 6c6f 796d 656e 7420 6173 200a 7765 6c6c  loyment as .well
-00000960: 2061 7320 6120 2a72 6571 7569 7265 6d65   as a *requireme
-00000970: 6e74 732e 7478 742a 2061 6e64 2061 6e20  nts.txt* and an 
-00000980: 6578 616d 706c 6520 6669 6c65 202a 6d61  example file *ma
-00000990: 696e 2e70 792a 2077 6869 6368 2064 656d  in.py* which dem
-000009a0: 6f6e 7374 7261 7465 7320 736f 6d65 2062  onstrates some b
-000009b0: 6173 6963 200a 7765 7472 6164 6520 7573  asic .wetrade us
-000009c0: 6167 653a 0a0a 2a2a 6d61 696e 2e70 792a  age:..**main.py*
-000009d0: 2a0a 0a2e 2e20 636f 6465 2d62 6c6f 636b  *.... code-block
-000009e0: 3a3a 2070 7974 686f 6e0a 0a20 2066 726f  :: python..  fro
-000009f0: 6d20 7765 7472 6164 652e 6170 6920 696d  m wetrade.api im
-00000a00: 706f 7274 2041 5049 436c 6965 6e74 0a20  port APIClient. 
-00000a10: 2066 726f 6d20 7765 7472 6164 652e 6163   from wetrade.ac
-00000a20: 636f 756e 7420 696d 706f 7274 2041 6363  count import Acc
-00000a30: 6f75 6e74 0a20 2066 726f 6d20 7765 7472  ount.  from wetr
-00000a40: 6164 652e 7175 6f74 6520 696d 706f 7274  ade.quote import
-00000a50: 2051 756f 7465 0a20 2066 726f 6d20 7765   Quote.  from we
-00000a60: 7472 6164 652e 6f72 6465 7220 696d 706f  trade.order impo
-00000a70: 7274 204c 696d 6974 4f72 6465 720a 2020  rt LimitOrder.  
-00000a80: 6672 6f6d 2077 6574 7261 6465 2e75 7469  from wetrade.uti
-00000a90: 6c73 2069 6d70 6f72 7420 7365 7475 705f  ls import setup_
-00000aa0: 6c6f 6767 696e 670a 0a0a 2020 6465 6620  logging...  def 
-00000ab0: 6d61 696e 2829 3a0a 2020 2020 7365 7475  main():.    setu
-00000ac0: 705f 6c6f 6767 696e 6728 290a 2020 2020  p_logging().    
-00000ad0: 636c 6965 6e74 203d 2041 5049 436c 6965  client = APIClie
-00000ae0: 6e74 2829 0a0a 2020 2020 6163 636f 756e  nt()..    accoun
-00000af0: 7420 3d20 4163 636f 756e 7428 636c 6965  t = Account(clie
-00000b00: 6e74 3d63 6c69 656e 7429 0a20 2020 2070  nt=client).    p
-00000b10: 7269 6e74 2827 4d79 2041 6363 6f75 6e74  rint('My Account
-00000b20: 204b 6579 3a20 272c 2061 6363 6f75 6e74   Key: ', account
-00000b30: 2e61 6363 6f75 6e74 5f6b 6579 290a 2020  .account_key).  
-00000b40: 2020 7072 696e 7428 274d 7920 4261 6c61    print('My Bala
-00000b50: 6e63 653a 2027 2c20 6163 636f 756e 742e  nce: ', account.
-00000b60: 6368 6563 6b5f 6261 6c61 6e63 6528 2929  check_balance())
-00000b70: 0a0a 2020 2020 7175 6f74 6520 3d20 5175  ..    quote = Qu
-00000b80: 6f74 6528 636c 6965 6e74 3d63 6c69 656e  ote(client=clien
-00000b90: 742c 2073 796d 626f 6c3d 2741 4150 4c27  t, symbol='AAPL'
-00000ba0: 290a 2020 2020 7072 696e 7428 274c 6173  ).    print('Las
-00000bb0: 7420 5175 6f74 6520 5072 6963 653a 2027  t Quote Price: '
-00000bc0: 2c20 7175 6f74 652e 6765 745f 6c61 7374  , quote.get_last
-00000bd0: 5f70 7269 6365 2829 290a 0a0a 2020 6966  _price())...  if
-00000be0: 205f 5f6e 616d 655f 5f20 3d3d 2027 5f5f   __name__ == '__
-00000bf0: 6d61 696e 5f5f 273a 0a20 2020 206d 6169  main__':.    mai
-00000c00: 6e28 290a 0a0a 4f74 6865 7220 696e 666f  n()...Other info
-00000c10: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  .-------------..
-00000c20: 6060 7765 7472 6164 6560 6020 7761 7320  ``wetrade`` was 
-00000c30: 696e 6974 6961 6c6c 7920 6465 7369 676e  initially design
-00000c40: 6564 2074 6f20 7275 6e20 6865 6164 6c65  ed to run headle
-00000c50: 7373 6c79 2061 6e64 2068 6173 2062 7569  ssly and has bui
-00000c60: 6c74 2d69 6e20 6861 6e64 6c69 6e67 200a  lt-in handling .
-00000c70: 666f 7220 6d6f 7374 2065 7870 6563 7465  for most expecte
-00000c80: 6420 6272 6f6b 6572 6167 652c 2073 6572  d brokerage, ser
-00000c90: 7665 722c 2061 6e64 2041 5049 2065 7272  ver, and API err
-00000ca0: 6f72 732e 204f 7572 2067 6f61 6c20 6973  ors. Our goal is
-00000cb0: 2074 6f20 636f 6e73 6973 7465 6e74 6c79   to consistently
-00000cc0: 0a61 6464 206e 6577 2066 756e 6374 696f  .add new functio
-00000cd0: 6e61 6c69 7479 2074 6f20 7375 7070 6f72  nality to suppor
-00000ce0: 7420 6164 6469 7469 6f6e 616c 2075 7365  t additional use
-00000cf0: 2063 6173 6573 2e20 4966 2079 6f75 2068   cases. If you h
-00000d00: 6176 6520 616e 7920 636f 6d6d 656e 7473  ave any comments
-00000d10: 206f 7220 0a73 7567 6765 7374 696f 6e73   or .suggestions
-00000d20: 2066 6f72 206e 6577 2066 6561 7475 7265   for new feature
-00000d30: 732c 2064 6f6e 2774 2068 6573 6974 6174  s, don't hesitat
-00000d40: 6520 746f 2063 7265 6174 6520 616e 2069  e to create an i
-00000d50: 7373 7565 206f 7220 7265 6163 6820 6f75  ssue or reach ou
-00000d60: 7420 746f 200a 6077 6574 7261 6465 2e69  t to .`wetrade.i
-00000d70: 6e62 6f78 4067 6d61 696c 2e63 6f6d 203c  nbox@gmail.com <
-00000d80: 6d61 696c 746f 3a77 6574 7261 6465 2e69  mailto:wetrade.i
-00000d90: 6e62 6f78 4067 6d61 696c 2e63 6f6d 3e60  nbox@gmail.com>`
-00000da0: 5f5f 2e0a 0a0a 2a2a 4469 7363 6c61 696d  __....**Disclaim
-00000db0: 6572 3a2a 2a20 2a77 6574 7261 6465 2069  er:** *wetrade i
-00000dc0: 7320 616e 2075 6e6f 6666 6963 6961 6c20  s an unofficial 
-00000dd0: 4150 4920 6c69 6272 6172 7920 616e 6420  API library and 
-00000de0: 636f 6d65 7320 7769 7468 206e 6f20 7761  comes with no wa
-00000df0: 7272 616e 7479 0a6f 6620 616e 7920 6b69  rranty.of any ki
-00000e00: 6e64 2e20 4974 2069 7320 696e 206e 6f20  nd. It is in no 
-00000e10: 7761 7920 656e 646f 7273 6564 2062 7920  way endorsed by 
-00000e20: 6f72 2061 6666 696c 6961 7465 6420 7769  or affiliated wi
-00000e30: 7468 2045 2a54 5241 4445 2046 696e 616e  th E*TRADE Finan
-00000e40: 6369 616c 200a 6f72 2061 6e79 2061 7373  cial .or any ass
-00000e50: 6f63 6961 7465 6420 6f72 6761 6e69 7a61  ociated organiza
-00000e60: 7469 6f6e 2e20 4d61 6b65 2073 7572 6520  tion. Make sure 
-00000e70: 746f 2072 6561 6420 616e 6420 756e 6465  to read and unde
-00000e80: 7273 7461 6e64 2074 6865 2074 6572 6d73  rstand the terms
-00000e90: 206f 6620 0a73 6572 7669 6365 206f 6620   of .service of 
-00000ea0: 7468 6520 756e 6465 726c 7969 6e67 2041  the underlying A
-00000eb0: 5049 2062 6566 6f72 6520 7573 696e 6720  PI before using 
-00000ec0: 7468 6973 2070 6163 6b61 6765 2e20 5468  this package. Th
-00000ed0: 6973 2061 7574 686f 7273 2061 6363 6570  is authors accep
-00000ee0: 7420 0a6e 6f20 7265 7370 6f6e 7369 6269  t .no responsibi
-00000ef0: 6c69 7479 2066 6f72 2061 6e79 2064 616d  lity for any dam
-00000f00: 6167 6520 7468 6174 206d 6967 6874 2073  age that might s
-00000f10: 7465 6d20 6672 6f6d 2075 7365 206f 6620  tem from use of 
-00000f20: 7468 6973 2070 6163 6b61 6765 2e20 0a53  this package. .S
-00000f30: 6565 2074 6865 204c 4943 454e 5345 2066  ee the LICENSE f
-00000f40: 696c 6520 666f 7220 6d6f 7265 2064 6574  ile for more det
-00000f50: 6169 6c73 2e2a                           ails.*
+00000430: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 496e 206f  ----------..In o
+00000440: 7264 6572 2074 6f20 6163 6365 7373 2074  rder to access t
+00000450: 6865 2045 2d54 7261 6465 2041 5049 2c20  he E-Trade API, 
+00000460: 796f 7527 6c6c 206e 6565 6420 746f 2066  you'll need to f
+00000470: 6f6c 6c6f 7720 7468 6520 3420 7374 6570  ollow the 4 step
+00000480: 7320 6465 7461 696c 6564 206f 6e20 7468  s detailed on th
+00000490: 650a 6045 2d54 7261 6465 2064 6576 656c  e.`E-Trade devel
+000004a0: 6f70 6572 2067 6574 7469 6e67 2073 7461  oper getting sta
+000004b0: 7274 6564 2070 6167 6520 3c68 7474 7073  rted page <https
+000004c0: 3a2f 2f64 6576 656c 6f70 6572 2e65 7472  ://developer.etr
+000004d0: 6164 652e 636f 6d2f 6765 7474 696e 672d  ade.com/getting-
+000004e0: 7374 6172 7465 642f 3e60 5f5f 0a74 6865  started/>`__.the
+000004f0: 6e20 7265 7175 6573 7420 616e 2041 5049  n request an API
+00000500: 206b 6579 2074 6872 6f75 6768 2060 7468   key through `th
+00000510: 6520 6c69 6e6b 6564 2070 6167 6520 3c68  e linked page <h
+00000520: 7474 7073 3a2f 2f75 732e 6574 7261 6465  ttps://us.etrade
+00000530: 2e63 6f6d 2f65 7478 2f72 6973 2f61 7069  .com/etx/ris/api
+00000540: 6b65 792f 3e60 5f5f 2e0a 4974 2773 2061  key/>`__..It's a
+00000550: 6c73 6f20 7265 636f 6d6d 656e 6465 6420  lso recommended 
+00000560: 7468 6174 2079 6f75 2065 6e61 626c 6520  that you enable 
+00000570: 7265 616c 2d74 696d 6520 6461 7461 2069  real-time data i
+00000580: 6e20 7468 6520 0a60 7468 6520 7375 6273  n the .`the subs
+00000590: 6372 6970 7469 6f6e 2063 656e 7465 7220  cription center 
+000005a0: 3c68 7474 7073 3a2f 2f75 732e 6574 7261  <https://us.etra
+000005b0: 6465 2e63 6f6d 2f65 7478 2f70 7879 2f6d  de.com/etx/pxy/m
+000005c0: 792d 7072 6f66 696c 652f 7375 6273 6372  y-profile/subscr
+000005d0: 6970 7469 6f6e 2d63 656e 7465 722f 3e60  iption-center/>`
+000005e0: 5f5f 0a73 6f20 7468 6174 2079 6f75 2064  __.so that you d
+000005f0: 6f6e 2774 2072 6563 6569 7665 2064 656c  on't receive del
+00000600: 6179 6564 2071 756f 7465 732e 200a 0a49  ayed quotes. ..I
+00000610: 6e73 7461 6c6c 2060 6077 6574 7261 6465  nstall ``wetrade
+00000620: 6060 3a0a 0a49 7427 7320 6120 676f 6f64  ``:..It's a good
+00000630: 2069 6465 6120 746f 2063 7265 6174 6520   idea to create 
+00000640: 6120 6e65 7720 7669 7274 7561 6c20 656e  a new virtual en
+00000650: 7669 726f 6e6d 656e 7420 666f 7220 6120  vironment for a 
+00000660: 6e65 7720 5079 7468 6f6e 2070 726f 6a65  new Python proje
+00000670: 6374 0a0a 2e2e 2063 6f64 652d 626c 6f63  ct.... code-bloc
+00000680: 6b3a 3a20 7368 656c 6c0a 0a20 2023 2063  k:: shell..  # c
+00000690: 7265 6174 6520 7665 6e76 0a20 2070 7974  reate venv.  pyt
+000006a0: 686f 6e33 202d 6d20 7665 6e76 2076 656e  hon3 -m venv ven
+000006b0: 760a 2020 2320 656e 7465 7220 7665 6e76  v.  # enter venv
+000006c0: 0a20 2073 6f75 7263 6520 7665 6e76 2f62  .  source venv/b
+000006d0: 696e 2f61 6374 6976 6174 650a 0a57 6520  in/activate..We 
+000006e0: 6361 6e20 7468 656e 2069 6e73 7461 6c6c  can then install
+000006f0: 2060 6077 6574 7261 6465 6060 2069 6e74   ``wetrade`` int
+00000700: 6f20 6f75 7220 7665 6e76 2e20 466f 7220  o our venv. For 
+00000710: 6175 746f 6d61 7469 6320 6c6f 6769 6e2c  automatic login,
+00000720: 2077 6527 6c6c 2061 6c73 6f0a 6e65 6564   we'll also.need
+00000730: 2074 6f20 696e 7374 616c 6c20 6f75 7220   to install our 
+00000740: 6272 6f77 7365 722e 0a0a 2e2e 2063 6f64  browser..... cod
+00000750: 652d 626c 6f63 6b3a 3a20 7368 656c 6c0a  e-block:: shell.
+00000760: 0a20 2070 6970 2069 6e73 7461 6c6c 2077  .  pip install w
+00000770: 6574 7261 6465 0a20 2070 6c61 7977 7269  etrade.  playwri
+00000780: 6768 7420 696e 7374 616c 6c20 6669 7265  ght install fire
+00000790: 666f 780a 0a4e 6578 742c 2079 6f75 276c  fox..Next, you'l
+000007a0: 6c20 6765 7420 676f 696e 6720 696e 206e  l get going in n
+000007b0: 6f20 7469 6d65 2075 7369 6e67 206f 7572  o time using our
+000007c0: 2061 7574 6f6d 6174 6564 206e 6577 2070   automated new p
+000007d0: 726f 6a65 6374 2073 6372 6970 7421 0a0a  roject script!..
+000007e0: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
+000007f0: 7368 656c 6c0a 0a20 2070 7974 686f 6e20  shell..  python 
+00000800: 2d6d 2077 6574 7261 6465 206e 6577 2d70  -m wetrade new-p
+00000810: 726f 6a65 6374 0a0a 596f 7527 6c6c 206e  roject..You'll n
+00000820: 6f77 2073 6565 2061 2068 616e 6466 756c  ow see a handful
+00000830: 206f 6620 6669 6c65 7320 696e 2079 6f75   of files in you
+00000840: 7220 7072 6f6a 6563 7420 6469 7265 6374  r project direct
+00000850: 6f72 7920 696e 636c 7564 696e 6720 6120  ory including a 
+00000860: 2a73 6574 7469 6e67 732e 7079 2a0a 6669  *settings.py*.fi
+00000870: 6c65 2077 6865 7265 2079 6f75 276c 6c20  le where you'll 
+00000880: 656e 7465 7220 796f 7572 2075 7365 7220  enter your user 
+00000890: 616e 6420 4150 4920 696e 666f 2061 6e64  and API info and
+000008a0: 2068 6176 6520 7468 6520 6f70 7469 6f6e   have the option
+000008b0: 2074 6f20 636f 6e66 6967 7572 6520 7661   to configure va
+000008c0: 7269 6f75 730a 6060 7765 7472 6164 6560  rious.``wetrade`
+000008d0: 6020 7365 7474 696e 6773 2e20 496e 2074  ` settings. In t
+000008e0: 6869 7320 6669 6c65 2c20 796f 7527 6c6c  his file, you'll
+000008f0: 2065 6e74 6572 2079 6f75 7220 7573 6572   enter your user
+00000900: 6e61 6d65 2c20 7061 7373 776f 7264 2c20  name, password, 
+00000910: 636c 6965 6e74 5f6b 6579 2c20 0a61 6e64  client_key, .and
+00000920: 2063 6c69 656e 745f 7365 6372 6574 2073   client_secret s
+00000930: 6f20 6060 7765 7472 6164 6560 6020 6361  o ``wetrade`` ca
+00000940: 6e20 6c6f 6720 696e 746f 2079 6f75 7220  n log into your 
+00000950: 6163 636f 756e 742e 0a0a 496e 2061 6464  account...In add
+00000960: 6974 696f 6e20 746f 202a 7365 7474 696e  ition to *settin
+00000970: 6773 2e70 792a 2c20 7765 2776 6520 616c  gs.py*, we've al
+00000980: 736f 2063 7265 6174 6564 2061 202a 446f  so created a *Do
+00000990: 636b 6572 6669 6c65 2a20 666f 7220 6561  ckerfile* for ea
+000009a0: 7379 2064 6570 6c6f 796d 656e 7420 6173  sy deployment as
+000009b0: 200a 7765 6c6c 2061 7320 6120 2a72 6571   .well as a *req
+000009c0: 7569 7265 6d65 6e74 732e 7478 742a 2061  uirements.txt* a
+000009d0: 6e64 2061 6e20 6578 616d 706c 6520 6669  nd an example fi
+000009e0: 6c65 202a 6d61 696e 2e70 792a 2077 6869  le *main.py* whi
+000009f0: 6368 2064 656d 6f6e 7374 7261 7465 7320  ch demonstrates 
+00000a00: 736f 6d65 2062 6173 6963 200a 7765 7472  some basic .wetr
+00000a10: 6164 6520 7573 6167 653a 0a0a 2a2a 6d61  ade usage:..**ma
+00000a20: 696e 2e70 792a 2a0a 0a2e 2e20 636f 6465  in.py**.... code
+00000a30: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
+00000a40: 0a20 2066 726f 6d20 7765 7472 6164 652e  .  from wetrade.
+00000a50: 6170 6920 696d 706f 7274 2041 5049 436c  api import APICl
+00000a60: 6965 6e74 0a20 2066 726f 6d20 7765 7472  ient.  from wetr
+00000a70: 6164 652e 6163 636f 756e 7420 696d 706f  ade.account impo
+00000a80: 7274 2041 6363 6f75 6e74 0a20 2066 726f  rt Account.  fro
+00000a90: 6d20 7765 7472 6164 652e 7175 6f74 6520  m wetrade.quote 
+00000aa0: 696d 706f 7274 2051 756f 7465 0a20 2066  import Quote.  f
+00000ab0: 726f 6d20 7765 7472 6164 652e 6f72 6465  rom wetrade.orde
+00000ac0: 7220 696d 706f 7274 204c 696d 6974 4f72  r import LimitOr
+00000ad0: 6465 720a 2020 6672 6f6d 2077 6574 7261  der.  from wetra
+00000ae0: 6465 2e75 7469 6c73 2069 6d70 6f72 7420  de.utils import 
+00000af0: 7365 7475 705f 6c6f 6767 696e 670a 0a0a  setup_logging...
+00000b00: 2020 6465 6620 6d61 696e 2829 3a0a 2020    def main():.  
+00000b10: 2020 2320 5365 7475 7020 6c6f 6767 696e    # Setup loggin
+00000b20: 6720 286f 7074 696f 6e61 6c29 2061 6e64  g (optional) and
+00000b30: 2041 5049 436c 6965 6e74 0a20 2020 2073   APIClient.    s
+00000b40: 6574 7570 5f6c 6f67 6769 6e67 2829 0a20  etup_logging(). 
+00000b50: 2020 2063 6c69 656e 7420 3d20 4150 4943     client = APIC
+00000b60: 6c69 656e 7428 290a 0a20 2020 2023 2043  lient()..    # C
+00000b70: 6865 636b 206f 7574 2079 6f75 7220 6163  heck out your ac
+00000b80: 636f 756e 740a 2020 2020 6163 636f 756e  count.    accoun
+00000b90: 7420 3d20 4163 636f 756e 7428 636c 6965  t = Account(clie
+00000ba0: 6e74 3d63 6c69 656e 7429 0a20 2020 2070  nt=client).    p
+00000bb0: 7269 6e74 2827 4d79 2041 6363 6f75 6e74  rint('My Account
+00000bc0: 204b 6579 3a20 272c 2061 6363 6f75 6e74   Key: ', account
+00000bd0: 2e61 6363 6f75 6e74 5f6b 6579 290a 2020  .account_key).  
+00000be0: 2020 7072 696e 7428 274d 7920 4261 6c61    print('My Bala
+00000bf0: 6e63 653a 2027 2c20 6163 636f 756e 742e  nce: ', account.
+00000c00: 6368 6563 6b5f 6261 6c61 6e63 6528 2929  check_balance())
+00000c10: 0a0a 2020 2020 2320 4765 7420 6120 7374  ..    # Get a st
+00000c20: 6f63 6b20 7175 6f74 650a 2020 2020 7175  ock quote.    qu
+00000c30: 6f74 6520 3d20 5175 6f74 6528 636c 6965  ote = Quote(clie
+00000c40: 6e74 3d63 6c69 656e 742c 2073 796d 626f  nt=client, symbo
+00000c50: 6c3d 2749 424d 2729 0a20 2020 2070 7269  l='IBM').    pri
+00000c60: 6e74 2866 274c 6173 7420 7b71 756f 7465  nt(f'Last {quote
+00000c70: 2e73 796d 626f 6c7d 2051 756f 7465 2050  .symbol} Quote P
+00000c80: 7269 6365 3a20 272c 2071 756f 7465 2e67  rice: ', quote.g
+00000c90: 6574 5f6c 6173 745f 7072 6963 6528 2929  et_last_price())
+00000ca0: 0a0a 2020 2020 2320 506c 6163 6520 736f  ..    # Place so
+00000cb0: 6d65 206f 7264 6572 7320 616e 6420 7374  me orders and st
+00000cc0: 7566 660a 2020 2020 6f72 6465 7231 203d  uff.    order1 =
+00000cd0: 204c 696d 6974 4f72 6465 7228 0a20 2020   LimitOrder(.   
+00000ce0: 2020 2020 2063 6c69 656e 7420 3d20 636c       client = cl
+00000cf0: 6965 6e74 2c0a 2020 2020 2020 2020 6163  ient,.        ac
+00000d00: 636f 756e 745f 6b65 7920 3d20 6163 636f  count_key = acco
+00000d10: 756e 742e 6163 636f 756e 745f 6b65 792c  unt.account_key,
+00000d20: 0a20 2020 2020 2020 2073 796d 626f 6c20  .        symbol 
+00000d30: 3d20 274e 5644 4127 2c0a 2020 2020 2020  = 'NVDA',.      
+00000d40: 2020 6163 7469 6f6e 203d 2027 4255 5927    action = 'BUY'
+00000d50: 2c0a 2020 2020 2020 2020 7175 616e 7469  ,.        quanti
+00000d60: 7479 203d 2031 2c0a 2020 2020 2020 2020  ty = 1,.        
+00000d70: 7072 6963 6520 3d20 3530 2e30 3029 0a20  price = 50.00). 
+00000d80: 2020 206f 7264 6572 312e 706c 6163 655f     order1.place_
+00000d90: 6f72 6465 7228 290a 2020 2020 6f72 6465  order().    orde
+00000da0: 7231 2e72 756e 5f77 6865 6e5f 7374 6174  r1.run_when_stat
+00000db0: 7573 280a 2020 2020 2020 2020 2743 414e  us(.        'CAN
+00000dc0: 4345 4c4c 4544 272c 200a 2020 2020 2020  CELLED', .      
+00000dd0: 2020 6675 6e63 203d 2070 7269 6e74 2c20    func = print, 
+00000de0: 0a20 2020 2020 2020 2066 756e 635f 6172  .        func_ar
+00000df0: 6773 203d 205b 2754 6573 7420 6d65 7373  gs = ['Test mess
+00000e00: 6167 6527 5d29 0a20 2020 200a 2020 2020  age']).    .    
+00000e10: 6f72 6465 7232 203d 204c 696d 6974 4f72  order2 = LimitOr
+00000e20: 6465 7228 0a20 2020 2020 2020 2063 6c69  der(.        cli
+00000e30: 656e 7420 3d20 636c 6965 6e74 2c0a 2020  ent = client,.  
+00000e40: 2020 2020 2020 6163 636f 756e 745f 6b65        account_ke
+00000e50: 7920 3d20 6163 636f 756e 742e 6163 636f  y = account.acco
+00000e60: 756e 745f 6b65 792c 0a20 2020 2020 2020  unt_key,.       
+00000e70: 2073 796d 626f 6c20 3d20 274e 464c 5827   symbol = 'NFLX'
+00000e80: 2c0a 2020 2020 2020 2020 6163 7469 6f6e  ,.        action
+00000e90: 203d 2027 4255 5927 2c0a 2020 2020 2020   = 'BUY',.      
+00000ea0: 2020 7175 616e 7469 7479 203d 2031 2c0a    quantity = 1,.
+00000eb0: 2020 2020 2020 2020 7072 6963 6520 3d20          price = 
+00000ec0: 3530 2e30 3029 0a20 2020 206f 7264 6572  50.00).    order
+00000ed0: 322e 706c 6163 655f 6f72 6465 7228 290a  2.place_order().
+00000ee0: 2020 2020 6f72 6465 7232 2e72 756e 5f77      order2.run_w
+00000ef0: 6865 6e5f 7374 6174 7573 280a 2020 2020  hen_status(.    
+00000f00: 2020 2020 2743 414e 4345 4c4c 4544 272c      'CANCELLED',
+00000f10: 0a20 2020 2020 2020 206f 7264 6572 312e  .        order1.
+00000f20: 6361 6e63 656c 5f6f 7264 6572 290a 2020  cancel_order).  
+00000f30: 2020 0a20 2020 206f 7264 6572 322e 6361    .    order2.ca
+00000f40: 6e63 656c 5f6f 7264 6572 2829 0a0a 0a4f  ncel_order()...O
+00000f50: 7468 6572 2069 6e66 6f0a 2d2d 2d2d 2d2d  ther info.------
+00000f60: 2d2d 2d2d 2d2d 2d0a 0a60 6077 6574 7261  -------..``wetra
+00000f70: 6465 6060 2077 6173 2069 6e69 7469 616c  de`` was initial
+00000f80: 6c79 2064 6573 6967 6e65 6420 746f 2072  ly designed to r
+00000f90: 756e 2068 6561 646c 6573 736c 7920 616e  un headlessly an
+00000fa0: 6420 6861 7320 6275 696c 742d 696e 2068  d has built-in h
+00000fb0: 616e 646c 696e 6720 666f 7220 0a6d 6f73  andling for .mos
+00000fc0: 7420 6578 7065 6374 6564 2062 726f 6b65  t expected broke
+00000fd0: 7261 6765 2c20 7365 7276 6572 2c20 616e  rage, server, an
+00000fe0: 6420 4150 4920 6572 726f 7273 2e20 5468  d API errors. Th
+00000ff0: 6973 2061 6e64 2074 6865 206d 616a 6f72  is and the major
+00001000: 6974 7920 6f66 206f 7468 6572 200a 6060  ity of other .``
+00001010: 7765 7472 6164 6560 6020 6675 6e63 7469  wetrade`` functi
+00001020: 6f6e 616c 6974 7920 6973 2065 6e74 6972  onality is entir
+00001030: 656c 7920 6f70 7469 6f6e 616c 2074 6f20  ely optional to 
+00001040: 7573 652c 2061 6e64 206f 7572 206d 6f64  use, and our mod
+00001050: 756c 6172 2073 7472 7563 7475 7265 200a  ular structure .
+00001060: 616c 6c6f 7773 2079 6f75 2074 6f20 7574  allows you to ut
+00001070: 696c 697a 6520 6173 206d 7563 6820 6f72  ilize as much or
+00001080: 2061 7320 6c69 7474 6c65 206f 6620 7468   as little of th
+00001090: 6520 6c69 6272 6172 7920 6173 2079 6f75  e library as you
+000010a0: 2764 206c 696b 652e 204f 7572 2067 6f61  'd like. Our goa
+000010b0: 6c20 0a69 7320 746f 2063 6f6e 7369 7374  l .is to consist
+000010c0: 656e 746c 7920 6164 6420 6e65 7720 6675  ently add new fu
+000010d0: 6e63 7469 6f6e 616c 6974 7920 746f 2073  nctionality to s
+000010e0: 7570 706f 7274 2061 6464 6974 696f 6e61  upport additiona
+000010f0: 6c20 7573 6520 6361 7365 732e 2049 6620  l use cases. If 
+00001100: 796f 7520 0a68 6176 6520 616e 7920 636f  you .have any co
+00001110: 6d6d 656e 7473 206f 7220 7375 6767 6573  mments or sugges
+00001120: 7469 6f6e 7320 666f 7220 6e65 7720 6665  tions for new fe
+00001130: 6174 7572 6573 2c20 646f 6e27 7420 6865  atures, don't he
+00001140: 7369 7461 7465 2074 6f20 6372 6561 7465  sitate to create
+00001150: 2061 6e20 0a69 7373 7565 206f 7220 7265   an .issue or re
+00001160: 6163 6820 6f75 7420 746f 3a20 6077 6574  ach out to: `wet
+00001170: 7261 6465 2e69 6e62 6f78 4067 6d61 696c  rade.inbox@gmail
+00001180: 2e63 6f6d 203c 6d61 696c 746f 3a77 6574  .com <mailto:wet
+00001190: 7261 6465 2e69 6e62 6f78 4067 6d61 696c  rade.inbox@gmail
+000011a0: 2e63 6f6d 3e60 5f5f 2e0a 0a0a 2a2a 4469  .com>`__....**Di
+000011b0: 7363 6c61 696d 6572 3a2a 2a20 2a77 6574  sclaimer:** *wet
+000011c0: 7261 6465 2069 7320 616e 2075 6e6f 6666  rade is an unoff
+000011d0: 6963 6961 6c20 4150 4920 6c69 6272 6172  icial API librar
+000011e0: 7920 616e 6420 636f 6d65 7320 7769 7468  y and comes with
+000011f0: 206e 6f20 7761 7272 616e 7479 0a6f 6620   no warranty.of 
+00001200: 616e 7920 6b69 6e64 2e20 4974 2069 7320  any kind. It is 
+00001210: 696e 206e 6f20 7761 7920 656e 646f 7273  in no way endors
+00001220: 6564 2062 7920 6f72 2061 6666 696c 6961  ed by or affilia
+00001230: 7465 6420 7769 7468 2045 2a54 5241 4445  ted with E*TRADE
+00001240: 2046 696e 616e 6369 616c 200a 6f72 2061   Financial .or a
+00001250: 6e79 2061 7373 6f63 6961 7465 6420 6f72  ny associated or
+00001260: 6761 6e69 7a61 7469 6f6e 2e20 4d61 6b65  ganization. Make
+00001270: 2073 7572 6520 746f 2072 6561 6420 616e   sure to read an
+00001280: 6420 756e 6465 7273 7461 6e64 2074 6865  d understand the
+00001290: 2074 6572 6d73 206f 6620 0a73 6572 7669   terms of .servi
+000012a0: 6365 206f 6620 7468 6520 756e 6465 726c  ce of the underl
+000012b0: 7969 6e67 2041 5049 2062 6566 6f72 6520  ying API before 
+000012c0: 7573 696e 6720 7468 6973 2070 6163 6b61  using this packa
+000012d0: 6765 2e20 5468 6973 2061 7574 686f 7273  ge. This authors
+000012e0: 2061 6363 6570 7420 0a6e 6f20 7265 7370   accept .no resp
+000012f0: 6f6e 7369 6269 6c69 7479 2066 6f72 2061  onsibility for a
+00001300: 6e79 2064 616d 6167 6520 7468 6174 206d  ny damage that m
+00001310: 6967 6874 2073 7465 6d20 6672 6f6d 2075  ight stem from u
+00001320: 7365 206f 6620 7468 6973 2070 6163 6b61  se of this packa
+00001330: 6765 2e20 0a53 6565 2074 6865 204c 4943  ge. .See the LIC
+00001340: 454e 5345 2066 696c 6520 666f 7220 6d6f  ENSE file for mo
+00001350: 7265 2064 6574 6169 6c73 2e2a            re details.*
```

### Comparing `wetrade-0.1.0/setup.py` & `wetrade-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.rst', 'r') as f:
   long_description = f.read()
 
 setuptools.setup(
   name = 'wetrade',
-  version = '0.1.0',
+  version = '0.1.1',
   author = 'Mason Krause',
   description = 'An E-Trade python library built for active stock trading',
   long_description = long_description,
   packages = setuptools.find_packages(),
   include_package_data = True,
   python_requires = '>=3.7',
   install_requires = [
```

### Comparing `wetrade-0.1.0/tests/mock_api/account_responses.py` & `wetrade-0.1.1/tests/mock_api/account_responses.py`

 * *Files identical despite different names*

### Comparing `wetrade-0.1.0/tests/mock_api/mock_api.py` & `wetrade-0.1.1/tests/mock_api/mock_api.py`

 * *Files identical despite different names*

### Comparing `wetrade-0.1.0/tests/mock_api/order_responses.py` & `wetrade-0.1.1/tests/mock_api/order_responses.py`

 * *Files identical despite different names*

### Comparing `wetrade-0.1.0/tests/mock_api/quote_responses.py` & `wetrade-0.1.1/tests/mock_api/quote_responses.py`

 * *Files identical despite different names*

### Comparing `wetrade-0.1.0/tests/order/test_base_order.py` & `wetrade-0.1.1/tests/order/test_base_order.py`

 * *Files identical despite different names*

### Comparing `wetrade-0.1.0/tests/quote/test_quote.py` & `wetrade-0.1.1/tests/quote/test_quote.py`

 * *Files identical despite different names*

### Comparing `wetrade-0.1.0/tests/test_account.py` & `wetrade-0.1.1/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `wetrade-0.1.0/tests/test_api.py` & `wetrade-0.1.1/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 import unittest
 from wetrade.api import APIClient
-from wetrade.user_session import UserSession
+from wetrade.user_session import SimpleUserSession
 from .sandbox_responses import account_responses, quote_responses, order_responses
 try:
   from settings import config_options
 except ModuleNotFoundError:
   from wetrade.project_template.settings import config_options
 
 
-class SimpleUserSession(UserSession):
-  def handle_request(self, http_method, args, kwargs):
-    return self.session.request(http_method, *args, **kwargs, timeout=30)
-
 class TestAPIClient(unittest.TestCase):
   @classmethod
   def setUpClass(cls):
     cls.user_session = SimpleUserSession(config=config_options['sandbox'])
     cls.client = APIClient(cls.user_session)
 
   def test_request_account_list(self):
```

### Comparing `wetrade-0.1.0/wetrade/account.py` & `wetrade-0.1.1/wetrade/account.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,58 @@
 import time
 from wetrade.api import APIClient
 from wetrade.utils import log_in_background
 
 class Account:
+  '''
+  :param APIClient client: your :ref:`APIClient <api_client>`
+  :param str account_key: (optional) manually specify your account key 
+  '''
   def __init__(self, client:APIClient, account_key=''):
     self.client = client
     self.account_key = account_key if account_key else self.list_accounts()[0]['accountIdKey']
 
   def list_accounts(self):
+    '''
+    Provides details on all brokerage accounts connected to the active E-Trade user account
+    '''
     response, status_code = self.client.request_account_list()
     try:
       accounts = response['AccountListResponse']['Accounts']['Account']
       return accounts
     except Exception as e:
       log_in_background(
         called_from = 'list_accounts',
         tags = ['user-message'], 
         message = time.strftime('%H:%M:%S', time.localtime()) + ': Error getting account list, retrying',
         e = e,
         account_key = self.account_key)
       return self.list_accounts()
 
   def check_balance(self):
+    '''
+    Returns the balance of your account
+    '''
     response, status_code = self.client.request_account_balance(account_key=self.account_key)
     try:
       balance = response['BalanceResponse']['Computed']['cashAvailableForInvestment']
       return balance
     except Exception as e:
       log_in_background(
         called_from = 'list_accounts',
         tags = ['user-message'], 
         message = time.strftime('%H:%M:%S', time.localtime()) + ': Error getting account balance, retrying',
         e = e,
         account_key = self.account_key)
       return self.check_balance()
 
   def view_portfolio(self):
+    '''
+    Provides details for your account portfolio
+    '''
     response, status_code = self.client.request_account_portfolio(account_key=self.account_key)
     try:
       portfolio = {} if status_code == 204 else response['PortfolioResponse']['AccountPortfolio']
       return portfolio
     except Exception as e:
       log_in_background(
         called_from = 'list_accounts',
```

### Comparing `wetrade-0.1.0/wetrade/order/base_order.py` & `wetrade-0.1.1/wetrade/order/base_order.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,24 @@
 from contextlib import suppress
 from wetrade.api import APIClient
 from wetrade.utils import start_thread, log_in_background
 from .lookup_msg import lookup_error_msg, lookup_user_msg
 
 
 class BaseOrder:
+  '''
+  A base order class containing methods use in other order types
+
+  :param APIClient client: your :ref:`APIClient <api_client>`
+  :param str account_key: your account key
+  :param str symbol: the symbol of your security
+  :param str action: The action for your order (BUY, SELL, BUY_TO_COVER, SELL_SHORT, BUY_OPEN, BUY_CLOSE, SELL_OPEN, SELL_CLOSE, EXCHANGE)
+  :param int quantity: the quantity for your order
+  :param float price: the price for your order
+  '''
   def __init__(self, client:APIClient, account_key, symbol, action, quantity, price):
     self.client = client
     self.account_key = account_key
     self.symbol = symbol
     self.action = action
     self.quantity = quantity
     self.price = price
@@ -36,15 +46,15 @@
               'securityType': 'EQ',
               'symbol': self.symbol},
             'orderAction': self.action, # [BUY, SELL, BUY_TO_COVER, SELL_SHORT, BUY_OPEN, BUY_CLOSE, SELL_OPEN, SELL_CLOSE, EXCHANGE]
             'quantityType': 'QUANTITY',
             'quantity': self.quantity}}}}
     self.place_order_request = {}
 
-  def modify_order(self, action_type='preview'):
+  def __modify_order(self, action_type='preview'):
     if action_type == 'preview':
       response, status_code = self.client.request_order_preview(account_key=self.account_key, order_data=self.preview_order_request)
       response_key = 'PreviewOrderResponse'
       msg_ref = 'previewing'
     elif action_type == 'place':
       response, status_code = self.client.request_order_place(account_key=self.account_key, order_data=self.place_order_request)
       response_key = 'PlaceOrderResponse'
@@ -61,38 +71,39 @@
       return # maybe log incorrect action specified  
     if response_key in response:
       return response[response_key]
     elif 'Error' in response:
       error_code = response['Error']['code']
       error_msg = lookup_error_msg(error_code=error_code, msg_ref=msg_ref, order_id=self.order_id)
       log_in_background(
-        called_from = 'modify_order',
+        called_from = '__modify_order',
         tags = ['user-message'], 
         message = time.strftime('%H:%M:%S', time.localtime()) + error_msg,
         account_key = self.account_key,
         symbol = self.symbol)
       if error_code in [1508, 163, 1524]:
         time.sleep(1)
-        return self.modify_order(action_type)
+        return self.__modify_order(action_type)
 
   def preview_order(self):
-    preview_response = self.modify_order('preview')
+    preview_response = self.__modify_order('preview')
     if preview_response:
       self.place_order_request = {
         'PlaceOrderRequest': {
           'orderType': preview_response['orderType'],
           'clientOrderId': self.client_order_id,
           'PreviewIds': preview_response['PreviewIds'],
           'Order': preview_response['Order']}}
     return preview_response
   
   def place_order(self):
+    '''Places your order'''
     preview = self.preview_order()
     if preview:
-      order_response = self.modify_order('place')
+      order_response = self.__modify_order('place')
       if order_response:
         self.order_id = order_response['OrderIds'][0]['orderId']
         log_in_background(
           called_from = 'place_order',
           tags = ['user-message'], 
           account_key = self.account_key,
           symbol = self.symbol,
@@ -101,63 +112,70 @@
   
   def preview_update_price(self, new_price):
     self.client_order_id = random.randint(1000000000, 9999999999)
     self.preview_order_request['PreviewOrderRequest']['Order']['priceType'] = self.order_type
     self.preview_order_request['PreviewOrderRequest']['Order']['limitPrice'] = new_price
     self.preview_order_request['PreviewOrderRequest']['Order']['stopPrice'] = new_price
     self.preview_order_request['PreviewOrderRequest']['Order']['stopLimitPrice'] = new_price
-    preview_response = self.modify_order('preview_update')
+    preview_response = self.__modify_order('preview_update')
     if preview_response:
       self.place_order_request = {
         'PlaceOrderRequest': {
           'orderType': preview_response['orderType'],
           'clientOrderId': self.client_order_id,
           'PreviewIds': preview_response['PreviewIds'],
           'Order': preview_response['Order']}}
     return preview_response
   
   def update_price(self, new_price):
+    '''
+    Updates the price of an already placed order
+    
+    :param float new_price: the new price for your order
+    '''
     old_id = self.order_id
     self.updating = True
     preview = self.preview_update_price(new_price)
     if preview:
-      order_response = self.modify_order('update')
+      order_response = self.__modify_order('update')
       if order_response:
         self.order_id = order_response['OrderIds'][0]['orderId']
         self.price = new_price
         log_in_background(
           called_from = 'update_price',
           tags = ['user-message'], 
           account_key = self.account_key,
           symbol = self.symbol,
           message = lookup_user_msg('update_price', price=self.price, account_key=self.account_key, order_response=order_response, old_id=old_id))
       self.updating = False
       return order_response
     self.updating = False
   
   def to_market_order(self):
+    '''Converts an active, already-placed order into a market order which will execute immediately during market hours'''
     old_id = self.order_id
     self.updating = True
     self.order_type = 'MARKET'
     preview = self.preview_update_price(0.0)
     if preview:
-      order_response = self.modify_order('update')
+      order_response = self.__modify_order('update')
       if order_response:
         self.order_id = order_response['OrderIds'][0]['orderId']
         log_in_background(
           called_from = 'to_market_order',
           tags = ['user-message'], 
           account_key = self.account_key,
           symbol = self.symbol,
           message = lookup_user_msg('to_market_order', price=self.price, account_key=self.account_key, order_response=order_response, old_id=old_id))
       self.updating = False
       return order_response
     self.updating = False
 
   def cancel_order(self):
+    '''Cancels your active, already-placed order'''
     response, status_code = self.client.request_order_cancel(account_key=self.account_key, order_id=self.order_id, symbol=self.symbol)
     msg_num = 0
     with suppress(Exception):
       msg_num = response['CancelOrderResponse']['Messages']['Message'][0]['code']
     if msg_num in [5011, 4186]:
       log_in_background(
         called_from = 'cancel_order',
@@ -178,47 +196,56 @@
         message = '{}: Could not cancel order {} (Account: {}), check logs'.format(
           time.strftime('%H:%M:%S', time.localtime()),
           response['CancelOrderResponse']['orderId'],
           self.account_key))
       return False
 
   def check_status(self):
+    '''Checks the status of an already placed order'''
     response, status_code = self.client.request_order_status(account_key=self.account_key, order_id=self.order_id, symbol=self.symbol)
     status = ''
     execution_price = 0.0
     with suppress(Exception):
       status = response['OrdersResponse']['Order'][0]['OrderDetail'][0]['status']
       execution_price = response['OrdersResponse']['Order'][0]['OrderDetail'][0]['Instrument'][0]['averageExecutionPrice']
     if status == 'EXECUTED' and execution_price != 0:
       self.price = execution_price
     self.status = status
     return status
 
-  def handle_rejected_order(self):
+  def __handle_rejected_order(self):
     # # Need to reset client_order_id after rejection to resend, etc (see example below)
     # self.updating = True
     # self.client_order_id = random.randint(1000000000, 9999999999)
     # # Make any changes here
     # self.place_order()
     # self.updating = False
     log_in_background(
       called_from = 'wait_for_status',
       tags = ['user-message'], 
       account_key = self.account_key,
       symbol = self.symbol,
       message = '{}: Order {} REJECTED - no longer waiting (Account: {})'.format(time.strftime('%H:%M:%S', time.localtime()), self.order_id, self.account_key))
 
   def wait_for_status(self, status, then=None, args=[], kwargs={}): # [OPEN, EXECUTED, CANCELLED, INDIVIDUAL_FILLS, CANCEL_REQUESTED, EXPIRED, REJECTED]
+    '''
+    Waits for your order to reach your specified status then runs an optional callback function
+    
+    :param str status: the status to wait for (OPEN, EXECUTED, CANCELLED, INDIVIDUAL_FILLS, CANCEL_REQUESTED, EXPIRED, REJECTED)
+    :param then: (optional) a callback function to run after waiting for status
+    :param list args: a list of args for your function
+    :param dict kwargs: a dict containing kwargs for your function
+    '''
     waiting = True
     stop_for = ['CANCELLED','EXECUTED','EXPIRED']
     while waiting:
       if self.updating == False:
         order_status = self.check_status()
         if order_status == 'REJECTED': # special handling for rejected orders
-          return self.handle_rejected_order()
+          return self.__handle_rejected_order()
         if order_status == 'CANCELLED': # Double check canceled order for corner case waiting on new order_id
           time.sleep(1)
           order_status = self.check_status()
         if order_status == status:
           waiting = False
           if then:
             return then(*args, **kwargs)
@@ -232,9 +259,17 @@
             account_key = self.account_key,
             symbol = self.symbol,
             message = '{}: Order {} {} - no longer waiting (Account: {})'.format(time.strftime('%H:%M:%S', time.localtime()), self.order_id, order_status, self.account_key))
           return
       time.sleep(.4) # throttle to avoid rate limit 
 
   def run_when_status(self, status, func, func_args=[], func_kwargs={}):
+    '''
+    Runs a callback when your order reaches a certain status without waiting
+    
+    :param str status: your anticipated status (OPEN, EXECUTED, CANCELLED, INDIVIDUAL_FILLS, CANCEL_REQUESTED, EXPIRED, REJECTED)
+    :param then: (optional) a callback function to run after status is met
+    :param list args: a list of args for your function
+    :param dict kwargs: a dict containing kwargs for your function
+    '''
     args = [status, func, func_args, func_kwargs]
     start_thread(self.wait_for_status, args=args)
```

### Comparing `wetrade-0.1.0/wetrade/order/converting_stop_order.py` & `wetrade-0.1.1/wetrade/order/converting_stop_order.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,29 +3,32 @@
 from wetrade.order import StopOrder
 from wetrade.utils import log_in_background
 from .lookup_msg import lookup_error_msg
 
 
 # Stop order that converts to a market order if rejected or out of range 
 class ConvertingStopOrder(StopOrder):
-  def handle_rejected_order(self):
+  '''
+  A stop order that converts to a limit order when rejected or current price is above stop price for a sell order or when current price is below stop price for a buy order
+  '''
+  def __handle_rejected_order(self):
     self.updating = True
     self.client_order_id = random.randint(1000000000, 9999999999)
     self.order_type =  'MARKET'
     self.preview_order_request['PreviewOrderRequest']['Order']['priceType'] = 'MARKET'
     self.place_order()
     self.updating = False
     log_in_background(
       called_from = 'wait_for_status',
       tags = ['user-message'], 
       account_key = self.account_key,
       symbol = self.symbol,
       message = '{}: Order {} REJECTED , replacing as MARKET order (Account: {})'.format(time.strftime('%H:%M:%S', time.localtime()), self.order_id, self.account_key))
     
-  def modify_order(self, action_type='preview'):
+  def __modify_order(self, action_type='preview'):
     if action_type == 'preview':
       response, status_code = self.client.request_order_preview(account_key=self.account_key, order_data=self.preview_order_request)
       response_key = 'PreviewOrderResponse'
       msg_ref = 'previewing'
     elif action_type == 'place':
       response, status_code = self.client.request_order_place(account_key=self.account_key, order_data=self.place_order_request)
       response_key = 'PlaceOrderResponse'
@@ -42,19 +45,19 @@
       return # maybe log incorrect action specified  
     if response_key in response:
       return response[response_key]
     elif 'Error' in response:
       error_code = response['Error']['code']
       error_msg = lookup_error_msg(error_code=error_code, msg_ref=msg_ref, order_id=self.order_id)
       log_in_background(
-        called_from = 'modify_order',
+        called_from = '__modify_order',
         tags = ['user-message'], 
         message = time.strftime('%H:%M:%S', time.localtime()) + error_msg,
         account_key = self.account_key,
         symbol = self.symbol)
       if error_code in [1508, 163, 1524]:
         time.sleep(1)
-        return self.modify_order(action_type)
+        return self.__modify_order(action_type)
       elif error_code in [2084, 2085]:
         self.order_type =  'MARKET'
         self.preview_order_request['PreviewOrderRequest']['Order']['priceType'] = 'MARKET'
-        return self.modify_order(action_type)
+        return self.__modify_order(action_type)
```

### Comparing `wetrade-0.1.0/wetrade/order/lookup_msg.py` & `wetrade-0.1.1/wetrade/order/lookup_msg.py`

 * *Files identical despite different names*

### Comparing `wetrade-0.1.0/wetrade/project_template/settings.py` & `wetrade-0.1.1/wetrade/project_template/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,11 @@
-# Google Cloud settings (optional)
-# need GOOGLE_APPLICATION_CREDENTIALS env var set to json path
-enable_cloud_logging = False
-quote_bucket = 'your-quote-bucket'
-# E-trade settings
+# E-Trade settings
 login_method = 'auto' # 'auto', 'manual'
 use_2fa = False # needed to disable SMS auth - requires totp_secret
-config_id = 'prod'
+config_id = 'sandbox'
 config_options = {
   'sandbox':{
     'base_url': 'https://apisb.etrade.com/',
     'client_key': 'SANDBOX_CLIENT_KEY',
     'client_secret': 'SANDBOX_CLIENT_SECRET',
     'username': 'USERNAME',
     'password': 'PASSWORD',
@@ -17,9 +13,13 @@
   'prod':{
     'base_url': 'https://api.etrade.com/',
     'client_key': 'PROD_CLIENT_KEY',
     'client_secret': 'PROD_CLIENT_SECRET',
     'username': 'USERNAME',
     'password': 'PASSWORD',
     'totp_secret': 'TOTP_SECRET'}}
+# Google Cloud settings (optional)
+# need GOOGLE_APPLICATION_CREDENTIALS env var set to json path
+enable_cloud_logging = False
+quote_bucket = 'your-quote-bucket'
 
 config = config_options[config_id]
```

### Comparing `wetrade-0.1.0/wetrade/quote/data_frame_quote.py` & `wetrade-0.1.1/wetrade/quote/data_frame_quote.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,20 +4,26 @@
 import google.cloud.storage
 import polars as pl 
 import pandas as pd
 from .quote import Quote
 from wetrade.api import APIClient
 from wetrade.utils import log_in_background, check_market_hours
 try:
-  from settings import quote_bucket
+  import settings
 except ModuleNotFoundError:
-  from wetrade.project_template.settings import quote_bucket
+  import wetrade.project_template.settings as settings
 
 
 class DataFrameQuote(Quote):
+  '''
+  A Quote that uses a DataFrame to keep track of quote details and enable complex calculations
+
+  :param APIClient client: your :ref:`APIClient <api_client>`
+  :param str symbol: the symbol of your security
+  '''
   def __init__(self, client:APIClient, symbol):
     super().__init__()
     self.data = pl.DataFrame(schema={ #maybe use numpy array instead of polars df
       'datetime': pl.Datetime,
       'datetime_epoch': pl.Int64,
       'ask': pl.Float64,
       'ask_size': pl.Int64,
@@ -27,20 +33,20 @@
       'bid_time': pl.Datetime,
       'last_trade': pl.Float64,
       'last_trade_time': pl.Int64,
       '30s_average': pl.Float64,
       '10s_average': pl.Float64})
     self.smoothed_price = 0.0
 
-  def monitor_quote(self):
+  def __monitor_quote(self):
     if self.monitoring_active == False:
       market_close = check_market_hours()['close']
       if time.strftime('%H:%M', time.localtime()) > market_close:
         log_in_background(
-          called_from = 'monitor_quote',
+          called_from = '__monitor_quote',
           tags = ['user-message'], 
           symbol = self.symbol,
           message = '{}: Markets are closed'.format(time.strftime('%H:%M:%S', time.localtime())))
       else:
         self.monitoring_active = True
       while self.monitoring_active == True and time.strftime('%H:%M', time.localtime()) < market_close:
         quote_data = self.get_quote()
@@ -61,27 +67,37 @@
         self.data = self.data.set_sorted('datetime').with_columns([
           pl.col('last_trade').rolling_mean(window_size='30s', by='datetime', closed='both').alias('30s_average'),
           pl.col('last_trade').rolling_mean(window_size='10s', by='datetime', closed='both').alias('10s_average')])
         self.smoothed_price = self.data[-1, '10s_average']
       time.sleep(.5)
 
   def export_data(self):
+    '''
+    Exports a DataFrame containing your quote data as a .pkl file saved to *./export/data*
+    '''
     filename = datetime.datetime.today().strftime('%Y_%m_%d') + '-' + self.ticker
     df = self.data.to_pandas()
     df.to_pickle('./export/data/{}.pkl'.format(filename))
 
   def upload_quote_data(self):
-    log_in_background(
-      called_from = 'upload_quote_data',
-      tags = ['user-message'], 
-      message = '{}: Uploading quote data to Google Cloud'.format(
-        datetime.datetime.now().strftime('%H:%M:%S')))
-    filename = datetime.datetime.today().strftime('%Y_%m_%d') + '-' + self.ticker
-    df = self.data.to_pandas()
-    storage_client = google.cloud.storage.Client()
-    bucket = storage_client.bucket(quote_bucket)
-    blob = bucket.blob(filename)
-    with blob.open(mode='wb') as f:
-      pickle.dump(df, f)
+    '''
+    Uploads a DataFrame to a Google Cloud Storage bucket specified in :ref:`settings.py <settings>`
+    '''
+    if hasattr(settings, 'quote_bucket'):
+      log_in_background(
+        called_from = 'upload_quote_data',
+        tags = ['user-message'], 
+        message = '{}: Uploading quote data to Google Cloud'.format(
+          datetime.datetime.now().strftime('%H:%M:%S')))
+      filename = datetime.datetime.today().strftime('%Y_%m_%d') + '-' + self.ticker
+      df = self.data.to_pandas()
+      storage_client = google.cloud.storage.Client()
+      bucket = storage_client.bucket(settings.quote_bucket)
+      blob = bucket.blob(filename)
+      with blob.open(mode='wb') as f:
+        pickle.dump(df, f)
 
   def get_pd_data(self):
+    '''
+    Returns a pandas DataFrame containing your quote data
+    '''
     return self.data.to_pandas()
```

### Comparing `wetrade-0.1.0/wetrade/user_session.py` & `wetrade-0.1.1/wetrade/user_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 from pyotp import TOTP
 from contextlib import suppress
 from playwright.sync_api import sync_playwright
 from authlib.integrations.requests_client import OAuth1Session
 from wetrade.utils import log_in_background, parse_response_data
 try: 
   import settings
-  from settings import config as default_config
 except ModuleNotFoundError:
   import wetrade.project_template.settings as settings
-  from wetrade.project_template.settings import config as default_config
 
 
-def get_text_code(authorize_url, config=default_config):
+def get_text_code(authorize_url, config={}):
+  config = settings.config if config == {} else config
   headless_login = settings.headless_login if hasattr(settings, 'headless_login') else True
   if settings.login_method == 'manual':
     print('login_url', authorize_url)
     return input('login through url and enter code:')
   else:
     if settings.use_2fa == True:
       totp = TOTP(config['totp_secret'])
@@ -53,15 +52,16 @@
         log_in_background(
           called_from = 'get_text_code',
           tags = ['user-message'], 
           message = time.strftime('%H:%M:%S', time.localtime()) + ': Login failed',
           e = e)
         return
 
-def new_session(config=default_config):
+def new_session(config={}):
+  config = settings.config if config == {} else config
   client = OAuth1Session(
     client_id = config['client_key'], 
     client_secret = config['client_secret'],
     redirect_uri = 'oob')
   request_token = client.fetch_request_token(
     url = 'https://api.etrade.com/oauth/request_token',
     params = {'format': 'json'})
@@ -77,17 +77,17 @@
       called_from = 'new_session',
       tags = ['user-message'], 
       message = time.strftime('%H:%M:%S', time.localtime()) + ': Error getting access token, retrying login',
       e = e)
     return new_session(config)
   
 class UserSession:
-  def __init__(self, config=default_config):
-    self.config = config
-    self.session = new_session(config)
+  def __init__(self, config={}):
+    self.config = settings.config if config == {} else config
+    self.session = new_session(self.config)
     self.logged_in = True
     
   def login(self):
     self.logged_in = False
     try:
       self.session = new_session(self.config)
       self.logged_in = True
@@ -182,8 +182,12 @@
       return r
     else:
       log_in_background(
         called_from = 'UserSession.handle_request',
         message = time.strftime('%H:%M:%S', time.localtime()) + ': Waiting for login',
         tags = ['user-message'])
       time.sleep(3)
-      return self.handle_request(http_method, args, kwargs)
+      return self.handle_request(http_method, args, kwargs)
+
+class SimpleUserSession(UserSession):
+  def handle_request(self, http_method, args, kwargs):
+    return self.session.request(http_method, *args, **kwargs, timeout=30)
```

### Comparing `wetrade-0.1.0/wetrade/utils.py` & `wetrade-0.1.1/wetrade/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,39 +18,41 @@
   try:
     return r.json()
   except: # r.status_code == 204 (no content) and other non-parsable requests 
     return str(r.content)
   
 def log_in_background(called_from, r=None, url='', tags=[], account_key='', symbol='', message='', e=None):
   start_thread(pretty_print, args=[called_from, r, url, tags, account_key, symbol, message, e])
-  if settings.enable_cloud_logging == True:
+  if hasattr(settings, 'enable_cloud_logging') and settings.enable_cloud_logging == True:
     start_thread(log, args=[called_from, r, url, tags, account_key, symbol, message, e])
 
 def pretty_print(called_from, r=None, url='', tags=[], account_key='', symbol='', message='', e=None):
   if message != '':
     print(message)
   if e:
     print('e', e)
     # traceback.print_exception(type(e), e, e.__traceback__)
   if r != None:
     response = parse_response_data(r)
+    # print('RESPONSE: ')
+    # pprint.pprint(response)
     if 'Error' in response:
       response_tags = ['response', 'error']
       pprint.pprint({
         'called_from': called_from,
         'tags': [*tags, *response_tags],
         'account_key': account_key,
         'config': settings.config_id,
         'symbol': symbol,
         'url': url,
         'status_code': r.status_code, 
         'response': response})
 
 def setup_logging():
-  if settings.enable_cloud_logging == True:
+  if hasattr(settings, 'enable_cloud_logging') and settings.enable_cloud_logging == True:
     client = google.cloud.logging.Client()
     client.setup_logging()
 
 def log(called_from, r=None, url='', tags=[], account_key='', symbol='', message='', e=None):
   if r != None:
     response = parse_response_data(r)
     log_level = 30 if 'Error' in response else 20
@@ -81,15 +83,16 @@
     logging.error({ 
       'called_from': called_from,
       'config': settings.config_id,
       'message': str(e),
       'tb_info': tb_str})
     
 # This doesn't really belong here but E-trade doesn't have market hours endpoint
-def check_market_hours(day_str=time.strftime('%Y-%m-%d', time.localtime())):
+def check_market_hours(day_str=''):
+  day_str = time.strftime('%Y-%m-%d', time.localtime()) if day_str == '' else day_str
   key = settings.hours_key if hasattr(settings, 'hours_key') else 'PKNL4NZJEHKGDPLL8CVY'
   secret = settings.hours_secret if hasattr(settings, 'hours_secret') else 'sxMOohHeLG6DODKv0tu237flYuwVaM0rvoea0M2F'
   params = {'start': day_str, 'end': day_str}
   headers = {'APCA-API-KEY-ID': key, 'APCA-API-SECRET-KEY': secret}
   r = requests.get('https://paper-api.alpaca.markets/v2/calendar', params=params, headers=headers)
   results = parse_response_data(r)
   if results == []:
```

### Comparing `wetrade-0.1.0/wetrade.egg-info/PKG-INFO` & `wetrade-0.1.1/wetrade.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wetrade
-Version: 0.1.0
+Version: 0.1.1
 Summary: An E-Trade python library built for active stock trading
 Author: Mason Krause
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: authlib
 Requires-Dist: playwright
 Requires-Dist: urllib3==1.26.16
@@ -19,16 +19,16 @@
 ``wetrade``: An E-Trade Python library built for automated stock trading 
 =========================================================================
 
 ``wetrade`` overview
 --------------------
 
 ``wetrade`` is an unofficial `E-Trade API <https://developer.etrade.com/home/>`__ 
-library originally built as part of a headless trading system. It provides a lot 
-of useful built-in functionality, and was designed to be flexible and extensible
+library initially created for use in headless trading systems. It provides a lot 
+of helpful built-in functionality, and was designed to be flexible and extensible
 and to accommodate a wide variety of stock trading needs.
 
 Features include:
 
 * Automated login and authentication supporting 2FA
 * Easy setup and configuration
 * Quotes, account info, and custom ordering
@@ -53,30 +53,32 @@
 `the subscription center <https://us.etrade.com/etx/pxy/my-profile/subscription-center/>`__
 so that you don't receive delayed quotes. 
 
 Install ``wetrade``:
 
 It's a good idea to create a new virtual environment for a new Python project
 
-.. code-block:: console
+.. code-block:: shell
 
   # create venv
   python3 -m venv venv
   # enter venv
   source venv/bin/activate
 
-We can then install ``wetrade`` into our venv
+We can then install ``wetrade`` into our venv. For automatic login, we'll also
+need to install our browser.
 
-.. code-block:: console
+.. code-block:: shell
 
   pip install wetrade
+  playwright install firefox
 
 Next, you'll get going in no time using our automated new project script!
 
-.. code-block:: console
+.. code-block:: shell
 
   python -m wetrade new-project
 
 You'll now see a handful of files in your project directory including a *settings.py*
 file where you'll enter your user and API info and have the option to configure various
 ``wetrade`` settings. In this file, you'll enter your username, password, client_key, 
 and client_secret so ``wetrade`` can log into your account.
@@ -93,37 +95,66 @@
   from wetrade.account import Account
   from wetrade.quote import Quote
   from wetrade.order import LimitOrder
   from wetrade.utils import setup_logging
 
 
   def main():
+    # Setup logging (optional) and APIClient
     setup_logging()
     client = APIClient()
 
+    # Check out your account
     account = Account(client=client)
     print('My Account Key: ', account.account_key)
     print('My Balance: ', account.check_balance())
 
-    quote = Quote(client=client, symbol='AAPL')
-    print('Last Quote Price: ', quote.get_last_price())
-
-
-  if __name__ == '__main__':
-    main()
+    # Get a stock quote
+    quote = Quote(client=client, symbol='IBM')
+    print(f'Last {quote.symbol} Quote Price: ', quote.get_last_price())
+
+    # Place some orders and stuff
+    order1 = LimitOrder(
+        client = client,
+        account_key = account.account_key,
+        symbol = 'NVDA',
+        action = 'BUY',
+        quantity = 1,
+        price = 50.00)
+    order1.place_order()
+    order1.run_when_status(
+        'CANCELLED', 
+        func = print, 
+        func_args = ['Test message'])
+    
+    order2 = LimitOrder(
+        client = client,
+        account_key = account.account_key,
+        symbol = 'NFLX',
+        action = 'BUY',
+        quantity = 1,
+        price = 50.00)
+    order2.place_order()
+    order2.run_when_status(
+        'CANCELLED',
+        order1.cancel_order)
+    
+    order2.cancel_order()
 
 
 Other info
 -------------
 
-``wetrade`` was initially designed to run headlessly and has built-in handling 
-for most expected brokerage, server, and API errors. Our goal is to consistently
-add new functionality to support additional use cases. If you have any comments or 
-suggestions for new features, don't hesitate to create an issue or reach out to 
-`wetrade.inbox@gmail.com <mailto:wetrade.inbox@gmail.com>`__.
+``wetrade`` was initially designed to run headlessly and has built-in handling for 
+most expected brokerage, server, and API errors. This and the majority of other 
+``wetrade`` functionality is entirely optional to use, and our modular structure 
+allows you to utilize as much or as little of the library as you'd like. Our goal 
+is to consistently add new functionality to support additional use cases. If you 
+have any comments or suggestions for new features, don't hesitate to create an 
+issue or reach out to: `wetrade.inbox@gmail.com <mailto:wetrade.inbox@gmail.com>`__.
 
 
 **Disclaimer:** *wetrade is an unofficial API library and comes with no warranty
 of any kind. It is in no way endorsed by or affiliated with E*TRADE Financial 
 or any associated organization. Make sure to read and understand the terms of 
 service of the underlying API before using this package. This authors accept 
 no responsibility for any damage that might stem from use of this package.
```

### Comparing `wetrade-0.1.0/wetrade.egg-info/SOURCES.txt` & `wetrade-0.1.1/wetrade.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -33,10 +33,13 @@
 wetrade/order/lookup_msg.py
 wetrade/project_template/Dockerfile
 wetrade/project_template/__init__.py
 wetrade/project_template/main.py
 wetrade/project_template/new_project.py
 wetrade/project_template/requirements.txt
 wetrade/project_template/settings.py
+wetrade/project_template/__pycache__/__init__.cpython-311.pyc
+wetrade/project_template/__pycache__/settings.cpython-311.pyc
 wetrade/quote/__init__.py
 wetrade/quote/data_frame_quote.py
+wetrade/quote/multi_quote.py
 wetrade/quote/quote.py
```

