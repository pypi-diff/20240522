# Comparing `tmp/hypercrawl-lite-0.1.0.tar.gz` & `tmp/hypercrawl-lite-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypercrawl-lite-0.1.0.tar", last modified: Wed May 22 11:55:18 2024, max compression
+gzip compressed data, was "hypercrawl-lite-0.1.1.tar", last modified: Wed May 22 11:57:59 2024, max compression
```

## Comparing `hypercrawl-lite-0.1.0.tar` & `hypercrawl-lite-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-05-22 11:55:18.371540 hypercrawl-lite-0.1.0/
--rw-r--r--   0 akhouriudit   (501) staff       (20)      294 2024-05-22 11:55:18.371410 hypercrawl-lite-0.1.0/PKG-INFO
--rw-r--r--   0 akhouriudit   (501) staff       (20)        0 2024-05-22 11:51:05.000000 hypercrawl-lite-0.1.0/README.md
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-05-22 11:55:18.371220 hypercrawl-lite-0.1.0/hypercrawl_lite.egg-info/
--rw-r--r--   0 akhouriudit   (501) staff       (20)      294 2024-05-22 11:55:18.000000 hypercrawl-lite-0.1.0/hypercrawl_lite.egg-info/PKG-INFO
--rw-r--r--   0 akhouriudit   (501) staff       (20)      254 2024-05-22 11:55:18.000000 hypercrawl-lite-0.1.0/hypercrawl_lite.egg-info/SOURCES.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)        1 2024-05-22 11:55:18.000000 hypercrawl-lite-0.1.0/hypercrawl_lite.egg-info/dependency_links.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       65 2024-05-22 11:55:18.000000 hypercrawl-lite-0.1.0/hypercrawl_lite.egg-info/entry_points.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       24 2024-05-22 11:55:18.000000 hypercrawl-lite-0.1.0/hypercrawl_lite.egg-info/requires.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)        1 2024-05-22 11:55:18.000000 hypercrawl-lite-0.1.0/hypercrawl_lite.egg-info/top_level.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       38 2024-05-22 11:55:18.371662 hypercrawl-lite-0.1.0/setup.cfg
--rw-r--r--   0 akhouriudit   (501) staff       (20)      643 2024-05-22 11:55:15.000000 hypercrawl-lite-0.1.0/setup.py
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-05-22 11:57:59.953405 hypercrawl-lite-0.1.1/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      294 2024-05-22 11:57:59.953263 hypercrawl-lite-0.1.1/PKG-INFO
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        0 2024-05-22 11:51:05.000000 hypercrawl-lite-0.1.1/README.md
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-05-22 11:57:59.953037 hypercrawl-lite-0.1.1/hypercrawl_lite.egg-info/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      294 2024-05-22 11:57:59.000000 hypercrawl-lite-0.1.1/hypercrawl_lite.egg-info/PKG-INFO
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      254 2024-05-22 11:57:59.000000 hypercrawl-lite-0.1.1/hypercrawl_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        1 2024-05-22 11:57:59.000000 hypercrawl-lite-0.1.1/hypercrawl_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       65 2024-05-22 11:57:59.000000 hypercrawl-lite-0.1.1/hypercrawl_lite.egg-info/entry_points.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       24 2024-05-22 11:57:59.000000 hypercrawl-lite-0.1.1/hypercrawl_lite.egg-info/requires.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        1 2024-05-22 11:57:59.000000 hypercrawl-lite-0.1.1/hypercrawl_lite.egg-info/top_level.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       38 2024-05-22 11:57:59.953446 hypercrawl-lite-0.1.1/setup.cfg
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      643 2024-05-22 11:57:49.000000 hypercrawl-lite-0.1.1/setup.py
```

### Comparing `hypercrawl-lite-0.1.0/setup.py` & `hypercrawl-lite-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hypercrawl-lite',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         'requests',
         'beautifulsoup4',
     ],
     entry_points={
         'console_scripts': [
```

