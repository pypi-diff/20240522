# Comparing `tmp/datakart-1.6.7.tar.gz` & `tmp/datakart-1.6.8.tar.gz`

## Comparing `datakart-1.6.7.tar` & `datakart-1.6.8.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 datakart-1.6.7/requirements.txt
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 datakart-1.6.7/.vscode/settings.json
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/__init__.py
--rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/core/datagokr.py
--rw-r--r--   0        0        0    13624 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/core/ecos.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/core/jusogokr.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/core/kakao.py
--rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/core/naver.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/core/naver_ad.py
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/core/sgis.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/core/assets/_converter.py
--rw-r--r--   0        0        0    21232 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/core/assets/na_biztp.json
--rw-r--r--   0        0        0     9483 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/core/assets/na_biztp.tsv
--rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/core/assets/na_event.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datakart-1.6.7/tests/__init__.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 datakart-1.6.7/.gitignore
--rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 datakart-1.6.7/LICENSE
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 datakart-1.6.7/README.md
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 datakart-1.6.7/pyproject.toml
--rw-r--r--   0        0        0    13864 2020-02-02 00:00:00.000000 datakart-1.6.7/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 datakart-1.6.8/requirements.txt
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 datakart-1.6.8/.vscode/settings.json
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 datakart-1.6.8/src/datakart/__init__.py
+-rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 datakart-1.6.8/src/datakart/core/datagokr.py
+-rw-r--r--   0        0        0    13624 2020-02-02 00:00:00.000000 datakart-1.6.8/src/datakart/core/ecos.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 datakart-1.6.8/src/datakart/core/jusogokr.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 datakart-1.6.8/src/datakart/core/kakao.py
+-rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 datakart-1.6.8/src/datakart/core/naver.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 datakart-1.6.8/src/datakart/core/naver_ad.py
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 datakart-1.6.8/src/datakart/core/sgis.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 datakart-1.6.8/src/datakart/core/assets/_converter.py
+-rw-r--r--   0        0        0    21232 2020-02-02 00:00:00.000000 datakart-1.6.8/src/datakart/core/assets/na_biztp.json
+-rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 datakart-1.6.8/src/datakart/core/assets/na_event.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datakart-1.6.8/tests/__init__.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 datakart-1.6.8/.gitignore
+-rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 datakart-1.6.8/LICENSE
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 datakart-1.6.8/README.md
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 datakart-1.6.8/pyproject.toml
+-rw-r--r--   0        0        0    13864 2020-02-02 00:00:00.000000 datakart-1.6.8/PKG-INFO
```

### Comparing `datakart-1.6.7/src/datakart/core/datagokr.py` & `datakart-1.6.8/src/datakart/core/datagokr.py`

 * *Files identical despite different names*

### Comparing `datakart-1.6.7/src/datakart/core/ecos.py` & `datakart-1.6.8/src/datakart/core/ecos.py`

 * *Files identical despite different names*

### Comparing `datakart-1.6.7/src/datakart/core/jusogokr.py` & `datakart-1.6.8/src/datakart/core/jusogokr.py`

 * *Files identical despite different names*

### Comparing `datakart-1.6.7/src/datakart/core/kakao.py` & `datakart-1.6.8/src/datakart/core/kakao.py`

 * *Files identical despite different names*

### Comparing `datakart-1.6.7/src/datakart/core/naver.py` & `datakart-1.6.8/src/datakart/core/naver.py`

 * *Files identical despite different names*

### Comparing `datakart-1.6.7/src/datakart/core/naver_ad.py` & `datakart-1.6.8/src/datakart/core/naver_ad.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,31 +5,14 @@
 import hmac
 import time
 from typing import Dict, List
 
 import requests
 
 
-def biztp_cd() -> List[Dict]:
-    import json
-    import pathlib
-
-    with open(pathlib.Path(__file__).parent / "assets" / "na_biztp.json") as fp:
-        return json.load(fp)
-
-
-def event_cd() -> List[Dict]:
-    # https://gist.github.com/naver-searchad/235202ffb08f9433b6f7cb10e45875f7#file-seasonal_event_code-md
-    import json
-    import pathlib
-
-    with open(pathlib.Path(__file__).parent / "assets" / "na_event.json") as fp:
-        return json.load(fp)
-
-
 class NaverAd:
     """NAVER Search Ad API"""
 
     def __init__(self, api_key: str, api_sec: str, cust_id: str) -> None:
         self.api_key: str = api_key
         self.api_sec: str = api_sec
         self.cust_id: str = cust_id
@@ -70,7 +53,24 @@
             **({"hintKeywords": keywords} if keywords else {}),
             **({"event": event} if event else {}),
             **({"month": month} if month else {}),
         }
         resp = requests.get(self.host_url + url, headers=headers, params=params)
         resp.raise_for_status()
         return resp.json()
+
+    @staticmethod
+    def biztp_cd() -> List[Dict]:
+        import json
+        import pathlib
+
+        with open(pathlib.Path(__file__).parent / "assets" / "na_biztp.json") as fp:
+            return json.load(fp)
+
+    @staticmethod
+    def event_cd() -> List[Dict]:
+        # https://gist.github.com/naver-searchad/235202ffb08f9433b6f7cb10e45875f7#file-seasonal_event_code-md
+        import json
+        import pathlib
+
+        with open(pathlib.Path(__file__).parent / "assets" / "na_event.json") as fp:
+            return json.load(fp)
```

### Comparing `datakart-1.6.7/src/datakart/core/sgis.py` & `datakart-1.6.8/src/datakart/core/sgis.py`

 * *Files identical despite different names*

### Comparing `datakart-1.6.7/src/datakart/core/assets/na_biztp.json` & `datakart-1.6.8/src/datakart/core/assets/na_biztp.json`

 * *Files identical despite different names*

### Comparing `datakart-1.6.7/src/datakart/core/assets/na_event.json` & `datakart-1.6.8/src/datakart/core/assets/na_event.json`

 * *Files identical despite different names*

### Comparing `datakart-1.6.7/.gitignore` & `datakart-1.6.8/.gitignore`

 * *Files identical despite different names*

### Comparing `datakart-1.6.7/LICENSE` & `datakart-1.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `datakart-1.6.7/pyproject.toml` & `datakart-1.6.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "datakart"
-version = "1.6.7"
+version = "1.6.8"
 authors = [
   { name="HYUNIL MOON", email="hyunil.moon@gmail.com" },
 ]
 description = "A small data kart package"
 readme = "README.md"
 keywords = ["datakart", "data", "kart", "ECOS", "SGIS", "NAVER", "Kakao", "K-data", "ecos.bok.or.kr", "data.go.kr", "kostat.go.kr", "juso.go.kr"]
 requires-python = ">=3.7"
```

### Comparing `datakart-1.6.7/PKG-INFO` & `datakart-1.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: datakart
-Version: 1.6.7
+Version: 1.6.8
 Summary: A small data kart package
 Project-URL: Homepage, https://github.com/himoon/datakart
 Project-URL: Issues, https://github.com/himoon/datakart/issues
 Author-email: HYUNIL MOON <hyunil.moon@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

