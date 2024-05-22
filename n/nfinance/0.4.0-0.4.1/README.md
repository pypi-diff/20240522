# Comparing `tmp/nfinance-0.4.0-py3-none-any.whl.zip` & `tmp/nfinance-0.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,14 @@
-Zip file size: 9732 bytes, number of entries: 14
--rw-r--r--  2.0 unx      456 b- defN 24-May-20 06:06 nfinance/__init__.py
--rw-r--r--  2.0 unx     2121 b- defN 24-May-20 06:06 nfinance/financials.py
--rw-r--r--  2.0 unx     1368 b- defN 24-May-20 06:05 nfinance/nfinance.py
--rw-r--r--  2.0 unx      481 b- defN 24-May-20 06:06 nfinance/rsi.py
--rw-r--r--  2.0 unx     1727 b- defN 24-May-20 06:06 nfinance/stock_data.py
--rw-r--r--  2.0 unx     3123 b- defN 24-May-20 06:06 nfinance/stock_listing.py
--rw-r--r--  2.0 unx       45 b- defN 24-May-20 06:06 tests/__init__.py
--rw-r--r--  2.0 unx     2979 b- defN 24-May-20 06:05 tests/test_nfinance.py
--rw-r--r--  2.0 unx     1485 b- defN 24-May-20 06:07 tests/test_stock_data.py
--rw-r--r--  2.0 unx     1064 b- defN 24-May-20 06:09 nfinance-0.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3422 b- defN 24-May-20 06:09 nfinance-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-20 06:09 nfinance-0.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 24-May-20 06:09 nfinance-0.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1087 b- defN 24-May-20 06:09 nfinance-0.4.0.dist-info/RECORD
-14 files, 19465 bytes uncompressed, 7944 bytes compressed:  59.2%
+Zip file size: 7954 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      456 b- defN 24-May-22 08:23 nfinance/__init__.py
+-rw-r--r--  2.0 unx     2121 b- defN 24-May-22 08:23 nfinance/financials.py
+-rw-r--r--  2.0 unx      481 b- defN 24-May-22 08:23 nfinance/rsi.py
+-rw-r--r--  2.0 unx     1727 b- defN 24-May-22 08:23 nfinance/stock_data.py
+-rw-r--r--  2.0 unx     3621 b- defN 24-May-22 08:24 nfinance/stock_listing.py
+-rw-r--r--  2.0 unx       45 b- defN 24-May-22 08:23 tests/__init__.py
+-rw-r--r--  2.0 unx     1485 b- defN 24-May-22 08:23 tests/test_stock_data.py
+-rw-r--r--  2.0 unx     1064 b- defN 24-May-22 08:26 nfinance-0.4.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3646 b- defN 24-May-22 08:26 nfinance-0.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-22 08:26 nfinance-0.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-May-22 08:26 nfinance-0.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      931 b- defN 24-May-22 08:26 nfinance-0.4.1.dist-info/RECORD
+12 files, 15684 bytes uncompressed, 6402 bytes compressed:  59.2%
```

## zipnote {}

```diff
@@ -1,43 +1,37 @@
 Filename: nfinance/__init__.py
 Comment: 
 
 Filename: nfinance/financials.py
 Comment: 
 
-Filename: nfinance/nfinance.py
-Comment: 
-
 Filename: nfinance/rsi.py
 Comment: 
 
 Filename: nfinance/stock_data.py
 Comment: 
 
 Filename: nfinance/stock_listing.py
 Comment: 
 
 Filename: tests/__init__.py
 Comment: 
 
-Filename: tests/test_nfinance.py
-Comment: 
-
 Filename: tests/test_stock_data.py
 Comment: 
 
-Filename: nfinance-0.4.0.dist-info/LICENSE
+Filename: nfinance-0.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: nfinance-0.4.0.dist-info/METADATA
+Filename: nfinance-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: nfinance-0.4.0.dist-info/WHEEL
+Filename: nfinance-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: nfinance-0.4.0.dist-info/top_level.txt
+Filename: nfinance-0.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: nfinance-0.4.0.dist-info/RECORD
+Filename: nfinance-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nfinance/stock_listing.py

