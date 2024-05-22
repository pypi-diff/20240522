# Comparing `tmp/fairbalance-0.1.4.tar.gz` & `tmp/fairbalance-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairbalance-0.1.4.tar", last modified: Wed May 22 09:00:26 2024, max compression
+gzip compressed data, was "fairbalance-0.1.5.tar", last modified: Wed May 22 09:16:00 2024, max compression
```

## Comparing `fairbalance-0.1.4.tar` & `fairbalance-0.1.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 09:00:26.473031 fairbalance-0.1.4/
--rw-rw-rw-   0        0        0      285 2024-05-21 09:43:17.000000 fairbalance-0.1.4/.gitignore
--rw-rw-rw-   0        0        0      602 2024-05-22 09:00:26.454700 fairbalance-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       92 2024-05-17 12:00:14.000000 fairbalance-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 09:00:25.734493 fairbalance-0.1.4/docs/
-drwxrwxrwx   0        0        0        0 2024-05-22 09:00:25.835160 fairbalance-0.1.4/docs/basics/
--rw-rw-rw-   0        0        0     1785 2024-05-21 09:06:34.000000 fairbalance-0.1.4/docs/basics/test.ipynb
-drwxrwxrwx   0        0        0        0 2024-05-22 09:00:25.873372 fairbalance-0.1.4/fairbalance/
--rw-rw-rw-   0        0        0       40 2024-05-22 08:39:56.000000 fairbalance-0.1.4/fairbalance/__init__.py
--rw-rw-rw-   0        0        0    12167 2024-05-21 13:36:53.000000 fairbalance-0.1.4/fairbalance/all_test.ipynb
-drwxrwxrwx   0        0        0        0 2024-05-22 09:00:25.987337 fairbalance-0.1.4/fairbalance/datasets/
--rw-rw-rw-   0        0        0      308 2024-05-16 13:58:22.000000 fairbalance-0.1.4/fairbalance/datasets/__init__.py
--rw-rw-rw-   0        0        0    11642 2024-05-22 08:59:05.000000 fairbalance-0.1.4/fairbalance/datasets/_datasets_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:00:26.005241 fairbalance-0.1.4/fairbalance/datasets/tests/
--rw-rw-rw-   0        0        0        0 2024-05-16 13:59:33.000000 fairbalance-0.1.4/fairbalance/datasets/tests/test_datasets_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:00:26.069573 fairbalance-0.1.4/fairbalance/metrics/
--rw-rw-rw-   0        0        0      377 2024-05-22 08:18:14.000000 fairbalance-0.1.4/fairbalance/metrics/__init__.py
--rw-rw-rw-   0        0        0    10470 2024-05-22 08:34:41.000000 fairbalance-0.1.4/fairbalance/metrics/_dataset_metrics.py
--rw-rw-rw-   0        0        0    12289 2024-05-22 08:34:39.000000 fairbalance-0.1.4/fairbalance/metrics/_fairness_analysis.py
--rw-rw-rw-   0        0        0     2851 2024-05-22 08:34:40.000000 fairbalance-0.1.4/fairbalance/metrics/_model_metrics.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:00:26.136612 fairbalance-0.1.4/fairbalance/metrics/tests/
--rw-rw-rw-   0        0        0        0 2024-05-15 13:38:19.000000 fairbalance-0.1.4/fairbalance/metrics/tests/__init__.py
--rw-rw-rw-   0        0        0      652 2024-05-21 09:26:17.000000 fairbalance-0.1.4/fairbalance/metrics/tests/test_dataset_metrics.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:38:54.000000 fairbalance-0.1.4/fairbalance/metrics/tests/test_model_metrics.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:00:26.185904 fairbalance-0.1.4/fairbalance/mitigation_strategies/
--rw-rw-rw-   0        0        0      324 2024-05-21 13:42:52.000000 fairbalance-0.1.4/fairbalance/mitigation_strategies/__init__.py
--rw-rw-rw-   0        0        0     8612 2024-05-22 08:34:47.000000 fairbalance-0.1.4/fairbalance/mitigation_strategies/_mitigation_strategies.py
--rw-rw-rw-   0        0        0     4763 2024-05-22 08:34:51.000000 fairbalance-0.1.4/fairbalance/mitigation_strategies/base.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:00:26.242326 fairbalance-0.1.4/fairbalance/processors/
--rw-rw-rw-   0        0        0      329 2024-05-21 14:45:40.000000 fairbalance-0.1.4/fairbalance/processors/__init__.py
--rw-rw-rw-   0        0        0     3089 2024-05-22 07:49:24.000000 fairbalance-0.1.4/fairbalance/processors/_processors.py
--rw-rw-rw-   0        0        0     8327 2024-05-22 08:34:34.000000 fairbalance-0.1.4/fairbalance/processors/base.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:00:26.345212 fairbalance-0.1.4/fairbalance/tools/
--rw-rw-rw-   0        0        0      605 2024-05-21 13:28:32.000000 fairbalance-0.1.4/fairbalance/tools/__init__.py
--rw-rw-rw-   0        0        0    10474 2024-05-17 08:27:03.000000 fairbalance-0.1.4/fairbalance/tools/_fairness_analysis.py
--rw-rw-rw-   0        0        0    17757 2024-05-21 15:06:52.000000 fairbalance-0.1.4/fairbalance/tools/_mitigator.py
--rw-rw-rw-   0        0        0    10322 2024-05-21 13:01:40.000000 fairbalance-0.1.4/fairbalance/tools/_processor.py
--rw-rw-rw-   0        0        0     2115 2024-05-21 07:39:27.000000 fairbalance-0.1.4/fairbalance/tools/_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:00:26.431312 fairbalance-0.1.4/fairbalance/tools/tests/
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:11.000000 fairbalance-0.1.4/fairbalance/tools/tests/__init__.py
--rw-rw-rw-   0        0        0     4296 2024-05-21 09:28:03.000000 fairbalance-0.1.4/fairbalance/tools/tests/test_fairness_analysis.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:32.000000 fairbalance-0.1.4/fairbalance/tools/tests/test_mitigator.py
--rw-rw-rw-   0        0        0        0 2024-05-21 09:43:17.000000 fairbalance-0.1.4/fairbalance/tools/tests/test_processor.py
--rw-rw-rw-   0        0        0        0 2024-05-15 13:39:56.000000 fairbalance-0.1.4/fairbalance/tools/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:00:25.957954 fairbalance-0.1.4/fairbalance.egg-info/
--rw-rw-rw-   0        0        0      602 2024-05-22 09:00:22.000000 fairbalance-0.1.4/fairbalance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1329 2024-05-22 09:00:25.000000 fairbalance-0.1.4/fairbalance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 09:00:22.000000 fairbalance-0.1.4/fairbalance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-05-22 09:00:22.000000 fairbalance-0.1.4/fairbalance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-22 09:00:22.000000 fairbalance-0.1.4/fairbalance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      134 2024-05-17 11:08:16.000000 fairbalance-0.1.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 09:00:26.473031 fairbalance-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      765 2024-05-22 09:00:09.000000 fairbalance-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:16:00.976534 fairbalance-0.1.5/
+-rw-rw-rw-   0        0        0      285 2024-05-21 09:43:17.000000 fairbalance-0.1.5/.gitignore
+-rw-rw-rw-   0        0        0      602 2024-05-22 09:16:00.954967 fairbalance-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       92 2024-05-17 12:00:14.000000 fairbalance-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 09:16:00.240931 fairbalance-0.1.5/docs/
+drwxrwxrwx   0        0        0        0 2024-05-22 09:16:00.343765 fairbalance-0.1.5/docs/basics/
+-rw-rw-rw-   0        0        0     1785 2024-05-21 09:06:34.000000 fairbalance-0.1.5/docs/basics/test.ipynb
+drwxrwxrwx   0        0        0        0 2024-05-22 09:16:00.378362 fairbalance-0.1.5/fairbalance/
+-rw-rw-rw-   0        0        0       40 2024-05-22 08:39:56.000000 fairbalance-0.1.5/fairbalance/__init__.py
+-rw-rw-rw-   0        0        0    12167 2024-05-21 13:36:53.000000 fairbalance-0.1.5/fairbalance/all_test.ipynb
+drwxrwxrwx   0        0        0        0 2024-05-22 09:16:00.504262 fairbalance-0.1.5/fairbalance/datasets/
+-rw-rw-rw-   0        0        0      308 2024-05-16 13:58:22.000000 fairbalance-0.1.5/fairbalance/datasets/__init__.py
+-rw-rw-rw-   0        0        0    11937 2024-05-22 09:14:40.000000 fairbalance-0.1.5/fairbalance/datasets/_datasets_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:16:00.523243 fairbalance-0.1.5/fairbalance/datasets/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-16 13:59:33.000000 fairbalance-0.1.5/fairbalance/datasets/tests/test_datasets_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:16:00.588683 fairbalance-0.1.5/fairbalance/metrics/
+-rw-rw-rw-   0        0        0      377 2024-05-22 08:18:14.000000 fairbalance-0.1.5/fairbalance/metrics/__init__.py
+-rw-rw-rw-   0        0        0    10470 2024-05-22 08:34:41.000000 fairbalance-0.1.5/fairbalance/metrics/_dataset_metrics.py
+-rw-rw-rw-   0        0        0    12289 2024-05-22 08:34:39.000000 fairbalance-0.1.5/fairbalance/metrics/_fairness_analysis.py
+-rw-rw-rw-   0        0        0     2851 2024-05-22 08:34:40.000000 fairbalance-0.1.5/fairbalance/metrics/_model_metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:16:00.632610 fairbalance-0.1.5/fairbalance/metrics/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:38:19.000000 fairbalance-0.1.5/fairbalance/metrics/tests/__init__.py
+-rw-rw-rw-   0        0        0      652 2024-05-21 09:26:17.000000 fairbalance-0.1.5/fairbalance/metrics/tests/test_dataset_metrics.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:38:54.000000 fairbalance-0.1.5/fairbalance/metrics/tests/test_model_metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:16:00.680333 fairbalance-0.1.5/fairbalance/mitigation_strategies/
+-rw-rw-rw-   0        0        0      324 2024-05-21 13:42:52.000000 fairbalance-0.1.5/fairbalance/mitigation_strategies/__init__.py
+-rw-rw-rw-   0        0        0     8612 2024-05-22 08:34:47.000000 fairbalance-0.1.5/fairbalance/mitigation_strategies/_mitigation_strategies.py
+-rw-rw-rw-   0        0        0     4763 2024-05-22 08:34:51.000000 fairbalance-0.1.5/fairbalance/mitigation_strategies/base.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:16:00.739100 fairbalance-0.1.5/fairbalance/processors/
+-rw-rw-rw-   0        0        0      329 2024-05-21 14:45:40.000000 fairbalance-0.1.5/fairbalance/processors/__init__.py
+-rw-rw-rw-   0        0        0     3089 2024-05-22 07:49:24.000000 fairbalance-0.1.5/fairbalance/processors/_processors.py
+-rw-rw-rw-   0        0        0     8327 2024-05-22 08:34:34.000000 fairbalance-0.1.5/fairbalance/processors/base.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:16:00.863144 fairbalance-0.1.5/fairbalance/tools/
+-rw-rw-rw-   0        0        0      605 2024-05-21 13:28:32.000000 fairbalance-0.1.5/fairbalance/tools/__init__.py
+-rw-rw-rw-   0        0        0    10474 2024-05-17 08:27:03.000000 fairbalance-0.1.5/fairbalance/tools/_fairness_analysis.py
+-rw-rw-rw-   0        0        0    17757 2024-05-21 15:06:52.000000 fairbalance-0.1.5/fairbalance/tools/_mitigator.py
+-rw-rw-rw-   0        0        0    10322 2024-05-21 13:01:40.000000 fairbalance-0.1.5/fairbalance/tools/_processor.py
+-rw-rw-rw-   0        0        0     2115 2024-05-21 07:39:27.000000 fairbalance-0.1.5/fairbalance/tools/_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:16:00.941939 fairbalance-0.1.5/fairbalance/tools/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:39:11.000000 fairbalance-0.1.5/fairbalance/tools/tests/__init__.py
+-rw-rw-rw-   0        0        0     4296 2024-05-21 09:28:03.000000 fairbalance-0.1.5/fairbalance/tools/tests/test_fairness_analysis.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:39:32.000000 fairbalance-0.1.5/fairbalance/tools/tests/test_mitigator.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:43:17.000000 fairbalance-0.1.5/fairbalance/tools/tests/test_processor.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:39:56.000000 fairbalance-0.1.5/fairbalance/tools/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:16:00.473545 fairbalance-0.1.5/fairbalance.egg-info/
+-rw-rw-rw-   0        0        0      602 2024-05-22 09:15:56.000000 fairbalance-0.1.5/fairbalance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1329 2024-05-22 09:15:59.000000 fairbalance-0.1.5/fairbalance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 09:15:56.000000 fairbalance-0.1.5/fairbalance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-05-22 09:15:56.000000 fairbalance-0.1.5/fairbalance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-22 09:15:56.000000 fairbalance-0.1.5/fairbalance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2024-05-17 11:08:16.000000 fairbalance-0.1.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 09:16:00.980606 fairbalance-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      765 2024-05-22 09:15:10.000000 fairbalance-0.1.5/setup.py
```

### Comparing `fairbalance-0.1.4/PKG-INFO` & `fairbalance-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairbalance
-Version: 0.1.4
+Version: 0.1.5
 Summary: bias mitigation by balancing target and/or protected attributes using resampling techniques
 Author: Pierre-Antoine Lequeu @ Fujitsu Luxembourg
 Author-email: pierre-antoine.lequeu@fujitsu.com
 Description-Content-Type: text/markdown
 Requires-Dist: folktables>=0.0.12
 Requires-Dist: imbalanced_learn==0.9.1
 Requires-Dist: numpy>=1.24.3
