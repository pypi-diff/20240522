# Comparing `tmp/parsel_get_selector_text-0.7.tar.gz` & `tmp/parsel_get_selector_text-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsel_get_selector_text-0.7.tar", last modified: Sat Jul 22 19:45:19 2023, max compression
+gzip compressed data, was "parsel_get_selector_text-0.8.tar", last modified: Wed May 22 21:21:46 2024, max compression
```

## Comparing `parsel_get_selector_text-0.7.tar` & `parsel_get_selector_text-0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2023-07-22 19:45:19.146475 parsel_get_selector_text-0.7/
--rw-r--r--   0 andrei    (1000) andrei    (1000)     1089 2023-04-23 23:41:13.000000 parsel_get_selector_text-0.7/LICENSE
--rw-r--r--   0 andrei    (1000) andrei    (1000)      722 2023-07-22 19:45:19.146475 parsel_get_selector_text-0.7/PKG-INFO
--rw-r--r--   0 andrei    (1000) andrei    (1000)       85 2023-04-23 22:53:37.000000 parsel_get_selector_text-0.7/README.md
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2023-07-22 19:45:19.146475 parsel_get_selector_text-0.7/parsel_get_selector_text/
--rw-r--r--   0 andrei    (1000) andrei    (1000)     2735 2023-07-22 19:42:20.000000 parsel_get_selector_text-0.7/parsel_get_selector_text/__init__.py
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2023-07-22 19:45:19.146475 parsel_get_selector_text-0.7/parsel_get_selector_text.egg-info/
--rw-r--r--   0 andrei    (1000) andrei    (1000)      722 2023-07-22 19:45:19.000000 parsel_get_selector_text-0.7/parsel_get_selector_text.egg-info/PKG-INFO
--rw-r--r--   0 andrei    (1000) andrei    (1000)      308 2023-07-22 19:45:19.000000 parsel_get_selector_text-0.7/parsel_get_selector_text.egg-info/SOURCES.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)        1 2023-07-22 19:45:19.000000 parsel_get_selector_text-0.7/parsel_get_selector_text.egg-info/dependency_links.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)       27 2023-07-22 19:45:19.000000 parsel_get_selector_text-0.7/parsel_get_selector_text.egg-info/requires.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)       25 2023-07-22 19:45:19.000000 parsel_get_selector_text-0.7/parsel_get_selector_text.egg-info/top_level.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)      886 2023-07-22 19:42:39.000000 parsel_get_selector_text-0.7/pyproject.toml
--rw-r--r--   0 andrei    (1000) andrei    (1000)       38 2023-07-22 19:45:19.146475 parsel_get_selector_text-0.7/setup.cfg
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-22 21:21:46.043172 parsel_get_selector_text-0.8/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     1089 2023-04-23 23:41:13.000000 parsel_get_selector_text-0.8/LICENSE
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     2745 2024-05-22 21:21:46.043172 parsel_get_selector_text-0.8/PKG-INFO
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     2036 2024-05-22 21:20:38.000000 parsel_get_selector_text-0.8/README.md
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-22 21:21:46.039839 parsel_get_selector_text-0.8/parsel_get_selector_text/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     2735 2023-07-22 19:42:20.000000 parsel_get_selector_text-0.8/parsel_get_selector_text/__init__.py
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-22 21:21:46.043172 parsel_get_selector_text-0.8/parsel_get_selector_text.egg-info/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     2745 2024-05-22 21:21:46.000000 parsel_get_selector_text-0.8/parsel_get_selector_text.egg-info/PKG-INFO
+-rw-r--r--   0 andrei    (1000) andrei    (1000)      308 2024-05-22 21:21:46.000000 parsel_get_selector_text-0.8/parsel_get_selector_text.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)        1 2024-05-22 21:21:46.000000 parsel_get_selector_text-0.8/parsel_get_selector_text.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       27 2024-05-22 21:21:46.000000 parsel_get_selector_text-0.8/parsel_get_selector_text.egg-info/requires.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       25 2024-05-22 21:21:46.000000 parsel_get_selector_text-0.8/parsel_get_selector_text.egg-info/top_level.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)      886 2024-05-22 21:21:19.000000 parsel_get_selector_text-0.8/pyproject.toml
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       38 2024-05-22 21:21:46.043172 parsel_get_selector_text-0.8/setup.cfg
```

### Comparing `parsel_get_selector_text-0.7/LICENSE` & `parsel_get_selector_text-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `parsel_get_selector_text-0.7/parsel_get_selector_text/__init__.py` & `parsel_get_selector_text-0.8/parsel_get_selector_text/__init__.py`

 * *Files identical despite different names*

### Comparing `parsel_get_selector_text-0.7/pyproject.toml` & `parsel_get_selector_text-0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [options]
 package_dir = "parsel_get_selector_text"
 packages = ["parsel_get_selector_text"]
 
 [project]
 name = "parsel_get_selector_text"
-version = "0.7"
+version = "0.8"
 authors = [
     {name = "Carlos A. Planchón", email = "carlosandresplanchonprestes@gmail.com"}
 ]
 description = "Extracts all text results from an XPath query on a parsel Selector object."
 classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
```

