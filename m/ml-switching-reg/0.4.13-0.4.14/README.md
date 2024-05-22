# Comparing `tmp/ml_switching_reg-0.4.13.tar.gz` & `tmp/ml_switching_reg-0.4.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_switching_reg-0.4.13.tar", max compression
+gzip compressed data, was "ml_switching_reg-0.4.14.tar", max compression
```

## Comparing `ml_switching_reg-0.4.13.tar` & `ml_switching_reg-0.4.14.tar`

### file list

```diff
@@ -1,24 +1,17 @@
--rw-r--r--   0        0        0       22 2023-03-20 16:35:01.352312 ml_switching_reg-0.4.13/ml_switching_reg/__init__.py
--rw-r--r--   0        0        0     5401 2023-01-31 20:23:42.007907 ml_switching_reg-0.4.13/ml_switching_reg/cm.py
--rw-r--r--   0        0        0    16767 2023-02-16 03:33:08.652519 ml_switching_reg-0.4.13/ml_switching_reg/mle.py
--rw-r--r--   0        0        0    23584 2023-01-31 20:23:42.015907 ml_switching_reg-0.4.13/ml_switching_reg/patches.py
--rw-r--r--   0        0        0   298123 2023-01-31 20:23:42.031907 ml_switching_reg-0.4.13/ml_switching_reg/saved_models/plots/2_0.0_plot.png
--rw-r--r--   0        0        0   300118 2023-01-31 20:23:42.039907 ml_switching_reg-0.4.13/ml_switching_reg/saved_models/plots/2_0.1_plot.png
--rw-r--r--   0        0        0   274860 2023-01-31 20:23:42.051907 ml_switching_reg-0.4.13/ml_switching_reg/saved_models/plots/2_0.5_plot.png
--rw-r--r--   0        0        0   309766 2023-01-31 20:23:42.063907 ml_switching_reg-0.4.13/ml_switching_reg/saved_models/plots/2_0.6_plot.png
--rw-r--r--   0        0        0   276914 2023-01-31 20:23:42.071907 ml_switching_reg-0.4.13/ml_switching_reg/saved_models/plots/2_0.9_plot.png
--rw-r--r--   0        0        0   256922 2023-01-31 20:23:42.079907 ml_switching_reg-0.4.13/ml_switching_reg/saved_models/plots/3_0.1_plot.png
--rw-r--r--   0        0        0   222879 2023-01-31 20:23:42.087907 ml_switching_reg-0.4.13/ml_switching_reg/saved_models/plots/3_0.5_plot.png
--rw-r--r--   0        0        0   223988 2023-01-31 20:23:42.099907 ml_switching_reg-0.4.13/ml_switching_reg/saved_models/plots/3_0.9_plot.png
--rw-r--r--   0        0        0   213962 2023-01-31 20:23:42.107907 ml_switching_reg-0.4.13/ml_switching_reg/saved_models/plots/4_0.1_plot.png
--rw-r--r--   0        0        0   213139 2023-01-31 20:23:42.115907 ml_switching_reg-0.4.13/ml_switching_reg/saved_models/plots/4_0.5_plot.png
--rw-r--r--   0        0        0        0 2023-01-31 20:23:42.119907 ml_switching_reg-0.4.13/ml_switching_reg/simulation/__init__.py
--rw-r--r--   0        0        0    10611 2023-01-31 20:23:42.119907 ml_switching_reg-0.4.13/ml_switching_reg/simulation/data_creation.py
--rw-r--r--   0        0        0    22394 2023-01-31 20:23:42.123907 ml_switching_reg-0.4.13/ml_switching_reg/simulation/monte_carlo.py
--rw-r--r--   0        0        0     1337 2023-01-31 20:23:42.127907 ml_switching_reg-0.4.13/ml_switching_reg/simulation/regression.py
--rw-r--r--   0        0        0      988 2023-01-31 20:23:42.131907 ml_switching_reg-0.4.13/ml_switching_reg/simulation/utils.py
--rw-r--r--   0        0        0     5564 2023-01-31 20:23:42.135907 ml_switching_reg-0.4.13/ml_switching_reg/simulation/visualization.py
--rw-r--r--   0        0        0      210 2023-01-31 20:23:42.139907 ml_switching_reg-0.4.13/ml_switching_reg/uganda-uber-paper.code-workspace
--rw-r--r--   0        0        0      760 2023-03-20 16:35:01.344312 ml_switching_reg-0.4.13/pyproject.toml
--rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 ml_switching_reg-0.4.13/setup.py
--rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 ml_switching_reg-0.4.13/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-12-06 15:07:39.222828 ml_switching_reg-0.4.14/ml_switching_reg/__init__.py
+-rw-r--r--   0        0        0     5401 2023-01-31 20:23:42.007907 ml_switching_reg-0.4.14/ml_switching_reg/cm.py
+-rw-r--r--   0        0        0    16761 2023-10-06 16:57:33.730126 ml_switching_reg-0.4.14/ml_switching_reg/mle.py
+-rw-r--r--   0        0        0    23584 2023-01-31 20:23:42.015907 ml_switching_reg-0.4.14/ml_switching_reg/patches.py
+-rw-r--r--   0        0        0   298123 2023-01-31 20:23:42.031907 ml_switching_reg-0.4.14/ml_switching_reg/saved_models/plots/2_0.0_plot.png
+-rw-r--r--   0        0        0   300118 2023-01-31 20:23:42.039907 ml_switching_reg-0.4.14/ml_switching_reg/saved_models/plots/2_0.1_plot.png
+-rw-r--r--   0        0        0   274860 2023-01-31 20:23:42.051907 ml_switching_reg-0.4.14/ml_switching_reg/saved_models/plots/2_0.5_plot.png
+-rw-r--r--   0        0        0   309766 2023-01-31 20:23:42.063907 ml_switching_reg-0.4.14/ml_switching_reg/saved_models/plots/2_0.6_plot.png
+-rw-r--r--   0        0        0   276914 2023-01-31 20:23:42.071907 ml_switching_reg-0.4.14/ml_switching_reg/saved_models/plots/2_0.9_plot.png
+-rw-r--r--   0        0        0   256922 2023-01-31 20:23:42.079907 ml_switching_reg-0.4.14/ml_switching_reg/saved_models/plots/3_0.1_plot.png
+-rw-r--r--   0        0        0   222879 2023-01-31 20:23:42.087907 ml_switching_reg-0.4.14/ml_switching_reg/saved_models/plots/3_0.5_plot.png
+-rw-r--r--   0        0        0   223988 2023-01-31 20:23:42.099907 ml_switching_reg-0.4.14/ml_switching_reg/saved_models/plots/3_0.9_plot.png
+-rw-r--r--   0        0        0   213962 2023-01-31 20:23:42.107907 ml_switching_reg-0.4.14/ml_switching_reg/saved_models/plots/4_0.1_plot.png
+-rw-r--r--   0        0        0   213139 2023-01-31 20:23:42.115907 ml_switching_reg-0.4.14/ml_switching_reg/saved_models/plots/4_0.5_plot.png
+-rw-r--r--   0        0        0      782 2023-12-06 15:07:39.214828 ml_switching_reg-0.4.14/pyproject.toml
+-rw-r--r--   0        0        0      906 1970-01-01 00:00:00.000000 ml_switching_reg-0.4.14/setup.py
+-rw-r--r--   0        0        0      832 1970-01-01 00:00:00.000000 ml_switching_reg-0.4.14/PKG-INFO
```

### Comparing `ml_switching_reg-0.4.13/ml_switching_reg/cm.py` & `ml_switching_reg-0.4.14/ml_switching_reg/cm.py`

 * *Files identical despite different names*

### Comparing `ml_switching_reg-0.4.13/ml_switching_reg/mle.py` & `ml_switching_reg-0.4.14/ml_switching_reg/mle.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                  drop_absorbed=False,
                  check_rank=True,
                  singletons = True,
                  check_absorbed=True,
                  cm=None,
                  **kwargs):
         
