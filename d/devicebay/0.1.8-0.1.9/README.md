# Comparing `tmp/devicebay-0.1.8.tar.gz` & `tmp/devicebay-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devicebay-0.1.8.tar", max compression
+gzip compressed data, was "devicebay-0.1.9.tar", max compression
```

## Comparing `devicebay-0.1.8.tar` & `devicebay-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-04-09 02:39:38.878817 devicebay-0.1.8/LICENSE
--rw-r--r--   0        0        0       35 2024-04-09 02:39:38.878906 devicebay-0.1.8/README.md
--rw-r--r--   0        0        0       89 2024-04-09 17:05:39.050602 devicebay-0.1.8/devicebay/__init__.py
--rw-r--r--   0        0        0     2862 2024-04-10 02:10:15.195691 devicebay-0.1.8/devicebay/base.py
--rw-r--r--   0        0        0       99 2024-04-09 21:42:18.657362 devicebay-0.1.8/devicebay/models.py
--rw-r--r--   0        0        0      342 2024-04-10 02:10:23.325065 devicebay-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 devicebay-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-09 02:39:38.878817 devicebay-0.1.9/LICENSE
+-rw-r--r--   0        0        0       35 2024-04-09 02:39:38.878906 devicebay-0.1.9/README.md
+-rw-r--r--   0        0        0       89 2024-04-09 17:05:39.050602 devicebay-0.1.9/devicebay/__init__.py
+-rw-r--r--   0        0        0     2862 2024-04-10 19:08:17.517891 devicebay-0.1.9/devicebay/base.py
+-rw-r--r--   0        0        0     2013 2024-04-10 18:36:43.082894 devicebay-0.1.9/devicebay/db/conn.py
+-rw-r--r--   0        0        0     1177 2024-04-10 18:40:09.387465 devicebay-0.1.9/devicebay/db/models.py
+-rw-r--r--   0        0        0     1126 2024-04-10 18:40:37.112751 devicebay-0.1.9/devicebay/models.py
+-rw-r--r--   0        0        0     9038 2024-04-10 18:40:35.159878 devicebay-0.1.9/devicebay/types.py
+-rw-r--r--   0        0        0      365 2024-04-11 18:00:02.018345 devicebay-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 devicebay-0.1.9/PKG-INFO
```

### Comparing `devicebay-0.1.8/LICENSE` & `devicebay-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `devicebay-0.1.8/devicebay/base.py` & `devicebay-0.1.9/devicebay/base.py`

 * *Files identical despite different names*

