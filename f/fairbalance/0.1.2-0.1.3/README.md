# Comparing `tmp/fairbalance-0.1.2.tar.gz` & `tmp/fairbalance-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairbalance-0.1.2.tar", last modified: Tue May 21 13:59:37 2024, max compression
+gzip compressed data, was "fairbalance-0.1.3.tar", last modified: Tue May 21 14:20:26 2024, max compression
```

## Comparing `fairbalance-0.1.2.tar` & `fairbalance-0.1.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 13:59:37.167178 fairbalance-0.1.2/
--rw-rw-rw-   0        0        0      285 2024-05-21 09:43:17.000000 fairbalance-0.1.2/.gitignore
--rw-rw-rw-   0        0        0      602 2024-05-21 13:59:37.104678 fairbalance-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       92 2024-05-17 12:00:14.000000 fairbalance-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 13:59:36.414172 fairbalance-0.1.2/fairbalance/
--rw-rw-rw-   0        0        0       54 2024-05-15 13:38:01.000000 fairbalance-0.1.2/fairbalance/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:59:36.606626 fairbalance-0.1.2/fairbalance/datasets/
--rw-rw-rw-   0        0        0      308 2024-05-16 13:58:22.000000 fairbalance-0.1.2/fairbalance/datasets/__init__.py
--rw-rw-rw-   0        0        0    11236 2024-05-17 08:03:24.000000 fairbalance-0.1.2/fairbalance/datasets/_datasets_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:59:36.637732 fairbalance-0.1.2/fairbalance/datasets/tests/
--rw-rw-rw-   0        0        0        0 2024-05-16 13:59:33.000000 fairbalance-0.1.2/fairbalance/datasets/tests/test_datasets_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:59:36.733250 fairbalance-0.1.2/fairbalance/metrics/
--rw-rw-rw-   0        0        0      263 2024-05-15 13:29:26.000000 fairbalance-0.1.2/fairbalance/metrics/__init__.py
--rw-rw-rw-   0        0        0     7673 2024-05-15 09:52:05.000000 fairbalance-0.1.2/fairbalance/metrics/_dataset_metrics.py
--rw-rw-rw-   0        0        0    10471 2024-05-21 13:49:32.000000 fairbalance-0.1.2/fairbalance/metrics/_fairness_analysis.py
--rw-rw-rw-   0        0        0     2849 2024-05-15 09:30:16.000000 fairbalance-0.1.2/fairbalance/metrics/_model_metrics.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:59:36.789404 fairbalance-0.1.2/fairbalance/metrics/tests/
--rw-rw-rw-   0        0        0        0 2024-05-15 13:38:19.000000 fairbalance-0.1.2/fairbalance/metrics/tests/__init__.py
--rw-rw-rw-   0        0        0      652 2024-05-21 09:26:17.000000 fairbalance-0.1.2/fairbalance/metrics/tests/test_dataset_metrics.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:38:54.000000 fairbalance-0.1.2/fairbalance/metrics/tests/test_model_metrics.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:59:36.839226 fairbalance-0.1.2/fairbalance/mitigation_strategies/
--rw-rw-rw-   0        0        0      324 2024-05-21 13:42:52.000000 fairbalance-0.1.2/fairbalance/mitigation_strategies/__init__.py
--rw-rw-rw-   0        0        0     4834 2024-05-21 13:45:35.000000 fairbalance-0.1.2/fairbalance/mitigation_strategies/_mitigation_strategies.py
--rw-rw-rw-   0        0        0     2972 2024-05-21 13:45:22.000000 fairbalance-0.1.2/fairbalance/mitigation_strategies/base.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:59:36.898707 fairbalance-0.1.2/fairbalance/processors/
--rw-rw-rw-   0        0        0      329 2024-05-21 13:58:55.000000 fairbalance-0.1.2/fairbalance/processors/__init__.py
--rw-rw-rw-   0        0        0     1352 2024-05-21 13:48:02.000000 fairbalance-0.1.2/fairbalance/processors/_processors.py
--rw-rw-rw-   0        0        0     7246 2024-05-21 13:47:39.000000 fairbalance-0.1.2/fairbalance/processors/base.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:59:37.009026 fairbalance-0.1.2/fairbalance/tools/
--rw-rw-rw-   0        0        0      605 2024-05-21 13:28:32.000000 fairbalance-0.1.2/fairbalance/tools/__init__.py
--rw-rw-rw-   0        0        0    10474 2024-05-17 08:27:03.000000 fairbalance-0.1.2/fairbalance/tools/_fairness_analysis.py
--rw-rw-rw-   0        0        0    23251 2024-05-21 13:35:16.000000 fairbalance-0.1.2/fairbalance/tools/_mitigator.py
--rw-rw-rw-   0        0        0    10322 2024-05-21 13:01:40.000000 fairbalance-0.1.2/fairbalance/tools/_processor.py
--rw-rw-rw-   0        0        0     2115 2024-05-21 07:39:27.000000 fairbalance-0.1.2/fairbalance/tools/_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:59:37.091353 fairbalance-0.1.2/fairbalance/tools/tests/
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:11.000000 fairbalance-0.1.2/fairbalance/tools/tests/__init__.py
--rw-rw-rw-   0        0        0     4296 2024-05-21 09:28:03.000000 fairbalance-0.1.2/fairbalance/tools/tests/test_fairness_analysis.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:32.000000 fairbalance-0.1.2/fairbalance/tools/tests/test_mitigator.py
--rw-rw-rw-   0        0        0        0 2024-05-21 09:43:17.000000 fairbalance-0.1.2/fairbalance/tools/tests/test_processor.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:56.000000 fairbalance-0.1.2/fairbalance/tools/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:59:36.540644 fairbalance-0.1.2/fairbalance.egg-info/
--rw-rw-rw-   0        0        0      602 2024-05-21 13:59:32.000000 fairbalance-0.1.2/fairbalance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1279 2024-05-21 13:59:35.000000 fairbalance-0.1.2/fairbalance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 13:59:32.000000 fairbalance-0.1.2/fairbalance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-05-21 13:59:32.000000 fairbalance-0.1.2/fairbalance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-21 13:59:32.000000 fairbalance-0.1.2/fairbalance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      134 2024-05-17 11:08:16.000000 fairbalance-0.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 13:59:37.167178 fairbalance-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      765 2024-05-21 13:59:13.000000 fairbalance-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:20:26.497603 fairbalance-0.1.3/
+-rw-rw-rw-   0        0        0      285 2024-05-21 09:43:17.000000 fairbalance-0.1.3/.gitignore
+-rw-rw-rw-   0        0        0      602 2024-05-21 14:20:26.480188 fairbalance-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       92 2024-05-17 12:00:14.000000 fairbalance-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 14:20:26.035687 fairbalance-0.1.3/fairbalance/
+-rw-rw-rw-   0        0        0       54 2024-05-15 13:38:01.000000 fairbalance-0.1.3/fairbalance/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:20:26.126505 fairbalance-0.1.3/fairbalance/datasets/
+-rw-rw-rw-   0        0        0      308 2024-05-16 13:58:22.000000 fairbalance-0.1.3/fairbalance/datasets/__init__.py
+-rw-rw-rw-   0        0        0    11236 2024-05-17 08:03:24.000000 fairbalance-0.1.3/fairbalance/datasets/_datasets_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:20:26.142219 fairbalance-0.1.3/fairbalance/datasets/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-16 13:59:33.000000 fairbalance-0.1.3/fairbalance/datasets/tests/test_datasets_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:20:26.197050 fairbalance-0.1.3/fairbalance/metrics/
+-rw-rw-rw-   0        0        0      263 2024-05-15 13:29:26.000000 fairbalance-0.1.3/fairbalance/metrics/__init__.py
+-rw-rw-rw-   0        0        0     7673 2024-05-15 09:52:05.000000 fairbalance-0.1.3/fairbalance/metrics/_dataset_metrics.py
+-rw-rw-rw-   0        0        0    10471 2024-05-21 13:49:32.000000 fairbalance-0.1.3/fairbalance/metrics/_fairness_analysis.py
+-rw-rw-rw-   0        0        0     2849 2024-05-15 09:30:16.000000 fairbalance-0.1.3/fairbalance/metrics/_model_metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:20:26.238903 fairbalance-0.1.3/fairbalance/metrics/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:38:19.000000 fairbalance-0.1.3/fairbalance/metrics/tests/__init__.py
+-rw-rw-rw-   0        0        0      652 2024-05-21 09:26:17.000000 fairbalance-0.1.3/fairbalance/metrics/tests/test_dataset_metrics.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:38:54.000000 fairbalance-0.1.3/fairbalance/metrics/tests/test_model_metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:20:26.275979 fairbalance-0.1.3/fairbalance/mitigation_strategies/
+-rw-rw-rw-   0        0        0      324 2024-05-21 13:42:52.000000 fairbalance-0.1.3/fairbalance/mitigation_strategies/__init__.py
+-rw-rw-rw-   0        0        0     5076 2024-05-21 14:19:21.000000 fairbalance-0.1.3/fairbalance/mitigation_strategies/_mitigation_strategies.py
+-rw-rw-rw-   0        0        0     2972 2024-05-21 13:45:22.000000 fairbalance-0.1.3/fairbalance/mitigation_strategies/base.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:20:26.322049 fairbalance-0.1.3/fairbalance/processors/
+-rw-rw-rw-   0        0        0      329 2024-05-21 13:58:55.000000 fairbalance-0.1.3/fairbalance/processors/__init__.py
+-rw-rw-rw-   0        0        0     1352 2024-05-21 13:48:02.000000 fairbalance-0.1.3/fairbalance/processors/_processors.py
+-rw-rw-rw-   0        0        0     7246 2024-05-21 13:47:39.000000 fairbalance-0.1.3/fairbalance/processors/base.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:20:26.396995 fairbalance-0.1.3/fairbalance/tools/
+-rw-rw-rw-   0        0        0      605 2024-05-21 13:28:32.000000 fairbalance-0.1.3/fairbalance/tools/__init__.py
+-rw-rw-rw-   0        0        0    10474 2024-05-17 08:27:03.000000 fairbalance-0.1.3/fairbalance/tools/_fairness_analysis.py
+-rw-rw-rw-   0        0        0    23251 2024-05-21 13:35:16.000000 fairbalance-0.1.3/fairbalance/tools/_mitigator.py
+-rw-rw-rw-   0        0        0    10322 2024-05-21 13:01:40.000000 fairbalance-0.1.3/fairbalance/tools/_processor.py
+-rw-rw-rw-   0        0        0     2115 2024-05-21 07:39:27.000000 fairbalance-0.1.3/fairbalance/tools/_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:20:26.474765 fairbalance-0.1.3/fairbalance/tools/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:39:11.000000 fairbalance-0.1.3/fairbalance/tools/tests/__init__.py
+-rw-rw-rw-   0        0        0     4296 2024-05-21 09:28:03.000000 fairbalance-0.1.3/fairbalance/tools/tests/test_fairness_analysis.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:39:32.000000 fairbalance-0.1.3/fairbalance/tools/tests/test_mitigator.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:43:17.000000 fairbalance-0.1.3/fairbalance/tools/tests/test_processor.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:39:56.000000 fairbalance-0.1.3/fairbalance/tools/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:20:26.102871 fairbalance-0.1.3/fairbalance.egg-info/
+-rw-rw-rw-   0        0        0      602 2024-05-21 14:20:22.000000 fairbalance-0.1.3/fairbalance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1279 2024-05-21 14:20:25.000000 fairbalance-0.1.3/fairbalance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 14:20:22.000000 fairbalance-0.1.3/fairbalance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-05-21 14:20:22.000000 fairbalance-0.1.3/fairbalance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-21 14:20:22.000000 fairbalance-0.1.3/fairbalance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2024-05-17 11:08:16.000000 fairbalance-0.1.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 14:20:26.497603 fairbalance-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      765 2024-05-21 14:20:07.000000 fairbalance-0.1.3/setup.py
```

### Comparing `fairbalance-0.1.2/PKG-INFO` & `fairbalance-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairbalance
-Version: 0.1.2
+Version: 0.1.3
 Summary: bias mitigation by balancing target and/or protected attributes using resampling techniques
 Author: Pierre-Antoine Lequeu @ Fujitsu Luxembourg
 Author-email: pierre-antoine.lequeu@fujitsu.com
 Description-Content-Type: text/markdown
 Requires-Dist: folktables>=0.0.12
 Requires-Dist: imbalanced_learn==0.9.1
 Requires-Dist: numpy>=1.24.3
