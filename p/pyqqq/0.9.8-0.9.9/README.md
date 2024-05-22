# Comparing `tmp/pyqqq-0.9.8.tar.gz` & `tmp/pyqqq-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.9.8.tar", max compression
+gzip compressed data, was "pyqqq-0.9.9.tar", max compression
```

## Comparing `pyqqq-0.9.8.tar` & `pyqqq-0.9.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.9.8/README.md
--rw-r--r--   0        0        0      773 2024-05-17 04:47:12.953268 pyqqq-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     1606 2024-04-30 07:51:35.706752 pyqqq-0.9.8/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.9.8/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.9.8/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    43409 2024-05-07 06:54:47.220204 pyqqq-0.9.8/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.9.8/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    24876 2024-05-17 02:28:30.291139 pyqqq-0.9.8/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.9.8/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.9.8/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   187522 2024-05-07 09:02:33.261786 pyqqq-0.9.8/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5356 2024-04-23 09:05:13.260008 pyqqq-0.9.8/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.9.8/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    24832 2024-05-17 02:31:00.627918 pyqqq-0.9.8/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.9.8/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.9.8/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.9.8/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     5484 2024-05-16 01:05:45.085685 pyqqq-0.9.8/pyqqq/data/daily.py
--rw-r--r--   0        0        0     9684 2024-05-03 09:30:10.903300 pyqqq-0.9.8/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     9628 2024-05-03 08:51:32.698077 pyqqq-0.9.8/pyqqq/data/minutes.py
--rw-r--r--   0        0        0     1521 2024-05-03 08:51:15.982807 pyqqq-0.9.8/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     4136 2024-05-03 08:53:53.080239 pyqqq-0.9.8/pyqqq/data/ticks.py
--rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.9.8/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.9.8/pyqqq/executors/__init__.py
--rw-r--r--   0        0        0    38035 2024-04-16 05:04:16.530450 pyqqq-0.9.8/pyqqq/executors/hook.py
--rw-r--r--   0        0        0        0 2024-04-15 09:10:29.432687 pyqqq-0.9.8/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0      519 2024-05-03 08:48:33.699191 pyqqq-0.9.8/pyqqq/utils/api_client.py
--rw-r--r--   0        0        0      941 2024-04-30 08:35:54.600146 pyqqq-0.9.8/pyqqq/utils/array.py
--rw-r--r--   0        0        0     3229 2024-04-30 08:36:37.055899 pyqqq-0.9.8/pyqqq/utils/compute.py
--rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.9.8/pyqqq/utils/display.py
--rw-r--r--   0        0        0     3962 2024-04-23 09:09:34.322415 pyqqq-0.9.8/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     2641 2024-04-30 08:36:57.232261 pyqqq-0.9.8/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     2233 2024-04-30 07:41:29.806969 pyqqq-0.9.8/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.9.8/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0    10571 2024-04-16 02:24:46.823810 pyqqq-0.9.8/pyqqq/utils/mock_api.py
--rw-r--r--   0        0        0     2065 2024-04-30 07:36:13.157361 pyqqq-0.9.8/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1553 1970-01-01 00:00:00.000000 pyqqq-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.9.9/README.md
+-rw-r--r--   0        0        0      773 2024-05-20 01:40:35.837345 pyqqq-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     1606 2024-04-30 07:51:35.706752 pyqqq-0.9.9/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.9.9/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.9.9/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    43409 2024-05-07 06:54:47.220204 pyqqq-0.9.9/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.9.9/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    24876 2024-05-17 02:28:30.291139 pyqqq-0.9.9/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.9.9/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.9.9/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   187522 2024-05-07 09:02:33.261786 pyqqq-0.9.9/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5356 2024-04-23 09:05:13.260008 pyqqq-0.9.9/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.9.9/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    24832 2024-05-17 02:31:00.627918 pyqqq-0.9.9/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.9.9/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.9.9/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.9.9/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     5484 2024-05-16 01:05:45.085685 pyqqq-0.9.9/pyqqq/data/daily.py
+-rw-r--r--   0        0        0    11727 2024-05-17 10:08:43.215074 pyqqq-0.9.9/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     9628 2024-05-03 08:51:32.698077 pyqqq-0.9.9/pyqqq/data/minutes.py
+-rw-r--r--   0        0        0     1521 2024-05-03 08:51:15.982807 pyqqq-0.9.9/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     4136 2024-05-03 08:53:53.080239 pyqqq-0.9.9/pyqqq/data/ticks.py
+-rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.9.9/pyqqq/datatypes.py
+-rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.9.9/pyqqq/executors/__init__.py
+-rw-r--r--   0        0        0    38035 2024-04-16 05:04:16.530450 pyqqq-0.9.9/pyqqq/executors/hook.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:10:29.432687 pyqqq-0.9.9/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0      519 2024-05-03 08:48:33.699191 pyqqq-0.9.9/pyqqq/utils/api_client.py
+-rw-r--r--   0        0        0      941 2024-04-30 08:35:54.600146 pyqqq-0.9.9/pyqqq/utils/array.py
+-rw-r--r--   0        0        0     3229 2024-04-30 08:36:37.055899 pyqqq-0.9.9/pyqqq/utils/compute.py
+-rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.9.9/pyqqq/utils/display.py
+-rw-r--r--   0        0        0     4231 2024-05-20 01:38:26.885972 pyqqq-0.9.9/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     2641 2024-04-30 08:36:57.232261 pyqqq-0.9.9/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     2233 2024-04-30 07:41:29.806969 pyqqq-0.9.9/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.9.9/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0    10571 2024-04-16 02:24:46.823810 pyqqq-0.9.9/pyqqq/utils/mock_api.py
+-rw-r--r--   0        0        0     2065 2024-04-30 07:36:13.157361 pyqqq-0.9.9/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1553 1970-01-01 00:00:00.000000 pyqqq-0.9.9/PKG-INFO
```

### Comparing `pyqqq-0.9.8/README.md` & `pyqqq-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyproject.toml` & `pyqqq-0.9.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.9.8"
+version = "0.9.9"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
```

### Comparing `pyqqq-0.9.8/pyqqq/__init__.py` & `pyqqq-0.9.9/pyqqq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.9.9/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.9.9/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.9.9/pyqqq/brokerage/ebest/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.9.9/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.9.9/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.9.9/pyqqq/brokerage/kis/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.9.9/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.9.9/pyqqq/brokerage/kis/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.9.9/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/data/daily.py` & `pyqqq-0.9.9/pyqqq/data/daily.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/data/domestic.py` & `pyqqq-0.9.9/pyqqq/data/domestic.py`

 * *Files 16% similar despite different names*

```diff
@@ -98,14 +98,72 @@
 
         df = pd.DataFrame(r.json())
         if not df.empty:
             df.set_index("code", inplace=True)
         return df
 
 
