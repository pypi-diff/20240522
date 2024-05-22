# Comparing `tmp/oxaigen-0.0.0.3.tar.gz` & `tmp/oxaigen-0.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxaigen-0.0.0.3.tar", max compression
+gzip compressed data, was "oxaigen-0.0.0.4.tar", max compression
```

## Comparing `oxaigen-0.0.0.3.tar` & `oxaigen-0.0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      251 2024-05-21 16:40:01.974635 oxaigen-0.0.0.3/README.md
--rw-r--r--   0        0        0      112 2024-05-21 18:27:06.168091 oxaigen-0.0.0.3/oxaigen/__init__.py
--rw-r--r--   0        0        0       24 2024-05-21 17:54:21.224181 oxaigen-0.0.0.3/oxaigen/src/__init__.py
--rw-r--r--   0        0        0       23 2024-05-21 18:25:26.885319 oxaigen-0.0.0.3/oxaigen/src/asset/__init__.py
--rw-r--r--   0        0        0     6035 2024-05-22 12:36:15.141134 oxaigen-0.0.0.3/oxaigen/src/asset/asset.py
--rw-r--r--   0        0        0       25 2024-05-21 16:33:07.147095 oxaigen-0.0.0.3/oxaigen/src/authentication/__init__.py
--rw-r--r--   0        0        0     2650 2024-05-22 12:30:34.462238 oxaigen-0.0.0.3/oxaigen/src/authentication/authentication.py
--rw-r--r--   0        0        0     1348 2024-05-22 11:51:20.803630 oxaigen-0.0.0.3/oxaigen/src/config.py
--rw-r--r--   0        0        0      127 2024-05-22 11:51:09.438253 oxaigen-0.0.0.3/oxaigen/src/constant.py
--rw-r--r--   0        0        0      439 2024-05-22 12:27:20.233246 oxaigen-0.0.0.3/oxaigen/src/main.py
--rw-r--r--   0        0        0       23 2024-05-22 01:05:48.100558 oxaigen-0.0.0.3/oxaigen/src/storage/__init__.py
--rw-r--r--   0        0        0     5077 2024-05-22 12:35:12.802233 oxaigen-0.0.0.3/oxaigen/src/storage/data_storage.py
--rw-r--r--   0        0        0       24 2024-05-21 16:40:38.535727 oxaigen-0.0.0.3/oxaigen/src/util/__init__.py
--rw-r--r--   0        0        0     1996 2024-05-22 00:18:31.367628 oxaigen-0.0.0.3/oxaigen/src/util/api.py
--rw-r--r--   0        0        0      976 2024-05-22 12:33:36.476086 oxaigen-0.0.0.3/oxaigen/src/util/exception.py
--rw-r--r--   0        0        0      254 2024-05-22 00:44:20.848444 oxaigen-0.0.0.3/oxaigen/src/util/logging.py
--rw-r--r--   0        0        0     3860 2024-05-22 00:06:58.773848 oxaigen-0.0.0.3/oxaigen/src/util/token.py
--rw-r--r--   0        0        0      823 2024-05-22 12:31:01.295414 oxaigen-0.0.0.3/oxaigen/src/util/util.py
--rw-r--r--   0        0        0      826 2024-05-22 12:37:00.961368 oxaigen-0.0.0.3/pyproject.toml
--rw-r--r--   0        0        0      804 1970-01-01 00:00:00.000000 oxaigen-0.0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      251 2024-05-21 16:40:01.974635 oxaigen-0.0.0.4/README.md
+-rw-r--r--   0        0        0      112 2024-05-21 18:27:06.168091 oxaigen-0.0.0.4/oxaigen/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-21 17:54:21.224181 oxaigen-0.0.0.4/oxaigen/src/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-21 18:25:26.885319 oxaigen-0.0.0.4/oxaigen/src/asset/__init__.py
+-rw-r--r--   0        0        0     6035 2024-05-22 12:36:15.141134 oxaigen-0.0.0.4/oxaigen/src/asset/asset.py
+-rw-r--r--   0        0        0       25 2024-05-21 16:33:07.147095 oxaigen-0.0.0.4/oxaigen/src/authentication/__init__.py
+-rw-r--r--   0        0        0     2650 2024-05-22 12:30:34.462238 oxaigen-0.0.0.4/oxaigen/src/authentication/authentication.py
+-rw-r--r--   0        0        0     1348 2024-05-22 11:51:20.803630 oxaigen-0.0.0.4/oxaigen/src/config.py
+-rw-r--r--   0        0        0      127 2024-05-22 11:51:09.438253 oxaigen-0.0.0.4/oxaigen/src/constant.py
+-rw-r--r--   0        0        0      439 2024-05-22 12:27:20.233246 oxaigen-0.0.0.4/oxaigen/src/main.py
+-rw-r--r--   0        0        0       23 2024-05-22 01:05:48.100558 oxaigen-0.0.0.4/oxaigen/src/storage/__init__.py
+-rw-r--r--   0        0        0     5077 2024-05-22 12:35:12.802233 oxaigen-0.0.0.4/oxaigen/src/storage/data_storage.py
+-rw-r--r--   0        0        0       24 2024-05-21 16:40:38.535727 oxaigen-0.0.0.4/oxaigen/src/util/__init__.py
+-rw-r--r--   0        0        0     1996 2024-05-22 00:18:31.367628 oxaigen-0.0.0.4/oxaigen/src/util/api.py
+-rw-r--r--   0        0        0      976 2024-05-22 12:33:36.476086 oxaigen-0.0.0.4/oxaigen/src/util/exception.py
+-rw-r--r--   0        0        0      254 2024-05-22 00:44:20.848444 oxaigen-0.0.0.4/oxaigen/src/util/logging.py
+-rw-r--r--   0        0        0     3860 2024-05-22 00:06:58.773848 oxaigen-0.0.0.4/oxaigen/src/util/token.py
+-rw-r--r--   0        0        0      823 2024-05-22 12:31:01.295414 oxaigen-0.0.0.4/oxaigen/src/util/util.py
+-rw-r--r--   0        0        0      825 2024-05-22 12:39:53.291569 oxaigen-0.0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 oxaigen-0.0.0.4/PKG-INFO
```

### Comparing `oxaigen-0.0.0.3/oxaigen/src/asset/asset.py` & `oxaigen-0.0.0.4/oxaigen/src/asset/asset.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.3/oxaigen/src/authentication/authentication.py` & `oxaigen-0.0.0.4/oxaigen/src/authentication/authentication.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.3/oxaigen/src/config.py` & `oxaigen-0.0.0.4/oxaigen/src/config.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.3/oxaigen/src/storage/data_storage.py` & `oxaigen-0.0.0.4/oxaigen/src/storage/data_storage.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.3/oxaigen/src/util/api.py` & `oxaigen-0.0.0.4/oxaigen/src/util/api.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.3/oxaigen/src/util/exception.py` & `oxaigen-0.0.0.4/oxaigen/src/util/exception.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.3/oxaigen/src/util/token.py` & `oxaigen-0.0.0.4/oxaigen/src/util/token.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.3/oxaigen/src/util/util.py` & `oxaigen-0.0.0.4/oxaigen/src/util/util.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.3/pyproject.toml` & `oxaigen-0.0.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "oxaigen"
-version = "0.0.0.3"
+version = "0.0.0.4"
 description = "Oxaigen Python SDK"
 authors = ["Luca Roggeveen Name <luca@oxaigen.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10.12"
-pydantic = "==1.10.8"
+pydantic = "==2.7.1"
 pandas = "^2.1.0"
 mlflow = "^2.10.2"
 scikit-learn = "^1.4.0"
 numpy = "^1.26.4"
 boto3 = "^1.34.44"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `oxaigen-0.0.0.3/PKG-INFO` & `oxaigen-0.0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: oxaigen
-Version: 0.0.0.3
+Version: 0.0.0.4
 Summary: Oxaigen Python SDK
 Author: Luca Roggeveen Name
 Author-email: luca@oxaigen.com
 Requires-Python: >=3.10.12,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.34.44,<2.0.0)
 Requires-Dist: mlflow (>=2.10.2,<3.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pandas (>=2.1.0,<3.0.0)
-Requires-Dist: pydantic (==1.10.8)
+Requires-Dist: pydantic (==2.7.1)
 Requires-Dist: scikit-learn (>=1.4.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 <div id="top"></div>
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
```

