# Comparing `tmp/mlregressions-1.0.2.tar.gz` & `tmp/mlregressions-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlregressions-1.0.2.tar", last modified: Wed May 22 09:10:10 2024, max compression
+gzip compressed data, was "mlregressions-1.0.3.tar", last modified: Wed May 22 09:43:21 2024, max compression
```

## Comparing `mlregressions-1.0.2.tar` & `mlregressions-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 09:10:10.500308 mlregressions-1.0.2/
--rw-rw-rw-   0        0        0     1095 2023-09-21 10:06:05.000000 mlregressions-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1425 2024-05-22 09:10:10.498740 mlregressions-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      850 2023-09-21 10:18:46.000000 mlregressions-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-22 09:10:10.500308 mlregressions-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      918 2024-05-22 09:09:51.000000 mlregressions-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:10:10.469360 mlregressions-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-22 09:10:10.477600 mlregressions-1.0.2/src/ML/
--rw-rw-rw-   0        0        0   140288 2024-05-07 06:51:34.000000 mlregressions-1.0.2/src/ML/MLRegressions.cp39-win_amd64.pyd
--rw-rw-rw-   0        0        0        0 2024-05-07 05:55:54.000000 mlregressions-1.0.2/src/ML/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:10:10.496747 mlregressions-1.0.2/src/MLRegressions.egg-info/
--rw-rw-rw-   0        0        0     1425 2024-05-22 09:10:10.000000 mlregressions-1.0.2/src/MLRegressions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2024-05-22 09:10:10.000000 mlregressions-1.0.2/src/MLRegressions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 09:10:10.000000 mlregressions-1.0.2/src/MLRegressions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2024-05-22 09:10:10.000000 mlregressions-1.0.2/src/MLRegressions.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 09:43:21.501559 mlregressions-1.0.3/
+-rw-rw-rw-   0        0        0     1095 2023-09-21 10:06:05.000000 mlregressions-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1426 2024-05-22 09:43:21.499533 mlregressions-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      850 2023-09-21 10:18:46.000000 mlregressions-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 09:43:21.501559 mlregressions-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      919 2024-05-22 09:14:56.000000 mlregressions-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:43:21.455323 mlregressions-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 09:43:21.477275 mlregressions-1.0.3/src/ML/
+-rw-rw-rw-   0        0        0   126464 2023-09-21 09:49:58.000000 mlregressions-1.0.3/src/ML/MLRegressions.cp311-win_amd64.pyd
+-rw-rw-rw-   0        0        0        0 2024-05-07 05:55:54.000000 mlregressions-1.0.3/src/ML/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:43:21.497413 mlregressions-1.0.3/src/MLRegressions.egg-info/
+-rw-rw-rw-   0        0        0     1426 2024-05-22 09:43:21.000000 mlregressions-1.0.3/src/MLRegressions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-22 09:43:21.000000 mlregressions-1.0.3/src/MLRegressions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 09:43:21.000000 mlregressions-1.0.3/src/MLRegressions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2024-05-22 09:43:21.000000 mlregressions-1.0.3/src/MLRegressions.egg-info/top_level.txt
```

### Comparing `mlregressions-1.0.2/LICENSE.txt` & `mlregressions-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlregressions-1.0.2/PKG-INFO` & `mlregressions-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: MLRegressions
-Version: 1.0.2
+Version: 1.0.3
 Summary: 5 ML Model are available to train bassed on provided dataset, user can select one regresion out of 5 for train.
 Author: DKVG
 Author-email: gadellidk@gmail.com
 Keywords: ML Regressions,MLRegressions Linear polynomial svr random-forest decision-tree regressors
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: ==3.9
+Requires-Python: ==3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 from MLRegressions import Regressors
 
 Example:
```

### Comparing `mlregressions-1.0.2/README.md` & `mlregressions-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mlregressions-1.0.2/setup.py` & `mlregressions-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="MLRegressions",
-    version="1.0.2",
+    version="1.0.3",
     author="DKVG",
     author_email="gadellidk@gmail.com",
     description="5 ML Model are available to train bassed on provided dataset, user can select one regresion out of 5 "
                 "for train.",
     long_description=long_description,
     package_data={'': ['*']},
     include_package_data=True,
@@ -17,10 +17,10 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
-    python_requires="==3.9",
+    python_requires="==3.10",
     keywords='ML Regressions, MLRegressions Linear polynomial svr random-forest decision-tree regressors',
 )
```

### Comparing `mlregressions-1.0.2/src/MLRegressions.egg-info/PKG-INFO` & `mlregressions-1.0.3/src/MLRegressions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: MLRegressions
-Version: 1.0.2
+Version: 1.0.3
 Summary: 5 ML Model are available to train bassed on provided dataset, user can select one regresion out of 5 for train.
 Author: DKVG
 Author-email: gadellidk@gmail.com
 Keywords: ML Regressions,MLRegressions Linear polynomial svr random-forest decision-tree regressors
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: ==3.9
+Requires-Python: ==3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 from MLRegressions import Regressors
 
 Example:
```