+def get_tickers(date: dtm.date = None, market: str = None):
+    """
+    주어진 날짜와 시장에 따른 주식 종목 코드와 관련 정보를 조회합니다.
+
+    이 함수는 지정된 날짜(기본값은 오늘)와 선택적 시장('KOSPI', 'KOSDAQ')에 대한 주식 종목 코드와 추가 정보를 API를 통해 요청합니다.
+    반환된 정보는 pandas DataFrame 형태로 제공되며, 데이터가 없는 경우 빈 DataFrame을 반환합니다. DataFrame은 'code'를 인덱스로 사용합니다.
+
+    Args:
+        date (Optional[dtm.date]): 조회할 날짜. 기본값은 현재 날짜입니다.
+        market (Optional[str]): 조회할 시장. 'KOSPI' 또는 'KOSDAQ' 중 선택할 수 있습니다.
+
+    Returns:
+        pd.DataFrame: 주식 종목 코드와 관련 정보를 포함하는 DataFrame. 'code' 컬럼은 인덱스로 설정됩니다.
+
+    Raises:
+        AssertionError: 잘못된 시장 이름이 입력된 경우 오류를 발생시킵니다.
+        HTTPError: API 요청이 실패했을 때 발생.
+
+    Examples:
+        >>> tickers = get_tickers(dtm.date(2023, 4, 1), 'KOSDAQ')
+        >>> print(tickers)
+               market    name
+        code
+        000020  KOSPI    동화약품
+        000040  KOSPI   KR모터스
+        000050  KOSPI      경방
+        000070  KOSPI   삼양홀딩스
+        000075  KOSPI  삼양홀딩스우
+    """
+    if market:
+        assert market in [
+            "KOSPI",
+            "KOSDAQ",
+        ], "market은 'KOSPI' 또는 'KOSDAQ'이어야 합니다."
+
+    if date is None:
+        date = dtm.date.today()
+
+    url = f"{c.PYQQQ_API_URL}/domestic-stock/tickers/{date.strftime('%Y%m%d')}"
+    params = {}
+    if market:
+        params["market"] = market
+
+    r = send_request("GET", url, params=params)
+    raise_for_status(r)
+
+    data = r.json()
+    rows = data["rows"]
+    cols = data["cols"]
+
+    if len(rows) == 0:
+        return pd.DataFrame()
+
+    df = pd.DataFrame(rows, columns=cols)
+    df.set_index("code", inplace=True)
+    return df
+
+
 def get_ticker_info(code: str) -> Optional[pd.DataFrame]:
     """
     종목의 기본정보를 조회합니다.
 
     Args:
         code (str): 조회할 종목의 코드
```

### Comparing `pyqqq-0.9.8/pyqqq/data/minutes.py` & `pyqqq-0.9.9/pyqqq/data/minutes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/data/realtime.py` & `pyqqq-0.9.9/pyqqq/data/realtime.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/data/ticks.py` & `pyqqq-0.9.9/pyqqq/data/ticks.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/datatypes.py` & `pyqqq-0.9.9/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/executors/hook.py` & `pyqqq-0.9.9/pyqqq/executors/hook.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/utils/api_client.py` & `pyqqq-0.9.9/pyqqq/utils/api_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/utils/array.py` & `pyqqq-0.9.9/pyqqq/utils/array.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/utils/compute.py` & `pyqqq-0.9.9/pyqqq/utils/compute.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/utils/display.py` & `pyqqq-0.9.9/pyqqq/utils/display.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/utils/kvstore.py` & `pyqqq-0.9.9/pyqqq/utils/kvstore.py`

 * *Files 7% similar despite different names*

```diff
@@ -132,14 +132,22 @@
         r = self._send_request("GET", url, params={"contextName": self.name})
         r.raise_for_status()
 
         data = r.json()
 
         return data if data else []
 
+    def clear(self):
+        """
+        KV store 에 저장된 모든 key-value 를 삭제한다.
+        """
+        url = f"{c.PYQQQ_API_URL}/kvstore/clear"
+        r = self._send_request("DELETE", url, json={"contextName": self.name})
+        r.raise_for_status()
+
     @retry(requests.HTTPError)
     def _send_request(self, method: str, url: str, **kwargs):
         api_key = get_api_key()
         if not api_key:
             raise ValueError("API key is not set")
 
         return requests.request(
```

### Comparing `pyqqq-0.9.8/pyqqq/utils/limiter.py` & `pyqqq-0.9.9/pyqqq/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/utils/logger.py` & `pyqqq-0.9.9/pyqqq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/utils/market_schedule.py` & `pyqqq-0.9.9/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/utils/mock_api.py` & `pyqqq-0.9.9/pyqqq/utils/mock_api.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/pyqqq/utils/retry.py` & `pyqqq-0.9.9/pyqqq/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.8/PKG-INFO` & `pyqqq-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.9.8
+Version: 0.9.9
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

