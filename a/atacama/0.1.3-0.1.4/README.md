# Comparing `tmp/atacama-0.1.3.tar.gz` & `tmp/atacama-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atacama-0.1.3.tar", max compression
+gzip compressed data, was "atacama-0.1.4.tar", max compression
```

## Comparing `atacama-0.1.3.tar` & `atacama-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       27 2024-03-29 21:04:18.753821 atacama-0.1.3/README_PUBLIC.md
--rw-r--r--   0        0        0       66 2024-03-29 21:04:18.753821 atacama-0.1.3/atacama/__init__.py
--rw-r--r--   0        0        0    19166 2024-03-29 21:04:18.753821 atacama-0.1.3/atacama/client.py
--rw-r--r--   0        0        0      523 2024-03-29 21:04:18.753821 atacama-0.1.3/atacama/exceptions.py
--rw-r--r--   0        0        0      815 2024-03-29 21:04:18.753821 atacama-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 atacama-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       27 2024-05-22 20:25:41.510126 atacama-0.1.4/README_PUBLIC.md
+-rw-r--r--   0        0        0       66 2024-05-22 20:25:41.510126 atacama-0.1.4/atacama/__init__.py
+-rw-r--r--   0        0        0    19166 2024-05-22 20:25:41.510126 atacama-0.1.4/atacama/client.py
+-rw-r--r--   0        0        0      523 2024-05-22 20:25:41.510126 atacama-0.1.4/atacama/exceptions.py
+-rw-r--r--   0        0        0      816 2024-05-22 20:25:41.510126 atacama-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      715 1970-01-01 00:00:00.000000 atacama-0.1.4/PKG-INFO
```

### Comparing `atacama-0.1.3/atacama/client.py` & `atacama-0.1.4/atacama/client.py`

 * *Files identical despite different names*

### Comparing `atacama-0.1.3/atacama/exceptions.py` & `atacama-0.1.4/atacama/exceptions.py`

 * *Files identical despite different names*

### Comparing `atacama-0.1.3/pyproject.toml` & `atacama-0.1.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "atacama"
-version = "0.1.3"
+version = "0.1.4"
 description = "Python API for LLM"
 authors = ["Virtualitics Engineering <dev@virtualitics.com>"]
 license = "MIT LICENSE"
 packages = [{include = "atacama"}]
 classifiers=[
     "Programming Language :: Python :: 3",
     "Operating System :: Microsoft :: Windows :: Windows 10",
@@ -13,15 +13,15 @@
     "License :: OSI Approved :: MIT License"
 ]
 readme = "README_PUBLIC.md"
 documentation = "https://python-poetry.org/docs/"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-requests = "2.31.0"
+requests = "^2.32.2"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "7.2.6"
 sphinx-autodoc-typehints = "1.24.0"
 sphinx-copybutton = "0.5.2"
 furo = "2023.9.10"
```

