# Comparing `tmp/fennel_invest_api-1.0.5.tar.gz` & `tmp/fennel_invest_api-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fennel_invest_api-1.0.5.tar", last modified: Tue May 21 13:56:53 2024, max compression
+gzip compressed data, was "fennel_invest_api-1.0.6.tar", last modified: Wed May 22 18:49:55 2024, max compression
```

## Comparing `fennel_invest_api-1.0.5.tar` & `fennel_invest_api-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:56:53.218773 fennel_invest_api-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 13:56:49.000000 fennel_invest_api-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-21 13:56:53.218773 fennel_invest_api-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-21 13:56:49.000000 fennel_invest_api-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:56:53.214773 fennel_invest_api-1.0.5/fennel_invest_api/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-21 13:56:49.000000 fennel_invest_api-1.0.5/fennel_invest_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-05-21 13:56:49.000000 fennel_invest_api-1.0.5/fennel_invest_api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-21 13:56:49.000000 fennel_invest_api-1.0.5/fennel_invest_api/fennel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:56:53.218773 fennel_invest_api-1.0.5/fennel_invest_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-21 13:56:53.000000 fennel_invest_api-1.0.5/fennel_invest_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-21 13:56:53.000000 fennel_invest_api-1.0.5/fennel_invest_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:56:53.000000 fennel_invest_api-1.0.5/fennel_invest_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 13:56:53.000000 fennel_invest_api-1.0.5/fennel_invest_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 13:56:53.000000 fennel_invest_api-1.0.5/fennel_invest_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:56:53.218773 fennel_invest_api-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-21 13:56:49.000000 fennel_invest_api-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:49:55.905927 fennel_invest_api-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-22 18:49:51.000000 fennel_invest_api-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-22 18:49:55.905927 fennel_invest_api-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-22 18:49:51.000000 fennel_invest_api-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:49:55.905927 fennel_invest_api-1.0.6/fennel_invest_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-22 18:49:51.000000 fennel_invest_api-1.0.6/fennel_invest_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-05-22 18:49:51.000000 fennel_invest_api-1.0.6/fennel_invest_api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-05-22 18:49:51.000000 fennel_invest_api-1.0.6/fennel_invest_api/fennel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:49:55.905927 fennel_invest_api-1.0.6/fennel_invest_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-22 18:49:55.000000 fennel_invest_api-1.0.6/fennel_invest_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-22 18:49:55.000000 fennel_invest_api-1.0.6/fennel_invest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 18:49:55.000000 fennel_invest_api-1.0.6/fennel_invest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 18:49:55.000000 fennel_invest_api-1.0.6/fennel_invest_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 18:49:55.000000 fennel_invest_api-1.0.6/fennel_invest_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 18:49:55.905927 fennel_invest_api-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-22 18:49:51.000000 fennel_invest_api-1.0.6/setup.py
```

### Comparing `fennel_invest_api-1.0.5/LICENSE` & `fennel_invest_api-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fennel_invest_api-1.0.5/PKG-INFO` & `fennel_invest_api-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fennel_invest_api
-Version: 1.0.5
+Version: 1.0.6
 Summary: Unofficial Fennel.com Invest API written in Python Requests
 Home-page: https://github.com/NelsonDane/fennel-invest-api
 Author: Nelson Dane
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: python-dotenv
```

### Comparing `fennel_invest_api-1.0.5/README.md` & `fennel_invest_api-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fennel_invest_api-1.0.5/fennel_invest_api/endpoints.py` & `fennel_invest_api-1.0.6/fennel_invest_api/endpoints.py`

 * *Files identical despite different names*

### Comparing `fennel_invest_api-1.0.5/fennel_invest_api/fennel.py` & `fennel_invest_api-1.0.6/fennel_invest_api/fennel.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,19 +71,17 @@
         if os.path.exists(filename):
             os.remove(filename)
         self.Bearer = None
         self.Refresh = None
         self.ID_Token = None
 
     def login(self, email, wait_for_code=True, code=None):