-        print("Initializing...")    
+        print("Initializing...")   
         
         self.cm = cm
         self.check_absorbed= check_absorbed 
         self.classifier_true_ind = classifier_true_ind
         if classifier_true_ind is not None:
             self._classifier_true_ind_name = classifier_true_ind.name
 
@@ -90,15 +90,15 @@
             endog.reset_index(2, inplace=True)
             exog.reset_index(2, inplace=True)
         else:
             self.classifier_ind = classifier_ind
             self._group = classifier_ind_name
     
         if not all([classifier_ind is not None, classifier_ind_name]):
-            raise Exception("If either `classifier_ind` or `classifier_ind_name` is defined, the other must be defined as well, but ")
+            raise Exception("If either `classifier_ind` or `classifier_ind_name` is defined, the other must be defined as well ")
                 
         self.classifier_pred = classifier_pred
         if self.classifier_pred is not None:
             self.classifier_map = {k:v for k,v in zip(self.classifier_pred.columns, self.classifier_ind.cat.categories)}
         
         endog_cat = (
             endog
```

### Comparing `ml_switching_reg-0.4.13/ml_switching_reg/patches.py` & `ml_switching_reg-0.4.14/ml_switching_reg/patches.py`

 * *Files identical despite different names*

### Comparing `ml_switching_reg-0.4.13/ml_switching_reg/saved_models/plots/2_0.0_plot.png` & `ml_switching_reg-0.4.14/ml_switching_reg/saved_models/plots/2_0.0_plot.png`

 * *Files identical despite different names*

### Comparing `ml_switching_reg-0.4.13/ml_switching_reg/saved_models/plots/2_0.1_plot.png` & `ml_switching_reg-0.4.14/ml_switching_reg/saved_models/plots/2_0.1_plot.png`

 * *Files identical despite different names*

### Comparing `ml_switching_reg-0.4.13/ml_switching_reg/saved_models/plots/2_0.5_plot.png` & `ml_switching_reg-0.4.14/ml_switching_reg/saved_models/plots/2_0.5_plot.png`

 * *Files identical despite different names*

### Comparing `ml_switching_reg-0.4.13/ml_switching_reg/saved_models/plots/2_0.6_plot.png` & `ml_switching_reg-0.4.14/ml_switching_reg/saved_models/plots/2_0.6_plot.png`

 * *Files identical despite different names*

### Comparing `ml_switching_reg-0.4.13/ml_switching_reg/saved_models/plots/2_0.9_plot.png` & `ml_switching_reg-0.4.14/ml_switching_reg/saved_models/plots/2_0.9_plot.png`

 * *Files identical despite different names*

### Comparing `ml_switching_reg-0.4.13/ml_switching_reg/saved_models/plots/3_0.1_plot.png` & `ml_switching_reg-0.4.14/ml_switching_reg/saved_models/plots/3_0.1_plot.png`

 * *Files identical despite different names*

### Comparing `ml_switching_reg-0.4.13/ml_switching_reg/saved_models/plots/3_0.5_plot.png` & `ml_switching_reg-0.4.14/ml_switching_reg/saved_models/plots/3_0.5_plot.png`

 * *Files identical despite different names*

### Comparing `ml_switching_reg-0.4.13/ml_switching_reg/saved_models/plots/3_0.9_plot.png` & `ml_switching_reg-0.4.14/ml_switching_reg/saved_models/plots/3_0.9_plot.png`

 * *Files identical despite different names*

### Comparing `ml_switching_reg-0.4.13/ml_switching_reg/saved_models/plots/4_0.1_plot.png` & `ml_switching_reg-0.4.14/ml_switching_reg/saved_models/plots/4_0.1_plot.png`

 * *Files identical despite different names*

### Comparing `ml_switching_reg-0.4.13/ml_switching_reg/saved_models/plots/4_0.5_plot.png` & `ml_switching_reg-0.4.14/ml_switching_reg/saved_models/plots/4_0.5_plot.png`

 * *Files identical despite different names*

### Comparing `ml_switching_reg-0.4.13/pyproject.toml` & `ml_switching_reg-0.4.14/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ml-switching-reg"
-version = "0.4.13"
+version = "0.4.14"
 description = "A robust estimator to machine learning prediction misclassification"
 authors = ["Aleksandr Michuda <amichuda@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 matplotlib = "3.4.3"
@@ -12,14 +12,15 @@
 linearmodels = "4.26"
 patsy = "0.5.2"
 scipy = "1.8.0"
 statsmodels = "0.13.2"
 pandas = "1.4.2"
 tqdm = "4.56.0"
 scikit-learn = "1.2.1"
+numba-stats = "1.1.0"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0",  "poetry-dynamic-versioning"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ml_switching_reg-0.4.13/setup.py` & `ml_switching_reg-0.4.14/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['ml_switching_reg', 'ml_switching_reg.simulation']
+['ml_switching_reg']
 
 package_data = \
 {'': ['*'], 'ml_switching_reg': ['saved_models/plots/*']}
 
 install_requires = \
 ['linearmodels==4.26',
  'matplotlib==3.4.3',
+ 'numba-stats==1.1.0',
  'numpy==1.24.2',
  'pandas==1.4.2',
  'patsy==0.5.2',
  'scikit-learn==1.2.1',
  'scipy==1.8.0',
  'statsmodels==0.13.2',
  'tqdm==4.56.0']
 
 setup_kwargs = {
     'name': 'ml-switching-reg',
-    'version': '0.4.13',
+    'version': '0.4.14',
     'description': 'A robust estimator to machine learning prediction misclassification',
     'long_description': 'None',
     'author': 'Aleksandr Michuda',
     'author_email': 'amichuda@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ml_switching_reg-0.4.13/PKG-INFO` & `ml_switching_reg-0.4.14/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: ml-switching-reg
-Version: 0.4.13
+Version: 0.4.14
 Summary: A robust estimator to machine learning prediction misclassification
 License: MIT
 Author: Aleksandr Michuda
 Author-email: amichuda@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: linearmodels (==4.26)
 Requires-Dist: matplotlib (==3.4.3)
+Requires-Dist: numba-stats (==1.1.0)
 Requires-Dist: numpy (==1.24.2)
 Requires-Dist: pandas (==1.4.2)
 Requires-Dist: patsy (==0.5.2)
 Requires-Dist: scikit-learn (==1.2.1)
 Requires-Dist: scipy (==1.8.0)
 Requires-Dist: statsmodels (==0.13.2)
 Requires-Dist: tqdm (==4.56.0)
```

