# Comparing `tmp/verifact-0.0.2.tar.gz` & `tmp/verifact-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verifact-0.0.2.tar", last modified: Wed May 22 17:59:10 2024, max compression
+gzip compressed data, was "verifact-0.0.3.tar", last modified: Wed May 22 19:16:07 2024, max compression
```

## Comparing `verifact-0.0.2.tar` & `verifact-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 yekyungkim (32790) yekyungkim (32790)        0 2024-05-22 17:59:10.262805 verifact-0.0.2/
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)     1068 2024-05-21 17:48:27.000000 verifact-0.0.2/LICENSE
--rw-r--r--   0 yekyungkim (32790) yekyungkim (32790)      521 2024-05-22 17:59:10.262805 verifact-0.0.2/PKG-INFO
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       11 2024-05-21 17:48:27.000000 verifact-0.0.2/README.md
-drwxrwxr-x   0 yekyungkim (32790) yekyungkim (32790)        0 2024-05-22 17:59:10.262805 verifact-0.0.2/VeriFact.egg-info/
--rw-r--r--   0 yekyungkim (32790) yekyungkim (32790)      521 2024-05-22 17:59:10.000000 verifact-0.0.2/VeriFact.egg-info/PKG-INFO
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)      185 2024-05-22 17:59:10.000000 verifact-0.0.2/VeriFact.egg-info/SOURCES.txt
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)        1 2024-05-22 17:59:10.000000 verifact-0.0.2/VeriFact.egg-info/dependency_links.txt
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       31 2024-05-22 17:59:10.000000 verifact-0.0.2/VeriFact.egg-info/requires.txt
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)        1 2024-05-22 17:59:10.000000 verifact-0.0.2/VeriFact.egg-info/top_level.txt
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       38 2024-05-22 17:59:10.262805 verifact-0.0.2/setup.cfg
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)      684 2024-05-22 17:57:47.000000 verifact-0.0.2/setup.py
+drwxrwxr-x   0 yekyungkim (32790) yekyungkim (32790)        0 2024-05-22 19:16:07.549517 verifact-0.0.3/
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)     1068 2024-05-21 17:48:27.000000 verifact-0.0.3/LICENSE
+-rw-r--r--   0 yekyungkim (32790) yekyungkim (32790)      521 2024-05-22 19:16:07.549517 verifact-0.0.3/PKG-INFO
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       11 2024-05-21 17:48:27.000000 verifact-0.0.3/README.md
+drwxrwxr-x   0 yekyungkim (32790) yekyungkim (32790)        0 2024-05-22 19:16:07.549517 verifact-0.0.3/VeriFact.egg-info/
+-rw-r--r--   0 yekyungkim (32790) yekyungkim (32790)      521 2024-05-22 19:16:07.000000 verifact-0.0.3/VeriFact.egg-info/PKG-INFO
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)      185 2024-05-22 19:16:07.000000 verifact-0.0.3/VeriFact.egg-info/SOURCES.txt
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)        1 2024-05-22 19:16:07.000000 verifact-0.0.3/VeriFact.egg-info/dependency_links.txt
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       31 2024-05-22 19:16:07.000000 verifact-0.0.3/VeriFact.egg-info/requires.txt
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)        1 2024-05-22 19:16:07.000000 verifact-0.0.3/VeriFact.egg-info/top_level.txt
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       38 2024-05-22 19:16:07.549517 verifact-0.0.3/setup.cfg
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)      684 2024-05-22 19:15:44.000000 verifact-0.0.3/setup.py
```

### Comparing `verifact-0.0.2/LICENSE` & `verifact-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `verifact-0.0.2/PKG-INFO` & `verifact-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VeriFact
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pip package for Verifact
 Home-page: https://github.com/mungg/VeriScore
 Author: Yixio Song
 Author-email: yixiaosong@umass.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `verifact-0.0.2/VeriFact.egg-info/PKG-INFO` & `verifact-0.0.3/VeriFact.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VeriFact
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pip package for Verifact
 Home-page: https://github.com/mungg/VeriScore
 Author: Yixio Song
 Author-email: yixiaosong@umass.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `verifact-0.0.2/setup.py` & `verifact-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
    name="VeriFact",
-   version="0.0.2",
+   version="0.0.3",
    packages=find_packages(),
    install_requires=[
        #'requests', 'numpy'
       'openai',
       'anthropic',
       'tiktoken',
       'tqdm'
```

