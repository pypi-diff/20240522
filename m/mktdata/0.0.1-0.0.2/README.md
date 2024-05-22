# Comparing `tmp/mktdata-0.0.1.tar.gz` & `tmp/mktdata-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mktdata-0.0.1.tar", last modified: Mon May 20 22:38:48 2024, max compression
+gzip compressed data, was "mktdata-0.0.2.tar", last modified: Wed May 22 01:55:16 2024, max compression
```

## Comparing `mktdata-0.0.1.tar` & `mktdata-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 22:38:48.261914 mktdata-0.0.1/
--rw-rw-rw-   0        0        0     7618 2024-05-20 22:38:48.260910 mktdata-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-20 22:38:48.252409 mktdata-0.0.1/mktdata.egg-info/
--rw-rw-rw-   0        0        0     7618 2024-05-20 22:38:48.000000 mktdata-0.0.1/mktdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      181 2024-05-20 22:38:48.000000 mktdata-0.0.1/mktdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 22:38:48.000000 mktdata-0.0.1/mktdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     4028 2024-05-20 22:38:48.000000 mktdata-0.0.1/mktdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-20 22:38:48.000000 mktdata-0.0.1/mktdata.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-20 22:38:48.253408 mktdata-0.0.1/models/
--rw-rw-rw-   0        0        0        0 2024-05-18 03:54:40.000000 mktdata-0.0.1/models/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-20 22:38:48.261914 mktdata-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      375 2024-05-20 22:38:44.000000 mktdata-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:55:16.286080 mktdata-0.0.2/
+-rw-rw-rw-   0        0        0       54 2024-05-22 01:55:16.285081 mktdata-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-22 01:55:16.284080 mktdata-0.0.2/mktdata.egg-info/
+-rw-rw-rw-   0        0        0       54 2024-05-22 01:55:16.000000 mktdata-0.0.2/mktdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      181 2024-05-22 01:55:16.000000 mktdata-0.0.2/mktdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 01:55:16.000000 mktdata-0.0.2/mktdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     4028 2024-05-22 01:55:16.000000 mktdata-0.0.2/mktdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-22 01:55:16.000000 mktdata-0.0.2/mktdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 01:55:16.285081 mktdata-0.0.2/models/
+-rw-rw-rw-   0        0        0        0 2024-05-18 03:54:40.000000 mktdata-0.0.2/models/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-22 01:55:16.286080 mktdata-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      375 2024-05-22 01:55:12.000000 mktdata-0.0.2/setup.py
```

### Comparing `mktdata-0.0.1/mktdata.egg-info/requires.txt` & `mktdata-0.0.2/mktdata.egg-info/requires.txt`

 * *Files identical despite different names*