```

### Comparing `fairbalance-0.1.2/fairbalance/datasets/_datasets_loader.py` & `fairbalance-0.1.3/fairbalance/datasets/_datasets_loader.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.2/fairbalance/metrics/_dataset_metrics.py` & `fairbalance-0.1.3/fairbalance/metrics/_dataset_metrics.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.2/fairbalance/metrics/_fairness_analysis.py` & `fairbalance-0.1.3/fairbalance/metrics/_fairness_analysis.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.2/fairbalance/metrics/_model_metrics.py` & `fairbalance-0.1.3/fairbalance/metrics/_model_metrics.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.2/fairbalance/metrics/tests/test_dataset_metrics.py` & `fairbalance-0.1.3/fairbalance/metrics/tests/test_dataset_metrics.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.2/fairbalance/mitigation_strategies/_mitigation_strategies.py` & `fairbalance-0.1.3/fairbalance/mitigation_strategies/_mitigation_strategies.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,17 @@
         super().__init__(sampler)
     
     def balance(self, dataset: pd.DataFrame, target: pd.DataFrame = None, protected_attributes: list = None, 
                        cont_columns: list = None, cat_columns: list = None) :
         
         df, protected_attribute = self._get_dataframe_and_protected_attribute(dataset, protected_attributes)
         
