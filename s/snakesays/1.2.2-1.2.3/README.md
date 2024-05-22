# Comparing `tmp/snakesays-1.2.2.tar.gz` & `tmp/snakesays-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakesays-1.2.2.tar", max compression
+gzip compressed data, was "snakesays-1.2.3.tar", max compression
```

## Comparing `snakesays-1.2.2.tar` & `snakesays-1.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      616 2024-01-06 04:34:03.375106 snakesays-1.2.2/pyproject.toml
--rw-r--r--   0        0        0      279 2024-01-06 02:25:11.785363 snakesays-1.2.2/README.md
--rw-r--r--   0        0        0        0 2024-01-06 03:05:40.702125 snakesays-1.2.2/snakesays/__init__.py
--rw-r--r--   0        0        0      135 2024-01-06 03:26:38.924574 snakesays-1.2.2/snakesays/__main__.py
--rw-r--r--   0        0        0      148 2024-01-06 03:26:38.966574 snakesays-1.2.2/snakesays/cli.py
--rw-r--r--   0        0        0      379 2024-01-06 03:26:39.010119 snakesays-1.2.2/snakesays/snake.py
--rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 snakesays-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      616 2024-05-22 08:04:42.078406 snakesays-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0      279 2024-01-06 02:25:11.785363 snakesays-1.2.3/README.md
+-rw-r--r--   0        0        0        0 2024-01-06 03:05:40.702125 snakesays-1.2.3/snakesays/__init__.py
+-rw-r--r--   0        0        0      136 2024-05-22 08:02:39.422979 snakesays-1.2.3/snakesays/__main__.py
+-rw-r--r--   0        0        0      149 2024-05-22 08:03:03.406441 snakesays-1.2.3/snakesays/cli.py
+-rw-r--r--   0        0        0      379 2024-01-06 03:26:39.010119 snakesays-1.2.3/snakesays/snake.py
+-rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 snakesays-1.2.3/PKG-INFO
```

### Comparing `snakesays-1.2.2/pyproject.toml` & `snakesays-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snakesays"
-version = "1.2.2"
+version = "1.2.3"
 description = "To display with effect of snake saying"
 authors = ["Ishan Mahajan <imahajan0007@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/ishan65/snakesays.git"
 repository = "https://github.com/ishan65/snakesays.git"
 
 [tool.poetry.dependencies]
```

### Comparing `snakesays-1.2.2/PKG-INFO` & `snakesays-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakesays
-Version: 1.2.2
+Version: 1.2.3
 Summary: To display with effect of snake saying
 Home-page: https://github.com/ishan65/snakesays.git
 Author: Ishan Mahajan
 Author-email: imahajan0007@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

