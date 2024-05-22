# Comparing `tmp/bbg_fetch-1.0.5.tar.gz` & `tmp/bbg_fetch-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbg_fetch-1.0.5.tar", max compression
+gzip compressed data, was "bbg_fetch-1.0.6.tar", max compression
```

## Comparing `bbg_fetch-1.0.5.tar` & `bbg_fetch-1.0.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     8317 2024-04-13 11:32:23.712854 bbg_fetch-1.0.5/bbg_fetch.py
--rw-r--r--   0        0        0     1491 2024-04-17 06:10:14.320231 bbg_fetch-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      437 2024-04-02 20:04:59.604378 bbg_fetch-1.0.5/README.md
--rw-r--r--   0        0        0     1904 1970-01-01 00:00:00.000000 bbg_fetch-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     9058 2024-05-22 19:37:07.454142 bbg_fetch-1.0.6/bbg_fetch.py
+-rw-r--r--   0        0        0     1491 2024-05-22 19:33:26.560081 bbg_fetch-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      437 2024-04-02 20:04:59.604378 bbg_fetch-1.0.6/README.md
+-rw-r--r--   0        0        0     1904 1970-01-01 00:00:00.000000 bbg_fetch-1.0.6/PKG-INFO
```

### Comparing `bbg_fetch-1.0.5/bbg_fetch.py` & `bbg_fetch-1.0.6/bbg_fetch.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 pip install --index-url=https://bcms.bloomberg.com/pip/simple blpapi
 GFUT
 """
 
 # packages
 import re
 import warnings
+
+import numpy as np
 import pandas as pd
 from enum import Enum
 from typing import List, Optional, Tuple
 from xbbg import blp
 
 DEFAULT_START_DATE = pd.Timestamp('01Jan1959')
 
@@ -146,19 +148,32 @@
     """
     ES1 Index to ES Index
     """
     ticker_split_wo_num = re.sub('\d+', '', future).split()
     return ticker_split_wo_num[0]
 
 
+def fetch_futures_contract_table(ticker: str = "ESA Index",
+                                 flds: List[str] = ('px_last', 'volume', 'fut_days_expire', # 'fut_month_yr',
+                                                    'last_tradeable_dt')
+                                 ) -> pd.DataFrame:
+    contracts = blp.bds(ticker, "FUT_CHAIN")
+    tickers = contracts['security_description']
+    df = blp.bdp(tickers=tickers, flds=flds)
+    tradable_tickers = tickers[np.in1d(tickers, df.index, assume_unique=True)]
+    df = df.loc[tradable_tickers, flds]
+    return df
+
+
 class UnitTests(Enum):
     FUNDAMENTALS = 1
     FIELDS_PER_TICKER = 2
     FIELD_PER_TICKERS = 3
     ACTIVE_FUTURES = 4
+    CONTRACT_TABLE = 5
 
 
 def run_unit_test(unit_test: UnitTests):
 
     if unit_test == UnitTests.FUNDAMENTALS:
         df = fetch_fundamentals(tickers=['AAPL US Equity', 'BAC US Equity'],
                                 fields=['Security_Name', 'GICS_Sector_Name', 'CRNCY'])
@@ -181,21 +196,25 @@
         # this = blp.bds("SPY US Equity", "opt_chain", single_date_override="20191010")
         # print(this)
 
     elif unit_test == UnitTests.ACTIVE_FUTURES:
         # field_data = blp.active_futures('ESA Index', dt='1997-09-10')
         # print(field_data)
 
-        field_data = fetch_active_futures(generic_ticker='S 1 Comdty')
+        field_data = fetch_active_futures(generic_ticker='ESA Equity')
         print(field_data)
 
+    elif unit_test == UnitTests.CONTRACT_TABLE:
+        df = fetch_futures_contract_table()
+        print(df)
+
 
 if __name__ == '__main__':
 
-    unit_test = UnitTests.ACTIVE_FUTURES
+    unit_test = UnitTests.CONTRACT_TABLE
 
     is_run_all_tests = False
     if is_run_all_tests:
         for unit_test in UnitTests:
             run_unit_test(unit_test=unit_test)
     else:
         run_unit_test(unit_test=unit_test)
```

### Comparing `bbg_fetch-1.0.5/pyproject.toml` & `bbg_fetch-1.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2262 6267 5f66 6574 6368  ame = "bbg_fetch
 00000020: 220d 0a76 6572 7369 6f6e 203d 2022 312e  "..version = "1.
-00000030: 302e 3522 0d0a 6465 7363 7269 7074 696f  0.5"..descriptio
+00000030: 302e 3622 0d0a 6465 7363 7269 7074 696f  0.6"..descriptio
 00000040: 6e20 3d20 2242 6c6f 6f6d 6265 7267 2066  n = "Bloomberg f
 00000050: 6574 6368 696e 6720 616e 616c 7974 6963  etching analytic
 00000060: 7320 7772 6170 7069 6e67 2078 6262 6720  s wrapping xbbg 
 00000070: 7061 636b 6167 6522 0d0a 6c69 6365 6e73  package"..licens
 00000080: 6520 3d20 224c 4943 454e 5345 2e74 7874  e = "LICENSE.txt
 00000090: 220d 0a61 7574 686f 7273 203d 205b 2241  "..authors = ["A
 000000a0: 7274 7572 2053 6570 7020 3c61 7274 7572  rtur Sepp <artur
```

### Comparing `bbg_fetch-1.0.5/PKG-INFO` & `bbg_fetch-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbg_fetch
-Version: 1.0.5
+Version: 1.0.6
 Summary: Bloomberg fetching analytics wrapping xbbg package
 Home-page: https://github.com/ArturSepp/BloombergFetch
 License: LICENSE.txt
 Keywords: quantitative,investing,portfolio optimization,systematic strategies,volatility
 Author: Artur Sepp
 Author-email: artursepp@gmail.com
 Maintainer: Artur Sepp
```

