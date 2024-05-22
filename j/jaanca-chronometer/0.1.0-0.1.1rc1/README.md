# Comparing `tmp/jaanca_chronometer-0.1.0.tar.gz` & `tmp/jaanca_chronometer-0.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca_chronometer-0.1.0.tar", last modified: Wed May 22 01:30:56 2024, max compression
+gzip compressed data, was "jaanca_chronometer-0.1.1rc1.tar", last modified: Wed May 22 02:12:59 2024, max compression
```

## Comparing `jaanca_chronometer-0.1.0.tar` & `jaanca_chronometer-0.1.1rc1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 01:30:56.166557 jaanca_chronometer-0.1.0/
--rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 jaanca_chronometer-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     4495 2024-05-22 01:30:56.165557 jaanca_chronometer-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3205 2024-05-22 01:18:07.000000 jaanca_chronometer-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 01:30:56.149511 jaanca_chronometer-0.1.0/jaanca_chronometer/
--rw-rw-rw-   0        0        0       70 2024-05-22 00:33:46.000000 jaanca_chronometer-0.1.0/jaanca_chronometer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 01:30:56.158558 jaanca_chronometer-0.1.0/jaanca_chronometer/utils/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.1.0/jaanca_chronometer/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 01:30:56.161558 jaanca_chronometer-0.1.0/jaanca_chronometer/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.1.0/jaanca_chronometer/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     1537 2024-05-10 16:55:55.000000 jaanca_chronometer-0.1.0/jaanca_chronometer/utils/helpers/chronometer.py
-drwxrwxrwx   0        0        0        0 2024-05-22 01:30:56.164558 jaanca_chronometer-0.1.0/jaanca_chronometer.egg-info/
--rw-rw-rw-   0        0        0     4495 2024-05-22 01:30:56.000000 jaanca_chronometer-0.1.0/jaanca_chronometer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2024-05-22 01:30:56.000000 jaanca_chronometer-0.1.0/jaanca_chronometer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 01:30:56.000000 jaanca_chronometer-0.1.0/jaanca_chronometer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-22 01:30:56.000000 jaanca_chronometer-0.1.0/jaanca_chronometer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 01:30:56.167826 jaanca_chronometer-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1624 2024-05-22 01:29:45.000000 jaanca_chronometer-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 02:12:59.041681 jaanca_chronometer-0.1.1rc1/
+-rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 jaanca_chronometer-0.1.1rc1/LICENSE.txt
+-rw-rw-rw-   0        0        0     4498 2024-05-22 02:12:59.040682 jaanca_chronometer-0.1.1rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     3205 2024-05-22 01:18:07.000000 jaanca_chronometer-0.1.1rc1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 02:12:59.022640 jaanca_chronometer-0.1.1rc1/jaanca_chronometer/
+-rw-rw-rw-   0        0        0       70 2024-05-22 00:33:46.000000 jaanca_chronometer-0.1.1rc1/jaanca_chronometer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 02:12:59.033789 jaanca_chronometer-0.1.1rc1/jaanca_chronometer/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.1.1rc1/jaanca_chronometer/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 02:12:59.036786 jaanca_chronometer-0.1.1rc1/jaanca_chronometer/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.1.1rc1/jaanca_chronometer/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1651 2024-05-22 02:12:10.000000 jaanca_chronometer-0.1.1rc1/jaanca_chronometer/utils/helpers/chronometer.py
+drwxrwxrwx   0        0        0        0 2024-05-22 02:12:59.038681 jaanca_chronometer-0.1.1rc1/jaanca_chronometer.egg-info/
+-rw-rw-rw-   0        0        0     4498 2024-05-22 02:12:58.000000 jaanca_chronometer-0.1.1rc1/jaanca_chronometer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2024-05-22 02:12:59.000000 jaanca_chronometer-0.1.1rc1/jaanca_chronometer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 02:12:58.000000 jaanca_chronometer-0.1.1rc1/jaanca_chronometer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-22 02:12:58.000000 jaanca_chronometer-0.1.1rc1/jaanca_chronometer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 02:12:59.042682 jaanca_chronometer-0.1.1rc1/setup.cfg
+-rw-rw-rw-   0        0        0     1627 2024-05-22 02:12:48.000000 jaanca_chronometer-0.1.1rc1/setup.py
```

### Comparing `jaanca_chronometer-0.1.0/LICENSE.txt` & `jaanca_chronometer-0.1.1rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca_chronometer-0.1.0/PKG-INFO` & `jaanca_chronometer-0.1.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-chronometer
-Version: 0.1.0
+Version: 0.1.1rc1
 Summary: A tool library created by jaanca that allows measuring the time between two moments in the source code.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-chronometer
 Author: Andres Cardona
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: timer stopwatch in interval format for databases
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jaanca_chronometer-0.1.0/README.md` & `jaanca_chronometer-0.1.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `jaanca_chronometer-0.1.0/jaanca_chronometer/utils/helpers/chronometer.py` & `jaanca_chronometer-0.1.1rc1/jaanca_chronometer/utils/helpers/chronometer.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         self.__end_time=0
     def get_elapsed_time(self)->Interval:
         '''Descripcion
         :return Interval(str): HH:mm:ss format supported for inserting records into databases and adding elapsed times
 
         ## Example
         ```Python
+        from jaanca_chronometer import Chronometer
         import time
 
         chronometer=Chronometer()
         chronometer.start()
         time.sleep(140)
         chronometer.stop()
         elapsed_time=str(chronometer.get_elapsed_time())
@@ -45,7 +46,9 @@
         '''
         elapsed_seconds = self.__end_time - self.__start_time
         hours = int(elapsed_seconds / 3600)
         minutes = int((elapsed_seconds % 3600) / 60)
         seconds = int(elapsed_seconds % 60)
         return Interval(hours, minutes, seconds)
 
+    def get_format_time(self)->str:
+        return "HH:mm:ss"
```

### Comparing `jaanca_chronometer-0.1.0/jaanca_chronometer.egg-info/PKG-INFO` & `jaanca_chronometer-0.1.1rc1/jaanca_chronometer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-chronometer
-Version: 0.1.0
+Version: 0.1.1rc1
 Summary: A tool library created by jaanca that allows measuring the time between two moments in the source code.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-chronometer
 Author: Andres Cardona
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: timer stopwatch in interval format for databases
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jaanca_chronometer-0.1.0/setup.py` & `jaanca_chronometer-0.1.1rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca-chronometer"
-VERSION = "0.1.0"
+VERSION = "0.1.1rc1"
 
 install_requires = []
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'A tool library created by {COMPANY_NAME} that allows measuring the time between two moments in the source code.',
```

