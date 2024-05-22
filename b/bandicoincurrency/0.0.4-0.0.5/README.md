# Comparing `tmp/bandicoincurrency-0.0.4.tar.gz` & `tmp/bandicoincurrency-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bandicoincurrency-0.0.4.tar", last modified: Wed May 22 04:50:56 2024, max compression
+gzip compressed data, was "bandicoincurrency-0.0.5.tar", last modified: Wed May 22 04:55:28 2024, max compression
```

## Comparing `bandicoincurrency-0.0.4.tar` & `bandicoincurrency-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 04:50:56.835635 bandicoincurrency-0.0.4/
--rw-r--r--   0 root         (0) root         (0)      412 2024-05-22 04:50:56.835635 bandicoincurrency-0.0.4/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)       62 2024-05-22 03:52:37.000000 bandicoincurrency-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 04:50:56.835635 bandicoincurrency-0.0.4/bandicoincurrency.egg-info/
--rw-r--r--   0 root         (0) root         (0)      412 2024-05-22 04:50:56.000000 bandicoincurrency-0.0.4/bandicoincurrency.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2024-05-22 04:50:56.000000 bandicoincurrency-0.0.4/bandicoincurrency.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 04:50:56.000000 bandicoincurrency-0.0.4/bandicoincurrency.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 04:50:56.000000 bandicoincurrency-0.0.4/bandicoincurrency.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 04:50:56.835635 bandicoincurrency-0.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      603 2024-05-22 04:50:48.000000 bandicoincurrency-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 04:55:28.293058 bandicoincurrency-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)      412 2024-05-22 04:55:28.293058 bandicoincurrency-0.0.5/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)       62 2024-05-22 03:52:37.000000 bandicoincurrency-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 04:55:28.293058 bandicoincurrency-0.0.5/bandicoincurrency.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      412 2024-05-22 04:55:28.000000 bandicoincurrency-0.0.5/bandicoincurrency.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2024-05-22 04:55:28.000000 bandicoincurrency-0.0.5/bandicoincurrency.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 04:55:28.000000 bandicoincurrency-0.0.5/bandicoincurrency.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 04:55:28.000000 bandicoincurrency-0.0.5/bandicoincurrency.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 04:55:28.293058 bandicoincurrency-0.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      603 2024-05-22 04:55:00.000000 bandicoincurrency-0.0.5/setup.py
```

### Comparing `bandicoincurrency-0.0.4/setup.py` & `bandicoincurrency-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="bandicoincurrency",
-    version="0.0.4",
+    version="0.0.5",
     author="cbt1",
     description="Bandicoin scratch project wrapper for external payments",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

