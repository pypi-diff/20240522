# Comparing `tmp/jaanca_chronometer-0.0.1rc1.tar.gz` & `tmp/jaanca_chronometer-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca_chronometer-0.0.1rc1.tar", last modified: Wed May 22 00:48:30 2024, max compression
+gzip compressed data, was "jaanca_chronometer-0.0.1rc2.tar", last modified: Wed May 22 01:03:39 2024, max compression
```

## Comparing `jaanca_chronometer-0.0.1rc1.tar` & `jaanca_chronometer-0.0.1rc2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 00:48:30.238542 jaanca_chronometer-0.0.1rc1/
--rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 jaanca_chronometer-0.0.1rc1/LICENSE.txt
--rw-rw-rw-   0        0        0    12468 2024-05-22 00:48:30.237539 jaanca_chronometer-0.0.1rc1/PKG-INFO
--rw-rw-rw-   0        0        0    11204 2024-05-22 00:31:29.000000 jaanca_chronometer-0.0.1rc1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 00:48:30.217540 jaanca_chronometer-0.0.1rc1/jaanca_chronometer/
--rw-rw-rw-   0        0        0       70 2024-05-22 00:33:46.000000 jaanca_chronometer-0.0.1rc1/jaanca_chronometer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 00:48:30.227544 jaanca_chronometer-0.0.1rc1/jaanca_chronometer/utils/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.0.1rc1/jaanca_chronometer/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 00:48:30.232584 jaanca_chronometer-0.0.1rc1/jaanca_chronometer/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.0.1rc1/jaanca_chronometer/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     1537 2024-05-10 16:55:55.000000 jaanca_chronometer-0.0.1rc1/jaanca_chronometer/utils/helpers/chronometer.py
-drwxrwxrwx   0        0        0        0 2024-05-22 00:48:30.235541 jaanca_chronometer-0.0.1rc1/jaanca_chronometer.egg-info/
--rw-rw-rw-   0        0        0    12468 2024-05-22 00:48:30.000000 jaanca_chronometer-0.0.1rc1/jaanca_chronometer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2024-05-22 00:48:30.000000 jaanca_chronometer-0.0.1rc1/jaanca_chronometer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 00:48:30.000000 jaanca_chronometer-0.0.1rc1/jaanca_chronometer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-22 00:48:30.000000 jaanca_chronometer-0.0.1rc1/jaanca_chronometer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 00:48:30.239542 jaanca_chronometer-0.0.1rc1/setup.cfg
--rw-rw-rw-   0        0        0     1598 2024-05-22 00:43:51.000000 jaanca_chronometer-0.0.1rc1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:03:39.291732 jaanca_chronometer-0.0.1rc2/
+-rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 jaanca_chronometer-0.0.1rc2/LICENSE.txt
+-rw-rw-rw-   0        0        0     4480 2024-05-22 01:03:39.291732 jaanca_chronometer-0.0.1rc2/PKG-INFO
+-rw-rw-rw-   0        0        0     3216 2024-05-22 01:02:56.000000 jaanca_chronometer-0.0.1rc2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 01:03:39.272710 jaanca_chronometer-0.0.1rc2/jaanca_chronometer/
+-rw-rw-rw-   0        0        0       70 2024-05-22 00:33:46.000000 jaanca_chronometer-0.0.1rc2/jaanca_chronometer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:03:39.283722 jaanca_chronometer-0.0.1rc2/jaanca_chronometer/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.0.1rc2/jaanca_chronometer/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:03:39.287723 jaanca_chronometer-0.0.1rc2/jaanca_chronometer/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.0.1rc2/jaanca_chronometer/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1537 2024-05-10 16:55:55.000000 jaanca_chronometer-0.0.1rc2/jaanca_chronometer/utils/helpers/chronometer.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:03:39.289723 jaanca_chronometer-0.0.1rc2/jaanca_chronometer.egg-info/
+-rw-rw-rw-   0        0        0     4480 2024-05-22 01:03:39.000000 jaanca_chronometer-0.0.1rc2/jaanca_chronometer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2024-05-22 01:03:39.000000 jaanca_chronometer-0.0.1rc2/jaanca_chronometer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 01:03:39.000000 jaanca_chronometer-0.0.1rc2/jaanca_chronometer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-22 01:03:39.000000 jaanca_chronometer-0.0.1rc2/jaanca_chronometer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 01:03:39.293732 jaanca_chronometer-0.0.1rc2/setup.cfg
+-rw-rw-rw-   0        0        0     1598 2024-05-22 01:03:18.000000 jaanca_chronometer-0.0.1rc2/setup.py
```

### Comparing `jaanca_chronometer-0.0.1rc1/LICENSE.txt` & `jaanca_chronometer-0.0.1rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca_chronometer-0.0.1rc1/jaanca_chronometer/utils/helpers/chronometer.py` & `jaanca_chronometer-0.0.1rc2/jaanca_chronometer/utils/helpers/chronometer.py`

 * *Files identical despite different names*

### Comparing `jaanca_chronometer-0.0.1rc1/setup.py` & `jaanca_chronometer-0.0.1rc2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca-chronometer"
-VERSION = "0.0.1rc1"
+VERSION = "0.0.1rc2"
 
 install_requires = []
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'A tool library created by {COMPANY_NAME} that allows measuring the time between two moments in the source code.',
```