```diff
@@ -1,8 +1,8 @@
-# stock_listing.py
+
 import requests
 import pandas as pd
 from tqdm import tqdm
 
 class StockListing:
     def __init__(self, market):
         self.market = market
@@ -22,31 +22,48 @@
             ".SOX": "https://api.stock.naver.com/index/.SOX/enrollStocks?page={page}&pageSize=10",
             "etf": "https://api.stock.naver.com/etf/priceTop?page={page}&pageSize=20",
             "largeCode": "https://api.stock.naver.com/etf/priceTop?page={page}&pageSize=20&{market}"
         }
         self.url = self.base_urls.get(self.market.split('=')[0], "https://m.stock.naver.com/api/stocks/marketValue/{market}?page={page}&pageSize=20")
 
     def fetch_stocks(self):
-        page = 1
+        special_stock_list = ['.DJI', '.INX', '.SOX']
+        special_stock_pages = {'.DJI': 4, '.INX': 51, '.SOX': 4}
+
+        if self.market in special_stock_list:
+            total_pages = special_stock_pages[self.market]
+            page_size = 10
+        else:
+            response = requests.get(self.url.format(market=self.market, page=1))
+            if response.status_code != 200:
+                raise Exception(f"API request failed with status code: {response.status_code}")
+            json_data = response.json()
+            total_stocks = json_data.get('totalCount', 0)
+            total_pages = (total_stocks // 20) + 1 if total_stocks % 20 != 0 else total_stocks // 20
+            page_size = 20
+
         stocks = []
-        response = requests.get(self.url.format(market=self.market, page=page))
-        if response.status_code != 200:
-            raise Exception(f"API request failed with status code: {response.status_code}")
-        json_data = response.json()
-        total_stocks = json_data.get('totalCount', 0)
-        total_pages = (total_stocks // 20) + 1 if total_stocks % 20 != 0 else total_stocks // 20
 
-        # Use tqdm to show progress bar
         for page in tqdm(range(1, total_pages + 1), desc=f"Fetching {self.market} stocks"):
             formatted_url = self.url.format(market=self.market, page=page)
             response = requests.get(formatted_url)
             if response.status_code != 200:
                 continue  # Skip to next iteration if there's an error
             json_data = response.json()
             new_stocks = pd.json_normalize(json_data.get("stocks", []))
             if not new_stocks.empty:
                 stocks.append(new_stocks)
 
         return pd.concat(stocks, ignore_index=True) if stocks else pd.DataFrame()
 
     def __str__(self):
         return f'StockListing for {self.market}'
+
+# Example usage:
+# listing = StockListing("KOSPI")
+# stocks_df = listing.fetch_stocks()
+# print(stocks_df)
+
+# Special stocks fetching example:
+# listing = StockListing(".DJI")
+# stocks_df = listing.fetch_stocks()
+# stocks_df.to_csv('.DJI.csv', index=False)
```

## Comparing `nfinance-0.4.0.dist-info/LICENSE` & `nfinance-0.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `nfinance-0.4.0.dist-info/METADATA` & `nfinance-0.4.1.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nfinance
-Version: 0.4.0
+Version: 0.4.1
 Summary: A simple finance data fetching library for Naver Finance data.
 Home-page: https://github.com/lega001/nfinance
 Author: lega001
 Author-email: lega01077970523@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -82,14 +82,17 @@
 ```
 ## 3-3. 사용 예제
 ```python
 import nfinance
 
 df_annual = nfinance.get_annual_financial('005930')  # 예시: 삼성전자 코드
 print(df_annual)
+print("df_annual['2019/12']['매출액']", df_annual['2019/12']['매출액'])
+print("df_annual.loc['매출액']", df_annual.loc['매출액'])
+print("df_annual.loc['매출액'].tolist()", df_annual.loc['매출액'].tolist())
 ```
 
 ## 4. LICENSE
 
 MIT 라이선스를 예로 듭니다. 실제로 사용하려면 올바른 라이선스를 선택해야 합니다.
 
 ```plaintext
```

## Comparing `nfinance-0.4.0.dist-info/RECORD` & `nfinance-0.4.1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 nfinance/__init__.py,sha256=JPqPpqat_GZctMZJdnP67pfQIug2STg0KVEO8njkOmI,456
 nfinance/financials.py,sha256=STKNdzWnLx2TntMgiYNERktVNiUs70ia1DxwOX02HzY,2121
-nfinance/nfinance.py,sha256=OuzdeujEjuHSeAmmyD-gaIOCl4dve1mTpjVMYWHla0Y,1368
 nfinance/rsi.py,sha256=aNaV5DNpCdEiZeY2-RnIwTOIf7wt1G8Kafz9aMr9JdY,481
 nfinance/stock_data.py,sha256=gQ9MSVZ_QMqbQslkE-vCplw_CH2-U1skKJDr8TAq_TE,1727
-nfinance/stock_listing.py,sha256=UCnjRdCzT3KytWBukgIon0rQjZkN3InuYNqtcOKS28E,3123
+nfinance/stock_listing.py,sha256=ZqON3AlmnIgDA1frfcdA3v0cKWS9icIpz8Z_mx5pVM0,3621
 tests/__init__.py,sha256=PG_aDJEGJwy2Ls4tNVDssNXIARlEqzKc4hB7FAEE31g,45
-tests/test_nfinance.py,sha256=d7-dD3BRqqhv-r9Cd1qykhhhiZryp0DCqLWyIG1pKR0,2979
 tests/test_stock_data.py,sha256=nobDuOLwlap9sPzyyIFKb05um2mbVrYOAlzeRqjO-jE,1485
-nfinance-0.4.0.dist-info/LICENSE,sha256=W-G02SIVZT605TQhaNoPMh3yDfjDdwj91mWwo-3-mcU,1064
-nfinance-0.4.0.dist-info/METADATA,sha256=pLNlU_xqgLONMi-kZZZ8sHnQ9bhRGKqw-srCsRMfQ_c,3422
-nfinance-0.4.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nfinance-0.4.0.dist-info/top_level.txt,sha256=lFnY9sT0iM6MkEPAa3XqYKwA9dUFIA8R31RYsU1nyzg,15
-nfinance-0.4.0.dist-info/RECORD,,
+nfinance-0.4.1.dist-info/LICENSE,sha256=W-G02SIVZT605TQhaNoPMh3yDfjDdwj91mWwo-3-mcU,1064
+nfinance-0.4.1.dist-info/METADATA,sha256=pBzvVp0fN2Px1HnLef5W6H3fnCvsp90qoXbWnXV5Lgc,3646
+nfinance-0.4.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nfinance-0.4.1.dist-info/top_level.txt,sha256=lFnY9sT0iM6MkEPAa3XqYKwA9dUFIA8R31RYsU1nyzg,15
+nfinance-0.4.1.dist-info/RECORD,,
```