+        if protected_attribute not in cat_columns :
+            cat_columns.append(protected_attribute)
+        
         X_processed, y_processed = self.sampler._process(df, target, cont_columns, cat_columns)
         X_resampled, y_resampled = self.sampler.fit_resample(X_processed, y_processed)
         X_final, y_final = self.sampler._unprocess(X_resampled, y_resampled)
         
         X_final = self._get_final_dataframe(X_final, protected_attributes, protected_attribute)
         
         return X_final, y_final     
@@ -30,14 +33,15 @@
     def __init__(self, sampler: BaseProcessor) :
         super().__init__(sampler)
 
     def balance(self, dataset: pd.DataFrame, target: pd.DataFrame = None, protected_attributes: list = None, 
                 cont_columns: list = None, cat_columns: list = None) :
         
         df, protected_attribute = self._get_dataframe_and_protected_attribute(dataset, protected_attributes)
+        
 
         X_processed, y_processed = self.sampler._process(df, target, cont_columns, cat_columns)
         
         protected_attribute_column = X_processed[protected_attribute]
         X_processed = X_processed.drop(columns=[protected_attribute])
         X_processed.loc[:,"target"] = y_processed
         new_cat_columns = [column for column in cat_columns if column != protected_attribute] + ["target"]
@@ -59,14 +63,17 @@
         super().__init__(sampler)
     
     def balance(self, dataset: pd.DataFrame, target: pd.DataFrame = None, protected_attributes: list = None, 
                 cont_columns: list = None, cat_columns: list = None) :
 
         df, protected_attribute = self._get_dataframe_and_protected_attribute(dataset, protected_attributes)
         
