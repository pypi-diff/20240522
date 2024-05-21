# Comparing `tmp/datakart-1.6.6.tar.gz` & `tmp/datakart-1.6.7.tar.gz`

## Comparing `datakart-1.6.6.tar` & `datakart-1.6.7.tar`

### file list

```diff
@@ -1,16 +1,20 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 datakart-1.6.6/requirements.txt
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 datakart-1.6.6/.vscode/settings.json
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 datakart-1.6.6/src/datakart/__init__.py
--rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 datakart-1.6.6/src/datakart/core/datagokr.py
--rw-r--r--   0        0        0    13624 2020-02-02 00:00:00.000000 datakart-1.6.6/src/datakart/core/ecos.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 datakart-1.6.6/src/datakart/core/jusogokr.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 datakart-1.6.6/src/datakart/core/kakao.py
--rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 datakart-1.6.6/src/datakart/core/naver.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 datakart-1.6.6/src/datakart/core/naver_ad.py
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 datakart-1.6.6/src/datakart/core/sgis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datakart-1.6.6/tests/__init__.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 datakart-1.6.6/.gitignore
--rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 datakart-1.6.6/LICENSE
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 datakart-1.6.6/README.md
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 datakart-1.6.6/pyproject.toml
--rw-r--r--   0        0        0    13864 2020-02-02 00:00:00.000000 datakart-1.6.6/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 datakart-1.6.7/requirements.txt
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 datakart-1.6.7/.vscode/settings.json
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/__init__.py
+-rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/core/datagokr.py
+-rw-r--r--   0        0        0    13624 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/core/ecos.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/core/jusogokr.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/core/kakao.py
+-rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/core/naver.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/core/naver_ad.py
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/core/sgis.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/core/assets/_converter.py
+-rw-r--r--   0        0        0    21232 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/core/assets/na_biztp.json
+-rw-r--r--   0        0        0     9483 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/core/assets/na_biztp.tsv
+-rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 datakart-1.6.7/src/datakart/core/assets/na_event.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datakart-1.6.7/tests/__init__.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 datakart-1.6.7/.gitignore
+-rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 datakart-1.6.7/LICENSE
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 datakart-1.6.7/README.md
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 datakart-1.6.7/pyproject.toml
+-rw-r--r--   0        0        0    13864 2020-02-02 00:00:00.000000 datakart-1.6.7/PKG-INFO
```

### Comparing `datakart-1.6.6/src/datakart/core/datagokr.py` & `datakart-1.6.7/src/datakart/core/datagokr.py`

 * *Files identical despite different names*

### Comparing `datakart-1.6.6/src/datakart/core/ecos.py` & `datakart-1.6.7/src/datakart/core/ecos.py`

 * *Files identical despite different names*

### Comparing `datakart-1.6.6/src/datakart/core/jusogokr.py` & `datakart-1.6.7/src/datakart/core/jusogokr.py`

 * *Files identical despite different names*

### Comparing `datakart-1.6.6/src/datakart/core/kakao.py` & `datakart-1.6.7/src/datakart/core/kakao.py`

 * *Files identical despite different names*

### Comparing `datakart-1.6.6/src/datakart/core/naver.py` & `datakart-1.6.7/src/datakart/core/naver.py`

 * *Files identical despite different names*

### Comparing `datakart-1.6.6/src/datakart/core/sgis.py` & `datakart-1.6.7/src/datakart/core/sgis.py`

 * *Files identical despite different names*

### Comparing `datakart-1.6.6/.gitignore` & `datakart-1.6.7/.gitignore`

 * *Files identical despite different names*

### Comparing `datakart-1.6.6/LICENSE` & `datakart-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `datakart-1.6.6/pyproject.toml` & `datakart-1.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "datakart"
-version = "1.6.6"
+version = "1.6.7"
 authors = [
   { name="HYUNIL MOON", email="hyunil.moon@gmail.com" },
 ]
 description = "A small data kart package"
 readme = "README.md"
 keywords = ["datakart", "data", "kart", "ECOS", "SGIS", "NAVER", "Kakao", "K-data", "ecos.bok.or.kr", "data.go.kr", "kostat.go.kr", "juso.go.kr"]
 requires-python = ">=3.7"
```

### Comparing `datakart-1.6.6/PKG-INFO` & `datakart-1.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: datakart
-Version: 1.6.6
+Version: 1.6.7
 Summary: A small data kart package
 Project-URL: Homepage, https://github.com/himoon/datakart
 Project-URL: Issues, https://github.com/himoon/datakart/issues
 Author-email: HYUNIL MOON <hyunil.moon@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

