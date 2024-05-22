# Comparing `tmp/fairbalance-0.1.3.tar.gz` & `tmp/fairbalance-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairbalance-0.1.3.tar", last modified: Tue May 21 14:20:26 2024, max compression
+gzip compressed data, was "fairbalance-0.1.4.tar", last modified: Wed May 22 09:00:26 2024, max compression
```

## Comparing `fairbalance-0.1.3.tar` & `fairbalance-0.1.4.tar`

### file list

```diff
@@ -1,49 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 14:20:26.497603 fairbalance-0.1.3/
--rw-rw-rw-   0        0        0      285 2024-05-21 09:43:17.000000 fairbalance-0.1.3/.gitignore
--rw-rw-rw-   0        0        0      602 2024-05-21 14:20:26.480188 fairbalance-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       92 2024-05-17 12:00:14.000000 fairbalance-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 14:20:26.035687 fairbalance-0.1.3/fairbalance/
--rw-rw-rw-   0        0        0       54 2024-05-15 13:38:01.000000 fairbalance-0.1.3/fairbalance/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:20:26.126505 fairbalance-0.1.3/fairbalance/datasets/
--rw-rw-rw-   0        0        0      308 2024-05-16 13:58:22.000000 fairbalance-0.1.3/fairbalance/datasets/__init__.py
--rw-rw-rw-   0        0        0    11236 2024-05-17 08:03:24.000000 fairbalance-0.1.3/fairbalance/datasets/_datasets_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:20:26.142219 fairbalance-0.1.3/fairbalance/datasets/tests/
--rw-rw-rw-   0        0        0        0 2024-05-16 13:59:33.000000 fairbalance-0.1.3/fairbalance/datasets/tests/test_datasets_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:20:26.197050 fairbalance-0.1.3/fairbalance/metrics/
--rw-rw-rw-   0        0        0      263 2024-05-15 13:29:26.000000 fairbalance-0.1.3/fairbalance/metrics/__init__.py
--rw-rw-rw-   0        0        0     7673 2024-05-15 09:52:05.000000 fairbalance-0.1.3/fairbalance/metrics/_dataset_metrics.py
--rw-rw-rw-   0        0        0    10471 2024-05-21 13:49:32.000000 fairbalance-0.1.3/fairbalance/metrics/_fairness_analysis.py
--rw-rw-rw-   0        0        0     2849 2024-05-15 09:30:16.000000 fairbalance-0.1.3/fairbalance/metrics/_model_metrics.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:20:26.238903 fairbalance-0.1.3/fairbalance/metrics/tests/
--rw-rw-rw-   0        0        0        0 2024-05-15 13:38:19.000000 fairbalance-0.1.3/fairbalance/metrics/tests/__init__.py
--rw-rw-rw-   0        0        0      652 2024-05-21 09:26:17.000000 fairbalance-0.1.3/fairbalance/metrics/tests/test_dataset_metrics.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:38:54.000000 fairbalance-0.1.3/fairbalance/metrics/tests/test_model_metrics.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:20:26.275979 fairbalance-0.1.3/fairbalance/mitigation_strategies/
--rw-rw-rw-   0        0        0      324 2024-05-21 13:42:52.000000 fairbalance-0.1.3/fairbalance/mitigation_strategies/__init__.py
--rw-rw-rw-   0        0        0     5076 2024-05-21 14:19:21.000000 fairbalance-0.1.3/fairbalance/mitigation_strategies/_mitigation_strategies.py
--rw-rw-rw-   0        0        0     2972 2024-05-21 13:45:22.000000 fairbalance-0.1.3/fairbalance/mitigation_strategies/base.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:20:26.322049 fairbalance-0.1.3/fairbalance/processors/
--rw-rw-rw-   0        0        0      329 2024-05-21 13:58:55.000000 fairbalance-0.1.3/fairbalance/processors/__init__.py
--rw-rw-rw-   0        0        0     1352 2024-05-21 13:48:02.000000 fairbalance-0.1.3/fairbalance/processors/_processors.py
--rw-rw-rw-   0        0        0     7246 2024-05-21 13:47:39.000000 fairbalance-0.1.3/fairbalance/processors/base.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:20:26.396995 fairbalance-0.1.3/fairbalance/tools/
--rw-rw-rw-   0        0        0      605 2024-05-21 13:28:32.000000 fairbalance-0.1.3/fairbalance/tools/__init__.py
--rw-rw-rw-   0        0        0    10474 2024-05-17 08:27:03.000000 fairbalance-0.1.3/fairbalance/tools/_fairness_analysis.py
--rw-rw-rw-   0        0        0    23251 2024-05-21 13:35:16.000000 fairbalance-0.1.3/fairbalance/tools/_mitigator.py
--rw-rw-rw-   0        0        0    10322 2024-05-21 13:01:40.000000 fairbalance-0.1.3/fairbalance/tools/_processor.py
--rw-rw-rw-   0        0        0     2115 2024-05-21 07:39:27.000000 fairbalance-0.1.3/fairbalance/tools/_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:20:26.474765 fairbalance-0.1.3/fairbalance/tools/tests/
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:11.000000 fairbalance-0.1.3/fairbalance/tools/tests/__init__.py
--rw-rw-rw-   0        0        0     4296 2024-05-21 09:28:03.000000 fairbalance-0.1.3/fairbalance/tools/tests/test_fairness_analysis.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:32.000000 fairbalance-0.1.3/fairbalance/tools/tests/test_mitigator.py
--rw-rw-rw-   0        0        0        0 2024-05-21 09:43:17.000000 fairbalance-0.1.3/fairbalance/tools/tests/test_processor.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:56.000000 fairbalance-0.1.3/fairbalance/tools/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:20:26.102871 fairbalance-0.1.3/fairbalance.egg-info/
--rw-rw-rw-   0        0        0      602 2024-05-21 14:20:22.000000 fairbalance-0.1.3/fairbalance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1279 2024-05-21 14:20:25.000000 fairbalance-0.1.3/fairbalance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 14:20:22.000000 fairbalance-0.1.3/fairbalance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-05-21 14:20:22.000000 fairbalance-0.1.3/fairbalance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-21 14:20:22.000000 fairbalance-0.1.3/fairbalance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      134 2024-05-17 11:08:16.000000 fairbalance-0.1.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 14:20:26.497603 fairbalance-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      765 2024-05-21 14:20:07.000000 fairbalance-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:00:26.473031 fairbalance-0.1.4/
+-rw-rw-rw-   0        0        0      285 2024-05-21 09:43:17.000000 fairbalance-0.1.4/.gitignore
+-rw-rw-rw-   0        0        0      602 2024-05-22 09:00:26.454700 fairbalance-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       92 2024-05-17 12:00:14.000000 fairbalance-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 09:00:25.734493 fairbalance-0.1.4/docs/
+drwxrwxrwx   0        0        0        0 2024-05-22 09:00:25.835160 fairbalance-0.1.4/docs/basics/
+-rw-rw-rw-   0        0        0     1785 2024-05-21 09:06:34.000000 fairbalance-0.1.4/docs/basics/test.ipynb
+drwxrwxrwx   0        0        0        0 2024-05-22 09:00:25.873372 fairbalance-0.1.4/fairbalance/
+-rw-rw-rw-   0        0        0       40 2024-05-22 08:39:56.000000 fairbalance-0.1.4/fairbalance/__init__.py
+-rw-rw-rw-   0        0        0    12167 2024-05-21 13:36:53.000000 fairbalance-0.1.4/fairbalance/all_test.ipynb
+drwxrwxrwx   0        0        0        0 2024-05-22 09:00:25.987337 fairbalance-0.1.4/fairbalance/datasets/
+-rw-rw-rw-   0        0        0      308 2024-05-16 13:58:22.000000 fairbalance-0.1.4/fairbalance/datasets/__init__.py
+-rw-rw-rw-   0        0        0    11642 2024-05-22 08:59:05.000000 fairbalance-0.1.4/fairbalance/datasets/_datasets_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:00:26.005241 fairbalance-0.1.4/fairbalance/datasets/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-16 13:59:33.000000 fairbalance-0.1.4/fairbalance/datasets/tests/test_datasets_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:00:26.069573 fairbalance-0.1.4/fairbalance/metrics/
+-rw-rw-rw-   0        0        0      377 2024-05-22 08:18:14.000000 fairbalance-0.1.4/fairbalance/metrics/__init__.py
+-rw-rw-rw-   0        0        0    10470 2024-05-22 08:34:41.000000 fairbalance-0.1.4/fairbalance/metrics/_dataset_metrics.py
+-rw-rw-rw-   0        0        0    12289 2024-05-22 08:34:39.000000 fairbalance-0.1.4/fairbalance/metrics/_fairness_analysis.py
+-rw-rw-rw-   0        0        0     2851 2024-05-22 08:34:40.000000 fairbalance-0.1.4/fairbalance/metrics/_model_metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:00:26.136612 fairbalance-0.1.4/fairbalance/metrics/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:38:19.000000 fairbalance-0.1.4/fairbalance/metrics/tests/__init__.py
+-rw-rw-rw-   0        0        0      652 2024-05-21 09:26:17.000000 fairbalance-0.1.4/fairbalance/metrics/tests/test_dataset_metrics.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:38:54.000000 fairbalance-0.1.4/fairbalance/metrics/tests/test_model_metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:00:26.185904 fairbalance-0.1.4/fairbalance/mitigation_strategies/
+-rw-rw-rw-   0        0        0      324 2024-05-21 13:42:52.000000 fairbalance-0.1.4/fairbalance/mitigation_strategies/__init__.py
+-rw-rw-rw-   0        0        0     8612 2024-05-22 08:34:47.000000 fairbalance-0.1.4/fairbalance/mitigation_strategies/_mitigation_strategies.py
+-rw-rw-rw-   0        0        0     4763 2024-05-22 08:34:51.000000 fairbalance-0.1.4/fairbalance/mitigation_strategies/base.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:00:26.242326 fairbalance-0.1.4/fairbalance/processors/
+-rw-rw-rw-   0        0        0      329 2024-05-21 14:45:40.000000 fairbalance-0.1.4/fairbalance/processors/__init__.py
+-rw-rw-rw-   0        0        0     3089 2024-05-22 07:49:24.000000 fairbalance-0.1.4/fairbalance/processors/_processors.py
+-rw-rw-rw-   0        0        0     8327 2024-05-22 08:34:34.000000 fairbalance-0.1.4/fairbalance/processors/base.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:00:26.345212 fairbalance-0.1.4/fairbalance/tools/
+-rw-rw-rw-   0        0        0      605 2024-05-21 13:28:32.000000 fairbalance-0.1.4/fairbalance/tools/__init__.py
+-rw-rw-rw-   0        0        0    10474 2024-05-17 08:27:03.000000 fairbalance-0.1.4/fairbalance/tools/_fairness_analysis.py
+-rw-rw-rw-   0        0        0    17757 2024-05-21 15:06:52.000000 fairbalance-0.1.4/fairbalance/tools/_mitigator.py
+-rw-rw-rw-   0        0        0    10322 2024-05-21 13:01:40.000000 fairbalance-0.1.4/fairbalance/tools/_processor.py
+-rw-rw-rw-   0        0        0     2115 2024-05-21 07:39:27.000000 fairbalance-0.1.4/fairbalance/tools/_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:00:26.431312 fairbalance-0.1.4/fairbalance/tools/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:39:11.000000 fairbalance-0.1.4/fairbalance/tools/tests/__init__.py
+-rw-rw-rw-   0        0        0     4296 2024-05-21 09:28:03.000000 fairbalance-0.1.4/fairbalance/tools/tests/test_fairness_analysis.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:39:32.000000 fairbalance-0.1.4/fairbalance/tools/tests/test_mitigator.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:43:17.000000 fairbalance-0.1.4/fairbalance/tools/tests/test_processor.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:39:56.000000 fairbalance-0.1.4/fairbalance/tools/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:00:25.957954 fairbalance-0.1.4/fairbalance.egg-info/
+-rw-rw-rw-   0        0        0      602 2024-05-22 09:00:22.000000 fairbalance-0.1.4/fairbalance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1329 2024-05-22 09:00:25.000000 fairbalance-0.1.4/fairbalance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 09:00:22.000000 fairbalance-0.1.4/fairbalance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-05-22 09:00:22.000000 fairbalance-0.1.4/fairbalance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-22 09:00:22.000000 fairbalance-0.1.4/fairbalance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2024-05-17 11:08:16.000000 fairbalance-0.1.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 09:00:26.473031 fairbalance-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      765 2024-05-22 09:00:09.000000 fairbalance-0.1.4/setup.py
```

### Comparing `fairbalance-0.1.3/PKG-INFO` & `fairbalance-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairbalance
-Version: 0.1.3
+Version: 0.1.4
 Summary: bias mitigation by balancing target and/or protected attributes using resampling techniques
 Author: Pierre-Antoine Lequeu @ Fujitsu Luxembourg
 Author-email: pierre-antoine.lequeu@fujitsu.com
 Description-Content-Type: text/markdown
 Requires-Dist: folktables>=0.0.12
 Requires-Dist: imbalanced_learn==0.9.1
 Requires-Dist: numpy>=1.24.3
```

### Comparing `fairbalance-0.1.3/fairbalance/datasets/_datasets_loader.py` & `fairbalance-0.1.4/fairbalance/datasets/_datasets_loader.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,31 +16,34 @@
         - Including the target column in the dataset.
         - Removing the "fnlwgt" column.
         - Replacing the values in the target column: ">50K" & ">50K." to 1 and "<=50k" & "<=50k." to 0.
         - dropping the rows with non-defined values.
     
     The returned dataset is ready-to-use.
     
-    Returns:
-        ([pd.DataFrame, str, list, list]): The dataset, the name of the target column, the list of categorical features and the list of continuous features.
+    Returns
+    ----------
+    [pd.DataFrame, pd.DataFrame, list, list] : The dataset, the target column, the list of categorical features and the list of continuous features.
     """
     data = fetch_ucirepo(id=2)
     
     adult_data = data.data.features.copy()
     targets = data.data.targets.copy()
     
-    adult_data.loc[:, "income"] = targets
     adult_data = adult_data.drop(columns=["fnlwgt"])
-    adult_data["income"] = adult_data["income"].replace({"<=50K.": 0, ">50K.": 1, ">50K": 1, "<=50K": 0})
+    targets["income"] = targets["income"].replace({"<=50K.": 0, ">50K.": 1, ">50K": 1, "<=50K": 0})
+    adult_data.loc[: "income"] = targets
     adult_data = adult_data.dropna()
+    targets = adult_data[["income"]]
+    adult_data = adult_data.drop()
     
     categorical_features = ["workclass", "marital-status", "occupation", "relationship", "native-country", "education", "sex", "race"]
     continuous_features = [feature for feature in adult_data.columns if feature not in categorical_features and feature != "income"]
     
-    return adult_data, "income", categorical_features,continuous_features
+    return adult_data, targets, categorical_features,continuous_features
 
 def load_bank_marketing() :
     """
     Load the bank marketing dataset from the uci ML repository. 
     More info: https://archive.ics.uci.edu/dataset/222/bank+marketing
     
     Prediction task to determine if an individual subscribed to a bank offer.
@@ -52,54 +55,57 @@
         - Removing the "poutcome" column.
         - Replacing the values in the target column: "yes" to 1 and "no" to 0.
         - Replacing the non-defined values in the "contact" column as "unknown".
         - dropping the rows with non-defined values.
     
     The returned dataset is ready-to-use.
     
-    Returns:
-        ([pd.DataFrame, str, list, list]): The dataset, the name of the target column, the list of categorical features and the list of continuous features.
+    Returns
+    ----------
+    [pd.DataFrame, pd.DataFrame, list, list] : The dataset, the target column, the list of categorical features and the list of continuous features.
     """
     data = fetch_ucirepo(id=222)
     
     bank_data = data.data.features.copy()
     targets = data.data.targets.copy()
-    bank_data.loc[:, "subscribed"] = targets
+    
+    targets = targets.rename(columns={"y" : "subscribed"})
     
     bank_data["age"] = bank_data["age"].apply(lambda x: "x>25" if x > 25 else "x<=25")
     
     bank_data = bank_data.drop(columns=["poutcome"])
     bank_data["contact"] = bank_data["contact"].fillna("unknown")
     bank_data = bank_data.dropna()
-    bank_data["subscribed"] = bank_data["subscribed"].replace({"yes": 1, "no": 0})
+    targets["subscribed"] = targets["subscribed"].replace({"yes": 1, "no": 0})
     
     categorical_features = ["job", "marital", "education", "default", "housing", "loan", "contact", "month", "day_of_week", "age"]
     continuous_features = [feature for feature in bank_data.columns if feature not in categorical_features and feature != "subscribed"]
     
-    return bank_data, "subscribed", categorical_features, continuous_features
+    return bank_data, targets, categorical_features, continuous_features
 
 def load_KDD_census() :
     """
+    /!\ The UCIML repo has some trouble downloading this dataset. Might take a while or even never achieve, without throwing an error.
     Load the bank KDD census income dataset from the uci ML repository. 
     More info: https://archive.ics.uci.edu/dataset/117/census+income+kdd
     
     Prediction task to determine the income of individuals in a binary manner. 
     The target column is "income", with values 1 and 0 (1: >50k, 0: <=50k).
     The protected attributes are the columns "sex" and "race" with the protected attributes "Male" and "White".
     
     The dataset goes through preprocessing steps and is not exactly the one shared by UCI. These steps include:
-        - Including the target column in the dataset.
         - Dropping the duplicates columns.
         - Replacing the values in the target column: "50000+." to 1 and "-50000" to 0.
         - dropping the rows with non-defined values.
     
     The returned dataset is ready-to-use.
     
-    Returns:
-        ([pd.DataFrame, str, list, list]): The dataset, the name of the target column, the list of categorical features and the list of continuous features.
+    Returns
+    ----------
+    [pd.DataFrame, str, list, list] : The dataset, the name of the target column, the list of categorical features and the list of continuous features.
     """
     data = fetch_ucirepo(id=117)
      
     kdd_data = data.data.features.copy()
     targets = data.data.targets.copy()
      
     colum_names = ["age","workclass","industry_code","occupation_code","education","enrolled_in_edu_inst_last_wk",
@@ -143,22 +149,26 @@
         states (list, optional): The US state(s) to include in the survey. Defaults to ["CA"].
         horizon (str, optional): Horizon of the survey. Available values are "1-Year" and "5-Year". Defaults to "1-Year".
         survey (str, optional): type of survey. Available values are "person" and "household". Defaults to 'person'.
 
     Prediction task to determine the given "target" in a binary manner. 
     The target column is encoded with values 1 and 0 (1: >50k, 0: <=50k).
     The protected attributes are the columns "SEX" and "RAC1P" with the protected attributes "1" and "1".
+    The protected attributes coding is as follow: 
+    SEX: {1 : "Male", 2 : "Female"}
+    RAC1P: {1 : "White", 2 : "Black", 3 : "Native_American", 4 : "Native_American", 5 : "Native_American", 6 : "Asian", 7 : "Islander", 8 : "Other", 9 : "Mixed" } 
     
     The dataset goes through preprocessing steps and is not exactly the one shared by the ACS. These steps include:
-        - Including the target column in the dataset.
+        - changing the target as type int
 
     The returned dataset is ready-to-use.
 
-    Returns:
-        ([pd.DataFrame, str, list, list]): The dataset, the name of the target column, the list of categorical features and the list of continuous features.
+    Returns
+    ----------
+    [pd.DataFrame, str, list, list] : The dataset, the name of the target column, the list of categorical features and the list of continuous features.
     """
     
     sex_map = {1 : "Male", 2 : "Female"}
     rac1p_map = {1 : "White", 2 : "Black", 3 : "Native_American", 4 : "Native_American", 5 : "Native_American", 6 : "Asian", 7 : "Islander", 8 : "Other", 9 : "Mixed" } 
     data_source = ACSDataSource(survey_year=survey_year, horizon=horizon, survey=survey, root_dir="./datasets/acs_data/raw")
     data = data_source.get_data(states=states, download=True)
     
@@ -175,18 +185,18 @@
         df, target_df, _ = ACSMobility.df_to_pandas(data)
         categorical_features = ['MAR','DIS','ESP','CIT','MIL','ANC','NATIVITY','RELP','DEAR','DEYE','DREM','GCL','COW','ESR','WKHP','JWMNP','PINCP']
     elif target == "traveltime":
         df, target_df, _ = ACSTravelTime.df_to_pandas(data)
         categorical_features = ['MAR','DIS','ESP','MIG','RELP','PUMA','ST','CIT','OCCP','JWTR','POWPUMA','POVPIP']
         
     target_df = target_df.astype(int)
-    target_df = target_df[target_df.columns[0]]
-    df.loc[:, target] = target_df
+    # target_df = target_df[target_df.columns[0]]
+
     # df.loc[:,"SEX"] = df["SEX"].apply(lambda x : sex_map[x])
     # df.loc[:,"RAC1P"] = df["RAC1P"].apply(lambda x : rac1p_map[x])
     
     categorical_features.append("SEX")
     categorical_features.append("RAC1P")
     
     continuous_features = [feature for feature in df.columns if feature not in categorical_features and feature != target]
     
-    return df, target, categorical_features, continuous_features
+    return df, target_df, categorical_features, continuous_features
```

### Comparing `fairbalance-0.1.3/fairbalance/metrics/_fairness_analysis.py` & `fairbalance-0.1.4/fairbalance/tools/_fairness_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pandas as pd
 
-from ..tools._utils import binarize_columns, sanity_checker
-from ._dataset_metrics import *
+from ._utils import binarize_columns
+from metrics import *
+from ._utils import sanity_checker
 
 class FairnessAnalysis(sanity_checker) :
     def __init__(self, dataset: pd.DataFrame, target : str, positive_output_target, protected_attributes: list, privileged_groups: dict) :
         """
         The FairnessAnalysis class gives an easy and straightforward way to assess the fairness and the biais of a dataset.
 
         Args:
```

### Comparing `fairbalance-0.1.3/fairbalance/metrics/_model_metrics.py` & `fairbalance-0.1.4/fairbalance/metrics/_model_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     
     assert x_true.shape[0] == len(y_true), "features dataframe and output should have the smae number of elements"
     assert len(y_pred) == len(y_true), "predicted output and true output should have the smae number of elements"
     
     assert attribute in list(x_true.columns), f"{attribute} is not a column of the dataframe"
     assert privileged_group in list(x_true[attribute].unique()), f"{privileged_group} is not a class of {attribute}"
 
+
 def EO(x_true, y_true, y_pred, attribute, privileged_group) :
     """Equal Opportunity \n
     P(Y' = 1 = 1 | S = 1, Y = 1) - P(Y' = 1 | S = 0, Y = 1).
 
     Args:
         x_true (_type_): _description_
         y_true (_type_): _description_
```

### Comparing `fairbalance-0.1.3/fairbalance/metrics/tests/test_dataset_metrics.py` & `fairbalance-0.1.4/fairbalance/metrics/tests/test_dataset_metrics.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.3/fairbalance/processors/base.py` & `fairbalance-0.1.4/fairbalance/processors/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,114 +1,125 @@
+from sys import prefix
 import pandas as pd
 from sklearn.calibration import LabelEncoder
 from sklearn.preprocessing import MinMaxScaler
 
-class BaseProcessor :
-    def _process(self, X, y, cont_columns, cat_columns) :
-        pass
-    
-    def _unprocess(self, X, y) :
-        pass
-    
-    def set_categorical_features(self, cat_features) :
-        self.categorical_features = cat_features
-        
+
 
 
 class Processor :
-    def __init__(self, prefix_sep: str = "~") :
-        """
-        Dataset processor to dummify, encode and scale columns and adapt it to learning or mitigation.
-        A Processor object shouldn't be used to process different datasets. If you need to process two different datasets, 
-        it is good practice to use two different processors.
-        
-        Args:
-            prefix_sex (str, optional) : the prefix separator for dummification and undummification. It shouldn't be in any columns name of the dataset. Default to "~". 
-        """
+    """Dataset processor to dummify, encode and scale columns and adapt it to learning or mitigation.
+    A Processor object shouldn't be used to process different datasets. If you need to process two different datasets, 
+    it is good practice to use two different processors.
+    
+    Parameters
+    ----------
+    prefix_sex : str, optional 
+        The prefix separator for dummification and undummification. It shouldn't be in any columns name of the dataset. Default to "~". 
+    """
 
+    def __init__(self, prefix_sep: str = "~") :
         self.prefix_sep = prefix_sep
         self.scalers = {}
         self.label_encoders = {}
         self.types = {}
     
     def _get_columns_types(self, dataset: pd.DataFrame) :
         self.types = dataset.dtypes
     
     def _dummify(self, dataset: pd.DataFrame, columns: list) :
-        """
-        Dummify the given columns using the prefix separator defined when initializing the Processor object.
-        For example, a column "Race" with values "Male" and "Female" and prefix_sep="~" will become two columns "Race~Male" and "Race~Female" with values 1 and 0.
-        
-        Args:
-            dataset (pd.Dataframe) : The dataset to transform
-            columns (list) : The columns to dummify
+        """Dummify the given columns using the prefix separator defined when initializing the Processor object.
+        For example, a column "Race" with values "Male" and "Female" and prefix_sep="~" will become two columns 
+        "Race~Male" and "Race~Female" with values 1 and 0.
+        
+        Parameters
+        ----------
+        dataset : pd.Dataframe 
+            The dataset to transform
+        columns : list 
+            The columns to dummify
         
         Returns 
-            ([pd.DataFrame]) : The dummified dataset  
+        ----------
+        [pd.DataFrame] : The dummified dataset  
         """
         for column in columns :
             assert column in dataset.columns, f"feature {column} not in the dataset"
             assert self.prefix_sep not in column, f"""'{self.prefix_sep}' is the prefix separator for the dummifying process, but is in the column name {column}""" 
         
         return pd.get_dummies(data = dataset, columns=columns, prefix_sep=self.prefix_sep, dtype='int')
     
     def _encode(self, dataset: pd.DataFrame, columns: list) :
-        """
-        Encode the given columns.
-        Encode the different labels of a column to give them Int values. for example, a column "Race" with values "Male" and "Female" would be transformed into 
-        a column "Race" with values 1 and 2 where 1 encodes "Male" and 2 encodes "Female".
-        
-        Args:
-            dataset (pd.Dataframe) : The dataset to transform
-            columns (list) : The columns to dummify
+        """Encode the given columns.
+        Encode the different labels of a column to give them Int values. for example, a column "Race" with values 
+        "Male" and "Female" would be transformed into a column "Race" with values 1 and 2 where 1 encodes "Male" and 
+        2 encodes "Female".
+        
+        Parameters
+        ----------
+        dataset : pd.Dataframe
+            The dataset to transform
+        columns : list
+            The columns to dummify
         
         Returns 
-            ([pd.DataFrame]) : The encoded dataset  
+        ----------
+        [pd.DataFrame] : The encoded dataset  
         """
         for feature in columns :
             assert feature in dataset.columns, f"feature {feature} not in the dataset"
             le = LabelEncoder()
             dataset[feature] = le.fit_transform(dataset[feature])
             self.label_encoders[feature] = le
        
         return dataset
             
     def _scale(self, dataset: pd.DataFrame, columns: list) :
         """
         Scale the given columns.
         Scales the columns using the skLearn StandardScaler.
         
-        Args:
-            dataset (pd.Dataframe) : The dataset to transform
-            columns (list) : The columns to dummify
-        
-        Returns 
-            ([pd.DataFrame]) : The scaled dataset  
+        Parameters
+        ----------
+        dataset : pd.Dataframe
+            The dataset to transform
+        columns : list 
+            The columns to dummify
+        
+        Returns
+        ----------
+        [pd.DataFrame] : The scaled dataset  
         """
         for feature in columns :
             assert feature in dataset.columns, f"feature {feature} not in the dataset"
             scaler = MinMaxScaler()
             dataset[feature] = scaler.fit_transform(dataset[feature].values.reshape(-1, 1))
             self.scalers[feature] = scaler
         
         return dataset
         
     def process(self, dataset: pd.DataFrame, dummify_cols: list = [], 
                 scale_cols: list = [], encode_cols: list = []) :
         """
         Process the datasets by dummifying, scaling and encoding the necessary columns.
 
-        Args:
-            dataset (pd.DataFrame): The dataset to transform.
-            dummify_cols (list, optional): The columns to dummifying. Defaults to [].
-            scale_cols (list, optional): The columns to scale. Defaults to [].
-            encode_cols (list, optional): The columns to encode. Defaults to [].
-
-        Returns:
-            ([pd.DataFrame]): The transformed dataset.
+        Parameters
+        ----------
+        dataset : pd.DataFrame 
+            The dataset to transform.
+        dummify_cols : list, optional 
+            The columns to dummifying. Defaults to [].
+        scale_cols : list, optional
+            he columns to scale. Defaults to [].
+        encode_cols : list, optional 
+            The columns to encode. Defaults to [].
+
+        Returns
+        ----------
+        [pd.DataFrame] : The transformed dataset.
         """
         df = dataset.copy()
         self._get_columns_types(df) 
 
         self.dummify_cols = dummify_cols
         self.scale_cols = scale_cols
         self.encode_cols = encode_cols
@@ -127,61 +138,73 @@
     
         return df
     
     
     def _undummify(self, dataset: pd.DataFrame) :
         """Undummify the columns previously dummified.
 
-        Args:
-            dataset (pd.DataFrame): The dataset to transform
+        Parameters
+        ----------
+        dataset : pd.DataFrame 
+            The dataset to transform
 
         Returns:
-            ([pd.dataFrame]): The transformed dataset
+        ----------
+        [pd.dataFrame] : The transformed dataset
         """
         undummified = self._undummify_df(dataset)
         for column in self.dummify_cols :
             undummified[column] = undummified[column].astype(self.types[column])
         return  undummified
     
     def _unencode(self, dataset: pd.DataFrame) :
         """Unencode the columns previously encoded.
 
-        Args:
-            dataset (pd.DataFrame): The dataset to transform
-
-        Returns:
-            ([pd.dataFrame]): The transformed dataset
+        Parameters
+        ----------
+        dataset : pd.DataFrame 
+            The dataset to transform
+
+        Returns
+        ----------
+        [pd.dataFrame] : The transformed dataset
         """
         for feature in self.encode_cols :
             le = self.label_encoders[feature]
             dataset[feature] = le.inverse_transform(dataset[feature])
         return dataset
     
     def _unscale(self, dataset: pd.DataFrame) :
         """Unscale the columns previously scaled.
 
-        Args:
-            dataset (pd.DataFrame): The dataset to transform
-
-        Returns:
-            ([pd.dataFrame]): The transformed dataset
+        Parameters
+        ----------
+        dataset : pd.DataFrame 
+            The dataset to transform
+
+        Returns
+        ----------
+        [pd.dataFrame] : The transformed dataset
         """
         for feature in self.scale_cols :
             scaler = self.scalers[feature]
             dataset[feature] = scaler.inverse_transform(dataset[[feature]])
         return dataset
     
     def unprocess(self, dataset: pd.DataFrame) :
         """Unprocess all the process made when Processor.process was called.
 
-        Args:
-            dataset (pd.DataFrame): The dataset to transform.
-
-        Returns:
-            ([pd.dataFrame]): The transformed dataset
+        Parameters
+        ----------
+        dataset : pd.DataFrame 
+            The dataset to transform.
+
+        Returns
+        ----------
+        [pd.dataFrame] : The transformed dataset
         """
         
         df = dataset.copy()
         
         #remove dummies
         if self.dummify_cols :
             df = self._undummify(df)
@@ -191,7 +214,34 @@
             df = self._unencode(df)
         
         #remove scaling
         if self.scale_cols :
             df = self._unscale(df)
             
         return df
+
+
+
+class BaseProcessor(Processor) :
+    """Dataset processor to dummify, encode and scale columns and adapt it to learning or mitigation.
+    A Processor object shouldn't be used to process different datasets. If you need to process two different datasets, 
+    it is good practice to use two different processors.
+    
+    Parameters
+    ----------
+    prefix_sex : str, optional 
+        The prefix separator for dummification and undummification. It shouldn't be in any columns name of the dataset. Default to "~". 
+    """
+    def __init__(self, prefix_sep: str = "~") :
+        
+        super().__init__(prefix_sep=prefix_sep)
+        
+    
+    def _process(self, X, y, cont_columns, cat_columns) :
+        pass
+    
+    def _unprocess(self, X, y) :
+        pass
+    
+    def set_categorical_features(self, cat_features) :
+        self.categorical_features = cat_features
+
```

### Comparing `fairbalance-0.1.3/fairbalance/tools/__init__.py` & `fairbalance-0.1.4/fairbalance/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.3/fairbalance/tools/_fairness_analysis.py` & `fairbalance-0.1.4/fairbalance/metrics/_fairness_analysis.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,106 @@
 import pandas as pd
 
-from ._utils import binarize_columns
-from metrics import *
-from ._utils import sanity_checker
+from ..tools._utils import binarize_columns, sanity_checker
+from ._dataset_metrics import *
 
 class FairnessAnalysis(sanity_checker) :
-    def __init__(self, dataset: pd.DataFrame, target : str, positive_output_target, protected_attributes: list, privileged_groups: dict) :
-        """
-        The FairnessAnalysis class gives an easy and straightforward way to assess the fairness and the biais of a dataset.
+    """The FairnessAnalysis class gives an easy and straightforward way to assess the fairness and the biais of a dataset.
 
