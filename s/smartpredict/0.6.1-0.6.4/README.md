# Comparing `tmp/smartpredict-0.6.1.tar.gz` & `tmp/smartpredict-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartpredict-0.6.1.tar", last modified: Wed May 22 04:42:05 2024, max compression
+gzip compressed data, was "smartpredict-0.6.4.tar", last modified: Wed May 22 05:07:52 2024, max compression
```

## Comparing `smartpredict-0.6.1.tar` & `smartpredict-0.6.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:42:05.427244 smartpredict-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-22 04:42:05.427244 smartpredict-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 04:42:05.427244 smartpredict-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-22 04:41:58.000000 smartpredict-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:42:05.427244 smartpredict-0.6.1/smartpredict/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-22 04:41:58.000000 smartpredict-0.6.1/smartpredict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-22 04:41:58.000000 smartpredict-0.6.1/smartpredict/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-22 04:41:58.000000 smartpredict-0.6.1/smartpredict/ensemble_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-22 04:41:58.000000 smartpredict-0.6.1/smartpredict/explainability.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-22 04:41:58.000000 smartpredict-0.6.1/smartpredict/feature_engineering.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-22 04:41:58.000000 smartpredict-0.6.1/smartpredict/hyperparameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-22 04:41:58.000000 smartpredict-0.6.1/smartpredict/model_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-22 04:41:58.000000 smartpredict-0.6.1/smartpredict/supervised.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:41:58.000000 smartpredict-0.6.1/smartpredict/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:42:05.427244 smartpredict-0.6.1/smartpredict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-22 04:42:05.000000 smartpredict-0.6.1/smartpredict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-22 04:42:05.000000 smartpredict-0.6.1/smartpredict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 04:42:05.000000 smartpredict-0.6.1/smartpredict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-22 04:42:05.000000 smartpredict-0.6.1/smartpredict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 04:42:05.000000 smartpredict-0.6.1/smartpredict.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:42:05.427244 smartpredict-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:41:58.000000 smartpredict-0.6.1/tests/test_smartpredict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:07:52.723295 smartpredict-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-22 05:07:52.719295 smartpredict-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 05:07:52.723295 smartpredict-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-22 05:07:49.000000 smartpredict-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:07:52.719295 smartpredict-0.6.4/smartpredict/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-22 05:07:49.000000 smartpredict-0.6.4/smartpredict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-22 05:07:49.000000 smartpredict-0.6.4/smartpredict/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-22 05:07:49.000000 smartpredict-0.6.4/smartpredict/ensemble_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-22 05:07:49.000000 smartpredict-0.6.4/smartpredict/explainability.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-22 05:07:49.000000 smartpredict-0.6.4/smartpredict/feature_engineering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-22 05:07:49.000000 smartpredict-0.6.4/smartpredict/hyperparameter_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-22 05:07:49.000000 smartpredict-0.6.4/smartpredict/model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-22 05:07:49.000000 smartpredict-0.6.4/smartpredict/supervised.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 05:07:49.000000 smartpredict-0.6.4/smartpredict/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:07:52.719295 smartpredict-0.6.4/smartpredict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-22 05:07:52.000000 smartpredict-0.6.4/smartpredict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-22 05:07:52.000000 smartpredict-0.6.4/smartpredict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 05:07:52.000000 smartpredict-0.6.4/smartpredict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-22 05:07:52.000000 smartpredict-0.6.4/smartpredict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 05:07:52.000000 smartpredict-0.6.4/smartpredict.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:07:52.719295 smartpredict-0.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 05:07:49.000000 smartpredict-0.6.4/tests/test_smartpredict.py
```

### Comparing `smartpredict-0.6.1/PKG-INFO` & `smartpredict-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartpredict
-Version: 0.6.1
+Version: 0.6.4
 Summary: An advanced machine learning library for effortless model training, evaluation, and selection.
 Home-page: https://github.com/SubaashNair/SmartPredict
 Author: Subashanan Nair
 Author-email: subaashnair12@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smartpredict-0.6.1/setup.py` & `smartpredict-0.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 if readme_path.exists():
     long_description = readme_path.read_text(encoding='utf-8')
 else:
     long_description = "SmartPredict: An advanced machine learning library for effortless model training, evaluation, and selection."
 
 setup(
     name="smartpredict",
-    version="0.6.1",  # Update the version number
+    version="0.6.4",  # Update the version number
     description="An advanced machine learning library for effortless model training, evaluation, and selection.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Subashanan Nair",
     author_email="subaashnair12@gmail.com",
     url="https://github.com/SubaashNair/SmartPredict",
     packages=find_packages(),
```

### Comparing `smartpredict-0.6.1/smartpredict/base.py` & `smartpredict-0.6.4/smartpredict/base.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.6.1/smartpredict/ensemble_methods.py` & `smartpredict-0.6.4/smartpredict/ensemble_methods.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.6.1/smartpredict/explainability.py` & `smartpredict-0.6.4/smartpredict/explainability.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.6.1/smartpredict/feature_engineering.py` & `smartpredict-0.6.4/smartpredict/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.6.1/smartpredict/hyperparameter_tuning.py` & `smartpredict-0.6.4/smartpredict/hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.6.1/smartpredict/model_selection.py` & `smartpredict-0.6.4/smartpredict/model_selection.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.6.1/smartpredict/supervised.py` & `smartpredict-0.6.4/smartpredict/supervised.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.6.1/smartpredict.egg-info/PKG-INFO` & `smartpredict-0.6.4/smartpredict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartpredict
-Version: 0.6.1
+Version: 0.6.4
 Summary: An advanced machine learning library for effortless model training, evaluation, and selection.
 Home-page: https://github.com/SubaashNair/SmartPredict
 Author: Subashanan Nair
 Author-email: subaashnair12@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

