# Comparing `tmp/bandicoincurrency-0.0.1.tar.gz` & `tmp/bandicoincurrency-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bandicoincurrency-0.0.1.tar", last modified: Wed May 22 04:03:01 2024, max compression
+gzip compressed data, was "bandicoincurrency-0.0.2.tar", last modified: Wed May 22 04:35:36 2024, max compression
```

## Comparing `bandicoincurrency-0.0.1.tar` & `bandicoincurrency-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 04:03:01.394919 bandicoincurrency-0.0.1/
--rw-r--r--   0 root         (0) root         (0)      412 2024-05-22 04:03:01.394919 bandicoincurrency-0.0.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)       62 2024-05-22 03:52:37.000000 bandicoincurrency-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 04:03:01.394919 bandicoincurrency-0.0.1/bandicoincurrency.egg-info/
--rw-r--r--   0 root         (0) root         (0)      412 2024-05-22 04:03:01.000000 bandicoincurrency-0.0.1/bandicoincurrency.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2024-05-22 04:03:01.000000 bandicoincurrency-0.0.1/bandicoincurrency.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 04:03:01.000000 bandicoincurrency-0.0.1/bandicoincurrency.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 04:03:01.000000 bandicoincurrency-0.0.1/bandicoincurrency.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 04:03:01.394919 bandicoincurrency-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      603 2024-05-22 03:53:35.000000 bandicoincurrency-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 04:35:36.804617 bandicoincurrency-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)      412 2024-05-22 04:35:36.804617 bandicoincurrency-0.0.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)       62 2024-05-22 03:52:37.000000 bandicoincurrency-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 04:35:36.804617 bandicoincurrency-0.0.2/bandicoincurrency.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      412 2024-05-22 04:35:36.000000 bandicoincurrency-0.0.2/bandicoincurrency.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2024-05-22 04:35:36.000000 bandicoincurrency-0.0.2/bandicoincurrency.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 04:35:36.000000 bandicoincurrency-0.0.2/bandicoincurrency.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 04:35:36.000000 bandicoincurrency-0.0.2/bandicoincurrency.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 04:35:36.804617 bandicoincurrency-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      603 2024-05-22 04:35:27.000000 bandicoincurrency-0.0.2/setup.py
```

### Comparing `bandicoincurrency-0.0.1/setup.py` & `bandicoincurrency-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="bandicoincurrency",
-    version="0.0.1",
+    version="0.0.2",
     author="cbt1",
     description="Bandicoin scratch project wrapper for external payments",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