```

### Comparing `fairbalance-0.1.4/docs/basics/test.ipynb` & `fairbalance-0.1.5/docs/basics/test.ipynb`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.4/fairbalance/all_test.ipynb` & `fairbalance-0.1.5/fairbalance/all_test.ipynb`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.4/fairbalance/datasets/_datasets_loader.py` & `fairbalance-0.1.5/fairbalance/datasets/_datasets_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,18 +27,18 @@
     data = fetch_ucirepo(id=2)
     
     adult_data = data.data.features.copy()
     targets = data.data.targets.copy()
     
     adult_data = adult_data.drop(columns=["fnlwgt"])
     targets["income"] = targets["income"].replace({"<=50K.": 0, ">50K.": 1, ">50K": 1, "<=50K": 0})
-    adult_data.loc[: "income"] = targets
+    adult_data.loc[:, "income"] = targets
     adult_data = adult_data.dropna()
     targets = adult_data[["income"]]
-    adult_data = adult_data.drop()
+    adult_data = adult_data.drop(columns=["income"])
     
     categorical_features = ["workclass", "marital-status", "occupation", "relationship", "native-country", "education", "sex", "race"]
     continuous_features = [feature for feature in adult_data.columns if feature not in categorical_features and feature != "income"]
     
     return adult_data, targets, categorical_features,continuous_features
 
 def load_bank_marketing() :
