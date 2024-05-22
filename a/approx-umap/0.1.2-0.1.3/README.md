# Comparing `tmp/approx_umap-0.1.2.tar.gz` & `tmp/approx_umap-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approx_umap-0.1.2.tar", max compression
+gzip compressed data, was "approx_umap-0.1.3.tar", max compression
```

## Comparing `approx_umap-0.1.2.tar` & `approx_umap-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1505 2024-04-03 17:09:04.702968 approx_umap-0.1.2/LICENSE
--rw-r--r--   0        0        0     2116 2024-04-12 11:32:14.902620 approx_umap-0.1.2/README.md
--rw-r--r--   0        0        0       46 2024-04-12 11:31:51.625854 approx_umap-0.1.2/approx_umap/__init__.py
--rw-r--r--   0        0        0     5512 2024-04-12 11:34:31.791489 approx_umap-0.1.2/approx_umap/approx_umap.py
--rw-r--r--   0        0        0      710 2024-04-12 11:36:38.157165 approx_umap-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 approx_umap-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1505 2024-04-03 17:09:04.702968 approx_umap-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2116 2024-04-12 11:32:14.902620 approx_umap-0.1.3/README.md
+-rw-r--r--   0        0        0       46 2024-04-14 07:53:15.581717 approx_umap-0.1.3/approx_umap/__init__.py
+-rw-r--r--   0        0        0     9282 2024-05-22 21:43:34.075895 approx_umap-0.1.3/approx_umap/approx_umap.py
+-rw-r--r--   0        0        0      751 2024-05-22 19:33:38.678082 approx_umap-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2859 1970-01-01 00:00:00.000000 approx_umap-0.1.3/PKG-INFO
```

### Comparing `approx_umap-0.1.2/LICENSE` & `approx_umap-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `approx_umap-0.1.2/README.md` & `approx_umap-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `approx_umap-0.1.2/pyproject.toml` & `approx_umap-0.1.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "approx-umap"
-version = "0.1.2"
+version = "0.1.3"
 description = "Modification of the UMAP algorithm to allow for fast approximate projections of new data points."
 authors = [
     "Pierre Guetschel <pierre.guetschel@donders.ru.nl>",
     "Peter Wassenaar <peter.wassenaar@ru.nl>",
 ]
 readme = "README.md"
 packages = [{ include = "approx_umap" }]
 license = "BSD-3-Clause"
 repository = "https://github.com/PierreGtch/approx-umap"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.10, <3.13"
 umap-learn = "^0.5.5"
+docstring-inheritance = "^2.2.0"
 
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
```

### Comparing `approx_umap-0.1.2/PKG-INFO` & `approx_umap-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: approx-umap
-Version: 0.1.2
+Version: 0.1.3
 Summary: Modification of the UMAP algorithm to allow for fast approximate projections of new data points.
 Home-page: https://github.com/PierreGtch/approx-umap
 License: BSD-3-Clause
 Author: Pierre Guetschel
 Author-email: pierre.guetschel@donders.ru.nl
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: docstring-inheritance (>=2.2.0,<3.0.0)
 Requires-Dist: umap-learn (>=0.5.5,<0.6.0)
 Project-URL: Repository, https://github.com/PierreGtch/approx-umap
 Description-Content-Type: text/markdown
 
 # Approximate UMAP
 
 Modification of the UMAP algorithm to allow for fast approximate projections of
```

