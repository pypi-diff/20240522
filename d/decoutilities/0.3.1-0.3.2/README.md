# Comparing `tmp/decoutilities-0.3.1.tar.gz` & `tmp/decoutilities-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoutilities-0.3.1.tar", last modified: Wed May 22 10:32:12 2024, max compression
+gzip compressed data, was "decoutilities-0.3.2.tar", last modified: Wed May 22 19:14:54 2024, max compression
```

## Comparing `decoutilities-0.3.1.tar` & `decoutilities-0.3.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 10:32:12.674676 decoutilities-0.3.1/
--rw-rw-rw-   0        0        0     1089 2024-05-08 11:01:18.000000 decoutilities-0.3.1/LICENSE
--rw-rw-rw-   0        0        0    19893 2024-05-22 10:32:12.658675 decoutilities-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    19410 2024-05-22 10:30:33.000000 decoutilities-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 10:32:12.102678 decoutilities-0.3.1/decoutilities/
--rw-rw-rw-   0        0        0     4740 2024-05-07 07:54:09.000000 decoutilities-0.3.1/decoutilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 10:32:12.325675 decoutilities-0.3.1/decoutilities/config/
--rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.3.1/decoutilities/config/__init__.py
--rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.3.1/decoutilities/config/config.py
--rw-rw-rw-   0        0        0     2736 2024-04-30 08:27:33.000000 decoutilities-0.3.1/decoutilities/config/configContainer.py
-drwxrwxrwx   0        0        0        0 2024-05-22 10:32:12.449679 decoutilities-0.3.1/decoutilities/data/
--rw-rw-rw-   0        0        0      104 2024-05-08 07:57:21.000000 decoutilities-0.3.1/decoutilities/data/__init__.py
--rw-rw-rw-   0        0        0     2154 2024-05-08 07:56:33.000000 decoutilities-0.3.1/decoutilities/data/dataEncryptor.py
--rw-rw-rw-   0        0        0     1671 2024-05-08 07:52:43.000000 decoutilities-0.3.1/decoutilities/data/keyManager.py
-drwxrwxrwx   0        0        0        0 2024-05-22 10:32:12.507673 decoutilities-0.3.1/decoutilities/inject/
--rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.3.1/decoutilities/inject/__init__.py
--rw-rw-rw-   0        0        0      569 2024-05-20 10:37:54.000000 decoutilities-0.3.1/decoutilities/inject/injector.py
-drwxrwxrwx   0        0        0        0 2024-05-22 10:32:12.551674 decoutilities-0.3.1/decoutilities/logger/
--rw-rw-rw-   0        0        0     1221 2024-05-21 05:28:53.000000 decoutilities-0.3.1/decoutilities/logger/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 10:32:12.597676 decoutilities-0.3.1/decoutilities/queue/
--rw-rw-rw-   0        0        0     1043 2024-05-07 08:05:33.000000 decoutilities-0.3.1/decoutilities/queue/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 10:32:12.614677 decoutilities-0.3.1/decoutilities/textUtils/
--rw-rw-rw-   0        0        0     2832 2024-05-21 06:12:32.000000 decoutilities-0.3.1/decoutilities/textUtils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 10:32:12.627679 decoutilities-0.3.1/decoutilities.egg-info/
--rw-rw-rw-   0        0        0    19893 2024-05-22 10:32:11.000000 decoutilities-0.3.1/decoutilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      571 2024-05-22 10:32:11.000000 decoutilities-0.3.1/decoutilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 10:32:11.000000 decoutilities-0.3.1/decoutilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-22 10:32:11.000000 decoutilities-0.3.1/decoutilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 10:32:12.675674 decoutilities-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      729 2024-05-22 10:30:56.000000 decoutilities-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 19:14:54.783233 decoutilities-0.3.2/
+-rw-rw-rw-   0        0        0     1089 2024-05-08 22:21:06.000000 decoutilities-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0    19893 2024-05-22 19:14:54.781130 decoutilities-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    19410 2024-05-22 19:14:30.000000 decoutilities-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 19:14:54.759403 decoutilities-0.3.2/decoutilities/
+-rw-rw-rw-   0        0        0     4740 2024-05-08 22:21:06.000000 decoutilities-0.3.2/decoutilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 19:14:54.767849 decoutilities-0.3.2/decoutilities/config/
+-rw-rw-rw-   0        0        0      104 2024-05-08 22:21:06.000000 decoutilities-0.3.2/decoutilities/config/__init__.py
+-rw-rw-rw-   0        0        0      994 2024-05-08 22:21:06.000000 decoutilities-0.3.2/decoutilities/config/config.py
+-rw-rw-rw-   0        0        0     2736 2024-05-08 22:21:06.000000 decoutilities-0.3.2/decoutilities/config/configContainer.py
+drwxrwxrwx   0        0        0        0 2024-05-22 19:14:54.770998 decoutilities-0.3.2/decoutilities/data/
+-rw-rw-rw-   0        0        0      104 2024-05-08 22:21:06.000000 decoutilities-0.3.2/decoutilities/data/__init__.py
+-rw-rw-rw-   0        0        0     2154 2024-05-08 22:21:06.000000 decoutilities-0.3.2/decoutilities/data/dataEncryptor.py
+-rw-rw-rw-   0        0        0     1671 2024-05-08 22:21:06.000000 decoutilities-0.3.2/decoutilities/data/keyManager.py
+drwxrwxrwx   0        0        0        0 2024-05-22 19:14:54.774739 decoutilities-0.3.2/decoutilities/inject/
+-rw-rw-rw-   0        0        0       44 2024-05-08 22:21:06.000000 decoutilities-0.3.2/decoutilities/inject/__init__.py
+-rw-rw-rw-   0        0        0      569 2024-05-18 20:23:23.000000 decoutilities-0.3.2/decoutilities/inject/injector.py
+drwxrwxrwx   0        0        0        0 2024-05-22 19:14:54.775799 decoutilities-0.3.2/decoutilities/logger/
+-rw-rw-rw-   0        0        0     1221 2024-05-22 19:14:30.000000 decoutilities-0.3.2/decoutilities/logger/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 19:14:54.777912 decoutilities-0.3.2/decoutilities/queue/
+-rw-rw-rw-   0        0        0     1043 2024-05-08 22:21:06.000000 decoutilities-0.3.2/decoutilities/queue/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 19:14:54.778983 decoutilities-0.3.2/decoutilities/textUtils/
+-rw-rw-rw-   0        0        0     2832 2024-05-22 19:14:30.000000 decoutilities-0.3.2/decoutilities/textUtils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 19:14:54.781130 decoutilities-0.3.2/decoutilities.egg-info/
+-rw-rw-rw-   0        0        0    19893 2024-05-22 19:14:54.000000 decoutilities-0.3.2/decoutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      571 2024-05-22 19:14:54.000000 decoutilities-0.3.2/decoutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 19:14:54.000000 decoutilities-0.3.2/decoutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-22 19:14:54.000000 decoutilities-0.3.2/decoutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 19:14:54.783233 decoutilities-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-05-22 19:14:30.000000 decoutilities-0.3.2/setup.py
```

### Comparing `decoutilities-0.3.1/LICENSE` & `decoutilities-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.1/PKG-INFO` & `decoutilities-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.3.1
+Version: 0.3.2
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `decoutilities-0.3.1/README.md` & `decoutilities-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.1/decoutilities/__init__.py` & `decoutilities-0.3.2/decoutilities/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.1/decoutilities/config/config.py` & `decoutilities-0.3.2/decoutilities/config/config.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.1/decoutilities/config/configContainer.py` & `decoutilities-0.3.2/decoutilities/config/configContainer.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.1/decoutilities/data/dataEncryptor.py` & `decoutilities-0.3.2/decoutilities/data/dataEncryptor.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.1/decoutilities/data/keyManager.py` & `decoutilities-0.3.2/decoutilities/data/keyManager.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.1/decoutilities/inject/injector.py` & `decoutilities-0.3.2/decoutilities/inject/injector.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.1/decoutilities/logger/__init__.py` & `decoutilities-0.3.2/decoutilities/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.1/decoutilities/queue/__init__.py` & `decoutilities-0.3.2/decoutilities/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.1/decoutilities/textUtils/__init__.py` & `decoutilities-0.3.2/decoutilities/textUtils/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.1/decoutilities.egg-info/PKG-INFO` & `decoutilities-0.3.2/decoutilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.3.1
+Version: 0.3.2
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `decoutilities-0.3.1/decoutilities.egg-info/SOURCES.txt` & `decoutilities-0.3.2/decoutilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.1/setup.py` & `decoutilities-0.3.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
 name='decoutilities',
-version='0.3.1',
+version='0.3.2',
 author='Hugo Torres',
 author_email='contact@redactado.es',
 description='Enhance the readability of your code with decorators and simplify the creation of configuration files.',
 packages=find_packages(include=['decoutilities', 'decoutilities.*']),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
```

