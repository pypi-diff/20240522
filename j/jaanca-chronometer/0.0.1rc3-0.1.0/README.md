# Comparing `tmp/jaanca_chronometer-0.0.1rc3.tar.gz` & `tmp/jaanca_chronometer-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca_chronometer-0.0.1rc3.tar", last modified: Wed May 22 01:19:40 2024, max compression
+gzip compressed data, was "jaanca_chronometer-0.1.0.tar", last modified: Wed May 22 01:30:56 2024, max compression
```

## Comparing `jaanca_chronometer-0.0.1rc3.tar` & `jaanca_chronometer-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 01:19:40.027385 jaanca_chronometer-0.0.1rc3/
--rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 jaanca_chronometer-0.0.1rc3/LICENSE.txt
--rw-rw-rw-   0        0        0     4498 2024-05-22 01:19:40.026370 jaanca_chronometer-0.0.1rc3/PKG-INFO
--rw-rw-rw-   0        0        0     3205 2024-05-22 01:18:07.000000 jaanca_chronometer-0.0.1rc3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 01:19:40.007658 jaanca_chronometer-0.0.1rc3/jaanca_chronometer/
--rw-rw-rw-   0        0        0       70 2024-05-22 00:33:46.000000 jaanca_chronometer-0.0.1rc3/jaanca_chronometer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 01:19:40.017629 jaanca_chronometer-0.0.1rc3/jaanca_chronometer/utils/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.0.1rc3/jaanca_chronometer/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 01:19:40.021366 jaanca_chronometer-0.0.1rc3/jaanca_chronometer/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.0.1rc3/jaanca_chronometer/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     1537 2024-05-10 16:55:55.000000 jaanca_chronometer-0.0.1rc3/jaanca_chronometer/utils/helpers/chronometer.py
-drwxrwxrwx   0        0        0        0 2024-05-22 01:19:40.025366 jaanca_chronometer-0.0.1rc3/jaanca_chronometer.egg-info/
--rw-rw-rw-   0        0        0     4498 2024-05-22 01:19:39.000000 jaanca_chronometer-0.0.1rc3/jaanca_chronometer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2024-05-22 01:19:39.000000 jaanca_chronometer-0.0.1rc3/jaanca_chronometer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 01:19:39.000000 jaanca_chronometer-0.0.1rc3/jaanca_chronometer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-22 01:19:39.000000 jaanca_chronometer-0.0.1rc3/jaanca_chronometer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 01:19:40.029367 jaanca_chronometer-0.0.1rc3/setup.cfg
--rw-rw-rw-   0        0        0     1627 2024-05-22 01:19:19.000000 jaanca_chronometer-0.0.1rc3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:30:56.166557 jaanca_chronometer-0.1.0/
+-rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 jaanca_chronometer-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     4495 2024-05-22 01:30:56.165557 jaanca_chronometer-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3205 2024-05-22 01:18:07.000000 jaanca_chronometer-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 01:30:56.149511 jaanca_chronometer-0.1.0/jaanca_chronometer/
+-rw-rw-rw-   0        0        0       70 2024-05-22 00:33:46.000000 jaanca_chronometer-0.1.0/jaanca_chronometer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:30:56.158558 jaanca_chronometer-0.1.0/jaanca_chronometer/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.1.0/jaanca_chronometer/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:30:56.161558 jaanca_chronometer-0.1.0/jaanca_chronometer/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.1.0/jaanca_chronometer/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1537 2024-05-10 16:55:55.000000 jaanca_chronometer-0.1.0/jaanca_chronometer/utils/helpers/chronometer.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:30:56.164558 jaanca_chronometer-0.1.0/jaanca_chronometer.egg-info/
+-rw-rw-rw-   0        0        0     4495 2024-05-22 01:30:56.000000 jaanca_chronometer-0.1.0/jaanca_chronometer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2024-05-22 01:30:56.000000 jaanca_chronometer-0.1.0/jaanca_chronometer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 01:30:56.000000 jaanca_chronometer-0.1.0/jaanca_chronometer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-22 01:30:56.000000 jaanca_chronometer-0.1.0/jaanca_chronometer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 01:30:56.167826 jaanca_chronometer-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1624 2024-05-22 01:29:45.000000 jaanca_chronometer-0.1.0/setup.py
```

### Comparing `jaanca_chronometer-0.0.1rc3/LICENSE.txt` & `jaanca_chronometer-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca_chronometer-0.0.1rc3/PKG-INFO` & `jaanca_chronometer-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-chronometer
-Version: 0.0.1rc3
+Version: 0.1.0
 Summary: A tool library created by jaanca that allows measuring the time between two moments in the source code.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-chronometer
 Author: Andres Cardona
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: timer stopwatch in interval format for databases
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jaanca_chronometer-0.0.1rc3/README.md` & `jaanca_chronometer-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `jaanca_chronometer-0.0.1rc3/jaanca_chronometer/utils/helpers/chronometer.py` & `jaanca_chronometer-0.1.0/jaanca_chronometer/utils/helpers/chronometer.py`

 * *Files identical despite different names*

### Comparing `jaanca_chronometer-0.0.1rc3/jaanca_chronometer.egg-info/PKG-INFO` & `jaanca_chronometer-0.1.0/jaanca_chronometer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-chronometer
-Version: 0.0.1rc3
+Version: 0.1.0
 Summary: A tool library created by jaanca that allows measuring the time between two moments in the source code.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-chronometer
 Author: Andres Cardona
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: timer stopwatch in interval format for databases
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jaanca_chronometer-0.0.1rc3/setup.py` & `jaanca_chronometer-0.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca-chronometer"
-VERSION = "0.0.1rc3"
+VERSION = "0.1.0"
 
 install_requires = []
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'A tool library created by {COMPANY_NAME} that allows measuring the time between two moments in the source code.',
```

