# Comparing `tmp/alpss-1.2.0.tar.gz` & `tmp/alpss-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpss-1.2.0.tar", last modified: Wed May 22 17:45:58 2024, max compression
+gzip compressed data, was "alpss-1.2.1.tar", last modified: Wed May 22 18:14:41 2024, max compression
```

## Comparing `alpss-1.2.0.tar` & `alpss-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 alirachidi   (501) staff       (20)        0 2024-05-22 17:45:58.673094 alpss-1.2.0/
-drwxr-xr-x   0 alirachidi   (501) staff       (20)        0 2024-05-22 17:45:58.670705 alpss-1.2.0/ALPSS/
--rw-r--r--   0 alirachidi   (501) staff       (20)        0 2024-04-26 15:08:10.000000 alpss-1.2.0/ALPSS/__init__.py
--rw-r--r--   0 alirachidi   (501) staff       (20)     3295 2024-04-26 15:05:32.000000 alpss-1.2.0/ALPSS/alpss_auto_run.py
--rw-r--r--   0 alirachidi   (501) staff       (20)    55169 2024-05-03 18:56:56.000000 alpss-1.2.0/ALPSS/alpss_main.py
--rw-r--r--   0 alirachidi   (501) staff       (20)     6527 2024-05-22 17:08:41.000000 alpss-1.2.0/ALPSS/alpss_run.py
-drwxr-xr-x   0 alirachidi   (501) staff       (20)        0 2024-05-22 17:45:58.672533 alpss-1.2.0/ALPSS.egg-info/
--rw-r--r--   0 alirachidi   (501) staff       (20)      979 2024-05-22 17:45:58.000000 alpss-1.2.0/ALPSS.egg-info/PKG-INFO
--rw-r--r--   0 alirachidi   (501) staff       (20)      275 2024-05-22 17:45:58.000000 alpss-1.2.0/ALPSS.egg-info/SOURCES.txt
--rw-r--r--   0 alirachidi   (501) staff       (20)        1 2024-05-22 17:45:58.000000 alpss-1.2.0/ALPSS.egg-info/dependency_links.txt
--rw-r--r--   0 alirachidi   (501) staff       (20)        7 2024-05-22 17:45:58.000000 alpss-1.2.0/ALPSS.egg-info/requires.txt
--rw-r--r--   0 alirachidi   (501) staff       (20)        6 2024-05-22 17:45:58.000000 alpss-1.2.0/ALPSS.egg-info/top_level.txt
--rw-r--r--   0 alirachidi   (501) staff       (20)    35149 2024-04-26 14:41:10.000000 alpss-1.2.0/LICENSE.md
--rw-r--r--   0 alirachidi   (501) staff       (20)      979 2024-05-22 17:45:58.672844 alpss-1.2.0/PKG-INFO
--rw-r--r--   0 alirachidi   (501) staff       (20)    10106 2024-05-22 17:42:11.000000 alpss-1.2.0/README.md
--rw-r--r--   0 alirachidi   (501) staff       (20)       38 2024-05-22 17:45:58.673156 alpss-1.2.0/setup.cfg
--rw-r--r--   0 alirachidi   (501) staff       (20)     1477 2024-05-03 17:48:40.000000 alpss-1.2.0/setup.py
-drwxr-xr-x   0 alirachidi   (501) staff       (20)        0 2024-05-22 17:45:58.672054 alpss-1.2.0/tests/
--rw-r--r--   0 alirachidi   (501) staff       (20)     1831 2024-05-03 17:24:25.000000 alpss-1.2.0/tests/test_inputs.py
+drwxr-xr-x   0 alirachidi   (501) staff       (20)        0 2024-05-22 18:14:41.250913 alpss-1.2.1/
+drwxr-xr-x   0 alirachidi   (501) staff       (20)        0 2024-05-22 18:14:41.248766 alpss-1.2.1/ALPSS/
+-rw-r--r--   0 alirachidi   (501) staff       (20)        0 2024-04-26 15:08:10.000000 alpss-1.2.1/ALPSS/__init__.py
+-rw-r--r--   0 alirachidi   (501) staff       (20)     3295 2024-04-26 15:05:32.000000 alpss-1.2.1/ALPSS/alpss_auto_run.py
+-rw-r--r--   0 alirachidi   (501) staff       (20)    55169 2024-05-03 18:56:56.000000 alpss-1.2.1/ALPSS/alpss_main.py
+-rw-r--r--   0 alirachidi   (501) staff       (20)     2222 2024-05-22 17:44:37.000000 alpss-1.2.1/ALPSS/alpss_run.ipynb
+-rw-r--r--   0 alirachidi   (501) staff       (20)     6527 2024-05-22 17:08:41.000000 alpss-1.2.1/ALPSS/alpss_run.py
+drwxr-xr-x   0 alirachidi   (501) staff       (20)        0 2024-05-22 18:14:41.250285 alpss-1.2.1/ALPSS.egg-info/
+-rw-r--r--   0 alirachidi   (501) staff       (20)      979 2024-05-22 18:14:41.000000 alpss-1.2.1/ALPSS.egg-info/PKG-INFO
+-rw-r--r--   0 alirachidi   (501) staff       (20)      309 2024-05-22 18:14:41.000000 alpss-1.2.1/ALPSS.egg-info/SOURCES.txt
+-rw-r--r--   0 alirachidi   (501) staff       (20)        1 2024-05-22 18:14:41.000000 alpss-1.2.1/ALPSS.egg-info/dependency_links.txt
+-rw-r--r--   0 alirachidi   (501) staff       (20)        7 2024-05-22 18:14:41.000000 alpss-1.2.1/ALPSS.egg-info/requires.txt
+-rw-r--r--   0 alirachidi   (501) staff       (20)        6 2024-05-22 18:14:41.000000 alpss-1.2.1/ALPSS.egg-info/top_level.txt
+-rw-r--r--   0 alirachidi   (501) staff       (20)    35149 2024-04-26 14:41:10.000000 alpss-1.2.1/LICENSE.md
+-rw-r--r--   0 alirachidi   (501) staff       (20)       30 2024-05-22 18:13:21.000000 alpss-1.2.1/MANIFEST.in
+-rw-r--r--   0 alirachidi   (501) staff       (20)      979 2024-05-22 18:14:41.250623 alpss-1.2.1/PKG-INFO
+-rw-r--r--   0 alirachidi   (501) staff       (20)    10106 2024-05-22 17:42:11.000000 alpss-1.2.1/README.md
+-rw-r--r--   0 alirachidi   (501) staff       (20)       38 2024-05-22 18:14:41.250987 alpss-1.2.1/setup.cfg
+-rw-r--r--   0 alirachidi   (501) staff       (20)     1615 2024-05-22 18:11:59.000000 alpss-1.2.1/setup.py
+drwxr-xr-x   0 alirachidi   (501) staff       (20)        0 2024-05-22 18:14:41.249778 alpss-1.2.1/tests/
+-rw-r--r--   0 alirachidi   (501) staff       (20)     1831 2024-05-03 17:24:25.000000 alpss-1.2.1/tests/test_inputs.py
```

### Comparing `alpss-1.2.0/ALPSS/alpss_auto_run.py` & `alpss-1.2.1/ALPSS/alpss_auto_run.py`

 * *Files identical despite different names*

### Comparing `alpss-1.2.0/ALPSS/alpss_main.py` & `alpss-1.2.1/ALPSS/alpss_main.py`

 * *Files identical despite different names*

### Comparing `alpss-1.2.0/ALPSS/alpss_run.py` & `alpss-1.2.1/ALPSS/alpss_run.py`

 * *Files identical despite different names*

### Comparing `alpss-1.2.0/ALPSS.egg-info/PKG-INFO` & `alpss-1.2.1/ALPSS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ALPSS
-Version: 1.2.0
+Version: 1.2.1
 Summary: Program for the automated analysis of photonic Doppler velocimetry spall signals with uncertainty. 
 Home-page: https://github.com/Jake-Diamond-9/ALPSS
 Author: Jacob M. Diamond
 Author-email: jdiamo15@jhu.edu
 License: GNU GPLv3
 Keywords: pdv,spall,high throughput,automated
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `alpss-1.2.0/LICENSE.md` & `alpss-1.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alpss-1.2.0/PKG-INFO` & `alpss-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ALPSS
-Version: 1.2.0
+Version: 1.2.1
 Summary: Program for the automated analysis of photonic Doppler velocimetry spall signals with uncertainty. 
 Home-page: https://github.com/Jake-Diamond-9/ALPSS
 Author: Jacob M. Diamond
 Author-email: jdiamo15@jhu.edu
 License: GNU GPLv3
 Keywords: pdv,spall,high throughput,automated
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `alpss-1.2.0/README.md` & `alpss-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `alpss-1.2.0/setup.py` & `alpss-1.2.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # imports
 import pathlib
 import setuptools
 
-version = "1.2.0"
+version = "1.2.1"
 
 long_description = "ALPSS is a program that is designed to automatically process PDV spall signals and will allow us to keep up with high-throughput experiments. ALPSS is also designed to function as a standalone spall signal processing program. All potential inputs are located within a single function, making it easy to adjust parameters and quickly assess results."
 setupkwargs = dict(
     name="ALPSS",
     packages=setuptools.find_packages(include=["ALPSS*"]),
     include_package_data=True,
     version=version,
     description=(
         "Program for the automated analysis of photonic Doppler velocimetry spall signals with uncertainty. "
     ),
+    package_data={
+        # Include any .ipynb files in the notebooks directory
+        'ALPSS': ['ALPSS/alpss_run.ipynb.ipynb'],
+    },
     long_description=long_description,
     author="Jacob M. Diamond",
     author_email="jdiamo15@jhu.edu",
     url="https://github.com/Jake-Diamond-9/ALPSS",
     # download_url=f",
     license="GNU GPLv3",
     python_requires=">=3.7,<=3.10",
```

### Comparing `alpss-1.2.0/tests/test_inputs.py` & `alpss-1.2.1/tests/test_inputs.py`

 * *Files identical despite different names*