-        # If creds exist, then see if they are valid
-        if self.Bearer is not None:
-            if self._verify_login():
-                return True
-            self._clear_credentials()
+        # If creds exist, check if they are valid/try to refresh
+        if self.Bearer is not None and self._verify_login():
+            return True
         if code is None:
             url = self.endpoints.retrieve_bearer_url()
             payload = {
                 "email": email,
                 "client_id": self.client_id,
                 "connection": "email",
                 "send": "code",
@@ -109,15 +107,14 @@
         if response.status_code != 200:
             raise Exception(f"Failed to login: {response.text}")
         response = response.json()
         self.Bearer = response["access_token"]
         self.Refresh = response["refresh_token"]
         self.ID_Token = response["id_token"]
         self.refresh_token()
-        self._save_credentials()
         self.get_account_ids()
         return True
 
     def refresh_token(self):
         url = self.endpoints.oauth_url()
         headers = self.endpoints.build_headers(accounts_host=True)
         payload = {
@@ -126,30 +123,34 @@
             "refresh_token": self.Refresh,
             "scope": "openid profile offline_access email",
         }
         response = self.session.post(url, json=payload, headers=headers)
         if response.status_code != 200:
             raise Exception(f"Failed to refresh bearer token: {response.text}")
         response = response.json()
-        self.Bearer = f"{response['access_token']}"
+        self.Bearer = response["access_token"]
         self.Refresh = response["refresh_token"]
         self.ID_Token = response["id_token"]
+        self._save_credentials()
         return response
 
     def _verify_login(self):
         # Test login by getting Account IDs
         try:
             self.get_account_ids()
             return True
         except Exception:
             try:
+                # Try to refresh token
                 self.refresh_token()
                 self.get_account_ids()
                 return True
             except Exception:
+                # Unable to refresh, clear credentials
+                self._clear_credentials()
                 return False
 
     @check_login
     def get_account_ids(self):
         query = self.endpoints.account_ids_query()
         headers = self.endpoints.build_headers(self.Bearer)
         response = self.session.post(
@@ -225,15 +226,17 @@
             raise Exception(
                 f"Market Open Request failed with status code {response.status_code}: {response.text}"
             )
         response = response.json()
         return response["data"]["securityMarketInfo"]["isOpen"]
 
     @check_login
-    def place_order(self, account_id, ticker, quantity, side, price="market", dry_run=False):
+    def place_order(
+        self, account_id, ticker, quantity, side, price="market", dry_run=False
+    ):
         if side.lower() not in ["buy", "sell"]:
             raise Exception("Side must be either 'buy' or 'sell'")
         # Check if market is open
         if not self.is_market_open():
             raise Exception("Market is closed. Cannot place order.")
         # Search for stock "isin"
         query = self.endpoints.stock_search_query(ticker)
@@ -250,15 +253,17 @@
             return search_response
         if len(search_response["data"]["searchSearch"]["searchSecurities"]) == 0:
             raise Exception(
                 f"No stock found with ticker {ticker}. Please check the app to see if it is valid."
             )
         isin = search_response["data"]["searchSearch"]["searchSecurities"][0]["isin"]
         # Place order
-        query = self.endpoints.stock_order_query(account_id, ticker, quantity, isin, side, price)
+        query = self.endpoints.stock_order_query(
+            account_id, ticker, quantity, isin, side, price
+        )
         order_response = self.session.post(
             self.endpoints.graphql, headers=headers, data=query
         )
         if order_response.status_code != 200:
             raise Exception(
                 f"Order Request failed with status code {order_response.status_code}: {order_response.text}"
             )
```

### Comparing `fennel_invest_api-1.0.5/fennel_invest_api.egg-info/PKG-INFO` & `fennel_invest_api-1.0.6/fennel_invest_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fennel_invest_api
-Version: 1.0.5
+Version: 1.0.6
 Summary: Unofficial Fennel.com Invest API written in Python Requests
 Home-page: https://github.com/NelsonDane/fennel-invest-api
 Author: Nelson Dane
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: python-dotenv
```