-        Args:
-            dataset (pd.DataFrame): The dataset to analyse, including the target column
-            target (str): The target column name
-            positive_output_target (str | int | float): the output considered positive for the given target
-            protected_attributes (list): list of the protected attributes of the dataset
-            privileged_group (dict): privileged class for each protected attribute 
+    Parameters
+    ----------
+    dataset : pd.DataFrame 
+        The dataset to analyse, including the target column.
+    target : str 
+        The target column name.
+    positive_output_target : Any
+        the output considered positive for the given target.
+    protected_attributes : list 
+        List of the protected attributes of the dataset.
+    privileged_group : dict 
+        privileged class for each protected attribute. 
+            
+    Attributes
+    ----------
+    **After self.get_disparate_impact_ratio() is called:**
+    disparate_impact_ratio : dict
+        The Disparate Impact Ratio for each unprivileged class of each protected attribute.
+    RMSDIR : dict
+        The Root Mean Squared of DIR the classes of each protected attribute. 
+
+    **After self.get_statistical_parity_difference() is called:**
+    statistical_parity_difference : dict
+        The statistical parity difference of each protected attribute.
+    
+    **After self.get_pointwise_mutual_information() is called:**
+    pointwise_mutual_information : dict
+        The pointiwise mutual information between each class of each protected attribute with each output.
+    pointwise_mutual_information_ratio : dict
+        The PMI of the unprivileged class over the PMI of the privileged class for each output.
+    RMSPMI : dict
+        The Root Mean Squared of the PMI of the classes of each protected attribute.
+    
+    **After self.get_balance() is called:**
+    balance : dict(pd.DataFrame)
+        The number of element of each class of each protected attribute.
+    balance_index : dict
+        The balance index of each protected attribute.
+    
+    **After self.get_fairness_score() is called:**
+    attribute_fairness_score : dict
+        The Composite Fairness Score (CFS) for each protected attribute.
+    fairness_score : float
+        The overall Composite Fairness Score (CFS) of the dataset.        
         """
-        
+    def __init__(self, dataset: pd.DataFrame, target : str, positive_output_target, protected_attributes: list, privileged_groups: dict) :
         super()._sanity_check(dataset, target, positive_output_target, protected_attributes, privileged_groups)
         
         self.dataset = dataset
         self.protected_attributes = protected_attributes
         self.privileged_groups = privileged_groups
         
         #set target attribute
         self.target = self.dataset[[target]]
         self.positive_output_target = positive_output_target
     
   
     def _make_binary_column(self, dataset :pd.DataFrame, protected_attribute: str, privileged_group: str) :
-        """
-        Returns a DataFrame which contains of column of the protected attribute with binary value (privileged and non_privileged)
-        and a column of the output with binary value (positive output and non_positive output)
+        """Returns a DataFrame which contains of column of the protected attribute with binary value (privileged and non_privileged)
+        and a column of the output with binary value (positive output and non_positive output).
         
-        Args:
-            dataset (pd.DataFrame): the dataset to trandform
-            protected_attributes (str): protected attributes you want to binarize
-            privileged_group (str): privileged class for the protected attribute 
-
-        Returns:
-            (pd.DataFrame): dataset with the binarized protected attribute (privileged_group, non_privileged_group)
+        Parameters
+        ----------
+        dataset : pd.DataFrame 
+            The dataset to trandform.
+        protected_attributes : str
+            The protected attributes you want to binarize.
+        privileged_group : str 
+            The privileged class for the protected attribute 
+
+        Returns
+        ----------
+        [pd.DataFrame] : dataset with the binarized protected attribute (privileged_group, non_privileged_group)
         """
 
         return binarize_columns(dataset, [protected_attribute], {protected_attribute: privileged_group})
     
         
     def get_disparate_impact_ratio(self, binary=False) :
         """
         The Disparate Impact Ratio (DIR) is the ratio of rate of favorable outcomes 
         for the unprivileged group to that of the privileged group.
             
-        Args:
-            binary (bool, optional): True if the protected attribute(s) and output should be binarized. Defaults to False.
-        
-        Returns:
-            ([dict, dict]): the DIR of each class of each protected attribute and the RMSDIR of each protected attribute
+        Parameters
+        ----------
+        binary : bool, optional
+            True if the protected attribute(s) and output should be binarized. Defaults to False.
+    
+        Returns
+        ----------
+        [dict, dict] : the DIR of each class of each protected attribute and the RMSDIR of each protected attribute
         """   
 
         self.disparate_impact_ratio = {}
         self.RMSDIR = {}
         data = self.dataset.copy()
         
         for protected_attribute in self.protected_attributes :
@@ -79,19 +121,22 @@
       
     
     def get_statistical_parity_difference(self, binary=False) :
         """
         The Statistical Parity Difference (SPD) is the difference of the rate of favorable outcomes 
         received by the unprivileged group to the privileged group.
             
-        Args:
-            binary (bool, optional): True if the protected attribute(s) and output should be binarized. Defaults to False.
-        
-        Returns:
-            ([dict]): The statistical parity difference of each protected attribute.
+        Parameters
+        ----------
+        binary : bool, optional 
+            True if the protected attribute(s) and output should be binarized. Defaults to False.
+        
+        Returns
+        ----------
+        [dict]: The statistical parity difference of each protected attribute.
         """
         
         
         self.statistical_parity_difference = {}
         data = self.dataset.copy()
         for protected_attribute in self.protected_attributes :
     
@@ -104,24 +149,26 @@
                                                                           self.target.columns[0], self.positive_output_target
                                                                           )
         
         return self.statistical_parity_difference
                     
     
     def get_pointwise_mutual_information(self, binary=False) :
-        """
-        The (Normalized) Pointwise Mutual Information is a measure of association. It compares the probability of two events happening together to this probability
-        if these events were independents.
+        """The (Normalized) Pointwise Mutual Information is a measure of association. It compares 
+        the probability of two events happening together to this probability if these events were independents.
         
-        Args:
-            binary (bool, optional): True if the protected attribute(s) and output should be binarized. Defaults to False.
-        
-        Returns:
-            ([dict, dict, dict]): The pointwise mutual information and pointwise mutual informaiton ratio fo each class of each protected attribute
-            ans the RMSPMI for each protected attribute.
+        Parameters
+        ----------
+        binary : bool, optional 
+            True if the protected attribute(s) and output should be binarized. Defaults to False.
+    
+        Returns
+        ----------
+        [dict, dict, dict] : The pointwise mutual information and pointwise mutual informaiton ratio fo each 
+        class of each protected attribute ans the RMSPMI for each protected attribute.
         """
 
 
         self.pointwise_mutual_information = {}
         self.pointwise_mutual_information_ratio = {}
         self.RMSPMI = {}
         
@@ -141,24 +188,27 @@
             self.pointwise_mutual_information_ratio[protected_attribute] = pmir
             self.RMSPMI[protected_attribute] = RMSPMI
                                      
         return pmi, pmir, RMSPMI
                 
  
     def get_balance(self, binary=False) :
-        """
-        The balance is the number of element for each class of the protected attributes. It can highlight potential biais when training a model.
-        The balance index gives a measure of the balance. 1 means that the features are perfectly balanced (all the classes of each feature has the 
-        same number of element), 0 is the worst case (one class has all the element)
-            
-        Args:
-            binary (bool, optional): True if the protected attribute(s) and output should be binarized. Defaults to False.
-        
-        Returns:
-            ([dict, dict]): the balance and the balance index of each protected_attribute
+        """The balance is the number of element for each class of the protected attributes. It can highlight 
+        potential biais when training a model. The balance index gives a measure of the balance. 1 means 
+        that the features are perfectly balanced (all the classes of each feature has the same number of 
+        element), 0 is the worst case (one class has all the element).
+            
+        Parameters
+        ----------
+        binary : bool, optional 
+            True if the protected attribute(s) and output should be binarized. Defaults to False.
+        
+        Returns
+        ----------
+        [dict, dict] : the balance and the balance index of each protected_attribute
         """
 
         
         self.balance = {}
         self.balance_index = {}
         data = self.dataset.copy()
         for protected_attribute in self.protected_attributes :
@@ -173,23 +223,25 @@
                     
         self.average_balance_index = sum(self.balance_index.values())/len(self.balance_index)
         
         return self.balance, self.balance_index
                  
    
     def get_fairness_score(self, binary=False) :
-        """
-        Average of the fairness scores for all prrotected attribute. \n 
+        """Average of the fairness scores for all prrotected attribute. \n 
         1 means the dataset is considered completely fair, 0 not fair at all.
         
-        Args:
-            binary (bool, optional): True if the protected attribute(s) and output should be binarized. Defaults to False.
-        
-        Returns:
-            ([dict, int]): The fairness score for each protected attribute and the fairness score of the dataset.
+        Parameters
+        ----------
+        binary : bool, optional 
+            True if the protected attribute(s) and output should be binarized. Defaults to False.
+        
+        Returns
+        ----------
+        [dict, int] : The fairness score for each protected attribute and the overall fairness score of the dataset.
         """
         
         final_score = 0
         data = self.dataset.copy()
         self.attribute_fairness_score = {}
         
         for protected_attribute in self.protected_attributes :
@@ -212,18 +264,21 @@
         
         return  self.attribute_fairness_score, self.fairness_score
         
         
     
     def get_fairness_analysis(self, binary=False) :
         """
-        evaluate and print the balance index, DIR, SPD, PMI and fairness score of the dataset. Does not return them, but they can be access through class attributes.
+        evaluate and print the balance index, DIR, SPD, PMI and fairness score of the dataset. 
+        Does not return them, but they can be access through class attributes.
 