@@ -70,15 +70,19 @@
     
     targets = targets.rename(columns={"y" : "subscribed"})
     
     bank_data["age"] = bank_data["age"].apply(lambda x: "x>25" if x > 25 else "x<=25")
     
     bank_data = bank_data.drop(columns=["poutcome"])
     bank_data["contact"] = bank_data["contact"].fillna("unknown")
+    bank_data.loc[:, "subscribed"] = targets
     bank_data = bank_data.dropna()
+    targets = bank_data[["subscribed"]]
+    bank_data = bank_data.drop(columns=["subscribed"])
+    
     targets["subscribed"] = targets["subscribed"].replace({"yes": 1, "no": 0})
     
     categorical_features = ["job", "marital", "education", "default", "housing", "loan", "contact", "month", "day_of_week", "age"]
     continuous_features = [feature for feature in bank_data.columns if feature not in categorical_features and feature != "subscribed"]
     
     return bank_data, targets, categorical_features, continuous_features
 
@@ -117,42 +121,50 @@
     
     kdd_data.columns = colum_names
     kdd_data.loc[:, "income"] = targets
     kdd_data = kdd_data.dropna()
     
     kdd_data = kdd_data.drop_duplicates(keep="first", inplace=False)
     
-    kdd_data["income"] = (kdd_data["income"] != "-50000").astype(int)
+    targets = kdd_data[["income"]]
+    kdd_data = kdd_data.drop(columns=["income"])
+    
+    targets["income"] = (targets["income"] != "-50000").astype(int)
     
     categorical_features = [
         "workclass","industry_code","occupation_code","education","enrolled_in_edu_inst_last_wk",
         "marital_status","major_industry_code","major_occupation_code","hispanic_origin","member_of_a_labour_union","reason_for_unemployment",
         "employment_status","tax_filler_status","region_of_previous_residence","state_of_previous_residence",
         "detailed_household_and_family_stat","detailed_household_summary_in_household","migration_code_change_in_msa","migration_code_change_in_reg",
         "migration_code_move_within_reg","live_in_this_house_1_year_ag","migration_prev_res_in_sunbelt","family_members_under_18","country_of_birth_father",
         "country_of_birth_mother","country_of_birth_self","citizenship","own_business_or_self_employed","fill_inc_questionnaire_for_veteran's_admin","veterans_benefits","year", "race", "sex"
         ]
     continuous_features = [feature for feature in kdd_data.columns if feature not in categorical_features and feature != "income"]
     
     
     
