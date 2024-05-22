# Comparing `tmp/antspynet-0.2.5.tar.gz` & `tmp/antspynet-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antspynet-0.2.5.tar", last modified: Wed May 22 14:38:01 2024, max compression
+gzip compressed data, was "antspynet-0.2.6.tar", last modified: Wed May 22 16:29:27 2024, max compression
```

## Comparing `antspynet-0.2.5.tar` & `antspynet-0.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-22 14:38:01.101995 antspynet-0.2.5/
--rw-r--r--   0 stnava     (501) staff       (20)    11357 2023-06-06 13:36:51.000000 antspynet-0.2.5/LICENSE.md
--rw-r--r--   0 stnava     (501) staff       (20)    11858 2024-05-22 14:38:01.101791 antspynet-0.2.5/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)    11027 2024-05-22 14:29:17.000000 antspynet-0.2.5/README.md
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-22 14:38:01.100848 antspynet-0.2.5/antspynet/
--rw-r--r--   0 stnava     (501) staff       (20)      130 2024-05-22 13:48:43.000000 antspynet-0.2.5/antspynet/__init__.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-22 14:38:01.101616 antspynet-0.2.5/antspynet.egg-info/
--rw-r--r--   0 stnava     (501) staff       (20)    11858 2024-05-22 14:38:01.000000 antspynet-0.2.5/antspynet.egg-info/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)      221 2024-05-22 14:38:01.000000 antspynet-0.2.5/antspynet.egg-info/SOURCES.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2024-05-22 14:38:01.000000 antspynet-0.2.5/antspynet.egg-info/dependency_links.txt
--rw-r--r--   0 stnava     (501) staff       (20)       83 2024-05-22 14:38:01.000000 antspynet-0.2.5/antspynet.egg-info/requires.txt
--rw-r--r--   0 stnava     (501) staff       (20)       10 2024-05-22 14:38:01.000000 antspynet-0.2.5/antspynet.egg-info/top_level.txt
--rw-r--r--   0 stnava     (501) staff       (20)      976 2024-05-22 14:27:59.000000 antspynet-0.2.5/pyproject.toml
--rw-r--r--   0 stnava     (501) staff       (20)       38 2024-05-22 14:38:01.102038 antspynet-0.2.5/setup.cfg
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-22 16:29:27.990886 antspynet-0.2.6/
+-rw-r--r--   0 stnava     (501) staff       (20)    11357 2023-06-06 13:36:51.000000 antspynet-0.2.6/LICENSE.md
+-rw-r--r--   0 stnava     (501) staff       (20)    11985 2024-05-22 16:29:27.990697 antspynet-0.2.6/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)    11162 2024-05-22 16:19:40.000000 antspynet-0.2.6/README.md
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-22 16:29:27.989716 antspynet-0.2.6/antspynet/
+-rw-r--r--   0 stnava     (501) staff       (20)      130 2024-05-22 15:07:21.000000 antspynet-0.2.6/antspynet/__init__.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-22 16:29:27.990499 antspynet-0.2.6/antspynet.egg-info/
+-rw-r--r--   0 stnava     (501) staff       (20)    11985 2024-05-22 16:29:27.000000 antspynet-0.2.6/antspynet.egg-info/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)      221 2024-05-22 16:29:27.000000 antspynet-0.2.6/antspynet.egg-info/SOURCES.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        1 2024-05-22 16:29:27.000000 antspynet-0.2.6/antspynet.egg-info/dependency_links.txt
+-rw-r--r--   0 stnava     (501) staff       (20)       90 2024-05-22 16:29:27.000000 antspynet-0.2.6/antspynet.egg-info/requires.txt
+-rw-r--r--   0 stnava     (501) staff       (20)       10 2024-05-22 16:29:27.000000 antspynet-0.2.6/antspynet.egg-info/top_level.txt
+-rw-r--r--   0 stnava     (501) staff       (20)      992 2024-05-22 16:26:08.000000 antspynet-0.2.6/pyproject.toml
+-rw-r--r--   0 stnava     (501) staff       (20)       38 2024-05-22 16:29:27.990919 antspynet-0.2.6/setup.cfg
```

### Comparing `antspynet-0.2.5/LICENSE.md` & `antspynet-0.2.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `antspynet-0.2.5/PKG-INFO` & `antspynet-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: antspynet
-Version: 0.2.5
+Version: 0.2.6
 Summary: A collection of deep learning architectures ported to the python language and tools for basic medical image processing.
 Author: Brian B. Avants, Nick Cullen
 Author-email: "Nicholas J. Tustison" <ntustison@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/ANTsX/ANTsPyNet
 Keywords: ANTsPyNet,deep learning,medical image processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy
-Requires-Dist: tensorflow
-Requires-Dist: keras
+Requires-Dist: tensorflow<=2.17,>=2.11
 Requires-Dist: antspyx>=0.4.2
 Requires-Dist: scikit-learn
 Requires-Dist: requests
 Requires-Dist: statsmodels
 Requires-Dist: matplotlib
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/antspynet?label=pypi%20downloads)
@@ -218,12 +217,15 @@
 
 ## License
 
 The ANTsPyNet package is released under an [Apache License](https://github.com/ANTsX/ANTsPyNet/blob/master/LICENSE.md).
 
 ## to publish a release
 
+before doing this - make sure you have a recent run of `pip-compile pyproject.toml`
+
 ```
 rm -r -f build/ antspynet.egg-info/ dist/
 python3 -m  build .