-        Args:
-            binary (bool, optional): True if the protected attribute(s) and output should be binarized. Defaults to False.
+        Parameters
+        ----------
+        binary : bool, optional 
+            True if the protected attribute(s) and output should be binarized. Defaults to False.
         """
         self.get_balance(binary)
         
         self.get_disparate_impact_ratio(binary)
         
         self.get_statistical_parity_difference(binary)
```

### Comparing `fairbalance-0.1.3/fairbalance/tools/_mitigator.py` & `fairbalance-0.1.4/fairbalance/tools/_mitigator.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,1451 +4,1107 @@
 00000030: 6e67 2069 6d70 6f72 7420 5261 6e64 6f6d  ng import Random
 00000040: 4f76 6572 5361 6d70 6c65 722c 2053 4d4f  OverSampler, SMO
 00000050: 5445 4e43 0d0a 6672 6f6d 2069 6d62 6c65  TENC..from imble
 00000060: 6172 6e2e 756e 6465 725f 7361 6d70 6c69  arn.under_sampli
 00000070: 6e67 2069 6d70 6f72 7420 5261 6e64 6f6d  ng import Random
 00000080: 556e 6465 7253 616d 706c 6572 0d0a 696d  UnderSampler..im
 00000090: 706f 7274 2066 756e 6374 6f6f 6c73 0d0a  port functools..
-000000a0: 0d0a 6672 6f6d 2074 6f72 6368 2069 6d70  ..from torch imp
-000000b0: 6f72 7420 6361 740d 0a66 726f 6d20 2e5f  ort cat..from ._
-000000c0: 7072 6f63 6573 736f 7220 696d 706f 7274  processor import
-000000d0: 2053 4d4f 5445 4e43 5072 6f63 6573 736f   SMOTENCProcesso
-000000e0: 722c 205f 5072 6f63 6573 736f 720d 0a0d  r, _Processor...
-000000f0: 0a66 726f 6d20 2e62 6173 6520 696d 706f  .from .base impo
-00000100: 7274 2042 6173 654d 6974 6967 6174 696f  rt BaseMitigatio
-00000110: 6e53 7472 6174 6567 792c 2042 6173 6550  nStrategy, BaseP
-00000120: 726f 6365 7373 6f72 0d0a 6672 6f6d 202e  rocessor..from .
-00000130: 5f75 7469 6c73 2069 6d70 6f72 7420 7361  _utils import sa
-00000140: 6e69 7479 5f63 6865 636b 6572 0d0a 0d0a  nity_checker....
-00000150: 0d0a 5341 4d50 4c49 4e47 5f46 554e 4354  ..SAMPLING_FUNCT
-00000160: 494f 4e53 203d 205b 2252 616e 646f 6d4f  IONS = ["RandomO
-00000170: 7665 7253 616d 706c 6572 222c 2022 534d  verSampler", "SM
-00000180: 4f54 454e 4322 2c20 2252 616e 646f 6d55  OTENC", "RandomU
-00000190: 6e64 6572 5361 6d70 6c65 7222 5d0d 0a0d  nderSampler"]...
-000001a0: 0a20 2020 0d0a 0d0a 636c 6173 7320 4261  .   ....class Ba
-000001b0: 6c61 6e63 654f 7574 7075 7428 4261 7365  lanceOutput(Base
-000001c0: 4d69 7469 6761 7469 6f6e 5374 7261 7465  MitigationStrate
-000001d0: 6779 2920 3a0d 0a20 2020 2022 2222 5465  gy) :..    """Te
-000001e0: 7374 0d0a 0d0a 2020 2020 4172 6773 3a0d  st....    Args:.
-000001f0: 0a20 2020 2020 2020 2042 6173 654d 6974  .        BaseMit
-00000200: 6967 6174 696f 6e53 7472 6174 6567 7920  igationStrategy 
-00000210: 285f 7479 7065 5f29 3a20 5f64 6573 6372  (_type_): _descr
-00000220: 6970 7469 6f6e 5f0d 0a20 2020 2022 2222  iption_..    """
-00000230: 0d0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-00000240: 5f5f 2873 656c 662c 2073 616d 706c 6572  __(self, sampler
-00000250: 3a20 4261 7365 5072 6f63 6573 736f 7229  : BaseProcessor)
-00000260: 203a 0d0a 2020 2020 2020 2020 7375 7065   :..        supe
-00000270: 7228 292e 5f5f 696e 6974 5f5f 2873 616d  r().__init__(sam
-00000280: 706c 6572 290d 0a20 2020 200d 0a20 2020  pler)..    ..   
-00000290: 2064 6566 2062 616c 616e 6365 2873 656c   def balance(sel
-000002a0: 662c 2064 6174 6173 6574 3a20 7064 2e44  f, dataset: pd.D
-000002b0: 6174 6146 7261 6d65 2c20 7461 7267 6574  ataFrame, target
-000002c0: 3a20 7064 2e44 6174 6146 7261 6d65 203d  : pd.DataFrame =
-000002d0: 204e 6f6e 652c 2070 726f 7465 6374 6564   None, protected
-000002e0: 5f61 7474 7269 6275 7465 733a 206c 6973  _attributes: lis
-000002f0: 7420 3d20 4e6f 6e65 2c20 0d0a 2020 2020  t = None, ..    
-00000300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000310: 2020 2063 6f6e 745f 636f 6c75 6d6e 733a     cont_columns:
-00000320: 206c 6973 7420 3d20 4e6f 6e65 2c20 6361   list = None, ca
-00000330: 745f 636f 6c75 6d6e 733a 206c 6973 7420  t_columns: list 
-00000340: 3d20 4e6f 6e65 2920 3a0d 0a20 2020 2020  = None) :..     
-00000350: 2020 200d 0a20 2020 2020 2020 2064 662c     ..        df,
-00000360: 2070 726f 7465 6374 6564 5f61 7474 7269   protected_attri
-00000370: 6275 7465 203d 2073 656c 662e 5f67 6574  bute = self._get
-00000380: 5f64 6174 6166 7261 6d65 5f61 6e64 5f70  _dataframe_and_p
-00000390: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
-000003a0: 7465 2864 6174 6173 6574 2c20 7072 6f74  te(dataset, prot
-000003b0: 6563 7465 645f 6174 7472 6962 7574 6573  ected_attributes
-000003c0: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
-000003d0: 2020 2020 2058 5f70 726f 6365 7373 6564       X_processed
-000003e0: 2c20 795f 7072 6f63 6573 7365 6420 3d20  , y_processed = 
-000003f0: 7365 6c66 2e73 616d 706c 6572 2e5f 7072  self.sampler._pr
-00000400: 6f63 6573 7328 6466 2c20 7461 7267 6574  ocess(df, target
-00000410: 2c20 636f 6e74 5f63 6f6c 756d 6e73 2c20  , cont_columns, 
-00000420: 6361 745f 636f 6c75 6d6e 7329 0d0a 2020  cat_columns)..  
-00000430: 2020 2020 2020 585f 7265 7361 6d70 6c65        X_resample
-00000440: 642c 2079 5f72 6573 616d 706c 6564 203d  d, y_resampled =
-00000450: 2073 656c 662e 7361 6d70 6c65 722e 6669   self.sampler.fi
-00000460: 745f 7265 7361 6d70 6c65 2858 5f70 726f  t_resample(X_pro
-00000470: 6365 7373 6564 2c20 795f 7072 6f63 6573  cessed, y_proces
-00000480: 7365 6429 0d0a 2020 2020 2020 2020 585f  sed)..        X_
-00000490: 6669 6e61 6c2c 2079 5f66 696e 616c 203d  final, y_final =
-000004a0: 2073 656c 662e 7361 6d70 6c65 722e 5f75   self.sampler._u
-000004b0: 6e70 726f 6365 7373 2858 5f72 6573 616d  nprocess(X_resam
-000004c0: 706c 6564 2c20 795f 7265 7361 6d70 6c65  pled, y_resample
-000004d0: 6429 0d0a 2020 2020 2020 2020 0d0a 2020  d)..        ..  
-000004e0: 2020 2020 2020 585f 6669 6e61 6c20 3d20        X_final = 
-000004f0: 7365 6c66 2e5f 6765 745f 6669 6e61 6c5f  self._get_final_
-00000500: 6461 7461 6672 616d 6528 585f 6669 6e61  dataframe(X_fina
-00000510: 6c2c 2070 726f 7465 6374 6564 5f61 7474  l, protected_att
-00000520: 7269 6275 7465 732c 2070 726f 7465 6374  ributes, protect
-00000530: 6564 5f61 7474 7269 6275 7465 290d 0a20  ed_attribute).. 
-00000540: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00000550: 2072 6574 7572 6e20 585f 6669 6e61 6c2c   return X_final,
-00000560: 2079 5f66 696e 616c 2020 2020 200d 0a0d   y_final     ...
-00000570: 0a0d 0a63 6c61 7373 2042 616c 616e 6365  ...class Balance
-00000580: 4174 7472 6962 7574 6573 2842 6173 654d  Attributes(BaseM
-00000590: 6974 6967 6174 696f 6e53 7472 6174 6567  itigationStrateg
-000005a0: 7929 203a 0d0a 2020 2020 6465 6620 5f5f  y) :..    def __
-000005b0: 696e 6974 5f5f 2873 656c 662c 2073 616d  init__(self, sam
-000005c0: 706c 6572 3a20 4261 7365 5072 6f63 6573  pler: BaseProces
-000005d0: 736f 7229 203a 0d0a 2020 2020 2020 2020  sor) :..        
-000005e0: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
-000005f0: 2873 616d 706c 6572 290d 0a0d 0a20 2020  (sampler)....   
-00000600: 2064 6566 2062 616c 616e 6365 2873 656c   def balance(sel
-00000610: 662c 2064 6174 6173 6574 3a20 7064 2e44  f, dataset: pd.D
-00000620: 6174 6146 7261 6d65 2c20 7461 7267 6574  ataFrame, target
-00000630: 3a20 7064 2e44 6174 6146 7261 6d65 203d  : pd.DataFrame =
-00000640: 204e 6f6e 652c 2070 726f 7465 6374 6564   None, protected
-00000650: 5f61 7474 7269 6275 7465 733a 206c 6973  _attributes: lis
-00000660: 7420 3d20 4e6f 6e65 2c20 0d0a 2020 2020  t = None, ..    
-00000670: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00000680: 5f63 6f6c 756d 6e73 3a20 6c69 7374 203d  _columns: list =
-00000690: 204e 6f6e 652c 2063 6174 5f63 6f6c 756d   None, cat_colum
-000006a0: 6e73 3a20 6c69 7374 203d 204e 6f6e 6529  ns: list = None)
-000006b0: 203a 0d0a 2020 2020 2020 2020 0d0a 2020   :..        ..  
-000006c0: 2020 2020 2020 6466 2c20 7072 6f74 6563        df, protec
-000006d0: 7465 645f 6174 7472 6962 7574 6520 3d20  ted_attribute = 
-000006e0: 7365 6c66 2e5f 6765 745f 6461 7461 6672  self._get_datafr
-000006f0: 616d 655f 616e 645f 7072 6f74 6563 7465  ame_and_protecte
-00000700: 645f 6174 7472 6962 7574 6528 6461 7461  d_attribute(data
-00000710: 7365 742c 2070 726f 7465 6374 6564 5f61  set, protected_a
-00000720: 7474 7269 6275 7465 7329 0d0a 0d0a 2020  ttributes)....  
-00000730: 2020 2020 2020 585f 7072 6f63 6573 7365        X_processe
-00000740: 642c 2079 5f70 726f 6365 7373 6564 203d  d, y_processed =
-00000750: 2073 656c 662e 7361 6d70 6c65 722e 5f70   self.sampler._p
-00000760: 726f 6365 7373 2864 662c 2074 6172 6765  rocess(df, targe
-00000770: 742c 2063 6f6e 745f 636f 6c75 6d6e 732c  t, cont_columns,
-00000780: 2063 6174 5f63 6f6c 756d 6e73 290d 0a20   cat_columns).. 
-00000790: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000007a0: 2070 726f 7465 6374 6564 5f61 7474 7269   protected_attri
-000007b0: 6275 7465 5f63 6f6c 756d 6e20 3d20 585f  bute_column = X_
-000007c0: 7072 6f63 6573 7365 645b 7072 6f74 6563  processed[protec
-000007d0: 7465 645f 6174 7472 6962 7574 655d 0d0a  ted_attribute]..
-000007e0: 2020 2020 2020 2020 585f 7072 6f63 6573          X_proces
-000007f0: 7365 6420 3d20 585f 7072 6f63 6573 7365  sed = X_processe
-00000800: 642e 6472 6f70 2863 6f6c 756d 6e73 3d5b  d.drop(columns=[
-00000810: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
-00000820: 7574 655d 290d 0a20 2020 2020 2020 2058  ute])..        X
-00000830: 5f70 726f 6365 7373 6564 2e6c 6f63 5b3a  _processed.loc[:
-00000840: 2c22 7461 7267 6574 225d 203d 2079 5f70  ,"target"] = y_p
-00000850: 726f 6365 7373 6564 0d0a 2020 2020 2020  rocessed..      
-00000860: 2020 6e65 775f 6361 745f 636f 6c75 6d6e    new_cat_column
-00000870: 7320 3d20 5b63 6f6c 756d 6e20 666f 7220  s = [column for 
-00000880: 636f 6c75 6d6e 2069 6e20 6361 745f 636f  column in cat_co
-00000890: 6c75 6d6e 7320 6966 2063 6f6c 756d 6e20  lumns if column 
-000008a0: 213d 2070 726f 7465 6374 6564 5f61 7474  != protected_att
-000008b0: 7269 6275 7465 5d20 2b20 5b22 7461 7267  ribute] + ["targ
-000008c0: 6574 225d 0d0a 2020 2020 2020 2020 6361  et"]..        ca
-000008d0: 745f 636f 6c75 6d6e 735f 6964 7320 3d20  t_columns_ids = 
-000008e0: 5b58 5f70 726f 6365 7373 6564 2e63 6f6c  [X_processed.col
-000008f0: 756d 6e73 2e67 6574 5f6c 6f63 2863 6f6c  umns.get_loc(col
-00000900: 5f6e 616d 6529 2066 6f72 2063 6f6c 5f6e  _name) for col_n
-00000910: 616d 6520 696e 206e 6577 5f63 6174 5f63  ame in new_cat_c
-00000920: 6f6c 756d 6e73 5d0d 0a20 2020 2020 2020  olumns]..       
-00000930: 2073 656c 662e 7361 6d70 6c65 722e 7365   self.sampler.se
-00000940: 745f 6361 7465 676f 7269 6361 6c5f 6665  t_categorical_fe
-00000950: 6174 7572 6573 2863 6174 5f63 6f6c 756d  atures(cat_colum
-00000960: 6e73 5f69 6473 290d 0a0d 0a20 2020 2020  ns_ids)....     
-00000970: 2020 2058 5f72 6573 616d 706c 6564 2c20     X_resampled, 
-00000980: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
-00000990: 7574 655f 7265 7361 6d70 6c65 6420 3d20  ute_resampled = 
-000009a0: 7365 6c66 2e73 616d 706c 6572 2e66 6974  self.sampler.fit
-000009b0: 5f72 6573 616d 706c 6528 585f 7072 6f63  _resample(X_proc
-000009c0: 6573 7365 642c 2070 726f 7465 6374 6564  essed, protected
-000009d0: 5f61 7474 7269 6275 7465 5f63 6f6c 756d  _attribute_colum
-000009e0: 6e29 0d0a 2020 2020 2020 2020 585f 7265  n)..        X_re
-000009f0: 7361 6d70 6c65 642e 6c6f 635b 3a2c 2070  sampled.loc[:, p
-00000a00: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
-00000a10: 7465 5d20 3d20 7072 6f74 6563 7465 645f  te] = protected_
-00000a20: 6174 7472 6962 7574 655f 7265 7361 6d70  attribute_resamp
-00000a30: 6c65 640d 0a20 2020 2020 2020 2079 5f72  led..        y_r
-00000a40: 6573 616d 706c 6564 203d 2058 5f72 6573  esampled = X_res
-00000a50: 616d 706c 6564 5b22 7461 7267 6574 225d  ampled["target"]
-00000a60: 0d0a 2020 2020 2020 2020 585f 7265 7361  ..        X_resa
-00000a70: 6d70 6c65 6420 3d20 585f 7265 7361 6d70  mpled = X_resamp
-00000a80: 6c65 642e 6472 6f70 2863 6f6c 756d 6e73  led.drop(columns
-00000a90: 3d5b 2274 6172 6765 7422 5d29 0d0a 2020  =["target"])..  
-00000aa0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00000ab0: 585f 6669 6e61 6c2c 2079 5f66 696e 616c  X_final, y_final
-00000ac0: 203d 2073 656c 662e 7361 6d70 6c65 722e   = self.sampler.
-00000ad0: 5f75 6e70 726f 6365 7373 2858 5f72 6573  _unprocess(X_res
-00000ae0: 616d 706c 6564 2c20 795f 7265 7361 6d70  ampled, y_resamp
-00000af0: 6c65 6429 0d0a 2020 2020 2020 2020 585f  led)..        X_
-00000b00: 6669 6e61 6c20 3d20 7365 6c66 2e5f 6765  final = self._ge
-00000b10: 745f 6669 6e61 6c5f 6461 7461 6672 616d  t_final_datafram
-00000b20: 6528 585f 6669 6e61 6c2c 2070 726f 7465  e(X_final, prote
-00000b30: 6374 6564 5f61 7474 7269 6275 7465 732c  cted_attributes,
-00000b40: 2070 726f 7465 6374 6564 5f61 7474 7269   protected_attri
-00000b50: 6275 7465 290d 0a0d 0a20 2020 2020 2020  bute)....       
-00000b60: 2072 6574 7572 6e20 585f 6669 6e61 6c2c   return X_final,
-00000b70: 2079 5f66 696e 616c 0d0a 2020 2020 2020   y_final..      
-00000b80: 2020 0d0a 636c 6173 7320 4261 6c61 6e63    ..class Balanc
-00000b90: 654f 7574 7075 7446 6f72 4174 7472 6962  eOutputForAttrib
-00000ba0: 7574 6573 2842 6173 654d 6974 6967 6174  utes(BaseMitigat
-00000bb0: 696f 6e53 7472 6174 6567 7929 203a 0d0a  ionStrategy) :..
-00000bc0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00000bd0: 2873 656c 662c 2073 616d 706c 6572 3a20  (self, sampler: 
-00000be0: 4261 7365 5072 6f63 6573 736f 7229 203a  BaseProcessor) :
-00000bf0: 0d0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
-00000c00: 292e 5f5f 696e 6974 5f5f 2873 616d 706c  ).__init__(sampl
-00000c10: 6572 290d 0a20 2020 200d 0a20 2020 2064  er)..    ..    d
-00000c20: 6566 2062 616c 616e 6365 2873 656c 662c  ef balance(self,
-00000c30: 2064 6174 6173 6574 3a20 7064 2e44 6174   dataset: pd.Dat
-00000c40: 6146 7261 6d65 2c20 7461 7267 6574 3a20  aFrame, target: 
-00000c50: 7064 2e44 6174 6146 7261 6d65 203d 204e  pd.DataFrame = N
-00000c60: 6f6e 652c 2070 726f 7465 6374 6564 5f61  one, protected_a
-00000c70: 7474 7269 6275 7465 733a 206c 6973 7420  ttributes: list 
-00000c80: 3d20 4e6f 6e65 2c20 0d0a 2020 2020 2020  = None, ..      
-00000c90: 2020 2020 2020 2020 2020 636f 6e74 5f63            cont_c
-00000ca0: 6f6c 756d 6e73 3a20 6c69 7374 203d 204e  olumns: list = N
-00000cb0: 6f6e 652c 2063 6174 5f63 6f6c 756d 6e73  one, cat_columns
-00000cc0: 3a20 6c69 7374 203d 204e 6f6e 6529 203a  : list = None) :
-00000cd0: 0d0a 0d0a 2020 2020 2020 2020 6466 2c20  ....        df, 
-00000ce0: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
-00000cf0: 7574 6520 3d20 7365 6c66 2e5f 6765 745f  ute = self._get_
-00000d00: 6461 7461 6672 616d 655f 616e 645f 7072  dataframe_and_pr
-00000d10: 6f74 6563 7465 645f 6174 7472 6962 7574  otected_attribut
-00000d20: 6528 6461 7461 7365 742c 2070 726f 7465  e(dataset, prote
-00000d30: 6374 6564 5f61 7474 7269 6275 7465 7329  cted_attributes)
-00000d40: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00000d50: 2020 2020 636c 6173 7365 7320 3d20 6c69      classes = li
-00000d60: 7374 2864 665b 7072 6f74 6563 7465 645f  st(df[protected_
-00000d70: 6174 7472 6962 7574 655d 2e75 6e69 7175  attribute].uniqu
-00000d80: 6528 2929 0d0a 2020 2020 2020 2020 6869  e())..        hi
-00000d90: 6768 6573 745f 722c 2063 6c61 7373 5f77  ghest_r, class_w
-00000da0: 6974 685f 6869 6768 6573 745f 7220 3d20  ith_highest_r = 
-00000db0: 7365 6c66 2e5f 6869 6768 6573 745f 7261  self._highest_ra
-00000dc0: 7469 6f28 6466 2c20 7461 7267 6574 2c20  tio(df, target, 
-00000dd0: 636c 6173 7365 732c 2070 726f 7465 6374  classes, protect
-00000de0: 6564 5f61 7474 7269 6275 7465 290d 0a20  ed_attribute).. 
-00000df0: 2020 2020 2020 2073 656c 662e 7361 6d70         self.samp
-00000e00: 6c65 722e 7361 6d70 6c69 6e67 5f73 7472  ler.sampling_str
-00000e10: 6174 6567 7920 3d20 6869 6768 6573 745f  ategy = highest_
-00000e20: 720d 0a20 2020 2020 2020 2058 5f66 696e  r..        X_fin
-00000e30: 616c 203d 2070 642e 4461 7461 4672 616d  al = pd.DataFram
-00000e40: 6528 636f 6c75 6d6e 7320 3d20 6466 2e63  e(columns = df.c
-00000e50: 6f6c 756d 6e73 290d 0a20 2020 2020 2020  olumns)..       
-00000e60: 2079 5f66 696e 616c 203d 2070 642e 5365   y_final = pd.Se
-00000e70: 7269 6573 2829 0d0a 2020 2020 2020 2020  ries()..        
-00000e80: 666f 7220 636c 6173 735f 2069 6e20 636c  for class_ in cl
-00000e90: 6173 7365 7320 3a0d 0a20 2020 2020 2020  asses :..       
-00000ea0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00000eb0: 2020 2020 2020 2023 206b 6565 7020 6f6e         # keep on
-00000ec0: 6c79 2074 6865 2072 6f77 7320 7769 7468  ly the rows with
-00000ed0: 2067 6976 656e 2063 6c61 7373 0d0a 2020   given class..  
-00000ee0: 2020 2020 2020 2020 2020 636c 6173 735f            class_
-00000ef0: 6466 203d 2064 665b 6466 5b70 726f 7465  df = df[df[prote
-00000f00: 6374 6564 5f61 7474 7269 6275 7465 5d20  cted_attribute] 
-00000f10: 3d3d 2063 6c61 7373 5f5d 0d0a 2020 2020  == class_]..    
-00000f20: 2020 2020 2020 2020 636c 6173 735f 7461          class_ta
-00000f30: 7267 6574 203d 2074 6172 6765 745b 6466  rget = target[df
-00000f40: 5b70 726f 7465 6374 6564 5f61 7474 7269  [protected_attri
-00000f50: 6275 7465 5d20 3d3d 2063 6c61 7373 5f5d  bute] == class_]
-00000f60: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-00000f70: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00000f80: 6c61 7373 5f20 213d 2063 6c61 7373 5f77  lass_ != class_w
-00000f90: 6974 685f 6869 6768 6573 745f 7220 3a20  ith_highest_r : 
-00000fa0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00000fb0: 2020 2023 2072 6573 616d 706c 6520 7468     # resample th
-00000fc0: 6520 7461 7267 6574 2066 6f72 2074 6869  e target for thi
-00000fd0: 7320 636c 6173 730d 0a20 2020 2020 2020  s class..       
-00000fe0: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-00000ff0: 636c 6173 735f 7461 7267 6574 2e75 6e69  class_target.uni
-00001000: 7175 6528 2929 203e 2031 203a 0d0a 2020  que()) > 1 :..  
-00001010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001020: 2020 585f 7072 6f63 6573 7365 642c 2079    X_processed, y
-00001030: 5f70 726f 6365 7373 6564 203d 2073 656c  _processed = sel
-00001040: 662e 7361 6d70 6c65 722e 5f70 726f 6365  f.sampler._proce
-00001050: 7373 2863 6c61 7373 5f64 662c 2063 6c61  ss(class_df, cla
-00001060: 7373 5f74 6172 6765 742c 2063 6f6e 745f  ss_target, cont_
-00001070: 636f 6c75 6d6e 732c 2063 6174 5f63 6f6c  columns, cat_col
-00001080: 756d 6e73 290d 0a20 2020 2020 2020 2020  umns)..         
-00001090: 2020 2020 2020 2020 2020 2058 5f72 6573             X_res
-000010a0: 616d 706c 6564 2c20 795f 7265 7361 6d70  ampled, y_resamp
-000010b0: 6c65 6420 3d20 7365 6c66 2e73 616d 706c  led = self.sampl
-000010c0: 6572 2e66 6974 5f72 6573 616d 706c 6528  er.fit_resample(
-000010d0: 585f 7072 6f63 6573 7365 642c 2079 5f70  X_processed, y_p
-000010e0: 726f 6365 7373 6564 290d 0a20 2020 2020  rocessed)..     
-000010f0: 2020 2020 2020 2020 2020 2020 2020 2058                 X
-00001100: 5f63 6c61 7373 5f66 696e 616c 2c20 795f  _class_final, y_
-00001110: 636c 6173 735f 6669 6e61 6c20 3d20 7365  class_final = se
-00001120: 6c66 2e73 616d 706c 6572 2e5f 756e 7072  lf.sampler._unpr
-00001130: 6f63 6573 7328 585f 7265 7361 6d70 6c65  ocess(X_resample
-00001140: 642c 2079 5f72 6573 616d 706c 6564 290d  d, y_resampled).
-00001150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001160: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00001170: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
-00001180: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00001190: 2020 2020 2020 2058 5f63 6c61 7373 5f66         X_class_f
-000011a0: 696e 616c 203d 2063 6c61 7373 5f64 660d  inal = class_df.
-000011b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000011c0: 2020 2020 2079 5f63 6c61 7373 5f66 696e       y_class_fin
-000011d0: 616c 203d 2063 6c61 7373 5f74 6172 6765  al = class_targe
-000011e0: 740d 0a20 2020 2020 2020 2020 2020 200d  t..            .
-000011f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001200: 2023 2061 7070 656e 6420 7468 6520 7265   # append the re
-00001210: 7361 6d70 6c65 6420 636c 6173 7320 696e  sampled class in
-00001220: 2066 696e 616c 2064 6673 0d0a 2020 2020   final dfs..    
-00001230: 2020 2020 2020 2020 2020 2020 585f 6669              X_fi
-00001240: 6e61 6c20 3d20 7064 2e63 6f6e 6361 7428  nal = pd.concat(
-00001250: 5b58 5f66 696e 616c 2c20 585f 636c 6173  [X_final, X_clas
-00001260: 735f 6669 6e61 6c5d 2c20 6967 6e6f 7265  s_final], ignore
-00001270: 5f69 6e64 6578 3d54 7275 6529 0d0a 2020  _index=True)..  
-00001280: 2020 2020 2020 2020 2020 2020 2020 795f                y_
-00001290: 6669 6e61 6c20 3d20 7064 2e63 6f6e 6361  final = pd.conca
-000012a0: 7428 5b79 5f66 696e 616c 2c20 795f 636c  t([y_final, y_cl
-000012b0: 6173 735f 6669 6e61 6c5d 290d 0a20 2020  ass_final])..   
-000012c0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-000012d0: 2020 2020 2020 2065 6c73 6520 3a0d 0a20         else :.. 
-000012e0: 2020 2020 2020 2020 2020 2020 2020 2058                 X
-000012f0: 5f66 696e 616c 203d 2070 642e 636f 6e63  _final = pd.conc
-00001300: 6174 285b 585f 6669 6e61 6c2c 2063 6c61  at([X_final, cla
-00001310: 7373 5f64 665d 2c20 6967 6e6f 7265 5f69  ss_df], ignore_i
-00001320: 6e64 6578 3d54 7275 6529 0d0a 2020 2020  ndex=True)..    
-00001330: 2020 2020 2020 2020 2020 2020 795f 6669              y_fi
-00001340: 6e61 6c20 3d20 7064 2e63 6f6e 6361 7428  nal = pd.concat(
-00001350: 5b79 5f66 696e 616c 2c20 636c 6173 735f  [y_final, class_
-00001360: 7461 7267 6574 5d29 0d0a 2020 2020 2020  target])..      
-00001370: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00001380: 2020 2020 0d0a 2020 2020 2020 2020 0d0a      ..        ..
-00001390: 2020 2020 2020 2020 585f 6669 6e61 6c20          X_final 
-000013a0: 3d20 7365 6c66 2e5f 6765 745f 6669 6e61  = self._get_fina
-000013b0: 6c5f 6461 7461 6672 616d 6528 585f 6669  l_dataframe(X_fi
-000013c0: 6e61 6c2c 2070 726f 7465 6374 6564 5f61  nal, protected_a
-000013d0: 7474 7269 6275 7465 732c 2070 726f 7465  ttributes, prote
-000013e0: 6374 6564 5f61 7474 7269 6275 7465 290d  cted_attribute).
-000013f0: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
-00001400: 6e20 585f 6669 6e61 6c2c 2079 5f66 696e  n X_final, y_fin
-00001410: 616c 0d0a 2020 2020 2020 2020 2020 2020  al..            
-00001420: 2020 2020 0d0a 636c 6173 7320 4d69 7469      ..class Miti
-00001430: 6761 746f 7228 7361 6e69 7479 5f63 6865  gator(sanity_che
-00001440: 636b 6572 2920 3a0d 0a0d 0a20 2020 2064  cker) :....    d
-00001450: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00001460: 2c20 6d65 7468 6f64 203d 2022 5261 6e64  , method = "Rand
-00001470: 6f6d 4f76 6572 5361 6d70 6c65 7222 2920  omOverSampler") 
-00001480: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-00001490: 2020 2020 2020 2020 4d69 7469 6761 746f          Mitigato
-000014a0: 7220 696d 706c 656d 656e 7420 6469 6666  r implement diff
-000014b0: 6572 656e 7420 7479 7065 7320 6f66 2062  erent types of b
-000014c0: 6961 6973 206d 6974 6967 6174 696f 6e20  iais mitigation 
-000014d0: 6279 2072 6573 616d 706c 696e 672e 0d0a  by resampling...
-000014e0: 0d0a 2020 2020 2020 2020 4172 6773 3a0d  ..        Args:.
-000014f0: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
-00001500: 686f 6420 2873 7472 2c20 6f70 7469 6f6e  hod (str, option
-00001510: 616c 293a 2072 6573 616d 706c 696e 6720  al): resampling 
-00001520: 6d65 7468 6f64 7320 696d 706c 656d 656e  methods implemen
-00001530: 7465 6420 6279 2069 6d62 6c65 6172 6e2e  ted by imblearn.
-00001540: 2050 6f73 7369 626c 6520 7661 6c75 6573   Possible values
-00001550: 2061 7265 2022 5261 6e64 6f6d 4f76 6572   are "RandomOver
-00001560: 5361 6d70 6c65 7222 2c20 0d0a 2020 2020  Sampler", ..    
-00001570: 2020 2020 2020 2020 2253 4d4f 5445 4e43          "SMOTENC
-00001580: 2220 616e 6420 2252 616e 646f 6d55 6e64  " and "RandomUnd
-00001590: 6572 5361 6d70 6c65 7222 2e20 2044 6566  erSampler".  Def
-000015a0: 6175 6c74 7320 746f 2022 5261 6e64 6f6d  aults to "Random
-000015b0: 4f76 6572 5361 6d70 6c65 7222 2e0d 0a20  OverSampler"... 
-000015c0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-000015d0: 2020 2020 0d0a 2020 2020 2020 2020 7365      ..        se
-000015e0: 6c66 2e5f 696e 6974 5f73 616e 6974 795f  lf._init_sanity_
-000015f0: 6368 6563 6b28 6d65 7468 6f64 290d 0a20  check(method).. 
-00001600: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00001610: 2073 656c 662e 6d65 7468 6f64 203d 206d   self.method = m
-00001620: 6574 686f 640d 0a20 2020 2020 2020 2073  ethod..        s
-00001630: 656c 662e 6d69 7469 6761 746f 725f 6675  elf.mitigator_fu
-00001640: 6e63 7469 6f6e 203d 207b 0d0a 2020 2020  nction = {..    
-00001650: 2020 2020 2020 2020 2252 616e 646f 6d4f          "RandomO
-00001660: 7665 7253 616d 706c 6572 2220 3a20 5261  verSampler" : Ra
-00001670: 6e64 6f6d 4f76 6572 5361 6d70 6c65 722c  ndomOverSampler,
-00001680: 0d0a 2020 2020 2020 2020 2020 2020 2022  ..             "
-00001690: 534d 4f54 454e 4322 203a 2053 4d4f 5445  SMOTENC" : SMOTE
-000016a0: 4e43 2c0d 0a20 2020 2020 2020 2020 2020  NC,..           
-000016b0: 2020 2252 616e 646f 6d55 6e64 6572 5361    "RandomUnderSa
-000016c0: 6d70 6c65 7222 203a 2052 616e 646f 6d55  mpler" : RandomU
-000016d0: 6e64 6572 5361 6d70 6c65 720d 0a20 2020  nderSampler..   
-000016e0: 2020 2020 207d 0d0a 2020 2020 0d0a 2020       }..    ..  
-000016f0: 2020 6465 6620 5f69 6e69 745f 7361 6e69    def _init_sani
-00001700: 7479 5f63 6865 636b 2873 656c 662c 206d  ty_check(self, m
-00001710: 6574 686f 6429 203a 0d0a 2020 2020 2020  ethod) :..      
-00001720: 2020 6173 7365 7274 206d 6574 686f 6420    assert method 
-00001730: 696e 2053 414d 504c 494e 475f 4655 4e43  in SAMPLING_FUNC
-00001740: 5449 4f4e 532c 2066 226d 6574 686f 6420  TIONS, f"method 
-00001750: 6e65 6564 2074 6f20 6265 2069 6e20 7b53  need to be in {S
-00001760: 414d 504c 494e 475f 4655 4e43 5449 4f4e  AMPLING_FUNCTION
-00001770: 537d 220d 0a0d 0a20 2020 200d 0a20 2020  S}"....    ..   
-00001780: 2064 6566 206d 6974 6967 6174 6528 7365   def mitigate(se
-00001790: 6c66 2c20 6d69 7469 6761 7469 6f6e 5f73  lf, mitigation_s
-000017a0: 7472 6174 6567 793a 2073 7472 2c20 6461  trategy: str, da
-000017b0: 7461 7365 743a 2070 642e 4461 7461 4672  taset: pd.DataFr
-000017c0: 616d 652c 2074 6172 6765 743a 2073 7472  ame, target: str
-000017d0: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
-000017e0: 2020 2020 2070 726f 7465 6374 6564 5f61       protected_a
-000017f0: 7474 7269 6275 7465 733a 206c 6973 7420  ttributes: list 
-00001800: 3d20 4e6f 6e65 2c20 636f 6e74 5f63 6f6c  = None, cont_col
-00001810: 756d 6e73 3a20 6c69 7374 203d 204e 6f6e  umns: list = Non
-00001820: 652c 2063 6174 5f63 6f6c 756d 6e73 3a20  e, cat_columns: 
-00001830: 6c69 7374 203d 204e 6f6e 6529 203a 0d0a  list = None) :..
-00001840: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00001850: 2020 2020 204d 6974 6967 6174 6520 6269       Mitigate bi
-00001860: 6173 2075 7369 6e67 2074 6865 2067 6976  as using the giv
-00001870: 656e 206d 6974 6967 6174 696f 6e20 7374  en mitigation st
-00001880: 7261 7465 6779 0d0a 0d0a 2020 2020 2020  rategy....      
-00001890: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
-000018a0: 2020 2020 206d 6974 6967 6174 696f 6e5f       mitigation_
-000018b0: 7374 7261 7465 6779 2028 7374 7229 3a20  strategy (str): 
-000018c0: 7468 6520 6d69 7469 6761 7469 6f6e 2073  the mitigation s
-000018d0: 7472 6174 6567 7920 746f 2075 7365 2e20  trategy to use. 
-000018e0: 506f 7373 6962 6c65 2076 616c 7565 7320  Possible values 
-000018f0: 6172 6520 2262 616c 616e 655f 6f75 7470  are "balane_outp
-00001900: 7574 222c 2022 6261 6c61 6e63 655f 7072  ut", "balance_pr
-00001910: 6f74 6563 7465 645f 6174 7472 6962 7574  otected_attribut
-00001920: 6522 2c20 2262 616c 616e 6365 5f6f 7574  e", "balance_out
-00001930: 7075 7420 666f 7220 6174 7472 6962 7574  put for attribut
-00001940: 6522 2061 6e64 2022 6261 6c61 6e63 655f  e" and "balance_
-00001950: 616c 6c22 2e20 0d0a 2020 2020 2020 2020  all". ..        
-00001960: 2020 2020 226e 6f6e 6522 2069 7320 616c      "none" is al
-00001970: 736f 2069 6d70 6c65 6d65 6e74 6564 2066  so implemented f
-00001980: 6f72 2062 656e 6368 6d61 726b 696e 6720  or benchmarking 
-00001990: 636f 6e73 6973 7465 6e63 7920 616e 6420  consistency and 
-000019a0: 7369 6d70 6c79 2072 6574 7572 6e20 7468  simply return th
-000019b0: 6520 696e 6974 6961 6c20 6461 7461 7365  e initial datase
-000019c0: 7420 616e 6420 7461 7267 6574 2e20 0d0a  t and target. ..
-000019d0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-000019e0: 7365 7420 2870 642e 4461 7461 4672 616d  set (pd.DataFram
-000019f0: 6529 3a20 6461 7461 7365 7420 746f 206d  e): dataset to m
-00001a00: 6974 6967 6174 652c 2074 6861 7420 696e  itigate, that in
-00001a10: 636c 7564 6573 2074 6865 2074 6172 6765  cludes the targe
-00001a20: 7420 636f 6c75 6d6e 2e0d 0a20 2020 2020  t column...     
-00001a30: 2020 2020 2020 2074 6172 6765 7420 2873         target (s
-00001a40: 7472 293a 2074 6865 2074 6172 6765 7420  tr): the target 
-00001a50: 636f 6c75 6d6e 206e 616d 650d 0a20 2020  column name..   
-00001a60: 2020 2020 2020 2020 2070 726f 7465 6374           protect
-00001a70: 6564 5f61 7474 7269 6275 7465 7320 286c  ed_attributes (l
-00001a80: 6973 742c 206f 7074 696f 6e61 6c29 3a20  ist, optional): 
-00001a90: 5468 6520 6174 7472 6962 7574 6528 7329  The attribute(s)
-00001aa0: 2074 6f20 6261 6c61 6e63 652e 204f 6e6c   to balance. Onl
-00001ab0: 7920 6e65 6365 7373 6172 7920 666f 7220  y necessary for 
-00001ac0: 6261 6c61 6e63 655f 7072 6f74 6563 7465  balance_protecte
-00001ad0: 645f 6174 7472 6962 7574 6520 616e 6420  d_attribute and 
-00001ae0: 6261 6c61 6e63 655f 6f75 7470 7574 5f66  balance_output_f
-00001af0: 6f72 5f61 7474 7269 6275 7465 2e20 4465  or_attribute. De
-00001b00: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0d  faults to None..
-00001b10: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-00001b20: 745f 636f 6c75 6d6e 7320 286c 6973 742c  t_columns (list,
-00001b30: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
-00001b40: 636f 6e74 696e 756f 7573 2063 6f6c 756d  continuous colum
-00001b50: 6e73 2069 6e20 7468 6520 6461 7461 7365  ns in the datase
-00001b60: 742e 204f 6e6c 7920 4e65 6365 7373 6172  t. Only Necessar
-00001b70: 7920 6966 2074 6865 2073 616d 706c 696e  y if the samplin
-00001b80: 6720 7374 7261 7465 6779 2069 7320 534d  g strategy is SM
-00001b90: 4f54 454e 432e 2044 6566 6175 6c74 7320  OTENC. Defaults 
-00001ba0: 746f 204e 6f6e 652e 0d0a 2020 2020 2020  to None...      
-00001bb0: 2020 2020 2020 6361 745f 636f 6c75 6d6e        cat_column
-00001bc0: 7320 286c 6973 742c 206f 7074 696f 6e61  s (list, optiona
-00001bd0: 6c29 3a20 5468 6520 6361 7465 676f 7269  l): The categori
-00001be0: 6361 6c20 636f 6c75 6d6e 7320 696e 2074  cal columns in t
-00001bf0: 6865 2064 6174 6173 6574 2e20 4f6e 6c79  he dataset. Only
-00001c00: 204e 6563 6573 7361 7279 2069 6620 7468   Necessary if th
-00001c10: 6520 7361 6d70 6c69 6e67 2073 7472 6174  e sampling strat
-00001c20: 6567 7920 6973 2053 4d4f 5445 4e43 2e20  egy is SMOTENC. 
-00001c30: 4465 6661 756c 7473 2074 6f20 4e6f 6e65  Defaults to None
-00001c40: 2e0d 0a0d 0a20 2020 2020 2020 2052 6169  .....        Rai
-00001c50: 7365 733a 0d0a 2020 2020 2020 2020 2020  ses:..          
-00001c60: 2020 5661 6c75 6545 7272 6f72 3a20 4966    ValueError: If
-00001c70: 2074 6865 206d 6974 6967 6174 696f 6e20   the mitigation 
-00001c80: 7374 7261 7465 6779 2064 6f65 7320 6e6f  strategy does no
-00001c90: 7420 6578 6973 740d 0a0d 0a20 2020 2020  t exist....     
-00001ca0: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
-00001cb0: 2020 2020 2020 2020 2028 5b70 642e 4461           ([pd.Da
-00001cc0: 7461 4672 616d 652c 2070 642e 4461 7461  taFrame, pd.Data
-00001cd0: 4672 616d 655d 293a 2074 6865 2062 616c  Frame]): the bal
-00001ce0: 616e 6365 6420 6461 7461 6672 616d 6573  anced dataframes
-00001cf0: 2066 6f72 2074 6865 2064 6174 6173 6574   for the dataset
-00001d00: 2061 6e64 2074 6865 2074 6172 6765 740d   and the target.
-00001d10: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00001d20: 2020 2020 2020 6966 206d 6974 6967 6174        if mitigat
-00001d30: 696f 6e5f 7374 7261 7465 6779 203d 3d20  ion_strategy == 
-00001d40: 2262 616c 616e 6365 5f6f 7574 7075 7422  "balance_output"
-00001d50: 203a 0d0a 2020 2020 2020 2020 2020 2020   :..            
-00001d60: 7265 7475 726e 2073 656c 662e 6261 6c61  return self.bala
-00001d70: 6e63 655f 6f75 7470 7574 2864 6174 6173  nce_output(datas
-00001d80: 6574 2c20 7461 7267 6574 2c20 7072 6f74  et, target, prot
-00001d90: 6563 7465 645f 6174 7472 6962 7574 6573  ected_attributes
-00001da0: 2c20 636f 6e74 5f63 6f6c 756d 6e73 2c20  , cont_columns, 
-00001db0: 6361 745f 636f 6c75 6d6e 7329 0d0a 2020  cat_columns)..  
-00001dc0: 2020 2020 2020 656c 6966 206d 6974 6967        elif mitig
-00001dd0: 6174 696f 6e5f 7374 7261 7465 6779 203d  ation_strategy =
-00001de0: 3d20 2262 616c 616e 6365 5f70 726f 7465  = "balance_prote
-00001df0: 6374 6564 5f61 7474 7269 6275 7465 2220  cted_attribute" 
-00001e00: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00001e10: 6574 7572 6e20 7365 6c66 2e62 616c 616e  eturn self.balan
-00001e20: 6365 5f70 726f 7465 6374 6564 5f61 7474  ce_protected_att
-00001e30: 7269 6275 7465 2864 6174 6173 6574 2c20  ribute(dataset, 
-00001e40: 7461 7267 6574 2c20 7072 6f74 6563 7465  target, protecte
-00001e50: 645f 6174 7472 6962 7574 6573 2c20 636f  d_attributes, co
-00001e60: 6e74 5f63 6f6c 756d 6e73 2c20 6361 745f  nt_columns, cat_
-00001e70: 636f 6c75 6d6e 7329 0d0a 2020 2020 2020  columns)..      
-00001e80: 2020 656c 6966 206d 6974 6967 6174 696f    elif mitigatio
-00001e90: 6e5f 7374 7261 7465 6779 203d 3d20 2262  n_strategy == "b
-00001ea0: 616c 616e 6365 5f6f 7574 7075 745f 666f  alance_output_fo
-00001eb0: 725f 6174 7472 6962 7574 6522 203a 0d0a  r_attribute" :..
-00001ec0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00001ed0: 726e 2073 656c 662e 6261 6c61 6e63 655f  rn self.balance_
-00001ee0: 6f75 7470 7574 5f66 6f72 5f61 7474 7269  output_for_attri
-00001ef0: 6275 7465 2864 6174 6173 6574 2c20 7461  bute(dataset, ta
-00001f00: 7267 6574 2c20 7072 6f74 6563 7465 645f  rget, protected_
-00001f10: 6174 7472 6962 7574 6573 2c20 636f 6e74  attributes, cont
-00001f20: 5f63 6f6c 756d 6e73 2c20 6361 745f 636f  _columns, cat_co
-00001f30: 6c75 6d6e 7329 0d0a 2020 2020 2020 2020  lumns)..        
-00001f40: 656c 6966 206d 6974 6967 6174 696f 6e5f  elif mitigation_
-00001f50: 7374 7261 7465 6779 203d 3d20 2262 616c  strategy == "bal
-00001f60: 616e 6365 5f61 6c6c 2220 3a0d 0a20 2020  ance_all" :..   
-00001f70: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00001f80: 7365 6c66 2e62 616c 616e 6365 5f61 6c6c  self.balance_all
-00001f90: 2864 6174 6173 6574 2c20 7461 7267 6574  (dataset, target
-00001fa0: 2c20 7072 6f74 6563 7465 645f 6174 7472  , protected_attr
-00001fb0: 6962 7574 6573 2c20 636f 6e74 5f63 6f6c  ibutes, cont_col
-00001fc0: 756d 6e73 2c20 6361 745f 636f 6c75 6d6e  umns, cat_column
-00001fd0: 7329 0d0a 2020 2020 2020 2020 656c 6966  s)..        elif
-00001fe0: 206d 6974 6967 6174 696f 6e5f 7374 7261   mitigation_stra
-00001ff0: 7465 6779 203d 3d20 226e 6f6e 6522 203a  tegy == "none" :
-00002000: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00002010: 7475 726e 2064 6174 6173 6574 2c20 7461  turn dataset, ta
-00002020: 7267 6574 0d0a 2020 2020 2020 2020 656c  rget..        el
-00002030: 7365 203a 0d0a 2020 2020 2020 2020 2020  se :..          
-00002040: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00002050: 6f72 0d0a 2020 2020 2020 2020 0d0a 2020  or..        ..  
-00002060: 2020 6465 6620 6261 6c61 6e63 655f 6f75    def balance_ou
-00002070: 7470 7574 2873 656c 662c 2064 6174 6173  tput(self, datas
-00002080: 6574 3a20 7064 2e44 6174 6146 7261 6d65  et: pd.DataFrame
-00002090: 2c20 7461 7267 6574 3a20 7374 722c 2070  , target: str, p
-000020a0: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
-000020b0: 7465 733a 206c 6973 7420 3d20 4e6f 6e65  tes: list = None
-000020c0: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
-000020d0: 2020 2020 2020 2020 2020 2063 6f6e 745f             cont_
-000020e0: 636f 6c75 6d6e 733a 206c 6973 7420 3d20  columns: list = 
-000020f0: 4e6f 6e65 2c20 6361 745f 636f 6c75 6d6e  None, cat_column
-00002100: 733a 206c 6973 7420 3d20 4e6f 6e65 2920  s: list = None) 
-00002110: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-00002120: 2020 2020 2020 2020 4261 6c61 6e63 6520          Balance 
-00002130: 7468 6520 6f75 7470 7574 2077 6974 6820  the output with 
-00002140: 6e6f 2072 6567 6172 6473 2074 6f20 7468  no regards to th
-00002150: 6520 7072 6f74 6563 7465 6420 6174 7472  e protected attr
-00002160: 6962 7574 6573 2e0d 0a20 2020 2020 2020  ibutes...       
-00002170: 200d 0a20 2020 2020 2020 2041 7267 733a   ..        Args:
-00002180: 200d 0a20 2020 2020 2020 2020 2020 2064   ..            d
-00002190: 6174 6173 6574 2028 7064 2e44 6174 6146  ataset (pd.DataF
-000021a0: 7261 6d65 293a 2064 6174 6173 6574 2074  rame): dataset t
-000021b0: 6f20 6d69 7469 6761 7465 2c20 7468 6174  o mitigate, that
-000021c0: 2069 6e63 6c75 6465 7320 7468 6520 7461   includes the ta
-000021d0: 7267 6574 2063 6f6c 756d 6e2e 0d0a 2020  rget column...  
-000021e0: 2020 2020 2020 2020 2020 7461 7267 6574            target
-000021f0: 2028 7374 7229 3a20 7468 6520 7461 7267   (str): the targ
-00002200: 6574 2063 6f6c 756d 6e20 6e61 6d65 0d0a  et column name..
-00002210: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
-00002220: 6563 7465 645f 6174 7472 6962 7574 6573  ected_attributes
-00002230: 2028 6c69 7374 2c20 6f70 7469 6f6e 616c   (list, optional
-00002240: 293a 2055 7365 6c65 7373 2066 6f72 2074  ): Useless for t
-00002250: 6869 7320 6d69 7469 6761 7469 6f6e 2073  his mitigation s
-00002260: 7472 6174 6567 792c 2062 7574 2069 6d70  trategy, but imp
-00002270: 6c65 6d65 6e74 6564 2066 6f72 2041 5049  lemented for API
-00002280: 2063 6f6e 7369 7374 656e 6379 2e20 4465   consistency. De
-00002290: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0d  faults to None..
-000022a0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-000022b0: 745f 636f 6c75 6d6e 7320 286c 6973 742c  t_columns (list,
-000022c0: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
-000022d0: 636f 6e74 696e 756f 7573 2063 6f6c 756d  continuous colum
-000022e0: 6e73 2069 6e20 7468 6520 6461 7461 7365  ns in the datase
-000022f0: 742e 204f 6e6c 7920 4e65 6365 7373 6172  t. Only Necessar
-00002300: 7920 6966 2074 6865 2073 616d 706c 696e  y if the samplin
-00002310: 6720 7374 7261 7465 6779 2069 7320 534d  g strategy is SM
-00002320: 4f54 454e 432e 2044 6566 6175 6c74 7320  OTENC. Defaults 
-00002330: 746f 204e 6f6e 652e 0d0a 2020 2020 2020  to None...      
-00002340: 2020 2020 2020 6361 745f 636f 6c75 6d6e        cat_column
-00002350: 7320 286c 6973 742c 206f 7074 696f 6e61  s (list, optiona
-00002360: 6c29 3a20 5468 6520 6361 7465 676f 7269  l): The categori
-00002370: 6361 6c20 636f 6c75 6d6e 7320 696e 2074  cal columns in t
-00002380: 6865 2064 6174 6173 6574 2e20 4f6e 6c79  he dataset. Only
-00002390: 204e 6563 6573 7361 7279 2069 6620 7468   Necessary if th
-000023a0: 6520 7361 6d70 6c69 6e67 2073 7472 6174  e sampling strat
-000023b0: 6567 7920 6973 2053 4d4f 5445 4e43 2e20  egy is SMOTENC. 
-000023c0: 4465 6661 756c 7473 2074 6f20 4e6f 6e65  Defaults to None
-000023d0: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
-000023e0: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
-000023f0: 2020 2028 5b70 642e 4461 7461 4672 616d     ([pd.DataFram
-00002400: 652c 2070 642e 4461 7461 4672 616d 655d  e, pd.DataFrame]
-00002410: 293a 2074 6865 2062 616c 616e 6365 6420  ): the balanced 
-00002420: 6461 7461 6672 616d 6573 2066 6f72 2074  dataframes for t
-00002430: 6865 2064 6174 6173 6574 2061 6e64 2074  he dataset and t
-00002440: 6865 2074 6172 6765 740d 0a20 2020 2020  he target..     
-00002450: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00002460: 7375 7065 7228 292e 5f73 616e 6974 795f  super()._sanity_
-00002470: 6368 6563 6b28 6461 7461 7365 742c 2074  check(dataset, t
-00002480: 6172 6765 742c 2070 726f 7465 6374 6564  arget, protected
-00002490: 5f61 7474 7269 6275 7465 733d 7072 6f74  _attributes=prot
-000024a0: 6563 7465 645f 6174 7472 6962 7574 6573  ected_attributes
-000024b0: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
-000024c0: 2020 2020 2023 6966 206e 6f74 2052 616e       #if not Ran
-000024d0: 646f 6d4f 7665 7253 616d 706c 6572 2c20  domOverSampler, 
-000024e0: 6e65 6564 2074 6f20 6f6e 652d 686f 7420  need to one-hot 
-000024f0: 656e 636f 6465 2065 7665 7279 2063 6174  encode every cat
-00002500: 6567 6f72 6963 616c 0d0a 2020 2020 2020  egorical..      
-00002510: 2020 6466 203d 2064 6174 6173 6574 2e63    df = dataset.c
-00002520: 6f70 7928 290d 0a20 2020 2020 2020 2074  opy()..        t
-00002530: 6172 6765 745f 6466 203d 2064 665b 7461  arget_df = df[ta
-00002540: 7267 6574 5d0d 0a20 2020 2020 2020 2064  rget]..        d
-00002550: 6620 3d20 6466 2e64 726f 7028 636f 6c75  f = df.drop(colu
-00002560: 6d6e 733d 7461 7267 6574 290d 0a20 2020  mns=target)..   
-00002570: 2020 2020 200d 0a20 2020 2020 2020 200d       ..        .
-00002580: 0a20 2020 2020 2020 2069 6620 7072 6f74  .        if prot
-00002590: 6563 7465 645f 6174 7472 6962 7574 6573  ected_attributes
-000025a0: 2061 6e64 206c 656e 2870 726f 7465 6374   and len(protect
-000025b0: 6564 5f61 7474 7269 6275 7465 7329 203e  ed_attributes) >
-000025c0: 2031 203a 0d0a 2020 2020 2020 2020 2020   1 :..          
-000025d0: 2020 6466 2c20 7072 6f74 6563 7465 645f    df, protected_
-000025e0: 6174 7472 6962 7574 6520 3d20 7365 6c66  attribute = self
-000025f0: 2e5f 6d61 6b65 5f73 7570 6572 5f70 726f  ._make_super_pro
-00002600: 7465 6374 6564 2864 6174 6173 6574 2c20  tected(dataset, 
-00002610: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
-00002620: 7574 6573 290d 0a20 2020 2020 2020 200d  utes)..        .
-00002630: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00002640: 2e6d 6574 686f 6420 696e 205b 2253 4d4f  .method in ["SMO
-00002650: 5445 4e43 225d 203a 0d0a 2020 2020 2020  TENC"] :..      
-00002660: 2020 2020 2020 2370 726f 6365 7373 0d0a        #process..
-00002670: 2020 2020 2020 2020 2020 2020 7072 6f63              proc
-00002680: 6573 736f 7220 3d20 5f50 726f 6365 7373  essor = _Process
-00002690: 6f72 2829 0d0a 2020 2020 2020 2020 2020  or()..          
-000026a0: 2020 7072 6f63 6573 7365 645f 6466 3d20    processed_df= 
-000026b0: 7072 6f63 6573 736f 722e 7072 6f63 6573  processor.proces
-000026c0: 7328 6466 2c20 7363 616c 655f 636f 6c73  s(df, scale_cols
-000026d0: 3d63 6f6e 745f 636f 6c75 6d6e 732c 2065  =cont_columns, e
-000026e0: 6e63 6f64 655f 636f 6c73 3d63 6174 5f63  ncode_cols=cat_c
-000026f0: 6f6c 756d 6e73 290d 0a0d 0a20 2020 2020  olumns)....     
-00002700: 2020 2020 2020 2023 2054 6865 6e20 7265         # Then re
-00002710: 7361 6d70 6c65 0d0a 2020 2020 2020 2020  sample..        
-00002720: 2020 2020 6361 745f 636f 6c75 6d6e 735f      cat_columns_
-00002730: 6964 7320 3d20 5b70 726f 6365 7373 6564  ids = [processed
-00002740: 5f64 662e 636f 6c75 6d6e 732e 6765 745f  _df.columns.get_
-00002750: 6c6f 6328 636f 6c5f 6e61 6d65 2920 666f  loc(col_name) fo
-00002760: 7220 636f 6c5f 6e61 6d65 2069 6e20 6361  r col_name in ca
-00002770: 745f 636f 6c75 6d6e 735d 0d0a 2020 2020  t_columns]..    
-00002780: 2020 2020 2020 2020 7361 6d70 6c65 7220          sampler 
-00002790: 3d20 7365 6c66 2e6d 6974 6967 6174 6f72  = self.mitigator
-000027a0: 5f66 756e 6374 696f 6e5b 7365 6c66 2e6d  _function[self.m
-000027b0: 6574 686f 645d 2863 6174 5f63 6f6c 756d  ethod](cat_colum
-000027c0: 6e73 5f69 6473 290d 0a20 2020 2020 2020  ns_ids)..       
-000027d0: 2020 2020 2058 5f72 6573 616d 706c 6564       X_resampled
-000027e0: 2c20 795f 7265 7361 6d70 6c65 6420 3d20  , y_resampled = 
-000027f0: 7361 6d70 6c65 722e 6669 745f 7265 7361  sampler.fit_resa
-00002800: 6d70 6c65 2870 726f 6365 7373 6564 5f64  mple(processed_d
-00002810: 662c 2074 6172 6765 745f 6466 290d 0a20  f, target_df).. 
-00002820: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00002830: 2020 2020 2020 2020 2023 2054 6865 6e20           # Then 
-00002840: 756e 7072 6f63 6573 7320 6974 0d0a 2020  unprocess it..  
-00002850: 2020 2020 2020 2020 2020 6466 5f66 696e            df_fin
-00002860: 616c 203d 2070 726f 6365 7373 6f72 2e75  al = processor.u
-00002870: 6e70 726f 6365 7373 2858 5f72 6573 616d  nprocess(X_resam
-00002880: 706c 6564 290d 0a20 2020 2020 2020 2020  pled)..         
-00002890: 2020 2074 6172 6765 745f 6669 6e61 6c20     target_final 
-000028a0: 3d20 795f 7265 7361 6d70 6c65 640d 0a0d  = y_resampled...
-000028b0: 0a20 2020 2020 2020 2065 6c73 6520 3a0d  .        else :.
-000028c0: 0a20 2020 2020 2020 2020 2020 2023 6a75  .            #ju
-000028d0: 7374 2072 6573 616d 706c 6572 0d0a 2020  st resampler..  
-000028e0: 2020 2020 2020 2020 2020 7361 6d70 6c65            sample
-000028f0: 7220 3d20 7365 6c66 2e6d 6974 6967 6174  r = self.mitigat
-00002900: 6f72 5f66 756e 6374 696f 6e5b 7365 6c66  or_function[self
-00002910: 2e6d 6574 686f 645d 2829 0d0a 2020 2020  .method]()..    
-00002920: 2020 2020 2020 2020 6466 5f66 696e 616c          df_final
-00002930: 2c20 7461 7267 6574 5f66 696e 616c 203d  , target_final =
-00002940: 2073 616d 706c 6572 2e66 6974 5f72 6573   sampler.fit_res
-00002950: 616d 706c 6528 6466 2c20 7461 7267 6574  ample(df, target
-00002960: 5f64 6629 0d0a 2020 2020 2020 2020 0d0a  _df)..        ..
-00002970: 2020 2020 2020 2020 6966 2070 726f 7465          if prote
-00002980: 6374 6564 5f61 7474 7269 6275 7465 7320  cted_attributes 
-00002990: 616e 6420 6c65 6e28 7072 6f74 6563 7465  and len(protecte
-000029a0: 645f 6174 7472 6962 7574 6573 2920 3e20  d_attributes) > 
-000029b0: 3120 3a0d 0a20 2020 2020 2020 2020 2020  1 :..           
-000029c0: 2064 665f 6669 6e61 6c20 3d20 6466 5f66   df_final = df_f
-000029d0: 696e 616c 2e64 726f 7028 636f 6c75 6d6e  inal.drop(column
-000029e0: 7320 3d20 7072 6f74 6563 7465 645f 6174  s = protected_at
-000029f0: 7472 6962 7574 6529 0d0a 2020 2020 2020  tribute)..      
-00002a00: 2020 0d0a 2020 2020 2020 2020 7265 7475    ..        retu
-00002a10: 726e 2064 665f 6669 6e61 6c2c 2074 6172  rn df_final, tar
-00002a20: 6765 745f 6669 6e61 6c0d 0a20 2020 2020  get_final..     
-00002a30: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
-00002a40: 2062 616c 616e 6365 5f70 726f 7465 6374   balance_protect
-00002a50: 6564 5f61 7474 7269 6275 7465 2873 656c  ed_attribute(sel
-00002a60: 662c 2064 6174 6173 6574 3a20 7064 2e44  f, dataset: pd.D
-00002a70: 6174 6146 7261 6d65 2c20 7461 7267 6574  ataFrame, target
-00002a80: 3a20 7374 722c 2070 726f 7465 6374 6564  : str, protected
-00002a90: 5f61 7474 7269 6275 7465 733a 206c 6973  _attributes: lis
-00002aa0: 742c 200d 0a20 2020 2020 2020 2020 2020  t, ..           
-00002ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ac0: 2020 2020 2020 2020 2063 6f6e 745f 636f           cont_co
-00002ad0: 6c75 6d6e 733a 206c 6973 7420 3d20 4e6f  lumns: list = No
-00002ae0: 6e65 2c20 6361 745f 636f 6c75 6d6e 733a  ne, cat_columns:
-00002af0: 206c 6973 7420 3d20 4e6f 6e65 2920 3a0d   list = None) :.
-00002b00: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00002b10: 2020 2020 2020 4261 6c61 6e63 6520 7468        Balance th
-00002b20: 6520 636c 6173 7365 7320 6f66 2061 2070  e classes of a p
-00002b30: 726f 7465 6374 6564 2061 7474 7269 6275  rotected attribu
-00002b40: 7465 2077 6974 6820 6e6f 2072 6567 6172  te with no regar
-00002b50: 6473 2074 6f20 7468 6520 6f75 7470 7574  ds to the output
-00002b60: 2e20 5c6e 0d0a 2020 2020 2020 2020 5368  . \n..        Sh
-00002b70: 6f75 6c64 2069 6d70 726f 7665 2074 6865  ould improve the
-00002b80: 2062 616c 616e 6365 2066 6f72 2074 6865   balance for the
-00002b90: 2070 726f 7465 6374 6564 2061 7474 7269   protected attri
-00002ba0: 6275 7465 2e0d 0a20 2020 2020 2020 200d  bute...        .
-00002bb0: 0a20 2020 2020 2020 2041 7267 733a 200d  .        Args: .
-00002bc0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00002bd0: 6173 6574 2028 7064 2e44 6174 6146 7261  aset (pd.DataFra
-00002be0: 6d65 293a 2064 6174 6173 6574 2074 6f20  me): dataset to 
-00002bf0: 6d69 7469 6761 7465 2c20 7468 6174 2069  mitigate, that i
-00002c00: 6e63 6c75 6465 7320 7468 6520 7461 7267  ncludes the targ
-00002c10: 6574 2063 6f6c 756d 6e2e 0d0a 2020 2020  et column...    
-00002c20: 2020 2020 2020 2020 7461 7267 6574 2028          target (
-00002c30: 7374 7229 3a20 7468 6520 7461 7267 6574  str): the target
-00002c40: 2063 6f6c 756d 6e20 6e61 6d65 0d0a 2020   column name..  
-00002c50: 2020 2020 2020 2020 2020 7072 6f74 6563            protec
-00002c60: 7465 645f 6174 7472 6962 7574 6573 2028  ted_attributes (
-00002c70: 6c69 7374 2c20 6f70 7469 6f6e 616c 293a  list, optional):
-00002c80: 2054 6865 2061 7474 7269 6275 7465 2873   The attribute(s
-00002c90: 2920 746f 2062 616c 616e 6365 2e20 4465  ) to balance. De
-00002ca0: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0d  faults to None..
-00002cb0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-00002cc0: 745f 636f 6c75 6d6e 7320 286c 6973 742c  t_columns (list,
-00002cd0: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
-00002ce0: 636f 6e74 696e 756f 7573 2063 6f6c 756d  continuous colum
-00002cf0: 6e73 2069 6e20 7468 6520 6461 7461 7365  ns in the datase
-00002d00: 742e 204f 6e6c 7920 4e65 6365 7373 6172  t. Only Necessar
-00002d10: 7920 6966 2074 6865 2073 616d 706c 696e  y if the samplin
-00002d20: 6720 7374 7261 7465 6779 2069 7320 534d  g strategy is SM
-00002d30: 4f54 454e 432e 2044 6566 6175 6c74 7320  OTENC. Defaults 
-00002d40: 746f 204e 6f6e 652e 0d0a 2020 2020 2020  to None...      
-00002d50: 2020 2020 2020 6361 745f 636f 6c75 6d6e        cat_column
-00002d60: 7320 286c 6973 742c 206f 7074 696f 6e61  s (list, optiona
-00002d70: 6c29 3a20 5468 6520 6361 7465 676f 7269  l): The categori
-00002d80: 6361 6c20 636f 6c75 6d6e 7320 696e 2074  cal columns in t
-00002d90: 6865 2064 6174 6173 6574 2e20 4f6e 6c79  he dataset. Only
-00002da0: 204e 6563 6573 7361 7279 2069 6620 7468   Necessary if th
-00002db0: 6520 7361 6d70 6c69 6e67 2073 7472 6174  e sampling strat
-00002dc0: 6567 7920 6973 2053 4d4f 5445 4e43 2e20  egy is SMOTENC. 
-00002dd0: 4465 6661 756c 7473 2074 6f20 4e6f 6e65  Defaults to None
-00002de0: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
-00002df0: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
-00002e00: 2020 2028 5b70 642e 4461 7461 4672 616d     ([pd.DataFram
-00002e10: 652c 2070 642e 4461 7461 4672 616d 655d  e, pd.DataFrame]
-00002e20: 293a 2074 6865 2062 616c 616e 6365 6420  ): the balanced 
-00002e30: 6461 7461 6672 616d 6573 2066 6f72 2074  dataframes for t
-00002e40: 6865 2064 6174 6173 6574 2061 6e64 2074  he dataset and t
-00002e50: 6865 2074 6172 6765 740d 0a20 2020 2020  he target..     
-00002e60: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00002e70: 7375 7065 7228 292e 5f73 616e 6974 795f  super()._sanity_
-00002e80: 6368 6563 6b28 6461 7461 7365 742c 2074  check(dataset, t
-00002e90: 6172 6765 742c 2070 726f 7465 6374 6564  arget, protected
-00002ea0: 5f61 7474 7269 6275 7465 733d 7072 6f74  _attributes=prot
-00002eb0: 6563 7465 645f 6174 7472 6962 7574 6573  ected_attributes
-00002ec0: 290d 0a20 2020 2020 2020 2064 6620 3d20  )..        df = 
-00002ed0: 6461 7461 7365 742e 636f 7079 2829 0d0a  dataset.copy()..
-00002ee0: 2020 2020 2020 2020 7461 7267 6574 5f64          target_d
-00002ef0: 6620 3d20 6466 5b74 6172 6765 745d 0d0a  f = df[target]..
-00002f00: 2020 2020 2020 2020 6466 203d 2064 662e          df = df.
-00002f10: 6472 6f70 2863 6f6c 756d 6e73 3d74 6172  drop(columns=tar
-00002f20: 6765 7429 0d0a 0d0a 2020 2020 2020 2020  get)....        
-00002f30: 6966 206c 656e 2870 726f 7465 6374 6564  if len(protected
-00002f40: 5f61 7474 7269 6275 7465 7329 203e 2031  _attributes) > 1
-00002f50: 203a 0d0a 2020 2020 2020 2020 2020 2020   :..            
-00002f60: 6466 2c20 7072 6f74 6563 7465 645f 6174  df, protected_at
-00002f70: 7472 6962 7574 6520 3d20 7365 6c66 2e5f  tribute = self._
-00002f80: 6d61 6b65 5f73 7570 6572 5f70 726f 7465  make_super_prote
-00002f90: 6374 6564 2864 6174 6173 6574 2c20 7072  cted(dataset, pr
-00002fa0: 6f74 6563 7465 645f 6174 7472 6962 7574  otected_attribut
-00002fb0: 6573 290d 0a20 2020 2020 2020 2065 6c73  es)..        els
-00002fc0: 6520 3a0d 0a20 2020 2020 2020 2020 2020  e :..           
-00002fd0: 2070 726f 7465 6374 6564 5f61 7474 7269   protected_attri
-00002fe0: 6275 7465 203d 2070 726f 7465 6374 6564  bute = protected
-00002ff0: 5f61 7474 7269 6275 7465 735b 305d 0d0a  _attributes[0]..
-00003000: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-00003010: 662e 6d65 7468 6f64 2069 6e20 5b22 534d  f.method in ["SM
-00003020: 4f54 454e 4322 5d20 3a0d 0a20 2020 2020  OTENC"] :..     
-00003030: 2020 2020 2020 2023 7072 6570 726f 6365         #preproce
-00003040: 7373 2075 7369 6e67 2074 6865 2070 726f  ss using the pro
-00003050: 7465 6374 6564 2061 7474 7269 6275 7465  tected attribute
-00003060: 2061 7320 6120 7461 7267 6574 0d0a 2020   as a target..  
-00003070: 2020 2020 2020 2020 2020 636f 6e74 5f63            cont_c
-00003080: 6f6c 5f62 7566 6620 3d20 5b66 6561 7475  ol_buff = [featu
-00003090: 7265 2066 6f72 2066 6561 7475 7265 2069  re for feature i
-000030a0: 6e20 636f 6e74 5f63 6f6c 756d 6e73 2069  n cont_columns i
-000030b0: 6620 6665 6174 7572 6520 213d 2070 726f  f feature != pro
-000030c0: 7465 6374 6564 5f61 7474 7269 6275 7465  tected_attribute
-000030d0: 5d0d 0a20 2020 2020 2020 2020 2020 2063  ]..            c
-000030e0: 6174 5f63 6f6c 5f62 7566 6620 3d20 5b66  at_col_buff = [f
-000030f0: 6561 7475 7265 2066 6f72 2066 6561 7475  eature for featu
-00003100: 7265 2069 6e20 6361 745f 636f 6c75 6d6e  re in cat_column
-00003110: 7320 6966 2066 6561 7475 7265 2021 3d20  s if feature != 
-00003120: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
-00003130: 7574 655d 0d0a 2020 2020 2020 2020 2020  ute]..          
-00003140: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00003150: 7072 6f63 6573 736f 7220 3d20 5f50 726f  processor = _Pro
-00003160: 6365 7373 6f72 2829 0d0a 2020 2020 2020  cessor()..      
-00003170: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00003180: 2020 2020 7072 6f63 6573 7365 645f 6466      processed_df
-00003190: 203d 2070 726f 6365 7373 6f72 2e70 726f   = processor.pro
-000031a0: 6365 7373 2864 662c 2073 6361 6c65 5f63  cess(df, scale_c
-000031b0: 6f6c 733d 636f 6e74 5f63 6f6c 5f62 7566  ols=cont_col_buf
-000031c0: 662c 2065 6e63 6f64 655f 636f 6c73 3d28  f, encode_cols=(
-000031d0: 6361 745f 636f 6c5f 6275 6666 202b 205b  cat_col_buff + [
-000031e0: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
-000031f0: 7574 655d 2929 0d0a 0d0a 2020 2020 2020  ute]))....      
-00003200: 2020 2020 2020 7072 6f74 6563 7465 645f        protected_
-00003210: 6174 7472 6962 7574 655f 636f 6c75 6d6e  attribute_column
-00003220: 203d 2070 726f 6365 7373 6564 5f64 665b   = processed_df[
-00003230: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
-00003240: 7574 655d 0d0a 2020 2020 2020 2020 2020  ute]..          
-00003250: 2020 7072 6f63 6573 7365 645f 6466 2e64    processed_df.d
-00003260: 726f 7028 636f 6c75 6d6e 7320 3d20 5b70  rop(columns = [p
-00003270: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
-00003280: 7465 5d2c 2069 6e70 6c61 6365 203d 2054  te], inplace = T
-00003290: 7275 6529 0d0a 2020 2020 2020 2020 2020  rue)..          
-000032a0: 2020 7072 6f63 6573 7365 645f 6466 2e6c    processed_df.l
-000032b0: 6f63 5b3a 2c74 6172 6765 745d 203d 2074  oc[:,target] = t
-000032c0: 6172 6765 745f 6466 0d0a 0d0a 2020 2020  arget_df....    
-000032d0: 2020 2020 2020 2020 6361 745f 636f 6c75          cat_colu
-000032e0: 6d6e 5f62 7566 6620 3d20 6361 745f 636f  mn_buff = cat_co
-000032f0: 6c5f 6275 6666 2e63 6f70 7928 290d 0a20  l_buff.copy().. 
-00003300: 2020 2020 2020 2020 2020 2063 6174 5f63             cat_c
-00003310: 6f6c 756d 6e5f 6275 6666 2e61 7070 656e  olumn_buff.appen
-00003320: 6428 7461 7267 6574 290d 0a20 2020 2020  d(target)..     
-00003330: 2020 2020 2020 2063 6174 5f63 6f6c 756d         cat_colum
-00003340: 6e5f 6964 7320 3d20 5b70 726f 6365 7373  n_ids = [process
-00003350: 6564 5f64 662e 636f 6c75 6d6e 732e 6765  ed_df.columns.ge
-00003360: 745f 6c6f 6328 636f 6c5f 6e61 6d65 2920  t_loc(col_name) 
-00003370: 666f 7220 636f 6c5f 6e61 6d65 2069 6e20  for col_name in 
-00003380: 6361 745f 636f 6c75 6d6e 5f62 7566 665d  cat_column_buff]
-00003390: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000033a0: 7361 6d70 6c65 7220 3d20 7365 6c66 2e6d  sampler = self.m
-000033b0: 6974 6967 6174 6f72 5f66 756e 6374 696f  itigator_functio
-000033c0: 6e5b 7365 6c66 2e6d 6574 686f 645d 2863  n[self.method](c
-000033d0: 6174 6567 6f72 6963 616c 5f66 6561 7475  ategorical_featu
-000033e0: 7265 733d 6361 745f 636f 6c75 6d6e 5f69  res=cat_column_i
-000033f0: 6473 290d 0a0d 0a20 2020 2020 2020 2020  ds)....         
-00003400: 2020 2058 5f72 6573 616d 706c 6564 2c20     X_resampled, 
-00003410: 6174 7472 6962 7574 655f 7265 7361 6d70  attribute_resamp
-00003420: 6c65 6420 3d20 7361 6d70 6c65 722e 6669  led = sampler.fi
-00003430: 745f 7265 7361 6d70 6c65 2870 726f 6365  t_resample(proce
-00003440: 7373 6564 5f64 662c 2070 726f 7465 6374  ssed_df, protect
-00003450: 6564 5f61 7474 7269 6275 7465 5f63 6f6c  ed_attribute_col
-00003460: 756d 6e29 0d0a 2020 2020 2020 2020 2020  umn)..          
-00003470: 2020 585f 7265 7361 6d70 6c65 642e 6c6f    X_resampled.lo
-00003480: 635b 3a2c 2070 726f 7465 6374 6564 5f61  c[:, protected_a
-00003490: 7474 7269 6275 7465 5d20 3d20 6174 7472  ttribute] = attr
-000034a0: 6962 7574 655f 7265 7361 6d70 6c65 640d  ibute_resampled.
-000034b0: 0a20 2020 2020 2020 2020 2020 0d0a 2020  .           ..  
-000034c0: 2020 2020 2020 2020 2020 6466 5f66 696e            df_fin
-000034d0: 616c 203d 2070 726f 6365 7373 6f72 2e75  al = processor.u
-000034e0: 6e70 726f 6365 7373 2858 5f72 6573 616d  nprocess(X_resam
-000034f0: 706c 6564 290d 0a20 2020 2020 2020 2020  pled)..         
-00003500: 2020 2074 6172 6765 745f 6669 6e61 6c20     target_final 
-00003510: 3d20 6466 5f66 696e 616c 5b74 6172 6765  = df_final[targe
-00003520: 745d 0d0a 2020 2020 2020 2020 2020 2020  t]..            
-00003530: 6466 5f66 696e 616c 2e64 726f 7028 636f  df_final.drop(co
-00003540: 6c75 6d6e 733d 5b74 6172 6765 745d 2c20  lumns=[target], 
-00003550: 696e 706c 6163 653d 5472 7565 290d 0a0d  inplace=True)...
-00003560: 0a20 2020 2020 2020 2065 6c73 6520 3a20  .        else : 
-00003570: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-00003580: 6f74 6563 7465 645f 6174 7472 6962 7574  otected_attribut
-00003590: 655f 636f 6c75 6d6e 203d 2064 665b 7072  e_column = df[pr
-000035a0: 6f74 6563 7465 645f 6174 7472 6962 7574  otected_attribut
-000035b0: 655d 0d0a 2020 2020 2020 2020 2020 2020  e]..            
-000035c0: 6466 2e64 726f 7028 636f 6c75 6d6e 7320  df.drop(columns 
-000035d0: 3d20 5b70 726f 7465 6374 6564 5f61 7474  = [protected_att
-000035e0: 7269 6275 7465 5d2c 2069 6e70 6c61 6365  ribute], inplace
-000035f0: 203d 2054 7275 6529 0d0a 2020 2020 2020   = True)..      
-00003600: 2020 2020 2020 6466 2e6c 6f63 5b3a 2c74        df.loc[:,t
-00003610: 6172 6765 745d 203d 2074 6172 6765 745f  arget] = target_
-00003620: 6466 0d0a 0d0a 2020 2020 2020 2020 2020  df....          
-00003630: 2020 7361 6d70 6c65 7220 3d20 7365 6c66    sampler = self
-00003640: 2e6d 6974 6967 6174 6f72 5f66 756e 6374  .mitigator_funct
-00003650: 696f 6e5b 7365 6c66 2e6d 6574 686f 645d  ion[self.method]
-00003660: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00003670: 585f 7265 7361 6d70 6c65 642c 2061 7474  X_resampled, att
-00003680: 7269 6275 7465 5f72 6573 616d 706c 6564  ribute_resampled
-00003690: 203d 2073 616d 706c 6572 2e66 6974 5f72   = sampler.fit_r
-000036a0: 6573 616d 706c 6528 6466 2c20 7072 6f74  esample(df, prot
-000036b0: 6563 7465 645f 6174 7472 6962 7574 655f  ected_attribute_
-000036c0: 636f 6c75 6d6e 290d 0a20 2020 2020 2020  column)..       
-000036d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000036e0: 2020 2058 5f72 6573 616d 706c 6564 2e6c     X_resampled.l
-000036f0: 6f63 5b3a 2c20 7072 6f74 6563 7465 645f  oc[:, protected_
-00003700: 6174 7472 6962 7574 655d 203d 2061 7474  attribute] = att
-00003710: 7269 6275 7465 5f72 6573 616d 706c 6564  ribute_resampled
-00003720: 0d0a 2020 2020 2020 2020 2020 2020 7461  ..            ta
-00003730: 7267 6574 5f66 696e 616c 203d 2058 5f72  rget_final = X_r
-00003740: 6573 616d 706c 6564 5b74 6172 6765 745d  esampled[target]
-00003750: 0d0a 2020 2020 2020 2020 2020 2020 6466  ..            df
-00003760: 5f66 696e 616c 203d 2058 5f72 6573 616d  _final = X_resam
-00003770: 706c 6564 2e64 726f 7028 636f 6c75 6d6e  pled.drop(column
-00003780: 733d 5b74 6172 6765 745d 290d 0a20 2020  s=[target])..   
-00003790: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
-000037a0: 6620 6c65 6e28 7072 6f74 6563 7465 645f  f len(protected_
-000037b0: 6174 7472 6962 7574 6573 2920 3e20 3120  attributes) > 1 
-000037c0: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
-000037d0: 665f 6669 6e61 6c20 3d20 6466 5f66 696e  f_final = df_fin
-000037e0: 616c 2e64 726f 7028 636f 6c75 6d6e 7320  al.drop(columns 
-000037f0: 3d20 7072 6f74 6563 7465 645f 6174 7472  = protected_attr
-00003800: 6962 7574 6529 2020 2020 0d0a 2020 2020  ibute)    ..    
-00003810: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00003820: 2064 665f 6669 6e61 6c2c 2074 6172 6765   df_final, targe
-00003830: 745f 6669 6e61 6c0d 0a20 2020 200d 0a20  t_final..    .. 
-00003840: 2020 2064 6566 2062 616c 616e 6365 5f6f     def balance_o
-00003850: 7574 7075 745f 666f 725f 6174 7472 6962  utput_for_attrib
-00003860: 7574 6528 7365 6c66 2c20 6461 7461 7365  ute(self, datase
-00003870: 743a 2070 642e 4461 7461 4672 616d 652c  t: pd.DataFrame,
-00003880: 2074 6172 6765 743a 2073 7472 2c20 7072   target: str, pr
-00003890: 6f74 6563 7465 645f 6174 7472 6962 7574  otected_attribut
-000038a0: 6573 3a20 6c69 7374 2c20 0d0a 2020 2020  es: list, ..    
-000038b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038d0: 2063 6f6e 745f 636f 6c75 6d6e 733a 206c   cont_columns: l
-000038e0: 6973 7420 3d20 4e6f 6e65 2c20 6361 745f  ist = None, cat_
-000038f0: 636f 6c75 6d6e 733a 206c 6973 7420 3d20  columns: list = 
-00003900: 4e6f 6e65 2920 3a0d 0a20 2020 2020 2020  None) :..       
-00003910: 2022 2222 0d0a 2020 2020 2020 2020 4261   """..        Ba
-00003920: 6c61 6e63 6520 7468 6520 6f75 7470 7574  lance the output
-00003930: 206f 6620 7468 6520 636c 6173 7365 7320   of the classes 
-00003940: 666f 7220 6120 6769 7665 6e20 7072 6f74  for a given prot
-00003950: 6563 7465 6420 6174 7472 6962 7574 652e  ected attribute.
-00003960: 205c 6e0d 0a20 2020 2020 2020 2053 686f   \n..        Sho
-00003970: 756c 6420 696d 7072 6f76 6520 7468 6520  uld improve the 
-00003980: 4449 5220 666f 7220 7468 6520 7072 6f74  DIR for the prot
-00003990: 6563 7465 6420 6174 7472 6962 7574 652e  ected attribute.
-000039a0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-000039b0: 2020 2020 4172 6773 3a20 0d0a 2020 2020      Args: ..    
-000039c0: 2020 2020 2020 2020 6461 7461 7365 7420          dataset 
-000039d0: 2870 642e 4461 7461 4672 616d 6529 3a20  (pd.DataFrame): 
-000039e0: 6461 7461 7365 7420 746f 206d 6974 6967  dataset to mitig
-000039f0: 6174 652c 2074 6861 7420 696e 636c 7564  ate, that includ
-00003a00: 6573 2074 6865 2074 6172 6765 7420 636f  es the target co
-00003a10: 6c75 6d6e 2e0d 0a20 2020 2020 2020 2020  lumn...         
-00003a20: 2020 2074 6172 6765 7420 2873 7472 293a     target (str):
-00003a30: 2074 6865 2074 6172 6765 7420 636f 6c75   the target colu
-00003a40: 6d6e 206e 616d 650d 0a20 2020 2020 2020  mn name..       
-00003a50: 2020 2020 2070 726f 7465 6374 6564 5f61       protected_a
-00003a60: 7474 7269 6275 7465 7320 286c 6973 742c  ttributes (list,
-00003a70: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
-00003a80: 6174 7472 6962 7574 6528 7329 2074 6f20  attribute(s) to 
-00003a90: 6261 6c61 6e63 652e 2044 6566 6175 6c74  balance. Default
-00003aa0: 7320 746f 204e 6f6e 652e 0d0a 2020 2020  s to None...    
-00003ab0: 2020 2020 2020 2020 636f 6e74 5f63 6f6c          cont_col
-00003ac0: 756d 6e73 2028 6c69 7374 2c20 6f70 7469  umns (list, opti
-00003ad0: 6f6e 616c 293a 2054 6865 2063 6f6e 7469  onal): The conti
-00003ae0: 6e75 6f75 7320 636f 6c75 6d6e 7320 696e  nuous columns in
-00003af0: 2074 6865 2064 6174 6173 6574 2e20 4f6e   the dataset. On
-00003b00: 6c79 204e 6563 6573 7361 7279 2069 6620  ly Necessary if 
-00003b10: 7468 6520 7361 6d70 6c69 6e67 2073 7472  the sampling str
-00003b20: 6174 6567 7920 6973 2053 4d4f 5445 4e43  ategy is SMOTENC
-00003b30: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
-00003b40: 6e65 2e0d 0a20 2020 2020 2020 2020 2020  ne...           
-00003b50: 2063 6174 5f63 6f6c 756d 6e73 2028 6c69   cat_columns (li
-00003b60: 7374 2c20 6f70 7469 6f6e 616c 293a 2054  st, optional): T
-00003b70: 6865 2063 6174 6567 6f72 6963 616c 2063  he categorical c
-00003b80: 6f6c 756d 6e73 2069 6e20 7468 6520 6461  olumns in the da
-00003b90: 7461 7365 742e 204f 6e6c 7920 4e65 6365  taset. Only Nece
-00003ba0: 7373 6172 7920 6966 2074 6865 2073 616d  ssary if the sam
-00003bb0: 706c 696e 6720 7374 7261 7465 6779 2069  pling strategy i
-00003bc0: 7320 534d 4f54 454e 432e 2044 6566 6175  s SMOTENC. Defau
-00003bd0: 6c74 7320 746f 204e 6f6e 652e 0d0a 0d0a  lts to None.....
-00003be0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00003bf0: 0d0a 2020 2020 2020 2020 2020 2020 285b  ..            ([
-00003c00: 7064 2e44 6174 6146 7261 6d65 2c20 7064  pd.DataFrame, pd
-00003c10: 2e44 6174 6146 7261 6d65 5d29 3a20 7468  .DataFrame]): th
-00003c20: 6520 6261 6c61 6e63 6564 2064 6174 6166  e balanced dataf
-00003c30: 7261 6d65 7320 666f 7220 7468 6520 6461  rames for the da
-00003c40: 7461 7365 7420 616e 6420 7468 6520 7461  taset and the ta
-00003c50: 7267 6574 0d0a 2020 2020 2020 2020 2222  rget..        ""
-00003c60: 220d 0a0d 0a20 2020 2020 2020 2073 7570  "....        sup
-00003c70: 6572 2829 2e5f 7361 6e69 7479 5f63 6865  er()._sanity_che
-00003c80: 636b 2864 6174 6173 6574 2c20 7461 7267  ck(dataset, targ
-00003c90: 6574 2c20 7072 6f74 6563 7465 645f 6174  et, protected_at
-00003ca0: 7472 6962 7574 6573 3d70 726f 7465 6374  tributes=protect
-00003cb0: 6564 5f61 7474 7269 6275 7465 7329 0d0a  ed_attributes)..
-00003cc0: 2020 2020 2020 2020 6466 203d 2064 6174          df = dat
-00003cd0: 6173 6574 2e63 6f70 7928 290d 0a0d 0a20  aset.copy().... 
-00003ce0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00003cf0: 2069 6620 6c65 6e28 7072 6f74 6563 7465   if len(protecte
-00003d00: 645f 6174 7472 6962 7574 6573 2920 3e20  d_attributes) > 
-00003d10: 3120 3a0d 0a20 2020 2020 2020 2020 2020  1 :..           
-00003d20: 2064 662c 2070 726f 7465 6374 6564 5f61   df, protected_a
-00003d30: 7474 7269 6275 7465 203d 2073 656c 662e  ttribute = self.
-00003d40: 5f6d 616b 655f 7375 7065 725f 7072 6f74  _make_super_prot
-00003d50: 6563 7465 6428 6461 7461 7365 742c 2070  ected(dataset, p
-00003d60: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
-00003d70: 7465 7329 0d0a 2020 2020 2020 2020 656c  tes)..        el
-00003d80: 7365 203a 0d0a 2020 2020 2020 2020 2020  se :..          
-00003d90: 2020 7072 6f74 6563 7465 645f 6174 7472    protected_attr
-00003da0: 6962 7574 6520 3d20 7072 6f74 6563 7465  ibute = protecte
-00003db0: 645f 6174 7472 6962 7574 6573 5b30 5d0d  d_attributes[0].
-00003dc0: 0a20 2020 200d 0a20 2020 2020 2020 2063  .    ..        c
-00003dd0: 6c61 7373 6573 203d 206c 6973 7428 6466  lasses = list(df
-00003de0: 5b70 726f 7465 6374 6564 5f61 7474 7269  [protected_attri
-00003df0: 6275 7465 5d2e 756e 6971 7565 2829 290d  bute].unique()).
-00003e00: 0a20 2020 2020 2020 2072 2c20 6d61 785f  .        r, max_
-00003e10: 636c 6173 7320 3d20 7365 6c66 2e5f 6869  class = self._hi
-00003e20: 6768 6573 745f 7261 7469 6f28 6466 2c20  ghest_ratio(df, 
-00003e30: 7461 7267 6574 2c20 636c 6173 7365 732c  target, classes,
-00003e40: 2070 726f 7465 6374 6564 5f61 7474 7269   protected_attri
-00003e50: 6275 7465 290d 0a20 2020 2020 2020 200d  bute)..        .
-00003e60: 0a20 2020 2020 2020 2066 6f72 2063 2069  .        for c i
-00003e70: 6e20 636c 6173 7365 7320 3a0d 0a20 2020  n classes :..   
-00003e80: 2020 2020 2020 2020 2069 6620 6320 213d           if c !=
-00003e90: 206d 6178 5f63 6c61 7373 203a 0d0a 2020   max_class :..  
-00003ea0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00003eb0: 6b65 6570 206f 6e6c 7920 7468 6520 726f  keep only the ro
-00003ec0: 7773 2077 6974 6820 6769 7665 6e20 636c  ws with given cl
-00003ed0: 6173 730d 0a20 2020 2020 2020 2020 2020  ass..           
-00003ee0: 2020 2020 2063 6c61 7373 5f64 6620 3d20       class_df = 
-00003ef0: 6466 5b64 665b 7072 6f74 6563 7465 645f  df[df[protected_
-00003f00: 6174 7472 6962 7574 655d 203d 3d20 635d  attribute] == c]
-00003f10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003f20: 2020 636c 6173 735f 7461 7267 6574 203d    class_target =
-00003f30: 2063 6c61 7373 5f64 665b 7461 7267 6574   class_df[target
-00003f40: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00003f50: 2020 2063 6c61 7373 5f64 6620 3d20 636c     class_df = cl
-00003f60: 6173 735f 6466 2e64 726f 7028 636f 6c75  ass_df.drop(colu
-00003f70: 6d6e 733d 5b74 6172 6765 745d 290d 0a20  mns=[target]).. 
-00003f80: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00003f90: 2020 2020 2020 2020 2020 2020 2023 2072               # r
-00003fa0: 6573 616d 706c 6520 7468 6520 7461 7267  esample the targ
-00003fb0: 6574 2066 6f72 2074 6869 7320 636c 6173  et for this clas
-00003fc0: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
-00003fd0: 2020 2069 6620 6c65 6e28 6c69 7374 2863     if len(list(c
-00003fe0: 6c61 7373 5f74 6172 6765 742e 756e 6971  lass_target.uniq
-00003ff0: 7565 2829 2929 2021 3d20 3120 3a0d 0a20  ue())) != 1 :.. 
-00004000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004010: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00004020: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00004030: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00004040: 6620 7365 6c66 2e6d 6574 686f 6420 696e  f self.method in
-00004050: 205b 2253 4d4f 5445 4e43 225d 203a 0d0a   ["SMOTENC"] :..
-00004060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004070: 2020 2020 2020 2020 636f 6e74 5f63 6f6c          cont_col
-00004080: 5f62 7566 6620 3d20 5b66 6561 7475 7265  _buff = [feature
-00004090: 2066 6f72 2066 6561 7475 7265 2069 6e20   for feature in 
-000040a0: 636f 6e74 5f63 6f6c 756d 6e73 2069 6620  cont_columns if 
-000040b0: 6665 6174 7572 6520 213d 2070 726f 7465  feature != prote
-000040c0: 6374 6564 5f61 7474 7269 6275 7465 5d0d  cted_attribute].
-000040d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000040e0: 2020 2020 2020 2020 2063 6174 5f63 6f6c           cat_col
-000040f0: 5f62 7566 6620 3d20 5b66 6561 7475 7265  _buff = [feature
-00004100: 2066 6f72 2066 6561 7475 7265 2069 6e20   for feature in 
-00004110: 6361 745f 636f 6c75 6d6e 7320 6966 2066  cat_columns if f
-00004120: 6561 7475 7265 2021 3d20 7072 6f74 6563  eature != protec
-00004130: 7465 645f 6174 7472 6962 7574 655d 0d0a  ted_attribute]..
-00004140: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00004150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004160: 2020 2020 2020 2370 7265 7072 6f63 6573        #preproces
-00004170: 7320 7573 696e 6720 7468 6520 7072 6f74  s using the prot
-00004180: 6563 7465 6420 6174 7472 6962 7574 6520  ected attribute 
-00004190: 6173 2061 2074 6172 6765 740d 0a20 2020  as a target..   
-000041a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041b0: 2020 2020 2070 726f 6365 7373 6f72 203d       processor =
-000041c0: 205f 5072 6f63 6573 736f 7228 290d 0a20   _Processor().. 
-000041d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041e0: 2020 2020 2020 2070 726f 6365 7373 6564         processed
-000041f0: 5f64 6620 3d20 7072 6f63 6573 736f 722e  _df = processor.
-00004200: 7072 6f63 6573 7328 636c 6173 735f 6466  process(class_df
-00004210: 2c20 7363 616c 655f 636f 6c73 3d63 6f6e  , scale_cols=con
-00004220: 745f 636f 6c5f 6275 6666 2c20 656e 636f  t_col_buff, enco
-00004230: 6465 5f63 6f6c 733d 2863 6174 5f63 6f6c  de_cols=(cat_col
-00004240: 5f62 7566 6620 2b20 5b70 726f 7465 6374  _buff + [protect
-00004250: 6564 5f61 7474 7269 6275 7465 5d29 290d  ed_attribute])).
-00004260: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00004270: 2020 2020 2020 2020 2020 2063 6174 5f63             cat_c
-00004280: 6f6c 756d 6e73 5f69 6473 203d 205b 7072  olumns_ids = [pr
-00004290: 6f63 6573 7365 645f 6466 2e63 6f6c 756d  ocessed_df.colum
-000042a0: 6e73 2e67 6574 5f6c 6f63 2863 6f6c 5f6e  ns.get_loc(col_n
-000042b0: 616d 6529 2066 6f72 2063 6f6c 5f6e 616d  ame) for col_nam
-000042c0: 6520 696e 2063 6174 5f63 6f6c 756d 6e73  e in cat_columns
-000042d0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000042e0: 2020 2020 2020 2020 2020 2073 616d 706c             sampl
-000042f0: 6572 203d 2053 4d4f 5445 4e43 2873 616d  er = SMOTENC(sam
-00004300: 706c 696e 675f 7374 7261 7465 6779 3d72  pling_strategy=r
-00004310: 2c20 6361 7465 676f 7269 6361 6c5f 6665  , categorical_fe
-00004320: 6174 7572 6573 3d63 6174 5f63 6f6c 756d  atures=cat_colum
-00004330: 6e73 5f69 6473 290d 0a20 2020 2020 2020  ns_ids)..       
-00004340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004350: 2058 5f72 6573 616d 706c 6564 2c20 636c   X_resampled, cl
-00004360: 6173 735f 7461 7267 6574 5f72 6573 616d  ass_target_resam
-00004370: 706c 6564 203d 2073 616d 706c 6572 2e66  pled = sampler.f
-00004380: 6974 5f72 6573 616d 706c 6528 7072 6f63  it_resample(proc
-00004390: 6573 7365 645f 6466 2c20 636c 6173 735f  essed_df, class_
-000043a0: 7461 7267 6574 290d 0a20 2020 2020 2020  target)..       
-000043b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043c0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000043d0: 2020 2020 2020 2020 2020 2063 6c61 7373             class
-000043e0: 5f72 6573 616d 706c 6564 203d 2070 726f  _resampled = pro
-000043f0: 6365 7373 6f72 2e75 6e70 726f 6365 7373  cessor.unprocess
-00004400: 2858 5f72 6573 616d 706c 6564 290d 0a20  (X_resampled).. 
-00004410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004420: 2020 2020 2020 2063 6c61 7373 5f72 6573         class_res
-00004430: 616d 706c 6564 2e6c 6f63 5b3a 2c20 7461  ampled.loc[:, ta
-00004440: 7267 6574 5d20 3d20 636c 6173 735f 7461  rget] = class_ta
-00004450: 7267 6574 5f72 6573 616d 706c 6564 0d0a  rget_resampled..
-00004460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004480: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004490: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
-000044a0: 6d65 7468 6f64 2069 6e20 5b22 5261 6e64  method in ["Rand
-000044b0: 6f6d 4f76 6572 5361 6d70 6c65 7222 5d20  omOverSampler"] 
-000044c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000044d0: 2020 2020 2020 2020 2020 2073 616d 706c             sampl
-000044e0: 6572 203d 2052 616e 646f 6d4f 7665 7253  er = RandomOverS
-000044f0: 616d 706c 6572 2873 616d 706c 696e 675f  ampler(sampling_
-00004500: 7374 7261 7465 6779 3d72 290d 0a20 2020  strategy=r)..   
-00004510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004520: 2020 2020 2063 6c61 7373 5f72 6573 616d       class_resam
-00004530: 706c 6564 2c20 636c 6173 735f 7461 7267  pled, class_targ
-00004540: 6574 5f72 6573 616d 706c 6564 203d 2073  et_resampled = s
-00004550: 616d 706c 6572 2e66 6974 5f72 6573 616d  ampler.fit_resam
-00004560: 706c 6528 636c 6173 735f 6466 2c20 636c  ple(class_df, cl
-00004570: 6173 735f 7461 7267 6574 290d 0a20 2020  ass_target)..   
-00004580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004590: 2020 2020 2063 6c61 7373 5f72 6573 616d       class_resam
-000045a0: 706c 6564 2e6c 6f63 5b3a 2c20 7461 7267  pled.loc[:, targ
-000045b0: 6574 5d20 3d20 636c 6173 735f 7461 7267  et] = class_targ
-000045c0: 6574 5f72 6573 616d 706c 6564 0d0a 2020  et_resampled..  
-000045d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045e0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000045f0: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
-00004600: 662e 6d65 7468 6f64 2069 6e20 5b22 5261  f.method in ["Ra
-00004610: 6e64 6f6d 556e 6465 7253 616d 706c 6572  ndomUnderSampler
-00004620: 225d 203a 0d0a 2020 2020 2020 2020 2020  "] :..          
-00004630: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-00004640: 6d70 6c65 7220 3d20 5261 6e64 6f6d 556e  mpler = RandomUn
-00004650: 6465 7253 616d 706c 6572 2873 616d 706c  derSampler(sampl
-00004660: 696e 675f 7374 7261 7465 6779 3d72 290d  ing_strategy=r).
-00004670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004680: 2020 2020 2020 2020 2063 6c61 7373 5f72           class_r
-00004690: 6573 616d 706c 6564 2c20 636c 6173 735f  esampled, class_
-000046a0: 7461 7267 6574 5f72 6573 616d 706c 6564  target_resampled
-000046b0: 203d 2073 616d 706c 6572 2e66 6974 5f72   = sampler.fit_r
-000046c0: 6573 616d 706c 6528 636c 6173 735f 6466  esample(class_df
-000046d0: 2c20 636c 6173 735f 7461 7267 6574 290d  , class_target).
-000046e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000046f0: 2020 2020 2020 2020 2063 6c61 7373 5f72           class_r
-00004700: 6573 616d 706c 6564 2e6c 6f63 5b3a 2c20  esampled.loc[:, 
-00004710: 7461 7267 6574 5d20 3d20 636c 6173 735f  target] = class_
-00004720: 7461 7267 6574 5f72 6573 616d 706c 6564  target_resampled
-00004730: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00004740: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00004750: 2020 2020 2020 2020 2020 656c 7365 203a            else :
-00004760: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004770: 2020 2020 2020 2369 6620 7468 6572 6520        #if there 
-00004780: 6973 206f 6e6c 7920 6f6e 6520 6f75 7470  is only one outp
-00004790: 7574 2066 6f72 2074 6865 2063 6c61 7373  ut for the class
-000047a0: 2c20 7468 6572 6520 6973 206e 6f20 7761  , there is no wa
-000047b0: 7920 746f 2072 6573 616d 706c 6520 6974  y to resample it
-000047c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000047d0: 2020 2020 2020 636c 6173 735f 7265 7361        class_resa
-000047e0: 6d70 6c65 6420 3d20 636c 6173 735f 6466  mpled = class_df
-000047f0: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
-00004800: 2020 2020 2020 2020 2020 2020 2063 6c61               cla
-00004810: 7373 5f72 6573 616d 706c 6564 2e6c 6f63  ss_resampled.loc
-00004820: 5b3a 2c74 6172 6765 745d 203d 2063 6c61  [:,target] = cla
-00004830: 7373 5f74 6172 6765 740d 0a20 2020 2020  ss_target..     
-00004840: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00004850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004860: 2023 2061 7070 656e 6420 7468 6520 7265   # append the re
-00004870: 7361 6d70 6c65 6420 636c 6173 7320 696e  sampled class in
-00004880: 2066 696e 616c 2064 660d 0a20 2020 2020   final df..     
-00004890: 2020 2020 2020 2020 2020 2023 2028 6472             # (dr
-000048a0: 6f70 2074 6865 2072 6f77 7320 7769 7468  op the rows with
-000048b0: 2074 6869 7320 636c 6173 7320 6669 7273   this class firs
-000048c0: 7420 746f 206e 6f74 2064 7570 6c69 6361  t to not duplica
-000048d0: 7465 6420 7468 656d 290d 0a20 2020 2020  ted them)..     
-000048e0: 2020 2020 2020 2020 2020 2064 6620 3d20             df = 
-000048f0: 6466 5b64 665b 7072 6f74 6563 7465 645f  df[df[protected_
-00004900: 6174 7472 6962 7574 655d 2021 3d20 635d  attribute] != c]
-00004910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004920: 2020 6466 203d 2070 642e 636f 6e63 6174    df = pd.concat
-00004930: 285b 6466 2c20 636c 6173 735f 7265 7361  ([df, class_resa
-00004940: 6d70 6c65 645d 2c20 6967 6e6f 7265 5f69  mpled], ignore_i
-00004950: 6e64 6578 3d54 7275 6529 0d0a 0d0a 0d0a  ndex=True)......
-00004960: 2020 2020 2020 2020 7461 7267 6574 5f64          target_d
-00004970: 6620 3d20 6466 5b74 6172 6765 745d 0d0a  f = df[target]..
-00004980: 2020 2020 2020 2020 6466 2e64 726f 7028          df.drop(
-00004990: 636f 6c75 6d6e 733d 5b74 6172 6765 745d  columns=[target]
-000049a0: 2c20 696e 706c 6163 653d 5472 7565 290d  , inplace=True).
-000049b0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-000049c0: 2020 2069 6620 6c65 6e28 7072 6f74 6563     if len(protec
-000049d0: 7465 645f 6174 7472 6962 7574 6573 2920  ted_attributes) 
-000049e0: 3e20 3120 3a0d 0a20 2020 2020 2020 2020  > 1 :..         
-000049f0: 2020 2064 6620 3d20 6466 2e64 726f 7028     df = df.drop(
-00004a00: 636f 6c75 6d6e 7320 3d20 7072 6f74 6563  columns = protec
-00004a10: 7465 645f 6174 7472 6962 7574 6529 0d0a  ted_attribute)..
-00004a20: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00004a30: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-00004a40: 662c 2074 6172 6765 745f 6466 0d0a 2020  f, target_df..  
-00004a50: 2020 0d0a 2020 2020 6465 6620 6261 6c61    ..    def bala
-00004a60: 6e63 655f 616c 6c28 7365 6c66 2c20 6461  nce_all(self, da
-00004a70: 7461 7365 743a 2070 642e 4461 7461 4672  taset: pd.DataFr
-00004a80: 616d 652c 2074 6172 6765 743a 2073 7472  ame, target: str
-00004a90: 2c20 7072 6f74 6563 7465 645f 6174 7472  , protected_attr
-00004aa0: 6962 7574 6573 3a20 6c69 7374 2c20 0d0a  ibutes: list, ..
-00004ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ac0: 2020 2020 636f 6e74 5f63 6f6c 756d 6e73      cont_columns
-00004ad0: 3a20 6c69 7374 203d 204e 6f6e 652c 2063  : list = None, c
-00004ae0: 6174 5f63 6f6c 756d 6e73 3a20 6c69 7374  at_columns: list
-00004af0: 203d 204e 6f6e 6529 203a 0d0a 2020 2020   = None) :..    
-00004b00: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00004b10: 2046 6972 7374 2062 616c 616e 6365 7320   First balances 
-00004b20: 7468 6520 7072 6f74 6563 7465 6420 6174  the protected at
-00004b30: 7472 6962 7574 6528 7329 2c20 616e 6420  tribute(s), and 
-00004b40: 7468 656e 2062 616c 616e 6365 2074 6865  then balance the
-00004b50: 6972 206f 7574 7075 742e 2047 6976 6573  ir output. Gives
-00004b60: 2061 6e20 616c 6d6f 7374 2070 6572 6665   an almost perfe
-00004b70: 6374 6c79 2062 616c 616e 6365 6420 6461  ctly balanced da
-00004b80: 7461 7365 7420 666f 7220 7468 6520 7072  taset for the pr
-00004b90: 6f74 6563 7465 6420 6174 7472 6962 7574  otected attribut
-00004ba0: 6528 7329 2e0d 0a0d 0a20 2020 2020 2020  e(s).....       
-00004bb0: 2041 7267 733a 200d 0a20 2020 2020 2020   Args: ..       
-00004bc0: 2020 2020 2064 6174 6173 6574 2028 7064       dataset (pd
-00004bd0: 2e44 6174 6146 7261 6d65 293a 2064 6174  .DataFrame): dat
-00004be0: 6173 6574 2074 6f20 6d69 7469 6761 7465  aset to mitigate
-00004bf0: 2c20 7468 6174 2069 6e63 6c75 6465 7320  , that includes 
-00004c00: 7468 6520 7461 7267 6574 2063 6f6c 756d  the target colum
-00004c10: 6e2e 0d0a 2020 2020 2020 2020 2020 2020  n...            
-00004c20: 7461 7267 6574 2028 7374 7229 3a20 7468  target (str): th
-00004c30: 6520 7461 7267 6574 2063 6f6c 756d 6e20  e target column 
-00004c40: 6e61 6d65 0d0a 2020 2020 2020 2020 2020  name..          
-00004c50: 2020 7072 6f74 6563 7465 645f 6174 7472    protected_attr
-00004c60: 6962 7574 6573 2028 6c69 7374 2c20 6f70  ibutes (list, op
-00004c70: 7469 6f6e 616c 293a 2054 6865 2061 7474  tional): The att
-00004c80: 7269 6275 7465 2873 2920 746f 2062 616c  ribute(s) to bal
-00004c90: 616e 6365 2e20 4465 6661 756c 7473 2074  ance. Defaults t
-00004ca0: 6f20 4e6f 6e65 2e0d 0a20 2020 2020 2020  o None...       
-00004cb0: 2020 2020 2063 6f6e 745f 636f 6c75 6d6e       cont_column
-00004cc0: 7320 286c 6973 742c 206f 7074 696f 6e61  s (list, optiona
-00004cd0: 6c29 3a20 5468 6520 636f 6e74 696e 756f  l): The continuo
-00004ce0: 7573 2063 6f6c 756d 6e73 2069 6e20 7468  us columns in th
-00004cf0: 6520 6461 7461 7365 742e 204f 6e6c 7920  e dataset. Only 
-00004d00: 4e65 6365 7373 6172 7920 6966 2074 6865  Necessary if the
-00004d10: 2073 616d 706c 696e 6720 7374 7261 7465   sampling strate
-00004d20: 6779 2069 7320 534d 4f54 454e 432e 2044  gy is SMOTENC. D
-00004d30: 6566 6175 6c74 7320 746f 204e 6f6e 652e  efaults to None.
-00004d40: 0d0a 2020 2020 2020 2020 2020 2020 6361  ..            ca
-00004d50: 745f 636f 6c75 6d6e 7320 286c 6973 742c  t_columns (list,
-00004d60: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
-00004d70: 6361 7465 676f 7269 6361 6c20 636f 6c75  categorical colu
-00004d80: 6d6e 7320 696e 2074 6865 2064 6174 6173  mns in the datas
-00004d90: 6574 2e20 4f6e 6c79 204e 6563 6573 7361  et. Only Necessa
-00004da0: 7279 2069 6620 7468 6520 7361 6d70 6c69  ry if the sampli
-00004db0: 6e67 2073 7472 6174 6567 7920 6973 2053  ng strategy is S
-00004dc0: 4d4f 5445 4e43 2e20 4465 6661 756c 7473  MOTENC. Defaults
-00004dd0: 2074 6f20 4e6f 6e65 2e0d 0a0d 0a20 2020   to None.....   
-00004de0: 2020 2020 2052 6574 7572 6e73 3a0d 0a20       Returns:.. 
-00004df0: 2020 2020 2020 2020 2020 2028 5b70 642e             ([pd.
-00004e00: 4461 7461 4672 616d 652c 2070 642e 4461  DataFrame, pd.Da
-00004e10: 7461 4672 616d 655d 293a 2074 6865 2062  taFrame]): the b
-00004e20: 616c 616e 6365 6420 6461 7461 6672 616d  alanced datafram
-00004e30: 6573 2066 6f72 2074 6865 2064 6174 6173  es for the datas
-00004e40: 6574 2061 6e64 2074 6865 2074 6172 6765  et and the targe
-00004e50: 740d 0a20 2020 2020 2020 2022 2222 0d0a  t..        """..
-00004e60: 2020 2020 2020 2020 6466 2c20 7420 3d20          df, t = 
-00004e70: 7365 6c66 2e62 616c 616e 6365 5f70 726f  self.balance_pro
-00004e80: 7465 6374 6564 5f61 7474 7269 6275 7465  tected_attribute
-00004e90: 2864 6174 6173 6574 2c20 7461 7267 6574  (dataset, target
-00004ea0: 2c20 7072 6f74 6563 7465 645f 6174 7472  , protected_attr
-00004eb0: 6962 7574 6573 2c20 636f 6e74 5f63 6f6c  ibutes, cont_col
-00004ec0: 756d 6e73 2c20 6361 745f 636f 6c75 6d6e  umns, cat_column
-00004ed0: 7329 200d 0a20 2020 2020 2020 2064 662e  s) ..        df.
-00004ee0: 6c6f 635b 3a2c 2074 6172 6765 745d 203d  loc[:, target] =
-00004ef0: 2074 0d0a 2020 2020 2020 2020 6466 2c20   t..        df, 
-00004f00: 7420 3d20 7365 6c66 2e62 616c 616e 6365  t = self.balance
-00004f10: 5f6f 7574 7075 745f 666f 725f 6174 7472  _output_for_attr
-00004f20: 6962 7574 6528 6466 2c20 7461 7267 6574  ibute(df, target
-00004f30: 2c20 7072 6f74 6563 7465 645f 6174 7472  , protected_attr
-00004f40: 6962 7574 6573 2c20 636f 6e74 5f63 6f6c  ibutes, cont_col
-00004f50: 756d 6e73 2c20 6361 745f 636f 6c75 6d6e  umns, cat_column
-00004f60: 7329 0d0a 2020 2020 2020 2020 0d0a 2020  s)..        ..  
-00004f70: 2020 2020 2020 7265 7475 726e 2064 662c        return df,
-00004f80: 2074 2020 2020 0d0a 2020 2020 2020 2020   t    ..        
-00004f90: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00004fa0: 2020 0d0a 2020 2020 6465 6620 5f68 6967    ..    def _hig
-00004fb0: 6865 7374 5f72 6174 696f 2873 656c 662c  hest_ratio(self,
-00004fc0: 2064 6174 6173 6574 3a20 7064 2e44 6174   dataset: pd.Dat
-00004fd0: 6146 7261 6d65 2c20 7461 7267 6574 3a20  aFrame, target: 
-00004fe0: 7374 722c 2063 6c61 7373 6573 3a20 6469  str, classes: di
-00004ff0: 6374 2c20 7072 6f74 6563 7465 645f 6174  ct, protected_at
-00005000: 7472 6962 7574 653a 2073 7472 2920 3a0d  tribute: str) :.
-00005010: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00005020: 2020 2020 2020 4769 7665 2074 6865 2068        Give the h
-00005030: 6967 6865 7374 2072 6174 696f 206f 6620  ighest ratio of 
-00005040: 706f 7369 7469 7665 206f 7574 7075 7420  positive output 
-00005050: 6f6e 206e 6567 6174 6976 6520 6f75 7470  on negative outp
-00005060: 7574 206f 6620 616c 6c20 7468 6520 636c  ut of all the cl
-00005070: 6173 7365 7320 6f66 2074 6865 2070 726f  asses of the pro
-00005080: 7465 6374 6564 2061 7474 7269 6275 7465  tected attribute
-00005090: 2e20 4e65 6365 7373 6172 7920 666f 7220  . Necessary for 
-000050a0: 6261 6c61 6e63 655f 6f75 7470 7574 5f66  balance_output_f
-000050b0: 6f72 5f61 7474 7269 6275 7465 2e0d 0a0d  or_attribute....
-000050c0: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
-000050d0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-000050e0: 7365 7420 2870 642e 4461 7461 4672 616d  set (pd.DataFram
-000050f0: 6529 3a20 6461 7461 7365 7420 746f 206d  e): dataset to m
-00005100: 6974 6967 6174 652c 2074 6861 7420 696e  itigate, that in
-00005110: 636c 7564 6573 2074 6865 2074 6172 6765  cludes the targe
-00005120: 7420 636f 6c75 6d6e 2e0d 0a20 2020 2020  t column...     
-00005130: 2020 2020 2020 2074 6172 6765 7420 2873         target (s
-00005140: 7472 293a 2074 6865 2074 6172 6765 7420  tr): the target 
-00005150: 636f 6c75 6d6e 206e 616d 650d 0a20 2020  column name..   
-00005160: 2020 2020 2020 2020 2063 6c61 7373 6573           classes
-00005170: 2028 6469 6374 293a 2074 6865 2063 6c61   (dict): the cla
-00005180: 7373 6573 206f 6620 7468 6520 7072 6f74  sses of the prot
-00005190: 6563 7465 6420 6174 7472 6962 7574 650d  ected attribute.
-000051a0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-000051b0: 7465 6374 6564 5f61 7474 7269 6275 7465  tected_attribute
-000051c0: 2028 7374 7229 3a20 7468 6520 7072 6f74   (str): the prot
-000051d0: 6563 7465 6420 6174 7472 6962 7574 6520  ected attribute 
-000051e0: 746f 2063 616c 6375 6c61 7465 2074 6865  to calculate the
-000051f0: 2068 6967 6865 7374 2072 6174 696f 2066   highest ratio f
-00005200: 6f72 2e0d 0a0d 0a20 2020 2020 2020 2052  or.....        R
-00005210: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
-00005220: 2020 2020 2028 5b66 6c6f 6174 2c20 7374       ([float, st
-00005230: 725d 293a 2074 6865 2068 6967 6865 7374  r]): the highest
-00005240: 2072 6174 696f 2061 6e64 2074 6865 2061   ratio and the a
-00005250: 7373 6f63 6961 7465 6420 636c 6173 730d  ssociated class.
-00005260: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00005270: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00005280: 725f 6d61 7820 3d20 300d 0a20 2020 2020  r_max = 0..     
-00005290: 2020 2063 5f6d 6178 203d 2063 6c61 7373     c_max = class
-000052a0: 6573 5b30 5d0d 0a20 2020 2020 2020 2066  es[0]..        f
-000052b0: 6f72 2063 2069 6e20 636c 6173 7365 7320  or c in classes 
-000052c0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-000052d0: 203d 2064 6174 6173 6574 5b64 6174 6173   = dataset[datas
-000052e0: 6574 5b70 726f 7465 6374 6564 5f61 7474  et[protected_att
-000052f0: 7269 6275 7465 5d20 3d3d 2063 5d5b 7461  ribute] == c][ta
-00005300: 7267 6574 5d2e 7661 6c75 655f 636f 756e  rget].value_coun
-00005310: 7473 2829 5b31 5d2f 6461 7461 7365 745b  ts()[1]/dataset[
-00005320: 6461 7461 7365 745b 7072 6f74 6563 7465  dataset[protecte
-00005330: 645f 6174 7472 6962 7574 655d 203d 3d20  d_attribute] == 
-00005340: 635d 5b74 6172 6765 745d 2e76 616c 7565  c][target].value
-00005350: 5f63 6f75 6e74 7328 295b 305d 0d0a 2020  _counts()[0]..  
-00005360: 2020 2020 2020 2020 2020 6966 2072 203e            if r >
-00005370: 2031 203a 0d0a 2020 2020 2020 2020 2020   1 :..          
-00005380: 2020 2020 2020 7220 3d20 312f 720d 0a20        r = 1/r.. 
-00005390: 2020 2020 2020 2020 2020 2069 6620 7220             if r 
-000053a0: 3e20 725f 6d61 7820 3a0d 0a20 2020 2020  > r_max :..     
-000053b0: 2020 2020 2020 2020 2020 2072 5f6d 6178             r_max
-000053c0: 203d 2072 0d0a 2020 2020 2020 2020 2020   = r..          
-000053d0: 2020 2020 2020 635f 6d61 7820 3d20 630d        c_max = c.
-000053e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000053f0: 725f 6d61 782c 2063 5f6d 6178 0d0a 2020  r_max, c_max..  
-00005400: 200d 0a20 2020 0d0a 2020 2020 6465 6620   ..   ..    def 
-00005410: 5f6d 616b 655f 7375 7065 725f 7072 6f74  _make_super_prot
-00005420: 6563 7465 6428 7365 6c66 2c20 6461 7461  ected(self, data
-00005430: 7365 743a 2070 642e 4461 7461 4672 616d  set: pd.DataFram
-00005440: 652c 2070 726f 7465 6374 6564 5f61 7474  e, protected_att
-00005450: 7269 6275 7465 733a 206c 6973 7429 203a  ributes: list) :
-00005460: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00005470: 2020 2020 2020 204d 616b 6520 6120 7375         Make a su
-00005480: 7065 7220 7072 6f74 6563 7465 6420 6174  per protected at
-00005490: 7472 6962 7574 6520 7468 6174 2069 7320  tribute that is 
-000054a0: 7468 6520 636f 6d62 696e 6174 696f 6e20  the combination 
-000054b0: 6f66 2061 6c6c 2067 6976 656e 2070 726f  of all given pro
-000054c0: 7465 6374 6564 2061 7474 7269 6275 7465  tected attribute
-000054d0: 7320 6361 6c6c 6564 2022 7072 6f74 6563  s called "protec
-000054e0: 7465 645f 7375 7065 7263 6c61 7373 220d  ted_superclass".
-000054f0: 0a0d 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00005500: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
-00005510: 7461 7365 7420 2870 642e 4461 7461 4672  taset (pd.DataFr
-00005520: 616d 6529 3a20 6461 7461 7365 7420 746f  ame): dataset to
-00005530: 206d 6974 6967 6174 652c 2074 6861 7420   mitigate, that 
-00005540: 696e 636c 7564 6573 2074 6865 2074 6172  includes the tar
-00005550: 6765 7420 636f 6c75 6d6e 2e0d 0a20 2020  get column...   
-00005560: 2020 2020 2020 2020 2070 726f 7465 6374           protect
-00005570: 6564 5f61 7474 7269 6275 7465 7320 286c  ed_attributes (l
-00005580: 6973 7429 3a20 7072 6f74 6563 7465 6420  ist): protected 
-00005590: 6174 7472 6962 7574 6573 2074 6f20 636f  attributes to co
-000055a0: 6d62 696e 650d 0a20 2020 2020 2020 2020  mbine..         
-000055b0: 2020 200d 0a20 2020 2020 2020 2052 6574     ..        Ret
-000055c0: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
-000055d0: 2020 2028 5b70 642e 4461 7461 4672 616d     ([pd.DataFram
-000055e0: 652c 2073 7472 5d29 3a20 7468 6520 7472  e, str]): the tr
-000055f0: 616e 7366 6f72 6d65 6420 6461 7461 7365  ansformed datase
-00005600: 7420 616e 6420 7468 6520 6e61 6d65 2022  t and the name "
-00005610: 7375 7065 7220 7072 6f74 6563 7465 6422  super protected"
-00005620: 2063 6f6c 756d 6e0d 0a20 2020 2020 2020   column..       
-00005630: 2022 2222 0d0a 0d0a 2020 2020 2020 2020   """....        
-00005640: 6466 203d 2064 6174 6173 6574 2e63 6f70  df = dataset.cop
-00005650: 7928 290d 0a20 2020 2020 2020 2073 7570  y()..        sup
-00005660: 6572 7072 6f74 6563 7465 645f 636f 6c75  erprotected_colu
-00005670: 6d6e 203d 2066 756e 6374 6f6f 6c73 2e72  mn = functools.r
-00005680: 6564 7563 6528 6c61 6d62 6461 2061 2c20  educe(lambda a, 
-00005690: 6220 3a20 6120 2b20 225f 2220 2b20 622c  b : a + "_" + b,
-000056a0: 2070 726f 7465 6374 6564 5f61 7474 7269   protected_attri
-000056b0: 6275 7465 7329 0d0a 2020 2020 2020 2020  butes)..        
-000056c0: 6466 5b73 7570 6572 7072 6f74 6563 7465  df[superprotecte
-000056d0: 645f 636f 6c75 6d6e 5d20 3d20 2222 0d0a  d_column] = ""..
-000056e0: 2020 2020 2020 2020 666f 7220 7072 6f74          for prot
-000056f0: 6563 7465 645f 6174 7472 6962 7574 6520  ected_attribute 
-00005700: 696e 2070 726f 7465 6374 6564 5f61 7474  in protected_att
-00005710: 7269 6275 7465 7320 3a0d 0a0d 0a20 2020  ributes :....   
-00005720: 2020 2020 2020 2020 2064 665b 7375 7065           df[supe
-00005730: 7270 726f 7465 6374 6564 5f63 6f6c 756d  rprotected_colum
-00005740: 6e5d 202b 3d20 6466 5b70 726f 7465 6374  n] += df[protect
-00005750: 6564 5f61 7474 7269 6275 7465 5d2e 6170  ed_attribute].ap
-00005760: 706c 7928 7374 7229 2020 2b20 225f 220d  ply(str)  + "_".
-00005770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005780: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00005790: 2020 6466 5b73 7570 6572 7072 6f74 6563    df[superprotec
-000057a0: 7465 645f 636f 6c75 6d6e 5d20 3d20 6466  ted_column] = df
-000057b0: 5b73 7570 6572 7072 6f74 6563 7465 645f  [superprotected_
-000057c0: 636f 6c75 6d6e 5d2e 6170 706c 7928 6c61  column].apply(la
-000057d0: 6d62 6461 2078 203a 2078 5b3a 2d31 5d29  mbda x : x[:-1])
-000057e0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-000057f0: 2020 2020 0d0a 2020 2020 2020 2020 7265      ..        re
-00005800: 7475 726e 2064 662c 2073 7570 6572 7072  turn df, superpr
-00005810: 6f74 6563 7465 645f 636f 6c75 6d6e 0d0a  otected_column..
-00005820: 2020 2020 0d0a 6966 205f 5f6e 616d 655f      ..if __name_
-00005830: 5f20 3d3d 2022 5f5f 6d61 696e 5f5f 2220  _ == "__main__" 
-00005840: 3a20 0d0a 2020 2020 6461 7461 203d 207b  : ..    data = {
-00005850: 0d0a 2020 2020 2766 6561 7475 7265 3127  ..    'feature1'
-00005860: 3a20 5b31 2c20 302c 2031 2c20 302c 2031  : [1, 0, 1, 0, 1
-00005870: 2c20 302c 2031 2c20 302c 2031 2c20 302c  , 0, 1, 0, 1, 0,
-00005880: 2031 2c20 302c 2031 2c20 302c 2031 2c20   1, 0, 1, 0, 1, 
-00005890: 302c 2031 2c20 302c 2031 2c20 305d 2c0d  0, 1, 0, 1, 0],.
-000058a0: 0a20 2020 2027 6665 6174 7572 6532 273a  .    'feature2':
-000058b0: 205b 352c 2036 2c20 372c 2038 2c20 392c   [5, 6, 7, 8, 9,
-000058c0: 2031 302c 2031 312c 2031 322c 2031 332c   10, 11, 12, 13,
-000058d0: 2031 342c 2031 352c 2031 362c 2031 372c   14, 15, 16, 17,
-000058e0: 2031 382c 2031 392c 2032 302c 2032 312c   18, 19, 20, 21,
-000058f0: 2032 322c 2032 332c 2032 345d 2c0d 0a20   22, 23, 24],.. 
-00005900: 2020 2027 7072 6f74 6563 7465 645f 6174     'protected_at
-00005910: 7472 6962 7574 6527 3a20 5b27 4127 2c20  tribute': ['A', 
-00005920: 2741 272c 2027 4127 2c20 2741 272c 2027  'A', 'A', 'A', '
-00005930: 4127 2c20 2742 272c 2027 4127 2c20 2742  A', 'B', 'A', 'B
-00005940: 272c 2027 4127 2c20 2742 272c 2027 4127  ', 'A', 'B', 'A'
-00005950: 2c20 2742 272c 2027 4127 2c20 2742 272c  , 'B', 'A', 'B',
-00005960: 2027 4127 2c20 2742 272c 2027 4127 2c20   'A', 'B', 'A', 
-00005970: 2742 272c 2027 4127 2c20 2742 275d 2c0d  'B', 'A', 'B'],.
-00005980: 0a20 2020 207d 0d0a 0d0a 2020 2020 6461  .    }....    da
-00005990: 7461 7365 7420 3d20 7064 2e44 6174 6146  taset = pd.DataF
-000059a0: 7261 6d65 2864 6174 6129 0d0a 2020 2020  rame(data)..    
-000059b0: 7461 7267 6574 203d 2070 642e 5365 7269  target = pd.Seri
-000059c0: 6573 285b 312c 2030 2c20 312c 2030 2c20  es([1, 0, 1, 0, 
-000059d0: 312c 2030 2c20 312c 2030 2c20 312c 2030  1, 0, 1, 0, 1, 0
-000059e0: 2c20 312c 2031 2c20 302c 2030 2c20 312c  , 1, 1, 0, 0, 1,
-000059f0: 2030 2c20 312c 2030 2c20 302c 2030 5d29   0, 1, 0, 0, 0])
-00005a00: 0d0a 2020 2020 0d0a 2020 2020 6261 6c61  ..    ..    bala
-00005a10: 6e63 6520 3d20 4261 6c61 6e63 6541 7474  nce = BalanceAtt
-00005a20: 7269 6275 7465 7328 534d 4f54 454e 4350  ributes(SMOTENCP
-00005a30: 726f 6365 7373 6f72 2829 290d 0a20 2020  rocessor())..   
-00005a40: 200d 0a20 2020 2058 2c20 793d 2062 616c   ..    X, y= bal
-00005a50: 616e 6365 2e62 616c 616e 6365 2864 6174  ance.balance(dat
-00005a60: 6173 6574 2c20 7461 7267 6574 2c20 5b22  aset, target, ["
-00005a70: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
-00005a80: 7574 6522 5d2c 2063 6f6e 745f 636f 6c75  ute"], cont_colu
-00005a90: 6d6e 733d 5b22 6665 6174 7572 6532 225d  mns=["feature2"]
-00005aa0: 2c20 6361 745f 636f 6c75 6d6e 733d 5b22  , cat_columns=["
-00005ab0: 6665 6174 7572 6531 222c 2022 7072 6f74  feature1", "prot
-00005ac0: 6563 7465 645f 6174 7472 6962 7574 6522  ected_attribute"
-00005ad0: 5d20 29                                  ] )
+000000a0: 0d0a 6672 6f6d 202e 5f70 726f 6365 7373  ..from ._process
+000000b0: 6f72 2069 6d70 6f72 7420 534d 4f54 454e  or import SMOTEN
+000000c0: 4350 726f 6365 7373 6f72 2c20 5f50 726f  CProcessor, _Pro
+000000d0: 6365 7373 6f72 0d0a 0d0a 6672 6f6d 202e  cessor....from .
+000000e0: 5f75 7469 6c73 2069 6d70 6f72 7420 7361  _utils import sa
+000000f0: 6e69 7479 5f63 6865 636b 6572 0d0a 0d0a  nity_checker....
+00000100: 0d0a 5341 4d50 4c49 4e47 5f46 554e 4354  ..SAMPLING_FUNCT
+00000110: 494f 4e53 203d 205b 2252 616e 646f 6d4f  IONS = ["RandomO
+00000120: 7665 7253 616d 706c 6572 222c 2022 534d  verSampler", "SM
+00000130: 4f54 454e 4322 2c20 2252 616e 646f 6d55  OTENC", "RandomU
+00000140: 6e64 6572 5361 6d70 6c65 7222 5d0d 0a0d  nderSampler"]...
+00000150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000160: 200d 0a63 6c61 7373 204d 6974 6967 6174   ..class Mitigat
+00000170: 6f72 2873 616e 6974 795f 6368 6563 6b65  or(sanity_checke
+00000180: 7229 203a 0d0a 0d0a 2020 2020 6465 6620  r) :....    def 
+00000190: 5f5f 696e 6974 5f5f 2873 656c 662c 206d  __init__(self, m
+000001a0: 6574 686f 6420 3d20 2252 616e 646f 6d4f  ethod = "RandomO
+000001b0: 7665 7253 616d 706c 6572 2229 203a 0d0a  verSampler") :..
+000001c0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+000001d0: 2020 2020 204d 6974 6967 6174 6f72 2069       Mitigator i
+000001e0: 6d70 6c65 6d65 6e74 2064 6966 6665 7265  mplement differe
+000001f0: 6e74 2074 7970 6573 206f 6620 6269 6169  nt types of biai
+00000200: 7320 6d69 7469 6761 7469 6f6e 2062 7920  s mitigation by 
+00000210: 7265 7361 6d70 6c69 6e67 2e0d 0a0d 0a20  resampling..... 
+00000220: 2020 2020 2020 2041 7267 733a 0d0a 2020         Args:..  
+00000230: 2020 2020 2020 2020 2020 6d65 7468 6f64            method
+00000240: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
+00000250: 3a20 7265 7361 6d70 6c69 6e67 206d 6574  : resampling met
+00000260: 686f 6473 2069 6d70 6c65 6d65 6e74 6564  hods implemented
+00000270: 2062 7920 696d 626c 6561 726e 2e20 506f   by imblearn. Po
+00000280: 7373 6962 6c65 2076 616c 7565 7320 6172  ssible values ar
+00000290: 6520 2252 616e 646f 6d4f 7665 7253 616d  e "RandomOverSam
+000002a0: 706c 6572 222c 200d 0a20 2020 2020 2020  pler", ..       
+000002b0: 2020 2020 2022 534d 4f54 454e 4322 2061       "SMOTENC" a
+000002c0: 6e64 2022 5261 6e64 6f6d 556e 6465 7253  nd "RandomUnderS
+000002d0: 616d 706c 6572 222e 2020 4465 6661 756c  ampler".  Defaul
+000002e0: 7473 2074 6f20 2252 616e 646f 6d4f 7665  ts to "RandomOve
+000002f0: 7253 616d 706c 6572 222e 0d0a 2020 2020  rSampler"...    
+00000300: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00000310: 200d 0a20 2020 2020 2020 2073 656c 662e   ..        self.
+00000320: 5f69 6e69 745f 7361 6e69 7479 5f63 6865  _init_sanity_che
+00000330: 636b 286d 6574 686f 6429 0d0a 2020 2020  ck(method)..    
+00000340: 2020 2020 0d0a 2020 2020 2020 2020 7365      ..        se
+00000350: 6c66 2e6d 6574 686f 6420 3d20 6d65 7468  lf.method = meth
+00000360: 6f64 0d0a 2020 2020 2020 2020 7365 6c66  od..        self
+00000370: 2e6d 6974 6967 6174 6f72 5f66 756e 6374  .mitigator_funct
+00000380: 696f 6e20 3d20 7b0d 0a20 2020 2020 2020  ion = {..       
+00000390: 2020 2020 2022 5261 6e64 6f6d 4f76 6572       "RandomOver
+000003a0: 5361 6d70 6c65 7222 203a 2052 616e 646f  Sampler" : Rando
+000003b0: 6d4f 7665 7253 616d 706c 6572 2c0d 0a20  mOverSampler,.. 
+000003c0: 2020 2020 2020 2020 2020 2020 2253 4d4f              "SMO
+000003d0: 5445 4e43 2220 3a20 534d 4f54 454e 432c  TENC" : SMOTENC,
+000003e0: 0d0a 2020 2020 2020 2020 2020 2020 2022  ..             "
+000003f0: 5261 6e64 6f6d 556e 6465 7253 616d 706c  RandomUnderSampl
+00000400: 6572 2220 3a20 5261 6e64 6f6d 556e 6465  er" : RandomUnde
+00000410: 7253 616d 706c 6572 0d0a 2020 2020 2020  rSampler..      
+00000420: 2020 7d0d 0a20 2020 200d 0a20 2020 2064    }..    ..    d
+00000430: 6566 205f 696e 6974 5f73 616e 6974 795f  ef _init_sanity_
+00000440: 6368 6563 6b28 7365 6c66 2c20 6d65 7468  check(self, meth
+00000450: 6f64 2920 3a0d 0a20 2020 2020 2020 2061  od) :..        a
+00000460: 7373 6572 7420 6d65 7468 6f64 2069 6e20  ssert method in 
+00000470: 5341 4d50 4c49 4e47 5f46 554e 4354 494f  SAMPLING_FUNCTIO
+00000480: 4e53 2c20 6622 6d65 7468 6f64 206e 6565  NS, f"method nee
+00000490: 6420 746f 2062 6520 696e 207b 5341 4d50  d to be in {SAMP
+000004a0: 4c49 4e47 5f46 554e 4354 494f 4e53 7d22  LING_FUNCTIONS}"
+000004b0: 0d0a 0d0a 2020 2020 0d0a 2020 2020 6465  ....    ..    de
+000004c0: 6620 6d69 7469 6761 7465 2873 656c 662c  f mitigate(self,
+000004d0: 206d 6974 6967 6174 696f 6e5f 7374 7261   mitigation_stra
+000004e0: 7465 6779 3a20 7374 722c 2064 6174 6173  tegy: str, datas
+000004f0: 6574 3a20 7064 2e44 6174 6146 7261 6d65  et: pd.DataFrame
+00000500: 2c20 7461 7267 6574 3a20 7374 722c 200d  , target: str, .
+00000510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000520: 2020 7072 6f74 6563 7465 645f 6174 7472    protected_attr
+00000530: 6962 7574 6573 3a20 6c69 7374 203d 204e  ibutes: list = N
+00000540: 6f6e 652c 2063 6f6e 745f 636f 6c75 6d6e  one, cont_column
+00000550: 733a 206c 6973 7420 3d20 4e6f 6e65 2c20  s: list = None, 
+00000560: 6361 745f 636f 6c75 6d6e 733a 206c 6973  cat_columns: lis
+00000570: 7420 3d20 4e6f 6e65 2920 3a0d 0a20 2020  t = None) :..   
+00000580: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00000590: 2020 4d69 7469 6761 7465 2062 6961 7320    Mitigate bias 
+000005a0: 7573 696e 6720 7468 6520 6769 7665 6e20  using the given 
+000005b0: 6d69 7469 6761 7469 6f6e 2073 7472 6174  mitigation strat
+000005c0: 6567 790d 0a0d 0a20 2020 2020 2020 2041  egy....        A
+000005d0: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
+000005e0: 2020 6d69 7469 6761 7469 6f6e 5f73 7472    mitigation_str
+000005f0: 6174 6567 7920 2873 7472 293a 2074 6865  ategy (str): the
+00000600: 206d 6974 6967 6174 696f 6e20 7374 7261   mitigation stra
+00000610: 7465 6779 2074 6f20 7573 652e 2050 6f73  tegy to use. Pos
+00000620: 7369 626c 6520 7661 6c75 6573 2061 7265  sible values are
+00000630: 2022 6261 6c61 6e65 5f6f 7574 7075 7422   "balane_output"
+00000640: 2c20 2262 616c 616e 6365 5f70 726f 7465  , "balance_prote
+00000650: 6374 6564 5f61 7474 7269 6275 7465 222c  cted_attribute",
+00000660: 2022 6261 6c61 6e63 655f 6f75 7470 7574   "balance_output
+00000670: 2066 6f72 2061 7474 7269 6275 7465 2220   for attribute" 
+00000680: 616e 6420 2262 616c 616e 6365 5f61 6c6c  and "balance_all
+00000690: 222e 200d 0a20 2020 2020 2020 2020 2020  ". ..           
+000006a0: 2022 6e6f 6e65 2220 6973 2061 6c73 6f20   "none" is also 
+000006b0: 696d 706c 656d 656e 7465 6420 666f 7220  implemented for 
+000006c0: 6265 6e63 686d 6172 6b69 6e67 2063 6f6e  benchmarking con
+000006d0: 7369 7374 656e 6379 2061 6e64 2073 696d  sistency and sim
+000006e0: 706c 7920 7265 7475 726e 2074 6865 2069  ply return the i
+000006f0: 6e69 7469 616c 2064 6174 6173 6574 2061  nitial dataset a
+00000700: 6e64 2074 6172 6765 742e 200d 0a20 2020  nd target. ..   
+00000710: 2020 2020 2020 2020 2064 6174 6173 6574           dataset
+00000720: 2028 7064 2e44 6174 6146 7261 6d65 293a   (pd.DataFrame):
+00000730: 2064 6174 6173 6574 2074 6f20 6d69 7469   dataset to miti
+00000740: 6761 7465 2c20 7468 6174 2069 6e63 6c75  gate, that inclu
+00000750: 6465 7320 7468 6520 7461 7267 6574 2063  des the target c
+00000760: 6f6c 756d 6e2e 0d0a 2020 2020 2020 2020  olumn...        
+00000770: 2020 2020 7461 7267 6574 2028 7374 7229      target (str)
+00000780: 3a20 7468 6520 7461 7267 6574 2063 6f6c  : the target col
+00000790: 756d 6e20 6e61 6d65 0d0a 2020 2020 2020  umn name..      
+000007a0: 2020 2020 2020 7072 6f74 6563 7465 645f        protected_
+000007b0: 6174 7472 6962 7574 6573 2028 6c69 7374  attributes (list
+000007c0: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
+000007d0: 2061 7474 7269 6275 7465 2873 2920 746f   attribute(s) to
+000007e0: 2062 616c 616e 6365 2e20 4f6e 6c79 206e   balance. Only n
+000007f0: 6563 6573 7361 7279 2066 6f72 2062 616c  ecessary for bal
+00000800: 616e 6365 5f70 726f 7465 6374 6564 5f61  ance_protected_a
+00000810: 7474 7269 6275 7465 2061 6e64 2062 616c  ttribute and bal
+00000820: 616e 6365 5f6f 7574 7075 745f 666f 725f  ance_output_for_
+00000830: 6174 7472 6962 7574 652e 2044 6566 6175  attribute. Defau
+00000840: 6c74 7320 746f 204e 6f6e 652e 0d0a 2020  lts to None...  
+00000850: 2020 2020 2020 2020 2020 636f 6e74 5f63            cont_c
+00000860: 6f6c 756d 6e73 2028 6c69 7374 2c20 6f70  olumns (list, op
+00000870: 7469 6f6e 616c 293a 2054 6865 2063 6f6e  tional): The con
+00000880: 7469 6e75 6f75 7320 636f 6c75 6d6e 7320  tinuous columns 
+00000890: 696e 2074 6865 2064 6174 6173 6574 2e20  in the dataset. 
+000008a0: 4f6e 6c79 204e 6563 6573 7361 7279 2069  Only Necessary i
+000008b0: 6620 7468 6520 7361 6d70 6c69 6e67 2073  f the sampling s
+000008c0: 7472 6174 6567 7920 6973 2053 4d4f 5445  trategy is SMOTE
+000008d0: 4e43 2e20 4465 6661 756c 7473 2074 6f20  NC. Defaults to 
+000008e0: 4e6f 6e65 2e0d 0a20 2020 2020 2020 2020  None...         
+000008f0: 2020 2063 6174 5f63 6f6c 756d 6e73 2028     cat_columns (
+00000900: 6c69 7374 2c20 6f70 7469 6f6e 616c 293a  list, optional):
+00000910: 2054 6865 2063 6174 6567 6f72 6963 616c   The categorical
+00000920: 2063 6f6c 756d 6e73 2069 6e20 7468 6520   columns in the 
+00000930: 6461 7461 7365 742e 204f 6e6c 7920 4e65  dataset. Only Ne
+00000940: 6365 7373 6172 7920 6966 2074 6865 2073  cessary if the s
+00000950: 616d 706c 696e 6720 7374 7261 7465 6779  ampling strategy
+00000960: 2069 7320 534d 4f54 454e 432e 2044 6566   is SMOTENC. Def
+00000970: 6175 6c74 7320 746f 204e 6f6e 652e 0d0a  aults to None...
+00000980: 0d0a 2020 2020 2020 2020 5261 6973 6573  ..        Raises
+00000990: 3a0d 0a20 2020 2020 2020 2020 2020 2056  :..            V
+000009a0: 616c 7565 4572 726f 723a 2049 6620 7468  alueError: If th
+000009b0: 6520 6d69 7469 6761 7469 6f6e 2073 7472  e mitigation str
+000009c0: 6174 6567 7920 646f 6573 206e 6f74 2065  ategy does not e
+000009d0: 7869 7374 0d0a 0d0a 2020 2020 2020 2020  xist....        
+000009e0: 5265 7475 726e 733a 0d0a 2020 2020 2020  Returns:..      
+000009f0: 2020 2020 2020 285b 7064 2e44 6174 6146        ([pd.DataF
+00000a00: 7261 6d65 2c20 7064 2e44 6174 6146 7261  rame, pd.DataFra
+00000a10: 6d65 5d29 3a20 7468 6520 6261 6c61 6e63  me]): the balanc
+00000a20: 6564 2064 6174 6166 7261 6d65 7320 666f  ed dataframes fo
+00000a30: 7220 7468 6520 6461 7461 7365 7420 616e  r the dataset an
+00000a40: 6420 7468 6520 7461 7267 6574 0d0a 2020  d the target..  
+00000a50: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00000a60: 2020 2069 6620 6d69 7469 6761 7469 6f6e     if mitigation
+00000a70: 5f73 7472 6174 6567 7920 3d3d 2022 6261  _strategy == "ba
+00000a80: 6c61 6e63 655f 6f75 7470 7574 2220 3a0d  lance_output" :.
+00000a90: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00000aa0: 7572 6e20 7365 6c66 2e62 616c 616e 6365  urn self.balance
+00000ab0: 5f6f 7574 7075 7428 6461 7461 7365 742c  _output(dataset,
+00000ac0: 2074 6172 6765 742c 2070 726f 7465 6374   target, protect
+00000ad0: 6564 5f61 7474 7269 6275 7465 732c 2063  ed_attributes, c
+00000ae0: 6f6e 745f 636f 6c75 6d6e 732c 2063 6174  ont_columns, cat
+00000af0: 5f63 6f6c 756d 6e73 290d 0a20 2020 2020  _columns)..     
+00000b00: 2020 2065 6c69 6620 6d69 7469 6761 7469     elif mitigati
+00000b10: 6f6e 5f73 7472 6174 6567 7920 3d3d 2022  on_strategy == "
+00000b20: 6261 6c61 6e63 655f 7072 6f74 6563 7465  balance_protecte
+00000b30: 645f 6174 7472 6962 7574 6522 203a 0d0a  d_attribute" :..
+00000b40: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00000b50: 726e 2073 656c 662e 6261 6c61 6e63 655f  rn self.balance_
+00000b60: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
+00000b70: 7574 6528 6461 7461 7365 742c 2074 6172  ute(dataset, tar
+00000b80: 6765 742c 2070 726f 7465 6374 6564 5f61  get, protected_a
+00000b90: 7474 7269 6275 7465 732c 2063 6f6e 745f  ttributes, cont_
+00000ba0: 636f 6c75 6d6e 732c 2063 6174 5f63 6f6c  columns, cat_col
+00000bb0: 756d 6e73 290d 0a20 2020 2020 2020 2065  umns)..        e
+00000bc0: 6c69 6620 6d69 7469 6761 7469 6f6e 5f73  lif mitigation_s
+00000bd0: 7472 6174 6567 7920 3d3d 2022 6261 6c61  trategy == "bala
+00000be0: 6e63 655f 6f75 7470 7574 5f66 6f72 5f61  nce_output_for_a
+00000bf0: 7474 7269 6275 7465 2220 3a0d 0a20 2020  ttribute" :..   
+00000c00: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00000c10: 7365 6c66 2e62 616c 616e 6365 5f6f 7574  self.balance_out
+00000c20: 7075 745f 666f 725f 6174 7472 6962 7574  put_for_attribut
+00000c30: 6528 6461 7461 7365 742c 2074 6172 6765  e(dataset, targe
+00000c40: 742c 2070 726f 7465 6374 6564 5f61 7474  t, protected_att
+00000c50: 7269 6275 7465 732c 2063 6f6e 745f 636f  ributes, cont_co
+00000c60: 6c75 6d6e 732c 2063 6174 5f63 6f6c 756d  lumns, cat_colum
+00000c70: 6e73 290d 0a20 2020 2020 2020 2065 6c69  ns)..        eli
+00000c80: 6620 6d69 7469 6761 7469 6f6e 5f73 7472  f mitigation_str
+00000c90: 6174 6567 7920 3d3d 2022 6261 6c61 6e63  ategy == "balanc
+00000ca0: 655f 616c 6c22 203a 0d0a 2020 2020 2020  e_all" :..      
+00000cb0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00000cc0: 662e 6261 6c61 6e63 655f 616c 6c28 6461  f.balance_all(da
+00000cd0: 7461 7365 742c 2074 6172 6765 742c 2070  taset, target, p
+00000ce0: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
+00000cf0: 7465 732c 2063 6f6e 745f 636f 6c75 6d6e  tes, cont_column
+00000d00: 732c 2063 6174 5f63 6f6c 756d 6e73 290d  s, cat_columns).
+00000d10: 0a20 2020 2020 2020 2065 6c69 6620 6d69  .        elif mi
+00000d20: 7469 6761 7469 6f6e 5f73 7472 6174 6567  tigation_strateg
+00000d30: 7920 3d3d 2022 6e6f 6e65 2220 3a0d 0a20  y == "none" :.. 
+00000d40: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00000d50: 6e20 6461 7461 7365 742c 2074 6172 6765  n dataset, targe
+00000d60: 740d 0a20 2020 2020 2020 2065 6c73 6520  t..        else 
+00000d70: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00000d80: 6169 7365 2056 616c 7565 4572 726f 720d  aise ValueError.
+00000d90: 0a20 2020 2020 2020 200d 0a20 2020 2064  .        ..    d
+00000da0: 6566 2062 616c 616e 6365 5f6f 7574 7075  ef balance_outpu
+00000db0: 7428 7365 6c66 2c20 6461 7461 7365 743a  t(self, dataset:
+00000dc0: 2070 642e 4461 7461 4672 616d 652c 2074   pd.DataFrame, t
+00000dd0: 6172 6765 743a 2073 7472 2c20 7072 6f74  arget: str, prot
+00000de0: 6563 7465 645f 6174 7472 6962 7574 6573  ected_attributes
+00000df0: 3a20 6c69 7374 203d 204e 6f6e 652c 200d  : list = None, .
+00000e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000e10: 2020 2020 2020 2020 636f 6e74 5f63 6f6c          cont_col
+00000e20: 756d 6e73 3a20 6c69 7374 203d 204e 6f6e  umns: list = Non
+00000e30: 652c 2063 6174 5f63 6f6c 756d 6e73 3a20  e, cat_columns: 
+00000e40: 6c69 7374 203d 204e 6f6e 6529 203a 0d0a  list = None) :..
+00000e50: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00000e60: 2020 2020 2042 616c 616e 6365 2074 6865       Balance the
+00000e70: 206f 7574 7075 7420 7769 7468 206e 6f20   output with no 
+00000e80: 7265 6761 7264 7320 746f 2074 6865 2070  regards to the p
+00000e90: 726f 7465 6374 6564 2061 7474 7269 6275  rotected attribu
+00000ea0: 7465 732e 0d0a 2020 2020 2020 2020 0d0a  tes...        ..
+00000eb0: 2020 2020 2020 2020 4172 6773 3a20 0d0a          Args: ..
+00000ec0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00000ed0: 7365 7420 2870 642e 4461 7461 4672 616d  set (pd.DataFram
+00000ee0: 6529 3a20 6461 7461 7365 7420 746f 206d  e): dataset to m
+00000ef0: 6974 6967 6174 652c 2074 6861 7420 696e  itigate, that in
+00000f00: 636c 7564 6573 2074 6865 2074 6172 6765  cludes the targe
+00000f10: 7420 636f 6c75 6d6e 2e0d 0a20 2020 2020  t column...     
+00000f20: 2020 2020 2020 2074 6172 6765 7420 2873         target (s
+00000f30: 7472 293a 2074 6865 2074 6172 6765 7420  tr): the target 
+00000f40: 636f 6c75 6d6e 206e 616d 650d 0a20 2020  column name..   
+00000f50: 2020 2020 2020 2020 2070 726f 7465 6374           protect
+00000f60: 6564 5f61 7474 7269 6275 7465 7320 286c  ed_attributes (l
+00000f70: 6973 742c 206f 7074 696f 6e61 6c29 3a20  ist, optional): 
+00000f80: 5573 656c 6573 7320 666f 7220 7468 6973  Useless for this
+00000f90: 206d 6974 6967 6174 696f 6e20 7374 7261   mitigation stra
+00000fa0: 7465 6779 2c20 6275 7420 696d 706c 656d  tegy, but implem
+00000fb0: 656e 7465 6420 666f 7220 4150 4920 636f  ented for API co
+00000fc0: 6e73 6973 7465 6e63 792e 2044 6566 6175  nsistency. Defau
+00000fd0: 6c74 7320 746f 204e 6f6e 652e 0d0a 2020  lts to None...  
+00000fe0: 2020 2020 2020 2020 2020 636f 6e74 5f63            cont_c
+00000ff0: 6f6c 756d 6e73 2028 6c69 7374 2c20 6f70  olumns (list, op
+00001000: 7469 6f6e 616c 293a 2054 6865 2063 6f6e  tional): The con
+00001010: 7469 6e75 6f75 7320 636f 6c75 6d6e 7320  tinuous columns 
+00001020: 696e 2074 6865 2064 6174 6173 6574 2e20  in the dataset. 
+00001030: 4f6e 6c79 204e 6563 6573 7361 7279 2069  Only Necessary i
+00001040: 6620 7468 6520 7361 6d70 6c69 6e67 2073  f the sampling s
+00001050: 7472 6174 6567 7920 6973 2053 4d4f 5445  trategy is SMOTE
+00001060: 4e43 2e20 4465 6661 756c 7473 2074 6f20  NC. Defaults to 
+00001070: 4e6f 6e65 2e0d 0a20 2020 2020 2020 2020  None...         
+00001080: 2020 2063 6174 5f63 6f6c 756d 6e73 2028     cat_columns (
+00001090: 6c69 7374 2c20 6f70 7469 6f6e 616c 293a  list, optional):
+000010a0: 2054 6865 2063 6174 6567 6f72 6963 616c   The categorical
+000010b0: 2063 6f6c 756d 6e73 2069 6e20 7468 6520   columns in the 
+000010c0: 6461 7461 7365 742e 204f 6e6c 7920 4e65  dataset. Only Ne
+000010d0: 6365 7373 6172 7920 6966 2074 6865 2073  cessary if the s
+000010e0: 616d 706c 696e 6720 7374 7261 7465 6779  ampling strategy
+000010f0: 2069 7320 534d 4f54 454e 432e 2044 6566   is SMOTENC. Def
+00001100: 6175 6c74 7320 746f 204e 6f6e 652e 0d0a  aults to None...
+00001110: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00001120: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00001130: 285b 7064 2e44 6174 6146 7261 6d65 2c20  ([pd.DataFrame, 
+00001140: 7064 2e44 6174 6146 7261 6d65 5d29 3a20  pd.DataFrame]): 
+00001150: 7468 6520 6261 6c61 6e63 6564 2064 6174  the balanced dat
+00001160: 6166 7261 6d65 7320 666f 7220 7468 6520  aframes for the 
+00001170: 6461 7461 7365 7420 616e 6420 7468 6520  dataset and the 
+00001180: 7461 7267 6574 0d0a 2020 2020 2020 2020  target..        
+00001190: 2222 220d 0a20 2020 2020 2020 2073 7570  """..        sup
+000011a0: 6572 2829 2e5f 7361 6e69 7479 5f63 6865  er()._sanity_che
+000011b0: 636b 2864 6174 6173 6574 2c20 7461 7267  ck(dataset, targ
+000011c0: 6574 2c20 7072 6f74 6563 7465 645f 6174  et, protected_at
+000011d0: 7472 6962 7574 6573 3d70 726f 7465 6374  tributes=protect
+000011e0: 6564 5f61 7474 7269 6275 7465 7329 0d0a  ed_attributes)..
+000011f0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00001200: 2020 2369 6620 6e6f 7420 5261 6e64 6f6d    #if not Random
+00001210: 4f76 6572 5361 6d70 6c65 722c 206e 6565  OverSampler, nee
+00001220: 6420 746f 206f 6e65 2d68 6f74 2065 6e63  d to one-hot enc
+00001230: 6f64 6520 6576 6572 7920 6361 7465 676f  ode every catego
+00001240: 7269 6361 6c0d 0a20 2020 2020 2020 2064  rical..        d
+00001250: 6620 3d20 6461 7461 7365 742e 636f 7079  f = dataset.copy
+00001260: 2829 0d0a 2020 2020 2020 2020 7461 7267  ()..        targ
+00001270: 6574 5f64 6620 3d20 6466 5b74 6172 6765  et_df = df[targe
+00001280: 745d 0d0a 2020 2020 2020 2020 6466 203d  t]..        df =
+00001290: 2064 662e 6472 6f70 2863 6f6c 756d 6e73   df.drop(columns
+000012a0: 3d74 6172 6765 7429 0d0a 2020 2020 2020  =target)..      
+000012b0: 2020 0d0a 2020 2020 2020 2020 0d0a 2020    ..        ..  
+000012c0: 2020 2020 2020 6966 2070 726f 7465 6374        if protect
+000012d0: 6564 5f61 7474 7269 6275 7465 7320 616e  ed_attributes an
+000012e0: 6420 6c65 6e28 7072 6f74 6563 7465 645f  d len(protected_
+000012f0: 6174 7472 6962 7574 6573 2920 3e20 3120  attributes) > 1 
+00001300: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
+00001310: 662c 2070 726f 7465 6374 6564 5f61 7474  f, protected_att
+00001320: 7269 6275 7465 203d 2073 656c 662e 5f6d  ribute = self._m
+00001330: 616b 655f 7375 7065 725f 7072 6f74 6563  ake_super_protec
+00001340: 7465 6428 6461 7461 7365 742c 2070 726f  ted(dataset, pro
+00001350: 7465 6374 6564 5f61 7474 7269 6275 7465  tected_attribute
+00001360: 7329 0d0a 2020 2020 2020 2020 0d0a 2020  s)..        ..  
+00001370: 2020 2020 2020 6966 2073 656c 662e 6d65        if self.me
+00001380: 7468 6f64 2069 6e20 5b22 534d 4f54 454e  thod in ["SMOTEN
+00001390: 4322 5d20 3a0d 0a20 2020 2020 2020 2020  C"] :..         
+000013a0: 2020 2023 7072 6f63 6573 730d 0a20 2020     #process..   
+000013b0: 2020 2020 2020 2020 2070 726f 6365 7373           process
+000013c0: 6f72 203d 205f 5072 6f63 6573 736f 7228  or = _Processor(
+000013d0: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
+000013e0: 726f 6365 7373 6564 5f64 663d 2070 726f  rocessed_df= pro
+000013f0: 6365 7373 6f72 2e70 726f 6365 7373 2864  cessor.process(d
+00001400: 662c 2073 6361 6c65 5f63 6f6c 733d 636f  f, scale_cols=co
+00001410: 6e74 5f63 6f6c 756d 6e73 2c20 656e 636f  nt_columns, enco
+00001420: 6465 5f63 6f6c 733d 6361 745f 636f 6c75  de_cols=cat_colu
+00001430: 6d6e 7329 0d0a 0d0a 2020 2020 2020 2020  mns)....        
+00001440: 2020 2020 2320 5468 656e 2072 6573 616d      # Then resam
+00001450: 706c 650d 0a20 2020 2020 2020 2020 2020  ple..           
+00001460: 2063 6174 5f63 6f6c 756d 6e73 5f69 6473   cat_columns_ids
+00001470: 203d 205b 7072 6f63 6573 7365 645f 6466   = [processed_df
+00001480: 2e63 6f6c 756d 6e73 2e67 6574 5f6c 6f63  .columns.get_loc
+00001490: 2863 6f6c 5f6e 616d 6529 2066 6f72 2063  (col_name) for c
+000014a0: 6f6c 5f6e 616d 6520 696e 2063 6174 5f63  ol_name in cat_c
+000014b0: 6f6c 756d 6e73 5d0d 0a20 2020 2020 2020  olumns]..       
+000014c0: 2020 2020 2073 616d 706c 6572 203d 2073       sampler = s
+000014d0: 656c 662e 6d69 7469 6761 746f 725f 6675  elf.mitigator_fu
+000014e0: 6e63 7469 6f6e 5b73 656c 662e 6d65 7468  nction[self.meth
+000014f0: 6f64 5d28 6361 745f 636f 6c75 6d6e 735f  od](cat_columns_
+00001500: 6964 7329 0d0a 2020 2020 2020 2020 2020  ids)..          
+00001510: 2020 585f 7265 7361 6d70 6c65 642c 2079    X_resampled, y
+00001520: 5f72 6573 616d 706c 6564 203d 2073 616d  _resampled = sam
+00001530: 706c 6572 2e66 6974 5f72 6573 616d 706c  pler.fit_resampl
+00001540: 6528 7072 6f63 6573 7365 645f 6466 2c20  e(processed_df, 
+00001550: 7461 7267 6574 5f64 6629 0d0a 2020 2020  target_df)..    
+00001560: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00001570: 2020 2020 2020 2320 5468 656e 2075 6e70        # Then unp
+00001580: 726f 6365 7373 2069 740d 0a20 2020 2020  rocess it..     
+00001590: 2020 2020 2020 2064 665f 6669 6e61 6c20         df_final 
+000015a0: 3d20 7072 6f63 6573 736f 722e 756e 7072  = processor.unpr
+000015b0: 6f63 6573 7328 585f 7265 7361 6d70 6c65  ocess(X_resample
+000015c0: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
+000015d0: 7461 7267 6574 5f66 696e 616c 203d 2079  target_final = y
+000015e0: 5f72 6573 616d 706c 6564 0d0a 0d0a 2020  _resampled....  
+000015f0: 2020 2020 2020 656c 7365 203a 0d0a 2020        else :..  
+00001600: 2020 2020 2020 2020 2020 236a 7573 7420            #just 
+00001610: 7265 7361 6d70 6c65 720d 0a20 2020 2020  resampler..     
+00001620: 2020 2020 2020 2073 616d 706c 6572 203d         sampler =
+00001630: 2073 656c 662e 6d69 7469 6761 746f 725f   self.mitigator_
+00001640: 6675 6e63 7469 6f6e 5b73 656c 662e 6d65  function[self.me
+00001650: 7468 6f64 5d28 290d 0a20 2020 2020 2020  thod]()..       
+00001660: 2020 2020 2064 665f 6669 6e61 6c2c 2074       df_final, t
+00001670: 6172 6765 745f 6669 6e61 6c20 3d20 7361  arget_final = sa
+00001680: 6d70 6c65 722e 6669 745f 7265 7361 6d70  mpler.fit_resamp
+00001690: 6c65 2864 662c 2074 6172 6765 745f 6466  le(df, target_df
+000016a0: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
+000016b0: 2020 2020 2069 6620 7072 6f74 6563 7465       if protecte
+000016c0: 645f 6174 7472 6962 7574 6573 2061 6e64  d_attributes and
+000016d0: 206c 656e 2870 726f 7465 6374 6564 5f61   len(protected_a
+000016e0: 7474 7269 6275 7465 7329 203e 2031 203a  ttributes) > 1 :
+000016f0: 0d0a 2020 2020 2020 2020 2020 2020 6466  ..            df
+00001700: 5f66 696e 616c 203d 2064 665f 6669 6e61  _final = df_fina
+00001710: 6c2e 6472 6f70 2863 6f6c 756d 6e73 203d  l.drop(columns =
+00001720: 2070 726f 7465 6374 6564 5f61 7474 7269   protected_attri
+00001730: 6275 7465 290d 0a20 2020 2020 2020 200d  bute)..        .
+00001740: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001750: 6466 5f66 696e 616c 2c20 7461 7267 6574  df_final, target
+00001760: 5f66 696e 616c 0d0a 2020 2020 2020 2020  _final..        
+00001770: 2020 2020 0d0a 2020 2020 6465 6620 6261      ..    def ba
+00001780: 6c61 6e63 655f 7072 6f74 6563 7465 645f  lance_protected_
+00001790: 6174 7472 6962 7574 6528 7365 6c66 2c20  attribute(self, 
+000017a0: 6461 7461 7365 743a 2070 642e 4461 7461  dataset: pd.Data
+000017b0: 4672 616d 652c 2074 6172 6765 743a 2073  Frame, target: s
+000017c0: 7472 2c20 7072 6f74 6563 7465 645f 6174  tr, protected_at
+000017d0: 7472 6962 7574 6573 3a20 6c69 7374 2c20  tributes: list, 
+000017e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000017f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001800: 2020 2020 2020 636f 6e74 5f63 6f6c 756d        cont_colum
+00001810: 6e73 3a20 6c69 7374 203d 204e 6f6e 652c  ns: list = None,
+00001820: 2063 6174 5f63 6f6c 756d 6e73 3a20 6c69   cat_columns: li
+00001830: 7374 203d 204e 6f6e 6529 203a 0d0a 2020  st = None) :..  
+00001840: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00001850: 2020 2042 616c 616e 6365 2074 6865 2063     Balance the c
+00001860: 6c61 7373 6573 206f 6620 6120 7072 6f74  lasses of a prot
+00001870: 6563 7465 6420 6174 7472 6962 7574 6520  ected attribute 
+00001880: 7769 7468 206e 6f20 7265 6761 7264 7320  with no regards 
+00001890: 746f 2074 6865 206f 7574 7075 742e 205c  to the output. \
+000018a0: 6e0d 0a20 2020 2020 2020 2053 686f 756c  n..        Shoul
+000018b0: 6420 696d 7072 6f76 6520 7468 6520 6261  d improve the ba
+000018c0: 6c61 6e63 6520 666f 7220 7468 6520 7072  lance for the pr
+000018d0: 6f74 6563 7465 6420 6174 7472 6962 7574  otected attribut
+000018e0: 652e 0d0a 2020 2020 2020 2020 0d0a 2020  e...        ..  
+000018f0: 2020 2020 2020 4172 6773 3a20 0d0a 2020        Args: ..  
+00001900: 2020 2020 2020 2020 2020 6461 7461 7365            datase
+00001910: 7420 2870 642e 4461 7461 4672 616d 6529  t (pd.DataFrame)
+00001920: 3a20 6461 7461 7365 7420 746f 206d 6974  : dataset to mit
+00001930: 6967 6174 652c 2074 6861 7420 696e 636c  igate, that incl
+00001940: 7564 6573 2074 6865 2074 6172 6765 7420  udes the target 
+00001950: 636f 6c75 6d6e 2e0d 0a20 2020 2020 2020  column...       
+00001960: 2020 2020 2074 6172 6765 7420 2873 7472       target (str
+00001970: 293a 2074 6865 2074 6172 6765 7420 636f  ): the target co
+00001980: 6c75 6d6e 206e 616d 650d 0a20 2020 2020  lumn name..     
+00001990: 2020 2020 2020 2070 726f 7465 6374 6564         protected
+000019a0: 5f61 7474 7269 6275 7465 7320 286c 6973  _attributes (lis
+000019b0: 742c 206f 7074 696f 6e61 6c29 3a20 5468  t, optional): Th
+000019c0: 6520 6174 7472 6962 7574 6528 7329 2074  e attribute(s) t
+000019d0: 6f20 6261 6c61 6e63 652e 2044 6566 6175  o balance. Defau
+000019e0: 6c74 7320 746f 204e 6f6e 652e 0d0a 2020  lts to None...  
+000019f0: 2020 2020 2020 2020 2020 636f 6e74 5f63            cont_c
+00001a00: 6f6c 756d 6e73 2028 6c69 7374 2c20 6f70  olumns (list, op
+00001a10: 7469 6f6e 616c 293a 2054 6865 2063 6f6e  tional): The con
+00001a20: 7469 6e75 6f75 7320 636f 6c75 6d6e 7320  tinuous columns 
+00001a30: 696e 2074 6865 2064 6174 6173 6574 2e20  in the dataset. 
+00001a40: 4f6e 6c79 204e 6563 6573 7361 7279 2069  Only Necessary i
+00001a50: 6620 7468 6520 7361 6d70 6c69 6e67 2073  f the sampling s
+00001a60: 7472 6174 6567 7920 6973 2053 4d4f 5445  trategy is SMOTE
+00001a70: 4e43 2e20 4465 6661 756c 7473 2074 6f20  NC. Defaults to 
+00001a80: 4e6f 6e65 2e0d 0a20 2020 2020 2020 2020  None...         
+00001a90: 2020 2063 6174 5f63 6f6c 756d 6e73 2028     cat_columns (
+00001aa0: 6c69 7374 2c20 6f70 7469 6f6e 616c 293a  list, optional):
+00001ab0: 2054 6865 2063 6174 6567 6f72 6963 616c   The categorical
+00001ac0: 2063 6f6c 756d 6e73 2069 6e20 7468 6520   columns in the 
+00001ad0: 6461 7461 7365 742e 204f 6e6c 7920 4e65  dataset. Only Ne
+00001ae0: 6365 7373 6172 7920 6966 2074 6865 2073  cessary if the s
+00001af0: 616d 706c 696e 6720 7374 7261 7465 6779  ampling strategy
+00001b00: 2069 7320 534d 4f54 454e 432e 2044 6566   is SMOTENC. Def
+00001b10: 6175 6c74 7320 746f 204e 6f6e 652e 0d0a  aults to None...
+00001b20: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00001b30: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00001b40: 285b 7064 2e44 6174 6146 7261 6d65 2c20  ([pd.DataFrame, 
+00001b50: 7064 2e44 6174 6146 7261 6d65 5d29 3a20  pd.DataFrame]): 
+00001b60: 7468 6520 6261 6c61 6e63 6564 2064 6174  the balanced dat
+00001b70: 6166 7261 6d65 7320 666f 7220 7468 6520  aframes for the 
+00001b80: 6461 7461 7365 7420 616e 6420 7468 6520  dataset and the 
+00001b90: 7461 7267 6574 0d0a 2020 2020 2020 2020  target..        
+00001ba0: 2222 220d 0a20 2020 2020 2020 2073 7570  """..        sup
+00001bb0: 6572 2829 2e5f 7361 6e69 7479 5f63 6865  er()._sanity_che
+00001bc0: 636b 2864 6174 6173 6574 2c20 7461 7267  ck(dataset, targ
+00001bd0: 6574 2c20 7072 6f74 6563 7465 645f 6174  et, protected_at
+00001be0: 7472 6962 7574 6573 3d70 726f 7465 6374  tributes=protect
+00001bf0: 6564 5f61 7474 7269 6275 7465 7329 0d0a  ed_attributes)..
+00001c00: 2020 2020 2020 2020 6466 203d 2064 6174          df = dat
+00001c10: 6173 6574 2e63 6f70 7928 290d 0a20 2020  aset.copy()..   
+00001c20: 2020 2020 2074 6172 6765 745f 6466 203d       target_df =
+00001c30: 2064 665b 7461 7267 6574 5d0d 0a20 2020   df[target]..   
+00001c40: 2020 2020 2064 6620 3d20 6466 2e64 726f       df = df.dro
+00001c50: 7028 636f 6c75 6d6e 733d 7461 7267 6574  p(columns=target
+00001c60: 290d 0a0d 0a20 2020 2020 2020 2069 6620  )....        if 
+00001c70: 6c65 6e28 7072 6f74 6563 7465 645f 6174  len(protected_at
+00001c80: 7472 6962 7574 6573 2920 3e20 3120 3a0d  tributes) > 1 :.
+00001c90: 0a20 2020 2020 2020 2020 2020 2064 662c  .            df,
+00001ca0: 2070 726f 7465 6374 6564 5f61 7474 7269   protected_attri
+00001cb0: 6275 7465 203d 2073 656c 662e 5f6d 616b  bute = self._mak
+00001cc0: 655f 7375 7065 725f 7072 6f74 6563 7465  e_super_protecte
+00001cd0: 6428 6461 7461 7365 742c 2070 726f 7465  d(dataset, prote
+00001ce0: 6374 6564 5f61 7474 7269 6275 7465 7329  cted_attributes)
+00001cf0: 0d0a 2020 2020 2020 2020 656c 7365 203a  ..        else :
+00001d00: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+00001d10: 6f74 6563 7465 645f 6174 7472 6962 7574  otected_attribut
+00001d20: 6520 3d20 7072 6f74 6563 7465 645f 6174  e = protected_at
+00001d30: 7472 6962 7574 6573 5b30 5d0d 0a0d 0a20  tributes[0].... 
+00001d40: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+00001d50: 6574 686f 6420 696e 205b 2253 4d4f 5445  ethod in ["SMOTE
+00001d60: 4e43 225d 203a 0d0a 2020 2020 2020 2020  NC"] :..        
+00001d70: 2020 2020 2370 7265 7072 6f63 6573 7320      #preprocess 
+00001d80: 7573 696e 6720 7468 6520 7072 6f74 6563  using the protec
+00001d90: 7465 6420 6174 7472 6962 7574 6520 6173  ted attribute as
+00001da0: 2061 2074 6172 6765 740d 0a20 2020 2020   a target..     
+00001db0: 2020 2020 2020 2063 6f6e 745f 636f 6c5f         cont_col_
+00001dc0: 6275 6666 203d 205b 6665 6174 7572 6520  buff = [feature 
+00001dd0: 666f 7220 6665 6174 7572 6520 696e 2063  for feature in c
+00001de0: 6f6e 745f 636f 6c75 6d6e 7320 6966 2066  ont_columns if f
+00001df0: 6561 7475 7265 2021 3d20 7072 6f74 6563  eature != protec
+00001e00: 7465 645f 6174 7472 6962 7574 655d 0d0a  ted_attribute]..
+00001e10: 2020 2020 2020 2020 2020 2020 6361 745f              cat_
+00001e20: 636f 6c5f 6275 6666 203d 205b 6665 6174  col_buff = [feat
+00001e30: 7572 6520 666f 7220 6665 6174 7572 6520  ure for feature 
+00001e40: 696e 2063 6174 5f63 6f6c 756d 6e73 2069  in cat_columns i
+00001e50: 6620 6665 6174 7572 6520 213d 2070 726f  f feature != pro
+00001e60: 7465 6374 6564 5f61 7474 7269 6275 7465  tected_attribute
+00001e70: 5d0d 0a20 2020 2020 2020 2020 2020 200d  ]..            .
+00001e80: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+00001e90: 6365 7373 6f72 203d 205f 5072 6f63 6573  cessor = _Proces
+00001ea0: 736f 7228 290d 0a20 2020 2020 2020 2020  sor()..         
+00001eb0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00001ec0: 2070 726f 6365 7373 6564 5f64 6620 3d20   processed_df = 
+00001ed0: 7072 6f63 6573 736f 722e 7072 6f63 6573  processor.proces
+00001ee0: 7328 6466 2c20 7363 616c 655f 636f 6c73  s(df, scale_cols
+00001ef0: 3d63 6f6e 745f 636f 6c5f 6275 6666 2c20  =cont_col_buff, 
+00001f00: 656e 636f 6465 5f63 6f6c 733d 2863 6174  encode_cols=(cat
+00001f10: 5f63 6f6c 5f62 7566 6620 2b20 5b70 726f  _col_buff + [pro
+00001f20: 7465 6374 6564 5f61 7474 7269 6275 7465  tected_attribute
+00001f30: 5d29 290d 0a0d 0a20 2020 2020 2020 2020  ]))....         
+00001f40: 2020 2070 726f 7465 6374 6564 5f61 7474     protected_att
+00001f50: 7269 6275 7465 5f63 6f6c 756d 6e20 3d20  ribute_column = 
+00001f60: 7072 6f63 6573 7365 645f 6466 5b70 726f  processed_df[pro
+00001f70: 7465 6374 6564 5f61 7474 7269 6275 7465  tected_attribute
+00001f80: 5d0d 0a20 2020 2020 2020 2020 2020 2070  ]..            p
+00001f90: 726f 6365 7373 6564 5f64 662e 6472 6f70  rocessed_df.drop
+00001fa0: 2863 6f6c 756d 6e73 203d 205b 7072 6f74  (columns = [prot
+00001fb0: 6563 7465 645f 6174 7472 6962 7574 655d  ected_attribute]
+00001fc0: 2c20 696e 706c 6163 6520 3d20 5472 7565  , inplace = True
+00001fd0: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
+00001fe0: 726f 6365 7373 6564 5f64 662e 6c6f 635b  rocessed_df.loc[
+00001ff0: 3a2c 7461 7267 6574 5d20 3d20 7461 7267  :,target] = targ
+00002000: 6574 5f64 660d 0a0d 0a20 2020 2020 2020  et_df....       
+00002010: 2020 2020 2063 6174 5f63 6f6c 756d 6e5f       cat_column_
+00002020: 6275 6666 203d 2063 6174 5f63 6f6c 5f62  buff = cat_col_b
+00002030: 7566 662e 636f 7079 2829 0d0a 2020 2020  uff.copy()..    
+00002040: 2020 2020 2020 2020 6361 745f 636f 6c75          cat_colu
+00002050: 6d6e 5f62 7566 662e 6170 7065 6e64 2874  mn_buff.append(t
+00002060: 6172 6765 7429 0d0a 2020 2020 2020 2020  arget)..        
+00002070: 2020 2020 6361 745f 636f 6c75 6d6e 5f69      cat_column_i
+00002080: 6473 203d 205b 7072 6f63 6573 7365 645f  ds = [processed_
+00002090: 6466 2e63 6f6c 756d 6e73 2e67 6574 5f6c  df.columns.get_l
+000020a0: 6f63 2863 6f6c 5f6e 616d 6529 2066 6f72  oc(col_name) for
+000020b0: 2063 6f6c 5f6e 616d 6520 696e 2063 6174   col_name in cat
+000020c0: 5f63 6f6c 756d 6e5f 6275 6666 5d0d 0a0d  _column_buff]...
+000020d0: 0a20 2020 2020 2020 2020 2020 2073 616d  .            sam
+000020e0: 706c 6572 203d 2073 656c 662e 6d69 7469  pler = self.miti
+000020f0: 6761 746f 725f 6675 6e63 7469 6f6e 5b73  gator_function[s
+00002100: 656c 662e 6d65 7468 6f64 5d28 6361 7465  elf.method](cate
+00002110: 676f 7269 6361 6c5f 6665 6174 7572 6573  gorical_features
+00002120: 3d63 6174 5f63 6f6c 756d 6e5f 6964 7329  =cat_column_ids)
+00002130: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00002140: 585f 7265 7361 6d70 6c65 642c 2061 7474  X_resampled, att
+00002150: 7269 6275 7465 5f72 6573 616d 706c 6564  ribute_resampled
+00002160: 203d 2073 616d 706c 6572 2e66 6974 5f72   = sampler.fit_r
+00002170: 6573 616d 706c 6528 7072 6f63 6573 7365  esample(processe
+00002180: 645f 6466 2c20 7072 6f74 6563 7465 645f  d_df, protected_
+00002190: 6174 7472 6962 7574 655f 636f 6c75 6d6e  attribute_column
+000021a0: 290d 0a20 2020 2020 2020 2020 2020 2058  )..            X
+000021b0: 5f72 6573 616d 706c 6564 2e6c 6f63 5b3a  _resampled.loc[:
+000021c0: 2c20 7072 6f74 6563 7465 645f 6174 7472  , protected_attr
+000021d0: 6962 7574 655d 203d 2061 7474 7269 6275  ibute] = attribu
+000021e0: 7465 5f72 6573 616d 706c 6564 0d0a 2020  te_resampled..  
+000021f0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00002200: 2020 2020 2020 2064 665f 6669 6e61 6c20         df_final 
+00002210: 3d20 7072 6f63 6573 736f 722e 756e 7072  = processor.unpr
+00002220: 6f63 6573 7328 585f 7265 7361 6d70 6c65  ocess(X_resample
+00002230: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
+00002240: 7461 7267 6574 5f66 696e 616c 203d 2064  target_final = d
+00002250: 665f 6669 6e61 6c5b 7461 7267 6574 5d0d  f_final[target].
+00002260: 0a20 2020 2020 2020 2020 2020 2064 665f  .            df_
+00002270: 6669 6e61 6c2e 6472 6f70 2863 6f6c 756d  final.drop(colum
+00002280: 6e73 3d5b 7461 7267 6574 5d2c 2069 6e70  ns=[target], inp
+00002290: 6c61 6365 3d54 7275 6529 0d0a 0d0a 2020  lace=True)....  
+000022a0: 2020 2020 2020 656c 7365 203a 200d 0a20        else : .. 
+000022b0: 2020 2020 2020 2020 2020 2070 726f 7465             prote
+000022c0: 6374 6564 5f61 7474 7269 6275 7465 5f63  cted_attribute_c
+000022d0: 6f6c 756d 6e20 3d20 6466 5b70 726f 7465  olumn = df[prote
+000022e0: 6374 6564 5f61 7474 7269 6275 7465 5d0d  cted_attribute].
+000022f0: 0a20 2020 2020 2020 2020 2020 2064 662e  .            df.
+00002300: 6472 6f70 2863 6f6c 756d 6e73 203d 205b  drop(columns = [
+00002310: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
+00002320: 7574 655d 2c20 696e 706c 6163 6520 3d20  ute], inplace = 
+00002330: 5472 7565 290d 0a20 2020 2020 2020 2020  True)..         
+00002340: 2020 2064 662e 6c6f 635b 3a2c 7461 7267     df.loc[:,targ
+00002350: 6574 5d20 3d20 7461 7267 6574 5f64 660d  et] = target_df.
+00002360: 0a0d 0a20 2020 2020 2020 2020 2020 2073  ...            s
+00002370: 616d 706c 6572 203d 2073 656c 662e 6d69  ampler = self.mi
+00002380: 7469 6761 746f 725f 6675 6e63 7469 6f6e  tigator_function
+00002390: 5b73 656c 662e 6d65 7468 6f64 5d28 290d  [self.method]().
+000023a0: 0a20 2020 2020 2020 2020 2020 2058 5f72  .            X_r
+000023b0: 6573 616d 706c 6564 2c20 6174 7472 6962  esampled, attrib
+000023c0: 7574 655f 7265 7361 6d70 6c65 6420 3d20  ute_resampled = 
+000023d0: 7361 6d70 6c65 722e 6669 745f 7265 7361  sampler.fit_resa
+000023e0: 6d70 6c65 2864 662c 2070 726f 7465 6374  mple(df, protect
+000023f0: 6564 5f61 7474 7269 6275 7465 5f63 6f6c  ed_attribute_col
+00002400: 756d 6e29 0d0a 2020 2020 2020 2020 2020  umn)..          
+00002410: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00002420: 585f 7265 7361 6d70 6c65 642e 6c6f 635b  X_resampled.loc[
+00002430: 3a2c 2070 726f 7465 6374 6564 5f61 7474  :, protected_att
+00002440: 7269 6275 7465 5d20 3d20 6174 7472 6962  ribute] = attrib
+00002450: 7574 655f 7265 7361 6d70 6c65 640d 0a20  ute_resampled.. 
+00002460: 2020 2020 2020 2020 2020 2074 6172 6765             targe
+00002470: 745f 6669 6e61 6c20 3d20 585f 7265 7361  t_final = X_resa
+00002480: 6d70 6c65 645b 7461 7267 6574 5d0d 0a20  mpled[target].. 
+00002490: 2020 2020 2020 2020 2020 2064 665f 6669             df_fi
+000024a0: 6e61 6c20 3d20 585f 7265 7361 6d70 6c65  nal = X_resample
+000024b0: 642e 6472 6f70 2863 6f6c 756d 6e73 3d5b  d.drop(columns=[
+000024c0: 7461 7267 6574 5d29 0d0a 2020 2020 2020  target])..      
+000024d0: 2020 0d0a 2020 2020 2020 2020 6966 206c    ..        if l
+000024e0: 656e 2870 726f 7465 6374 6564 5f61 7474  en(protected_att
+000024f0: 7269 6275 7465 7329 203e 2031 203a 0d0a  ributes) > 1 :..
+00002500: 2020 2020 2020 2020 2020 2020 6466 5f66              df_f
+00002510: 696e 616c 203d 2064 665f 6669 6e61 6c2e  inal = df_final.
+00002520: 6472 6f70 2863 6f6c 756d 6e73 203d 2070  drop(columns = p
+00002530: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
+00002540: 7465 2920 2020 200d 0a20 2020 200d 0a20  te)    ..    .. 
+00002550: 2020 2020 2020 2072 6574 7572 6e20 6466         return df
+00002560: 5f66 696e 616c 2c20 7461 7267 6574 5f66  _final, target_f
+00002570: 696e 616c 0d0a 2020 2020 0d0a 2020 2020  inal..    ..    
+00002580: 6465 6620 6261 6c61 6e63 655f 6f75 7470  def balance_outp
+00002590: 7574 5f66 6f72 5f61 7474 7269 6275 7465  ut_for_attribute
+000025a0: 2873 656c 662c 2064 6174 6173 6574 3a20  (self, dataset: 
+000025b0: 7064 2e44 6174 6146 7261 6d65 2c20 7461  pd.DataFrame, ta
+000025c0: 7267 6574 3a20 7374 722c 2070 726f 7465  rget: str, prote
+000025d0: 6374 6564 5f61 7474 7269 6275 7465 733a  cted_attributes:
+000025e0: 206c 6973 742c 200d 0a20 2020 2020 2020   list, ..       
+000025f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002600: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00002610: 6e74 5f63 6f6c 756d 6e73 3a20 6c69 7374  nt_columns: list
+00002620: 203d 204e 6f6e 652c 2063 6174 5f63 6f6c   = None, cat_col
+00002630: 756d 6e73 3a20 6c69 7374 203d 204e 6f6e  umns: list = Non
+00002640: 6529 203a 0d0a 2020 2020 2020 2020 2222  e) :..        ""
+00002650: 220d 0a20 2020 2020 2020 2042 616c 616e  "..        Balan
+00002660: 6365 2074 6865 206f 7574 7075 7420 6f66  ce the output of
+00002670: 2074 6865 2063 6c61 7373 6573 2066 6f72   the classes for
+00002680: 2061 2067 6976 656e 2070 726f 7465 6374   a given protect
+00002690: 6564 2061 7474 7269 6275 7465 2e20 5c6e  ed attribute. \n
+000026a0: 0d0a 2020 2020 2020 2020 5368 6f75 6c64  ..        Should
+000026b0: 2069 6d70 726f 7665 2074 6865 2044 4952   improve the DIR
+000026c0: 2066 6f72 2074 6865 2070 726f 7465 6374   for the protect
+000026d0: 6564 2061 7474 7269 6275 7465 2e0d 0a20  ed attribute... 
+000026e0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000026f0: 2041 7267 733a 200d 0a20 2020 2020 2020   Args: ..       
+00002700: 2020 2020 2064 6174 6173 6574 2028 7064       dataset (pd
+00002710: 2e44 6174 6146 7261 6d65 293a 2064 6174  .DataFrame): dat
+00002720: 6173 6574 2074 6f20 6d69 7469 6761 7465  aset to mitigate
+00002730: 2c20 7468 6174 2069 6e63 6c75 6465 7320  , that includes 
+00002740: 7468 6520 7461 7267 6574 2063 6f6c 756d  the target colum
+00002750: 6e2e 0d0a 2020 2020 2020 2020 2020 2020  n...            
+00002760: 7461 7267 6574 2028 7374 7229 3a20 7468  target (str): th
+00002770: 6520 7461 7267 6574 2063 6f6c 756d 6e20  e target column 
+00002780: 6e61 6d65 0d0a 2020 2020 2020 2020 2020  name..          
+00002790: 2020 7072 6f74 6563 7465 645f 6174 7472    protected_attr
+000027a0: 6962 7574 6573 2028 6c69 7374 2c20 6f70  ibutes (list, op
+000027b0: 7469 6f6e 616c 293a 2054 6865 2061 7474  tional): The att
+000027c0: 7269 6275 7465 2873 2920 746f 2062 616c  ribute(s) to bal
+000027d0: 616e 6365 2e20 4465 6661 756c 7473 2074  ance. Defaults t
+000027e0: 6f20 4e6f 6e65 2e0d 0a20 2020 2020 2020  o None...       
+000027f0: 2020 2020 2063 6f6e 745f 636f 6c75 6d6e       cont_column
+00002800: 7320 286c 6973 742c 206f 7074 696f 6e61  s (list, optiona
+00002810: 6c29 3a20 5468 6520 636f 6e74 696e 756f  l): The continuo
+00002820: 7573 2063 6f6c 756d 6e73 2069 6e20 7468  us columns in th
+00002830: 6520 6461 7461 7365 742e 204f 6e6c 7920  e dataset. Only 
+00002840: 4e65 6365 7373 6172 7920 6966 2074 6865  Necessary if the
+00002850: 2073 616d 706c 696e 6720 7374 7261 7465   sampling strate
+00002860: 6779 2069 7320 534d 4f54 454e 432e 2044  gy is SMOTENC. D
+00002870: 6566 6175 6c74 7320 746f 204e 6f6e 652e  efaults to None.
+00002880: 0d0a 2020 2020 2020 2020 2020 2020 6361  ..            ca
+00002890: 745f 636f 6c75 6d6e 7320 286c 6973 742c  t_columns (list,
+000028a0: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+000028b0: 6361 7465 676f 7269 6361 6c20 636f 6c75  categorical colu
+000028c0: 6d6e 7320 696e 2074 6865 2064 6174 6173  mns in the datas
+000028d0: 6574 2e20 4f6e 6c79 204e 6563 6573 7361  et. Only Necessa
+000028e0: 7279 2069 6620 7468 6520 7361 6d70 6c69  ry if the sampli
+000028f0: 6e67 2073 7472 6174 6567 7920 6973 2053  ng strategy is S
+00002900: 4d4f 5445 4e43 2e20 4465 6661 756c 7473  MOTENC. Defaults
+00002910: 2074 6f20 4e6f 6e65 2e0d 0a0d 0a20 2020   to None.....   
+00002920: 2020 2020 2052 6574 7572 6e73 3a0d 0a20       Returns:.. 
+00002930: 2020 2020 2020 2020 2020 2028 5b70 642e             ([pd.
+00002940: 4461 7461 4672 616d 652c 2070 642e 4461  DataFrame, pd.Da
+00002950: 7461 4672 616d 655d 293a 2074 6865 2062  taFrame]): the b
+00002960: 616c 616e 6365 6420 6461 7461 6672 616d  alanced datafram
+00002970: 6573 2066 6f72 2074 6865 2064 6174 6173  es for the datas
+00002980: 6574 2061 6e64 2074 6865 2074 6172 6765  et and the targe
+00002990: 740d 0a20 2020 2020 2020 2022 2222 0d0a  t..        """..
+000029a0: 0d0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
+000029b0: 292e 5f73 616e 6974 795f 6368 6563 6b28  )._sanity_check(
+000029c0: 6461 7461 7365 742c 2074 6172 6765 742c  dataset, target,
+000029d0: 2070 726f 7465 6374 6564 5f61 7474 7269   protected_attri
+000029e0: 6275 7465 733d 7072 6f74 6563 7465 645f  butes=protected_
+000029f0: 6174 7472 6962 7574 6573 290d 0a20 2020  attributes)..   
+00002a00: 2020 2020 2064 6620 3d20 6461 7461 7365       df = datase
+00002a10: 742e 636f 7079 2829 0d0a 0d0a 2020 2020  t.copy()....    
+00002a20: 2020 2020 0d0a 2020 2020 2020 2020 6966      ..        if
+00002a30: 206c 656e 2870 726f 7465 6374 6564 5f61   len(protected_a
+00002a40: 7474 7269 6275 7465 7329 203e 2031 203a  ttributes) > 1 :
+00002a50: 0d0a 2020 2020 2020 2020 2020 2020 6466  ..            df
+00002a60: 2c20 7072 6f74 6563 7465 645f 6174 7472  , protected_attr
+00002a70: 6962 7574 6520 3d20 7365 6c66 2e5f 6d61  ibute = self._ma
+00002a80: 6b65 5f73 7570 6572 5f70 726f 7465 6374  ke_super_protect
+00002a90: 6564 2864 6174 6173 6574 2c20 7072 6f74  ed(dataset, prot
+00002aa0: 6563 7465 645f 6174 7472 6962 7574 6573  ected_attributes
+00002ab0: 290d 0a20 2020 2020 2020 2065 6c73 6520  )..        else 
+00002ac0: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+00002ad0: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
+00002ae0: 7465 203d 2070 726f 7465 6374 6564 5f61  te = protected_a
+00002af0: 7474 7269 6275 7465 735b 305d 0d0a 2020  ttributes[0]..  
+00002b00: 2020 0d0a 2020 2020 2020 2020 636c 6173    ..        clas
+00002b10: 7365 7320 3d20 6c69 7374 2864 665b 7072  ses = list(df[pr
+00002b20: 6f74 6563 7465 645f 6174 7472 6962 7574  otected_attribut
+00002b30: 655d 2e75 6e69 7175 6528 2929 0d0a 2020  e].unique())..  
+00002b40: 2020 2020 2020 722c 206d 6178 5f63 6c61        r, max_cla
+00002b50: 7373 203d 2073 656c 662e 5f68 6967 6865  ss = self._highe
+00002b60: 7374 5f72 6174 696f 2864 662c 2074 6172  st_ratio(df, tar
+00002b70: 6765 742c 2063 6c61 7373 6573 2c20 7072  get, classes, pr
+00002b80: 6f74 6563 7465 645f 6174 7472 6962 7574  otected_attribut
+00002b90: 6529 0d0a 2020 2020 2020 2020 0d0a 2020  e)..        ..  
+00002ba0: 2020 2020 2020 666f 7220 6320 696e 2063        for c in c
+00002bb0: 6c61 7373 6573 203a 0d0a 2020 2020 2020  lasses :..      
+00002bc0: 2020 2020 2020 6966 2063 2021 3d20 6d61        if c != ma
+00002bd0: 785f 636c 6173 7320 3a0d 0a20 2020 2020  x_class :..     
+00002be0: 2020 2020 2020 2020 2020 2023 206b 6565             # kee
+00002bf0: 7020 6f6e 6c79 2074 6865 2072 6f77 7320  p only the rows 
+00002c00: 7769 7468 2067 6976 656e 2063 6c61 7373  with given class
+00002c10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002c20: 2020 636c 6173 735f 6466 203d 2064 665b    class_df = df[
+00002c30: 6466 5b70 726f 7465 6374 6564 5f61 7474  df[protected_att
+00002c40: 7269 6275 7465 5d20 3d3d 2063 5d0d 0a20  ribute] == c].. 
+00002c50: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00002c60: 6c61 7373 5f74 6172 6765 7420 3d20 636c  lass_target = cl
+00002c70: 6173 735f 6466 5b74 6172 6765 745d 0d0a  ass_df[target]..
+00002c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c90: 636c 6173 735f 6466 203d 2063 6c61 7373  class_df = class
+00002ca0: 5f64 662e 6472 6f70 2863 6f6c 756d 6e73  _df.drop(columns
+00002cb0: 3d5b 7461 7267 6574 5d29 0d0a 2020 2020  =[target])..    
+00002cc0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00002cd0: 2020 2020 2020 2020 2020 2320 7265 7361            # resa
+00002ce0: 6d70 6c65 2074 6865 2074 6172 6765 7420  mple the target 
+00002cf0: 666f 7220 7468 6973 2063 6c61 7373 0d0a  for this class..
+00002d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d10: 6966 206c 656e 286c 6973 7428 636c 6173  if len(list(clas
+00002d20: 735f 7461 7267 6574 2e75 6e69 7175 6528  s_target.unique(
+00002d30: 2929 2920 213d 2031 203a 0d0a 2020 2020  ))) != 1 :..    
+00002d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002d60: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00002d70: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00002d80: 656c 662e 6d65 7468 6f64 2069 6e20 5b22  elf.method in ["
+00002d90: 534d 4f54 454e 4322 5d20 3a0d 0a20 2020  SMOTENC"] :..   
+00002da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002db0: 2020 2020 2063 6f6e 745f 636f 6c5f 6275       cont_col_bu
+00002dc0: 6666 203d 205b 6665 6174 7572 6520 666f  ff = [feature fo
+00002dd0: 7220 6665 6174 7572 6520 696e 2063 6f6e  r feature in con
+00002de0: 745f 636f 6c75 6d6e 7320 6966 2066 6561  t_columns if fea
+00002df0: 7475 7265 2021 3d20 7072 6f74 6563 7465  ture != protecte
+00002e00: 645f 6174 7472 6962 7574 655d 0d0a 2020  d_attribute]..  
+00002e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e20: 2020 2020 2020 6361 745f 636f 6c5f 6275        cat_col_bu
+00002e30: 6666 203d 205b 6665 6174 7572 6520 666f  ff = [feature fo
+00002e40: 7220 6665 6174 7572 6520 696e 2063 6174  r feature in cat
+00002e50: 5f63 6f6c 756d 6e73 2069 6620 6665 6174  _columns if feat
+00002e60: 7572 6520 213d 2070 726f 7465 6374 6564  ure != protected
+00002e70: 5f61 7474 7269 6275 7465 5d0d 0a20 2020  _attribute]..   
+00002e80: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00002e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ea0: 2020 2023 7072 6570 726f 6365 7373 2075     #preprocess u
+00002eb0: 7369 6e67 2074 6865 2070 726f 7465 6374  sing the protect
+00002ec0: 6564 2061 7474 7269 6275 7465 2061 7320  ed attribute as 
+00002ed0: 6120 7461 7267 6574 0d0a 2020 2020 2020  a target..      
+00002ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ef0: 2020 7072 6f63 6573 736f 7220 3d20 5f50    processor = _P
+00002f00: 726f 6365 7373 6f72 2829 0d0a 2020 2020  rocessor()..    
+00002f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f20: 2020 2020 7072 6f63 6573 7365 645f 6466      processed_df
+00002f30: 203d 2070 726f 6365 7373 6f72 2e70 726f   = processor.pro
+00002f40: 6365 7373 2863 6c61 7373 5f64 662c 2073  cess(class_df, s
+00002f50: 6361 6c65 5f63 6f6c 733d 636f 6e74 5f63  cale_cols=cont_c
+00002f60: 6f6c 5f62 7566 662c 2065 6e63 6f64 655f  ol_buff, encode_
+00002f70: 636f 6c73 3d28 6361 745f 636f 6c5f 6275  cols=(cat_col_bu
+00002f80: 6666 202b 205b 7072 6f74 6563 7465 645f  ff + [protected_
+00002f90: 6174 7472 6962 7574 655d 2929 0d0a 0d0a  attribute]))....
+00002fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002fb0: 2020 2020 2020 2020 6361 745f 636f 6c75          cat_colu
+00002fc0: 6d6e 735f 6964 7320 3d20 5b70 726f 6365  mns_ids = [proce
+00002fd0: 7373 6564 5f64 662e 636f 6c75 6d6e 732e  ssed_df.columns.
+00002fe0: 6765 745f 6c6f 6328 636f 6c5f 6e61 6d65  get_loc(col_name
+00002ff0: 2920 666f 7220 636f 6c5f 6e61 6d65 2069  ) for col_name i
+00003000: 6e20 6361 745f 636f 6c75 6d6e 735d 0d0a  n cat_columns]..
+00003010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003020: 2020 2020 2020 2020 7361 6d70 6c65 7220          sampler 
+00003030: 3d20 534d 4f54 454e 4328 7361 6d70 6c69  = SMOTENC(sampli
+00003040: 6e67 5f73 7472 6174 6567 793d 722c 2063  ng_strategy=r, c
+00003050: 6174 6567 6f72 6963 616c 5f66 6561 7475  ategorical_featu
+00003060: 7265 733d 6361 745f 636f 6c75 6d6e 735f  res=cat_columns_
+00003070: 6964 7329 0d0a 2020 2020 2020 2020 2020  ids)..          
+00003080: 2020 2020 2020 2020 2020 2020 2020 585f                X_
+00003090: 7265 7361 6d70 6c65 642c 2063 6c61 7373  resampled, class
+000030a0: 5f74 6172 6765 745f 7265 7361 6d70 6c65  _target_resample
+000030b0: 6420 3d20 7361 6d70 6c65 722e 6669 745f  d = sampler.fit_
+000030c0: 7265 7361 6d70 6c65 2870 726f 6365 7373  resample(process
+000030d0: 6564 5f64 662c 2063 6c61 7373 5f74 6172  ed_df, class_tar
+000030e0: 6765 7429 0d0a 2020 2020 2020 2020 2020  get)..          
+000030f0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00003100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003110: 2020 2020 2020 2020 636c 6173 735f 7265          class_re
+00003120: 7361 6d70 6c65 6420 3d20 7072 6f63 6573  sampled = proces
+00003130: 736f 722e 756e 7072 6f63 6573 7328 585f  sor.unprocess(X_
+00003140: 7265 7361 6d70 6c65 6429 0d0a 2020 2020  resampled)..    
+00003150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003160: 2020 2020 636c 6173 735f 7265 7361 6d70      class_resamp
+00003170: 6c65 642e 6c6f 635b 3a2c 2074 6172 6765  led.loc[:, targe
+00003180: 745d 203d 2063 6c61 7373 5f74 6172 6765  t] = class_targe
+00003190: 745f 7265 7361 6d70 6c65 640d 0a20 2020  t_resampled..   
+000031a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031b0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+000031c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031d0: 2020 2065 6c69 6620 7365 6c66 2e6d 6574     elif self.met
+000031e0: 686f 6420 696e 205b 2252 616e 646f 6d4f  hod in ["RandomO
+000031f0: 7665 7253 616d 706c 6572 225d 203a 0d0a  verSampler"] :..
+00003200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003210: 2020 2020 2020 2020 7361 6d70 6c65 7220          sampler 
+00003220: 3d20 5261 6e64 6f6d 4f76 6572 5361 6d70  = RandomOverSamp
+00003230: 6c65 7228 7361 6d70 6c69 6e67 5f73 7472  ler(sampling_str
+00003240: 6174 6567 793d 7229 0d0a 2020 2020 2020  ategy=r)..      
+00003250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003260: 2020 636c 6173 735f 7265 7361 6d70 6c65    class_resample
+00003270: 642c 2063 6c61 7373 5f74 6172 6765 745f  d, class_target_
+00003280: 7265 7361 6d70 6c65 6420 3d20 7361 6d70  resampled = samp
+00003290: 6c65 722e 6669 745f 7265 7361 6d70 6c65  ler.fit_resample
+000032a0: 2863 6c61 7373 5f64 662c 2063 6c61 7373  (class_df, class
+000032b0: 5f74 6172 6765 7429 0d0a 2020 2020 2020  _target)..      
+000032c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032d0: 2020 636c 6173 735f 7265 7361 6d70 6c65    class_resample
+000032e0: 642e 6c6f 635b 3a2c 2074 6172 6765 745d  d.loc[:, target]
+000032f0: 203d 2063 6c61 7373 5f74 6172 6765 745f   = class_target_
+00003300: 7265 7361 6d70 6c65 640d 0a20 2020 2020  resampled..     
+00003310: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00003320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003330: 2020 2020 2065 6c69 6620 7365 6c66 2e6d       elif self.m
+00003340: 6574 686f 6420 696e 205b 2252 616e 646f  ethod in ["Rando
+00003350: 6d55 6e64 6572 5361 6d70 6c65 7222 5d20  mUnderSampler"] 
+00003360: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00003370: 2020 2020 2020 2020 2020 2073 616d 706c             sampl
+00003380: 6572 203d 2052 616e 646f 6d55 6e64 6572  er = RandomUnder
+00003390: 5361 6d70 6c65 7228 7361 6d70 6c69 6e67  Sampler(sampling
+000033a0: 5f73 7472 6174 6567 793d 7229 0d0a 2020  _strategy=r)..  
+000033b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033c0: 2020 2020 2020 636c 6173 735f 7265 7361        class_resa
+000033d0: 6d70 6c65 642c 2063 6c61 7373 5f74 6172  mpled, class_tar
+000033e0: 6765 745f 7265 7361 6d70 6c65 6420 3d20  get_resampled = 
+000033f0: 7361 6d70 6c65 722e 6669 745f 7265 7361  sampler.fit_resa
+00003400: 6d70 6c65 2863 6c61 7373 5f64 662c 2063  mple(class_df, c
+00003410: 6c61 7373 5f74 6172 6765 7429 0d0a 2020  lass_target)..  
+00003420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003430: 2020 2020 2020 636c 6173 735f 7265 7361        class_resa
+00003440: 6d70 6c65 642e 6c6f 635b 3a2c 2074 6172  mpled.loc[:, tar
+00003450: 6765 745d 203d 2063 6c61 7373 5f74 6172  get] = class_tar
+00003460: 6765 745f 7265 7361 6d70 6c65 6420 2020  get_resampled   
+00003470: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00003480: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00003490: 2020 2020 2020 2065 6c73 6520 3a0d 0a20         else :.. 
+000034a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034b0: 2020 2023 6966 2074 6865 7265 2069 7320     #if there is 
+000034c0: 6f6e 6c79 206f 6e65 206f 7574 7075 7420  only one output 
+000034d0: 666f 7220 7468 6520 636c 6173 732c 2074  for the class, t
+000034e0: 6865 7265 2069 7320 6e6f 2077 6179 2074  here is no way t
+000034f0: 6f20 7265 7361 6d70 6c65 2069 740d 0a20  o resample it.. 
+00003500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003510: 2020 2063 6c61 7373 5f72 6573 616d 706c     class_resampl
+00003520: 6564 203d 2063 6c61 7373 5f64 662e 636f  ed = class_df.co
+00003530: 7079 2829 0d0a 2020 2020 2020 2020 2020  py()..          
+00003540: 2020 2020 2020 2020 2020 636c 6173 735f            class_
+00003550: 7265 7361 6d70 6c65 642e 6c6f 635b 3a2c  resampled.loc[:,
+00003560: 7461 7267 6574 5d20 3d20 636c 6173 735f  target] = class_
+00003570: 7461 7267 6574 0d0a 2020 2020 2020 2020  target..        
+00003580: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00003590: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+000035a0: 6170 7065 6e64 2074 6865 2072 6573 616d  append the resam
+000035b0: 706c 6564 2063 6c61 7373 2069 6e20 6669  pled class in fi
+000035c0: 6e61 6c20 6466 0d0a 2020 2020 2020 2020  nal df..        
+000035d0: 2020 2020 2020 2020 2320 2864 726f 7020          # (drop 
+000035e0: 7468 6520 726f 7773 2077 6974 6820 7468  the rows with th
+000035f0: 6973 2063 6c61 7373 2066 6972 7374 2074  is class first t
+00003600: 6f20 6e6f 7420 6475 706c 6963 6174 6564  o not duplicated
+00003610: 2074 6865 6d29 0d0a 2020 2020 2020 2020   them)..        
+00003620: 2020 2020 2020 2020 6466 203d 2064 665b          df = df[
+00003630: 6466 5b70 726f 7465 6374 6564 5f61 7474  df[protected_att
+00003640: 7269 6275 7465 5d20 213d 2063 5d0d 0a20  ribute] != c].. 
+00003650: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00003660: 6620 3d20 7064 2e63 6f6e 6361 7428 5b64  f = pd.concat([d
+00003670: 662c 2063 6c61 7373 5f72 6573 616d 706c  f, class_resampl
+00003680: 6564 5d2c 2069 676e 6f72 655f 696e 6465  ed], ignore_inde
+00003690: 783d 5472 7565 290d 0a0d 0a0d 0a20 2020  x=True)......   
+000036a0: 2020 2020 2074 6172 6765 745f 6466 203d       target_df =
+000036b0: 2064 665b 7461 7267 6574 5d0d 0a20 2020   df[target]..   
+000036c0: 2020 2020 2064 662e 6472 6f70 2863 6f6c       df.drop(col
+000036d0: 756d 6e73 3d5b 7461 7267 6574 5d2c 2069  umns=[target], i
+000036e0: 6e70 6c61 6365 3d54 7275 6529 0d0a 2020  nplace=True)..  
+000036f0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00003700: 6966 206c 656e 2870 726f 7465 6374 6564  if len(protected
+00003710: 5f61 7474 7269 6275 7465 7329 203e 2031  _attributes) > 1
+00003720: 203a 0d0a 2020 2020 2020 2020 2020 2020   :..            
+00003730: 6466 203d 2064 662e 6472 6f70 2863 6f6c  df = df.drop(col
+00003740: 756d 6e73 203d 2070 726f 7465 6374 6564  umns = protected
+00003750: 5f61 7474 7269 6275 7465 290d 0a20 2020  _attribute)..   
+00003760: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00003770: 2020 2020 2072 6574 7572 6e20 6466 2c20       return df, 
+00003780: 7461 7267 6574 5f64 660d 0a20 2020 200d  target_df..    .
+00003790: 0a20 2020 2064 6566 2062 616c 616e 6365  .    def balance
+000037a0: 5f61 6c6c 2873 656c 662c 2064 6174 6173  _all(self, datas
+000037b0: 6574 3a20 7064 2e44 6174 6146 7261 6d65  et: pd.DataFrame
+000037c0: 2c20 7461 7267 6574 3a20 7374 722c 2070  , target: str, p
+000037d0: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
+000037e0: 7465 733a 206c 6973 742c 200d 0a20 2020  tes: list, ..   
+000037f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003800: 2063 6f6e 745f 636f 6c75 6d6e 733a 206c   cont_columns: l
+00003810: 6973 7420 3d20 4e6f 6e65 2c20 6361 745f  ist = None, cat_
+00003820: 636f 6c75 6d6e 733a 206c 6973 7420 3d20  columns: list = 
+00003830: 4e6f 6e65 2920 3a0d 0a20 2020 2020 2020  None) :..       
+00003840: 2022 2222 0d0a 2020 2020 2020 2020 4669   """..        Fi
+00003850: 7273 7420 6261 6c61 6e63 6573 2074 6865  rst balances the
+00003860: 2070 726f 7465 6374 6564 2061 7474 7269   protected attri
+00003870: 6275 7465 2873 292c 2061 6e64 2074 6865  bute(s), and the
+00003880: 6e20 6261 6c61 6e63 6520 7468 6569 7220  n balance their 
+00003890: 6f75 7470 7574 2e20 4769 7665 7320 616e  output. Gives an
+000038a0: 2061 6c6d 6f73 7420 7065 7266 6563 746c   almost perfectl
+000038b0: 7920 6261 6c61 6e63 6564 2064 6174 6173  y balanced datas
+000038c0: 6574 2066 6f72 2074 6865 2070 726f 7465  et for the prote
+000038d0: 6374 6564 2061 7474 7269 6275 7465 2873  cted attribute(s
+000038e0: 292e 0d0a 0d0a 2020 2020 2020 2020 4172  ).....        Ar
+000038f0: 6773 3a20 0d0a 2020 2020 2020 2020 2020  gs: ..          
+00003900: 2020 6461 7461 7365 7420 2870 642e 4461    dataset (pd.Da
+00003910: 7461 4672 616d 6529 3a20 6461 7461 7365  taFrame): datase
+00003920: 7420 746f 206d 6974 6967 6174 652c 2074  t to mitigate, t
+00003930: 6861 7420 696e 636c 7564 6573 2074 6865  hat includes the
+00003940: 2074 6172 6765 7420 636f 6c75 6d6e 2e0d   target column..
+00003950: 0a20 2020 2020 2020 2020 2020 2074 6172  .            tar
+00003960: 6765 7420 2873 7472 293a 2074 6865 2074  get (str): the t
+00003970: 6172 6765 7420 636f 6c75 6d6e 206e 616d  arget column nam
+00003980: 650d 0a20 2020 2020 2020 2020 2020 2070  e..            p
+00003990: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
+000039a0: 7465 7320 286c 6973 742c 206f 7074 696f  tes (list, optio
+000039b0: 6e61 6c29 3a20 5468 6520 6174 7472 6962  nal): The attrib
+000039c0: 7574 6528 7329 2074 6f20 6261 6c61 6e63  ute(s) to balanc
+000039d0: 652e 2044 6566 6175 6c74 7320 746f 204e  e. Defaults to N
+000039e0: 6f6e 652e 0d0a 2020 2020 2020 2020 2020  one...          
+000039f0: 2020 636f 6e74 5f63 6f6c 756d 6e73 2028    cont_columns (
+00003a00: 6c69 7374 2c20 6f70 7469 6f6e 616c 293a  list, optional):
+00003a10: 2054 6865 2063 6f6e 7469 6e75 6f75 7320   The continuous 
+00003a20: 636f 6c75 6d6e 7320 696e 2074 6865 2064  columns in the d
+00003a30: 6174 6173 6574 2e20 4f6e 6c79 204e 6563  ataset. Only Nec
+00003a40: 6573 7361 7279 2069 6620 7468 6520 7361  essary if the sa
+00003a50: 6d70 6c69 6e67 2073 7472 6174 6567 7920  mpling strategy 
+00003a60: 6973 2053 4d4f 5445 4e43 2e20 4465 6661  is SMOTENC. Defa
+00003a70: 756c 7473 2074 6f20 4e6f 6e65 2e0d 0a20  ults to None... 
+00003a80: 2020 2020 2020 2020 2020 2063 6174 5f63             cat_c
+00003a90: 6f6c 756d 6e73 2028 6c69 7374 2c20 6f70  olumns (list, op
+00003aa0: 7469 6f6e 616c 293a 2054 6865 2063 6174  tional): The cat
+00003ab0: 6567 6f72 6963 616c 2063 6f6c 756d 6e73  egorical columns
+00003ac0: 2069 6e20 7468 6520 6461 7461 7365 742e   in the dataset.
+00003ad0: 204f 6e6c 7920 4e65 6365 7373 6172 7920   Only Necessary 
+00003ae0: 6966 2074 6865 2073 616d 706c 696e 6720  if the sampling 
+00003af0: 7374 7261 7465 6779 2069 7320 534d 4f54  strategy is SMOT
+00003b00: 454e 432e 2044 6566 6175 6c74 7320 746f  ENC. Defaults to
+00003b10: 204e 6f6e 652e 0d0a 0d0a 2020 2020 2020   None.....      
+00003b20: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
+00003b30: 2020 2020 2020 2020 285b 7064 2e44 6174          ([pd.Dat
+00003b40: 6146 7261 6d65 2c20 7064 2e44 6174 6146  aFrame, pd.DataF
+00003b50: 7261 6d65 5d29 3a20 7468 6520 6261 6c61  rame]): the bala
+00003b60: 6e63 6564 2064 6174 6166 7261 6d65 7320  nced dataframes 
+00003b70: 666f 7220 7468 6520 6461 7461 7365 7420  for the dataset 
+00003b80: 616e 6420 7468 6520 7461 7267 6574 0d0a  and the target..
+00003b90: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00003ba0: 2020 2020 2064 662c 2074 203d 2073 656c       df, t = sel
+00003bb0: 662e 6261 6c61 6e63 655f 7072 6f74 6563  f.balance_protec
+00003bc0: 7465 645f 6174 7472 6962 7574 6528 6461  ted_attribute(da
+00003bd0: 7461 7365 742c 2074 6172 6765 742c 2070  taset, target, p
+00003be0: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
+00003bf0: 7465 732c 2063 6f6e 745f 636f 6c75 6d6e  tes, cont_column
+00003c00: 732c 2063 6174 5f63 6f6c 756d 6e73 2920  s, cat_columns) 
+00003c10: 0d0a 2020 2020 2020 2020 6466 2e6c 6f63  ..        df.loc
+00003c20: 5b3a 2c20 7461 7267 6574 5d20 3d20 740d  [:, target] = t.
+00003c30: 0a20 2020 2020 2020 2064 662c 2074 203d  .        df, t =
+00003c40: 2073 656c 662e 6261 6c61 6e63 655f 6f75   self.balance_ou
+00003c50: 7470 7574 5f66 6f72 5f61 7474 7269 6275  tput_for_attribu
+00003c60: 7465 2864 662c 2074 6172 6765 742c 2070  te(df, target, p
+00003c70: 726f 7465 6374 6564 5f61 7474 7269 6275  rotected_attribu
+00003c80: 7465 732c 2063 6f6e 745f 636f 6c75 6d6e  tes, cont_column
+00003c90: 732c 2063 6174 5f63 6f6c 756d 6e73 290d  s, cat_columns).
+00003ca0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00003cb0: 2020 2072 6574 7572 6e20 6466 2c20 7420     return df, t 
+00003cc0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00003cd0: 200d 0a20 2020 2020 2020 2020 2020 200d   ..            .
+00003ce0: 0a20 2020 2064 6566 205f 6869 6768 6573  .    def _highes
+00003cf0: 745f 7261 7469 6f28 7365 6c66 2c20 6461  t_ratio(self, da
+00003d00: 7461 7365 743a 2070 642e 4461 7461 4672  taset: pd.DataFr
+00003d10: 616d 652c 2074 6172 6765 743a 2073 7472  ame, target: str
+00003d20: 2c20 636c 6173 7365 733a 2064 6963 742c  , classes: dict,
+00003d30: 2070 726f 7465 6374 6564 5f61 7474 7269   protected_attri
+00003d40: 6275 7465 3a20 7374 7229 203a 0d0a 2020  bute: str) :..  
+00003d50: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00003d60: 2020 2047 6976 6520 7468 6520 6869 6768     Give the high
+00003d70: 6573 7420 7261 7469 6f20 6f66 2070 6f73  est ratio of pos
+00003d80: 6974 6976 6520 6f75 7470 7574 206f 6e20  itive output on 
+00003d90: 6e65 6761 7469 7665 206f 7574 7075 7420  negative output 
+00003da0: 6f66 2061 6c6c 2074 6865 2063 6c61 7373  of all the class
+00003db0: 6573 206f 6620 7468 6520 7072 6f74 6563  es of the protec
+00003dc0: 7465 6420 6174 7472 6962 7574 652e 204e  ted attribute. N
+00003dd0: 6563 6573 7361 7279 2066 6f72 2062 616c  ecessary for bal
+00003de0: 616e 6365 5f6f 7574 7075 745f 666f 725f  ance_output_for_
+00003df0: 6174 7472 6962 7574 652e 0d0a 0d0a 2020  attribute.....  
+00003e00: 2020 2020 2020 4172 6773 3a0d 0a20 2020        Args:..   
+00003e10: 2020 2020 2020 2020 2064 6174 6173 6574           dataset
+00003e20: 2028 7064 2e44 6174 6146 7261 6d65 293a   (pd.DataFrame):
+00003e30: 2064 6174 6173 6574 2074 6f20 6d69 7469   dataset to miti
+00003e40: 6761 7465 2c20 7468 6174 2069 6e63 6c75  gate, that inclu
+00003e50: 6465 7320 7468 6520 7461 7267 6574 2063  des the target c
+00003e60: 6f6c 756d 6e2e 0d0a 2020 2020 2020 2020  olumn...        
+00003e70: 2020 2020 7461 7267 6574 2028 7374 7229      target (str)
+00003e80: 3a20 7468 6520 7461 7267 6574 2063 6f6c  : the target col
+00003e90: 756d 6e20 6e61 6d65 0d0a 2020 2020 2020  umn name..      
+00003ea0: 2020 2020 2020 636c 6173 7365 7320 2864        classes (d
+00003eb0: 6963 7429 3a20 7468 6520 636c 6173 7365  ict): the classe
+00003ec0: 7320 6f66 2074 6865 2070 726f 7465 6374  s of the protect
+00003ed0: 6564 2061 7474 7269 6275 7465 0d0a 2020  ed attribute..  
+00003ee0: 2020 2020 2020 2020 2020 7072 6f74 6563            protec
+00003ef0: 7465 645f 6174 7472 6962 7574 6520 2873  ted_attribute (s
+00003f00: 7472 293a 2074 6865 2070 726f 7465 6374  tr): the protect
+00003f10: 6564 2061 7474 7269 6275 7465 2074 6f20  ed attribute to 
+00003f20: 6361 6c63 756c 6174 6520 7468 6520 6869  calculate the hi
+00003f30: 6768 6573 7420 7261 7469 6f20 666f 722e  ghest ratio for.
+00003f40: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
+00003f50: 726e 733a 0d0a 2020 2020 2020 2020 2020  rns:..          
+00003f60: 2020 285b 666c 6f61 742c 2073 7472 5d29    ([float, str])
+00003f70: 3a20 7468 6520 6869 6768 6573 7420 7261  : the highest ra
+00003f80: 7469 6f20 616e 6420 7468 6520 6173 736f  tio and the asso
+00003f90: 6369 6174 6564 2063 6c61 7373 0d0a 2020  ciated class..  
+00003fa0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00003fb0: 2020 200d 0a20 2020 2020 2020 2072 5f6d     ..        r_m
+00003fc0: 6178 203d 2030 0d0a 2020 2020 2020 2020  ax = 0..        
+00003fd0: 635f 6d61 7820 3d20 636c 6173 7365 735b  c_max = classes[
+00003fe0: 305d 0d0a 2020 2020 2020 2020 666f 7220  0]..        for 
+00003ff0: 6320 696e 2063 6c61 7373 6573 203a 0d0a  c in classes :..
+00004000: 2020 2020 2020 2020 2020 2020 7220 3d20              r = 
+00004010: 6461 7461 7365 745b 6461 7461 7365 745b  dataset[dataset[
+00004020: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
+00004030: 7574 655d 203d 3d20 635d 5b74 6172 6765  ute] == c][targe
+00004040: 745d 2e76 616c 7565 5f63 6f75 6e74 7328  t].value_counts(
+00004050: 295b 315d 2f64 6174 6173 6574 5b64 6174  )[1]/dataset[dat
+00004060: 6173 6574 5b70 726f 7465 6374 6564 5f61  aset[protected_a
+00004070: 7474 7269 6275 7465 5d20 3d3d 2063 5d5b  ttribute] == c][
+00004080: 7461 7267 6574 5d2e 7661 6c75 655f 636f  target].value_co
+00004090: 756e 7473 2829 5b30 5d0d 0a20 2020 2020  unts()[0]..     
+000040a0: 2020 2020 2020 2069 6620 7220 3e20 3120         if r > 1 
+000040b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000040c0: 2020 2072 203d 2031 2f72 0d0a 2020 2020     r = 1/r..    
+000040d0: 2020 2020 2020 2020 6966 2072 203e 2072          if r > r
+000040e0: 5f6d 6178 203a 0d0a 2020 2020 2020 2020  _max :..        
+000040f0: 2020 2020 2020 2020 725f 6d61 7820 3d20          r_max = 
+00004100: 720d 0a20 2020 2020 2020 2020 2020 2020  r..             
+00004110: 2020 2063 5f6d 6178 203d 2063 0d0a 2020     c_max = c..  
+00004120: 2020 2020 2020 7265 7475 726e 2072 5f6d        return r_m
+00004130: 6178 2c20 635f 6d61 780d 0a20 2020 0d0a  ax, c_max..   ..
+00004140: 2020 200d 0a20 2020 2064 6566 205f 6d61     ..    def _ma
+00004150: 6b65 5f73 7570 6572 5f70 726f 7465 6374  ke_super_protect
+00004160: 6564 2873 656c 662c 2064 6174 6173 6574  ed(self, dataset
+00004170: 3a20 7064 2e44 6174 6146 7261 6d65 2c20  : pd.DataFrame, 
+00004180: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
+00004190: 7574 6573 3a20 6c69 7374 2920 3a0d 0a20  utes: list) :.. 
+000041a0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+000041b0: 2020 2020 4d61 6b65 2061 2073 7570 6572      Make a super
+000041c0: 2070 726f 7465 6374 6564 2061 7474 7269   protected attri
+000041d0: 6275 7465 2074 6861 7420 6973 2074 6865  bute that is the
+000041e0: 2063 6f6d 6269 6e61 7469 6f6e 206f 6620   combination of 
+000041f0: 616c 6c20 6769 7665 6e20 7072 6f74 6563  all given protec
+00004200: 7465 6420 6174 7472 6962 7574 6573 2063  ted attributes c
+00004210: 616c 6c65 6420 2270 726f 7465 6374 6564  alled "protected
+00004220: 5f73 7570 6572 636c 6173 7322 0d0a 0d0a  _superclass"....
+00004230: 2020 2020 2020 2020 4172 6773 3a0d 0a20          Args:.. 
+00004240: 2020 2020 2020 2020 2020 2064 6174 6173             datas
+00004250: 6574 2028 7064 2e44 6174 6146 7261 6d65  et (pd.DataFrame
+00004260: 293a 2064 6174 6173 6574 2074 6f20 6d69  ): dataset to mi
+00004270: 7469 6761 7465 2c20 7468 6174 2069 6e63  tigate, that inc
+00004280: 6c75 6465 7320 7468 6520 7461 7267 6574  ludes the target
+00004290: 2063 6f6c 756d 6e2e 0d0a 2020 2020 2020   column...      
+000042a0: 2020 2020 2020 7072 6f74 6563 7465 645f        protected_
+000042b0: 6174 7472 6962 7574 6573 2028 6c69 7374  attributes (list
+000042c0: 293a 2070 726f 7465 6374 6564 2061 7474  ): protected att
+000042d0: 7269 6275 7465 7320 746f 2063 6f6d 6269  ributes to combi
+000042e0: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
+000042f0: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00004300: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00004310: 285b 7064 2e44 6174 6146 7261 6d65 2c20  ([pd.DataFrame, 
+00004320: 7374 725d 293a 2074 6865 2074 7261 6e73  str]): the trans
+00004330: 666f 726d 6564 2064 6174 6173 6574 2061  formed dataset a
+00004340: 6e64 2074 6865 206e 616d 6520 2273 7570  nd the name "sup
+00004350: 6572 2070 726f 7465 6374 6564 2220 636f  er protected" co
+00004360: 6c75 6d6e 0d0a 2020 2020 2020 2020 2222  lumn..        ""
+00004370: 220d 0a0d 0a20 2020 2020 2020 2064 6620  "....        df 
+00004380: 3d20 6461 7461 7365 742e 636f 7079 2829  = dataset.copy()
+00004390: 0d0a 2020 2020 2020 2020 7375 7065 7270  ..        superp
+000043a0: 726f 7465 6374 6564 5f63 6f6c 756d 6e20  rotected_column 
+000043b0: 3d20 6675 6e63 746f 6f6c 732e 7265 6475  = functools.redu
+000043c0: 6365 286c 616d 6264 6120 612c 2062 203a  ce(lambda a, b :
+000043d0: 2061 202b 2022 5f22 202b 2062 2c20 7072   a + "_" + b, pr
+000043e0: 6f74 6563 7465 645f 6174 7472 6962 7574  otected_attribut
+000043f0: 6573 290d 0a20 2020 2020 2020 2064 665b  es)..        df[
+00004400: 7375 7065 7270 726f 7465 6374 6564 5f63  superprotected_c
+00004410: 6f6c 756d 6e5d 203d 2022 220d 0a20 2020  olumn] = ""..   
+00004420: 2020 2020 2066 6f72 2070 726f 7465 6374       for protect
+00004430: 6564 5f61 7474 7269 6275 7465 2069 6e20  ed_attribute in 
+00004440: 7072 6f74 6563 7465 645f 6174 7472 6962  protected_attrib
+00004450: 7574 6573 203a 0d0a 0d0a 2020 2020 2020  utes :....      
+00004460: 2020 2020 2020 6466 5b73 7570 6572 7072        df[superpr
+00004470: 6f74 6563 7465 645f 636f 6c75 6d6e 5d20  otected_column] 
+00004480: 2b3d 2064 665b 7072 6f74 6563 7465 645f  += df[protected_
+00004490: 6174 7472 6962 7574 655d 2e61 7070 6c79  attribute].apply
+000044a0: 2873 7472 2920 202b 2022 5f22 0d0a 2020  (str)  + "_"..  
+000044b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044c0: 2020 2020 200d 0a20 2020 2020 2020 2064       ..        d
+000044d0: 665b 7375 7065 7270 726f 7465 6374 6564  f[superprotected
+000044e0: 5f63 6f6c 756d 6e5d 203d 2064 665b 7375  _column] = df[su
+000044f0: 7065 7270 726f 7465 6374 6564 5f63 6f6c  perprotected_col
+00004500: 756d 6e5d 2e61 7070 6c79 286c 616d 6264  umn].apply(lambd
+00004510: 6120 7820 3a20 785b 3a2d 315d 290d 0a20  a x : x[:-1]).. 
+00004520: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00004530: 200d 0a20 2020 2020 2020 2072 6574 7572   ..        retur
+00004540: 6e20 6466 2c20 7375 7065 7270 726f 7465  n df, superprote
+00004550: 6374 6564 5f63 6f6c 756d 6e0d 0a         cted_column..
```

### Comparing `fairbalance-0.1.3/fairbalance/tools/_processor.py` & `fairbalance-0.1.4/fairbalance/tools/_processor.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.3/fairbalance/tools/_utils.py` & `fairbalance-0.1.4/fairbalance/tools/_utils.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.3/fairbalance/tools/tests/test_fairness_analysis.py` & `fairbalance-0.1.4/fairbalance/tools/tests/test_fairness_analysis.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.3/fairbalance.egg-info/PKG-INFO` & `fairbalance-0.1.4/fairbalance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairbalance
-Version: 0.1.3
+Version: 0.1.4
 Summary: bias mitigation by balancing target and/or protected attributes using resampling techniques
 Author: Pierre-Antoine Lequeu @ Fujitsu Luxembourg
 Author-email: pierre-antoine.lequeu@fujitsu.com
 Description-Content-Type: text/markdown
 Requires-Dist: folktables>=0.0.12
 Requires-Dist: imbalanced_learn==0.9.1
 Requires-Dist: numpy>=1.24.3
```

### Comparing `fairbalance-0.1.3/fairbalance.egg-info/SOURCES.txt` & `fairbalance-0.1.4/fairbalance.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 .gitignore
 README.md
 requirements.txt
 setup.py
+docs/basics/test.ipynb
 fairbalance/__init__.py
+fairbalance/all_test.ipynb
 fairbalance.egg-info/PKG-INFO
 fairbalance.egg-info/SOURCES.txt
 fairbalance.egg-info/dependency_links.txt
 fairbalance.egg-info/requires.txt
 fairbalance.egg-info/top_level.txt
 fairbalance/datasets/__init__.py
 fairbalance/datasets/_datasets_loader.py
```

### Comparing `fairbalance-0.1.3/setup.py` & `fairbalance-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "fairbalance",
-    version = "0.1.3",
+    version = "0.1.4",
     author = "Pierre-Antoine Lequeu @ Fujitsu Luxembourg",
     author_email = "pierre-antoine.lequeu@fujitsu.com",
     description = "bias mitigation by balancing target and/or protected attributes using resampling techniques",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     packages = setuptools.find_packages(),
     install_requires=[
```