-    return kdd_data, "income", categorical_features, continuous_features
+    return kdd_data, targets, categorical_features, continuous_features
 
 def load_ACS(target="income", survey_year="2018",  states=["CA"], horizon="1-Year",survey='person') :
-    """
-    Loader for access to datasets derived from the US Census, using the Folktables open source python package.
+    """Loader for access to datasets derived from the US Census, using the Folktables open source python package.
     More information about the Folktables package: https://github.com/socialfoundations/folktables
     
-    Args:
-        targ (str, optional): The classification task. Available values are "income", "employment", "publiccoverage", 
+    Parameters
+    ----------
+    targ : str, optional
+        The classification task. Available values are "income", "employment", "publiccoverage", 
         "mobility" and "traveltime". Defaults to "income".
-        survey_year (str, optional): The year of the survey. Includes years from 2014. Defaults to "2018".
-        states (list, optional): The US state(s) to include in the survey. Defaults to ["CA"].
-        horizon (str, optional): Horizon of the survey. Available values are "1-Year" and "5-Year". Defaults to "1-Year".
-        survey (str, optional): type of survey. Available values are "person" and "household". Defaults to 'person'.
+    survey_year : str, optional 
+        The year of the survey. Includes years from 2014. Defaults to "2018".
+    states : list, optional 
+        The US state(s) to include in the survey. Defaults to ["CA"].
+    horizon : str, optional
+        Horizon of the survey. Available values are "1-Year" and "5-Year". Defaults to "1-Year".
+    survey : str, optional 
+        Type of survey. Available values are "person" and "household". Defaults to 'person'.
 
     Prediction task to determine the given "target" in a binary manner. 
     The target column is encoded with values 1 and 0 (1: >50k, 0: <=50k).
     The protected attributes are the columns "SEX" and "RAC1P" with the protected attributes "1" and "1".
     The protected attributes coding is as follow: 
     SEX: {1 : "Male", 2 : "Female"}
     RAC1P: {1 : "White", 2 : "Black", 3 : "Native_American", 4 : "Native_American", 5 : "Native_American", 6 : "Asian", 7 : "Islander", 8 : "Other", 9 : "Mixed" }
