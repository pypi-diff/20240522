# Comparing `tmp/myscale_callback-0.1.0.tar.gz` & `tmp/myscale_callback-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myscale_callback-0.1.0.tar", last modified: Tue May 21 06:02:12 2024, max compression
+gzip compressed data, was "myscale_callback-0.2.0.tar", last modified: Wed May 22 01:56:54 2024, max compression
```

## Comparing `myscale_callback-0.1.0.tar` & `myscale_callback-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-21 06:02:12.234823 myscale_callback-0.1.0/
--rw-r--r--   0 xuj        (501) staff       (20)     1064 2024-05-21 03:32:44.000000 myscale_callback-0.1.0/LICENSE
--rw-r--r--   0 xuj        (501) staff       (20)      359 2024-05-21 06:02:12.234655 myscale_callback-0.1.0/PKG-INFO
--rw-r--r--   0 xuj        (501) staff       (20)       18 2024-05-21 03:32:44.000000 myscale_callback-0.1.0/README.md
-drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-21 06:02:12.233688 myscale_callback-0.1.0/callback/
--rw-r--r--   0 xuj        (501) staff       (20)        0 2024-05-21 05:08:28.000000 myscale_callback-0.1.0/callback/__init__.py
--rw-r--r--   0 xuj        (501) staff       (20)     5569 2024-05-21 05:09:24.000000 myscale_callback-0.1.0/callback/consumer.py
--rw-r--r--   0 xuj        (501) staff       (20)    21572 2024-05-21 05:11:16.000000 myscale_callback-0.1.0/callback/handler.py
--rw-r--r--   0 xuj        (501) staff       (20)     3671 2024-05-21 05:11:16.000000 myscale_callback-0.1.0/callback/span_data.py
--rw-r--r--   0 xuj        (501) staff       (20)     6557 2024-05-21 05:11:16.000000 myscale_callback-0.1.0/callback/task_manager.py
-drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-21 06:02:12.234457 myscale_callback-0.1.0/myscale_callback.egg-info/
--rw-r--r--   0 xuj        (501) staff       (20)      359 2024-05-21 06:02:12.000000 myscale_callback-0.1.0/myscale_callback.egg-info/PKG-INFO
--rw-r--r--   0 xuj        (501) staff       (20)      334 2024-05-21 06:02:12.000000 myscale_callback-0.1.0/myscale_callback.egg-info/SOURCES.txt
--rw-r--r--   0 xuj        (501) staff       (20)        1 2024-05-21 06:02:12.000000 myscale_callback-0.1.0/myscale_callback.egg-info/dependency_links.txt
--rw-r--r--   0 xuj        (501) staff       (20)       85 2024-05-21 06:02:12.000000 myscale_callback-0.1.0/myscale_callback.egg-info/requires.txt
--rw-r--r--   0 xuj        (501) staff       (20)        9 2024-05-21 06:02:12.000000 myscale_callback-0.1.0/myscale_callback.egg-info/top_level.txt
--rw-r--r--   0 xuj        (501) staff       (20)       38 2024-05-21 06:02:12.234873 myscale_callback-0.1.0/setup.cfg
--rw-r--r--   0 xuj        (501) staff       (20)      607 2024-05-21 05:56:11.000000 myscale_callback-0.1.0/setup.py
+drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-22 01:56:54.817934 myscale_callback-0.2.0/
+-rw-r--r--   0 xuj        (501) staff       (20)     1064 2024-05-21 03:32:44.000000 myscale_callback-0.2.0/LICENSE
+-rw-r--r--   0 xuj        (501) staff       (20)      405 2024-05-22 01:56:54.817738 myscale_callback-0.2.0/PKG-INFO
+-rw-r--r--   0 xuj        (501) staff       (20)       18 2024-05-21 03:32:44.000000 myscale_callback-0.2.0/README.md
+drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-22 01:56:54.816910 myscale_callback-0.2.0/myscale_callback/
+-rw-r--r--   0 xuj        (501) staff       (20)        0 2024-05-21 05:08:28.000000 myscale_callback-0.2.0/myscale_callback/__init__.py
+-rw-r--r--   0 xuj        (501) staff       (20)     5569 2024-05-21 05:09:24.000000 myscale_callback-0.2.0/myscale_callback/consumer.py
+-rw-r--r--   0 xuj        (501) staff       (20)    21572 2024-05-21 05:11:16.000000 myscale_callback-0.2.0/myscale_callback/handler.py
+-rw-r--r--   0 xuj        (501) staff       (20)     3671 2024-05-21 05:11:16.000000 myscale_callback-0.2.0/myscale_callback/span_data.py
+-rw-r--r--   0 xuj        (501) staff       (20)     6557 2024-05-21 05:11:16.000000 myscale_callback-0.2.0/myscale_callback/task_manager.py
+drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-22 01:56:54.817577 myscale_callback-0.2.0/myscale_callback.egg-info/
+-rw-r--r--   0 xuj        (501) staff       (20)      405 2024-05-22 01:56:54.000000 myscale_callback-0.2.0/myscale_callback.egg-info/PKG-INFO
+-rw-r--r--   0 xuj        (501) staff       (20)      374 2024-05-22 01:56:54.000000 myscale_callback-0.2.0/myscale_callback.egg-info/SOURCES.txt
+-rw-r--r--   0 xuj        (501) staff       (20)        1 2024-05-22 01:56:54.000000 myscale_callback-0.2.0/myscale_callback.egg-info/dependency_links.txt
+-rw-r--r--   0 xuj        (501) staff       (20)       85 2024-05-22 01:56:54.000000 myscale_callback-0.2.0/myscale_callback.egg-info/requires.txt
+-rw-r--r--   0 xuj        (501) staff       (20)       17 2024-05-22 01:56:54.000000 myscale_callback-0.2.0/myscale_callback.egg-info/top_level.txt
+-rw-r--r--   0 xuj        (501) staff       (20)       38 2024-05-22 01:56:54.817974 myscale_callback-0.2.0/setup.cfg
+-rw-r--r--   0 xuj        (501) staff       (20)      665 2024-05-22 01:55:22.000000 myscale_callback-0.2.0/setup.py
```

### Comparing `myscale_callback-0.1.0/LICENSE` & `myscale_callback-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myscale_callback-0.1.0/callback/consumer.py` & `myscale_callback-0.2.0/myscale_callback/consumer.py`

 * *Files identical despite different names*

### Comparing `myscale_callback-0.1.0/callback/handler.py` & `myscale_callback-0.2.0/myscale_callback/handler.py`

 * *Files identical despite different names*

### Comparing `myscale_callback-0.1.0/callback/span_data.py` & `myscale_callback-0.2.0/myscale_callback/span_data.py`

 * *Files identical despite different names*

### Comparing `myscale_callback-0.1.0/callback/task_manager.py` & `myscale_callback-0.2.0/myscale_callback/task_manager.py`

 * *Files identical despite different names*

### Comparing `myscale_callback-0.1.0/setup.py` & `myscale_callback-0.2.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="myscale_callback",
-    version="0.1.0",
+    version="0.2.0",
     description="A package for MyScale Callback Handler",
+    author="Xu Jing",
+    author_email="xuj@myscale.com",
     url="https://github.com/myscale/myscale_callback.git",
     packages=find_packages(),
     install_requires=[
         "backoff>=2.2.1",
         "langchain>=0.2.0",
         "langchain-community>=0.2.0",
         "clickhouse-connect>=0.7.8"
```