-twine upload --repository antspynet dist/*
+python3 -m pip install --upgrade twine
+python3 -m twine upload --repository antspynet dist/*
 ```
```

### Comparing `antspynet-0.2.5/README.md` & `antspynet-0.2.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -195,12 +195,15 @@
 
 ## License
 
 The ANTsPyNet package is released under an [Apache License](https://github.com/ANTsX/ANTsPyNet/blob/master/LICENSE.md).
 
 ## to publish a release
 
+before doing this - make sure you have a recent run of `pip-compile pyproject.toml`
+
 ```
 rm -r -f build/ antspynet.egg-info/ dist/
 python3 -m  build .
-twine upload --repository antspynet dist/*
+python3 -m pip install --upgrade twine
+python3 -m twine upload --repository antspynet dist/*
 ```
```

### Comparing `antspynet-0.2.5/antspynet.egg-info/PKG-INFO` & `antspynet-0.2.6/antspynet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: antspynet
-Version: 0.2.5
+Version: 0.2.6
 Summary: A collection of deep learning architectures ported to the python language and tools for basic medical image processing.
 Author: Brian B. Avants, Nick Cullen
 Author-email: "Nicholas J. Tustison" <ntustison@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/ANTsX/ANTsPyNet
 Keywords: ANTsPyNet,deep learning,medical image processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy
-Requires-Dist: tensorflow
-Requires-Dist: keras
+Requires-Dist: tensorflow<=2.17,>=2.11
 Requires-Dist: antspyx>=0.4.2
 Requires-Dist: scikit-learn
 Requires-Dist: requests
 Requires-Dist: statsmodels
 Requires-Dist: matplotlib
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/antspynet?label=pypi%20downloads)
@@ -218,12 +217,15 @@
 
 ## License
 
 The ANTsPyNet package is released under an [Apache License](https://github.com/ANTsX/ANTsPyNet/blob/master/LICENSE.md).
 
 ## to publish a release
 
+before doing this - make sure you have a recent run of `pip-compile pyproject.toml`
+
 ```
 rm -r -f build/ antspynet.egg-info/ dist/
 python3 -m  build .
-twine upload --repository antspynet dist/*
+python3 -m pip install --upgrade twine
+python3 -m twine upload --repository antspynet dist/*
 ```
```

### Comparing `antspynet-0.2.5/pyproject.toml` & `antspynet-0.2.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "antspynet"
-version = "0.2.5"
+version = "0.2.6"
 description = "A collection of deep learning architectures ported to the python language and tools for basic medical image processing."
 readme = "README.md"
 authors = [
     {name = "Nicholas J. Tustison", email = "ntustison@gmail.com"},
     {name = "Brian B. Avants"},
     {name = "Nick Cullen"}
 ]
@@ -17,16 +17,16 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "numpy",
-    "tensorflow",
-    "keras",
+    "tensorflow>=2.11,<=2.17",
+#    "keras<3",
     "antspyx>=0.4.2",
     "scikit-learn",
     "requests",
     "statsmodels",
     "matplotlib"
 ]
```