```

### Comparing `fairbalance-0.1.4/fairbalance/metrics/_dataset_metrics.py` & `fairbalance-0.1.5/fairbalance/metrics/_dataset_metrics.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.4/fairbalance/metrics/_fairness_analysis.py` & `fairbalance-0.1.5/fairbalance/metrics/_fairness_analysis.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.4/fairbalance/metrics/_model_metrics.py` & `fairbalance-0.1.5/fairbalance/metrics/_model_metrics.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.4/fairbalance/metrics/tests/test_dataset_metrics.py` & `fairbalance-0.1.5/fairbalance/metrics/tests/test_dataset_metrics.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.4/fairbalance/mitigation_strategies/_mitigation_strategies.py` & `fairbalance-0.1.5/fairbalance/mitigation_strategies/_mitigation_strategies.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.4/fairbalance/mitigation_strategies/base.py` & `fairbalance-0.1.5/fairbalance/mitigation_strategies/base.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.4/fairbalance/processors/_processors.py` & `fairbalance-0.1.5/fairbalance/processors/_processors.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.4/fairbalance/processors/base.py` & `fairbalance-0.1.5/fairbalance/processors/base.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.4/fairbalance/tools/__init__.py` & `fairbalance-0.1.5/fairbalance/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.4/fairbalance/tools/_fairness_analysis.py` & `fairbalance-0.1.5/fairbalance/tools/_fairness_analysis.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.4/fairbalance/tools/_mitigator.py` & `fairbalance-0.1.5/fairbalance/tools/_mitigator.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.4/fairbalance/tools/_processor.py` & `fairbalance-0.1.5/fairbalance/tools/_processor.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.4/fairbalance/tools/_utils.py` & `fairbalance-0.1.5/fairbalance/tools/_utils.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.4/fairbalance/tools/tests/test_fairness_analysis.py` & `fairbalance-0.1.5/fairbalance/tools/tests/test_fairness_analysis.py`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.4/fairbalance.egg-info/PKG-INFO` & `fairbalance-0.1.5/fairbalance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairbalance
-Version: 0.1.4
+Version: 0.1.5
 Summary: bias mitigation by balancing target and/or protected attributes using resampling techniques
 Author: Pierre-Antoine Lequeu @ Fujitsu Luxembourg
 Author-email: pierre-antoine.lequeu@fujitsu.com
 Description-Content-Type: text/markdown
 Requires-Dist: folktables>=0.0.12
 Requires-Dist: imbalanced_learn==0.9.1
 Requires-Dist: numpy>=1.24.3
```

### Comparing `fairbalance-0.1.4/fairbalance.egg-info/SOURCES.txt` & `fairbalance-0.1.5/fairbalance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fairbalance-0.1.4/setup.py` & `fairbalance-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "fairbalance",
-    version = "0.1.4",
+    version = "0.1.5",
     author = "Pierre-Antoine Lequeu @ Fujitsu Luxembourg",
     author_email = "pierre-antoine.lequeu@fujitsu.com",
     description = "bias mitigation by balancing target and/or protected attributes using resampling techniques",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     packages = setuptools.find_packages(),
     install_requires=[
```

