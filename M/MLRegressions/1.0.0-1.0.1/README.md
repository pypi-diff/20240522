# Comparing `tmp/MLRegressions-1.0.0.tar.gz` & `tmp/mlregressions-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLRegressions-1.0.0.tar", last modified: Fri Sep 22 07:49:51 2023, max compression
+gzip compressed data, was "mlregressions-1.0.1.tar", last modified: Wed May 22 07:58:39 2024, max compression
```

## Comparing `MLRegressions-1.0.0.tar` & `mlregressions-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-09-22 07:49:51.983842 MLRegressions-1.0.0/
--rw-rw-rw-   0        0        0     1095 2023-09-21 10:06:05.000000 MLRegressions-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1426 2023-09-22 07:49:51.981841 MLRegressions-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      850 2023-09-21 10:18:46.000000 MLRegressions-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-09-22 07:49:51.983842 MLRegressions-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      919 2023-09-22 07:48:58.000000 MLRegressions-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-22 07:49:51.930839 MLRegressions-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-09-22 07:49:51.961875 MLRegressions-1.0.0/src/ML/
--rw-rw-rw-   0        0        0   126464 2023-09-21 09:49:58.000000 MLRegressions-1.0.0/src/ML/MLRegressions.cp311-win_amd64.pyd
--rw-rw-rw-   0        0        0       34 2023-09-22 06:16:58.000000 MLRegressions-1.0.0/src/ML/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-22 07:49:51.979842 MLRegressions-1.0.0/src/MLRegressions.egg-info/
--rw-rw-rw-   0        0        0     1426 2023-09-22 07:49:51.000000 MLRegressions-1.0.0/src/MLRegressions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-09-22 07:49:51.000000 MLRegressions-1.0.0/src/MLRegressions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-22 07:49:51.000000 MLRegressions-1.0.0/src/MLRegressions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2023-09-22 07:49:51.000000 MLRegressions-1.0.0/src/MLRegressions.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 07:58:39.584399 mlregressions-1.0.1/
+-rw-rw-rw-   0        0        0     1095 2023-09-21 10:06:05.000000 mlregressions-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1425 2024-05-22 07:58:39.582406 mlregressions-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      850 2023-09-21 10:18:46.000000 mlregressions-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 07:58:39.584399 mlregressions-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      918 2024-05-22 07:52:12.000000 mlregressions-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:58:39.527141 mlregressions-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 07:58:39.561587 mlregressions-1.0.1/src/ML/
+-rw-rw-rw-   0        0        0   140288 2024-05-07 06:51:34.000000 mlregressions-1.0.1/src/ML/MLRegressions.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0        0 2024-05-07 05:55:54.000000 mlregressions-1.0.1/src/ML/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:58:39.580261 mlregressions-1.0.1/src/MLRegressions.egg-info/
+-rw-rw-rw-   0        0        0     1425 2024-05-22 07:58:39.000000 mlregressions-1.0.1/src/MLRegressions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2024-05-22 07:58:39.000000 mlregressions-1.0.1/src/MLRegressions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 07:58:39.000000 mlregressions-1.0.1/src/MLRegressions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2024-05-22 07:58:39.000000 mlregressions-1.0.1/src/MLRegressions.egg-info/top_level.txt
```

### Comparing `MLRegressions-1.0.0/LICENSE.txt` & `mlregressions-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MLRegressions-1.0.0/PKG-INFO` & `mlregressions-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: MLRegressions
-Version: 1.0.0
+Version: 1.0.1
 Summary: 5 ML Model are available to train bassed on provided dataset, user can select one regresion out of 5 for train.
 Author: DKVG
 Author-email: gadellidk@gmail.com
 Keywords: ML Regressions,MLRegressions Linear polynomial svr random-forest decision-tree regressors
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 from MLRegressions import Regressors
 
 Example:
```

### Comparing `MLRegressions-1.0.0/README.md` & `mlregressions-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `MLRegressions-1.0.0/setup.py` & `mlregressions-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="MLRegressions",
-    version="1.0.0",
+    version="1.0.1",
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
-    python_requires=">=3.11",
+    python_requires=">=3.9",
     keywords='ML Regressions, MLRegressions Linear polynomial svr random-forest decision-tree regressors',
 )
```

### Comparing `MLRegressions-1.0.0/src/MLRegressions.egg-info/PKG-INFO` & `mlregressions-1.0.1/src/MLRegressions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: MLRegressions
-Version: 1.0.0
+Version: 1.0.1
 Summary: 5 ML Model are available to train bassed on provided dataset, user can select one regresion out of 5 for train.
 Author: DKVG
 Author-email: gadellidk@gmail.com
 Keywords: ML Regressions,MLRegressions Linear polynomial svr random-forest decision-tree regressors
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 from MLRegressions import Regressors
 
 Example:
```