+        if protected_attribute not in cat_columns :
+            cat_columns.append(protected_attribute)
+        
         classes = list(df[protected_attribute].unique())
         highest_r, class_with_highest_r = self._highest_ratio(df, target, classes, protected_attribute)
         self.sampler.sampling_strategy = highest_r
         X_final = pd.DataFrame(columns = df.columns)
         y_final = pd.Series()
         for class_ in classes :
```

### Comparing `fairbalance-0.1.2/fairbalance/mitigation_strategies/base.py` & `fairbalance-0.1.3/fairbalance/mitigation_strategies/base.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.2/fairbalance/processors/_processors.py` & `fairbalance-0.1.3/fairbalance/processors/_processors.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.2/fairbalance/processors/base.py` & `fairbalance-0.1.3/fairbalance/processors/base.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.2/fairbalance/tools/__init__.py` & `fairbalance-0.1.3/fairbalance/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.2/fairbalance/tools/_fairness_analysis.py` & `fairbalance-0.1.3/fairbalance/tools/_fairness_analysis.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.2/fairbalance/tools/_mitigator.py` & `fairbalance-0.1.3/fairbalance/tools/_mitigator.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.2/fairbalance/tools/_processor.py` & `fairbalance-0.1.3/fairbalance/tools/_processor.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.2/fairbalance/tools/_utils.py` & `fairbalance-0.1.3/fairbalance/tools/_utils.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.2/fairbalance/tools/tests/test_fairness_analysis.py` & `fairbalance-0.1.3/fairbalance/tools/tests/test_fairness_analysis.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.2/fairbalance.egg-info/PKG-INFO` & `fairbalance-0.1.3/fairbalance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairbalance
-Version: 0.1.2
+Version: 0.1.3
 Summary: bias mitigation by balancing target and/or protected attributes using resampling techniques
 Author: Pierre-Antoine Lequeu @ Fujitsu Luxembourg
 Author-email: pierre-antoine.lequeu@fujitsu.com
 Description-Content-Type: text/markdown
 Requires-Dist: folktables>=0.0.12
 Requires-Dist: imbalanced_learn==0.9.1
 Requires-Dist: numpy>=1.24.3
```

### Comparing `fairbalance-0.1.2/fairbalance.egg-info/SOURCES.txt` & `fairbalance-0.1.3/fairbalance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.2/setup.py` & `fairbalance-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "fairbalance",
-    version = "0.1.2",
+    version = "0.1.3",
     author = "Pierre-Antoine Lequeu @ Fujitsu Luxembourg",
     author_email = "pierre-antoine.lequeu@fujitsu.com",
     description = "bias mitigation by balancing target and/or protected attributes using resampling techniques",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     packages = setuptools.find_packages(),
     install_requires=[
```

