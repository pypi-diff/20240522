# Comparing `tmp/df_processors-0.1.1.tar.gz` & `tmp/df_processors-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "df_processors-0.1.1.tar", max compression
+gzip compressed data, was "df_processors-0.1.2.tar", max compression
```

## Comparing `df_processors-0.1.1.tar` & `df_processors-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-05-08 21:02:12.762087 df_processors-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-08 21:02:12.761818 df_processors-0.1.1/df_processors/__init__.py
--rw-r--r--   0        0        0     2887 2024-05-08 21:52:38.829688 df_processors-0.1.1/df_processors/_utils.py
--rw-r--r--   0        0        0     7917 2024-05-09 00:39:38.735570 df_processors-0.1.1/df_processors/create.py
--rw-r--r--   0        0        0     8648 2024-05-09 00:41:47.271741 df_processors-0.1.1/df_processors/impute.py
--rw-r--r--   0        0        0     3528 2024-05-09 00:41:13.458469 df_processors-0.1.1/df_processors/normalize.py
--rw-r--r--   0        0        0     1074 2024-05-22 16:44:07.285524 df_processors-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 df_processors-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       91 2024-05-22 16:45:58.184320 df_processors-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 21:02:12.761818 df_processors-0.1.2/df_processors/__init__.py
+-rw-r--r--   0        0        0     2887 2024-05-08 21:52:38.829688 df_processors-0.1.2/df_processors/_utils.py
+-rw-r--r--   0        0        0     7917 2024-05-09 00:39:38.735570 df_processors-0.1.2/df_processors/create.py
+-rw-r--r--   0        0        0     8648 2024-05-09 00:41:47.271741 df_processors-0.1.2/df_processors/impute.py
+-rw-r--r--   0        0        0     3528 2024-05-09 00:41:13.458469 df_processors-0.1.2/df_processors/normalize.py
+-rw-r--r--   0        0        0     1160 2024-05-22 16:49:03.993963 df_processors-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      925 1970-01-01 00:00:00.000000 df_processors-0.1.2/PKG-INFO
```

### Comparing `df_processors-0.1.1/df_processors/_utils.py` & `df_processors-0.1.2/df_processors/_utils.py`

 * *Files identical despite different names*

### Comparing `df_processors-0.1.1/df_processors/create.py` & `df_processors-0.1.2/df_processors/create.py`

 * *Files identical despite different names*

### Comparing `df_processors-0.1.1/df_processors/impute.py` & `df_processors-0.1.2/df_processors/impute.py`

 * *Files identical despite different names*

### Comparing `df_processors-0.1.1/df_processors/normalize.py` & `df_processors-0.1.2/df_processors/normalize.py`

 * *Files identical despite different names*

### Comparing `df_processors-0.1.1/pyproject.toml` & `df_processors-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "df-processors"
-version = "0.1.1"
+version = "0.1.2"
 description = "A Python library that provides utilities to process your pandas DataFrame."
 authors = ["khuyentran1401 <khuyentran1476@gmail.com>"]
 repository = "https://github.com/khuyentran1401/df-processors.git"
+documentation = "https://github.com/khuyentran1401/df-processors/blob/main/README.md"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^2.2.2"
 scikit-learn = "^1.4.2"
 scipy = "^1.13.0"
```

### Comparing `df_processors-0.1.1/PKG-INFO` & `df_processors-0.1.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: df-processors
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library that provides utilities to process your pandas DataFrame.
 Home-page: https://github.com/khuyentran1401/df-processors.git
 Author: khuyentran1401
 Author-email: khuyentran1476@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
 Requires-Dist: scipy (>=1.13.0,<2.0.0)
+Project-URL: Documentation, https://github.com/khuyentran1401/df-processors/blob/main/README.md
 Project-URL: Repository, https://github.com/khuyentran1401/df-processors.git
 Description-Content-Type: text/markdown
 
+# df-processors
 
+A Python library that provides utilities to process your pandas DataFrame.
```

