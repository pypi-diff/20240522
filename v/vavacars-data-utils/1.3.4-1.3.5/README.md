# Comparing `tmp/vavacars_data_utils-1.3.4.tar.gz` & `tmp/vavacars_data_utils-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vavacars_data_utils-1.3.4.tar", last modified: Wed Mar 20 08:47:38 2024, max compression
+gzip compressed data, was "vavacars_data_utils-1.3.5.tar", last modified: Wed May 22 12:31:24 2024, max compression
```

## Comparing `vavacars_data_utils-1.3.4.tar` & `vavacars_data_utils-1.3.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-03-20 08:47:38.695169 vavacars_data_utils-1.3.4/
--rwxrwxrwx   0 pga       (1000) pga       (1000)     3064 2024-03-20 08:47:38.691172 vavacars_data_utils-1.3.4/PKG-INFO
--rwxrwxrwx   0 pga       (1000) pga       (1000)     2321 2023-06-15 14:28:48.000000 vavacars_data_utils-1.3.4/README.md
--rwxrwxrwx   0 pga       (1000) pga       (1000)      124 2022-03-09 12:03:29.000000 vavacars_data_utils-1.3.4/pyproject.toml
--rwxrwxrwx   0 pga       (1000) pga       (1000)      816 2024-03-20 08:47:38.699168 vavacars_data_utils-1.3.4/setup.cfg
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-03-20 08:47:37.937419 vavacars_data_utils-1.3.4/test/
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-03-20 08:47:38.023553 vavacars_data_utils-1.3.4/test/utils/
--rwxrwxrwx   0 pga       (1000) pga       (1000)        0 2022-03-09 12:03:29.000000 vavacars_data_utils-1.3.4/test/utils/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     1159 2022-03-09 12:03:29.000000 vavacars_data_utils-1.3.4/test/utils/test_strings.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-03-20 08:47:38.037561 vavacars_data_utils-1.3.4/vava_utils/
--rwxrwxrwx   0 pga       (1000) pga       (1000)        0 2022-03-09 12:03:29.000000 vavacars_data_utils-1.3.4/vava_utils/__init__.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-03-20 08:47:38.070084 vavacars_data_utils-1.3.4/vava_utils/azure/
--rwxrwxrwx   0 pga       (1000) pga       (1000)       70 2022-05-04 13:49:57.000000 vavacars_data_utils-1.3.4/vava_utils/azure/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)    10204 2023-09-12 13:53:24.000000 vavacars_data_utils-1.3.4/vava_utils/azure/az_helper.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-03-20 08:47:38.105078 vavacars_data_utils-1.3.4/vava_utils/bigquery/
--rwxrwxrwx   0 pga       (1000) pga       (1000)       43 2023-06-15 14:28:48.000000 vavacars_data_utils-1.3.4/vava_utils/bigquery/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     1187 2023-06-15 14:28:48.000000 vavacars_data_utils-1.3.4/vava_utils/bigquery/bigquery_helper.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-03-20 08:47:38.137087 vavacars_data_utils-1.3.4/vava_utils/camunda/
--rwxrwxrwx   0 pga       (1000) pga       (1000)       85 2022-03-09 12:03:29.000000 vavacars_data_utils-1.3.4/vava_utils/camunda/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     4008 2023-05-16 14:47:25.000000 vavacars_data_utils-1.3.4/vava_utils/camunda/camunda_helper.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-03-20 08:47:38.170601 vavacars_data_utils-1.3.4/vava_utils/email/
--rwxrwxrwx   0 pga       (1000) pga       (1000)       37 2023-06-15 13:04:41.000000 vavacars_data_utils-1.3.4/vava_utils/email/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     3862 2023-06-29 09:16:49.000000 vavacars_data_utils-1.3.4/vava_utils/email/email_helper.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-03-20 08:47:38.203601 vavacars_data_utils-1.3.4/vava_utils/salesforce/
--rwxrwxrwx   0 pga       (1000) pga       (1000)       47 2023-06-09 14:13:08.000000 vavacars_data_utils-1.3.4/vava_utils/salesforce/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     2114 2024-03-20 08:46:56.000000 vavacars_data_utils-1.3.4/vava_utils/salesforce/salesforce_helper.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-03-20 08:47:38.260132 vavacars_data_utils-1.3.4/vava_utils/smartiq/
--rwxrwxrwx   0 pga       (1000) pga       (1000)      205 2022-04-25 14:18:59.000000 vavacars_data_utils-1.3.4/vava_utils/smartiq/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     7909 2022-04-25 14:18:59.000000 vavacars_data_utils-1.3.4/vava_utils/smartiq/smartiq_helper.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     9856 2022-06-16 14:27:47.000000 vavacars_data_utils-1.3.4/vava_utils/smartiq/smartiq_helper_v2.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-03-20 08:47:38.317132 vavacars_data_utils-1.3.4/vava_utils/sql/
--rwxrwxrwx   0 pga       (1000) pga       (1000)      160 2022-06-21 13:02:18.000000 vavacars_data_utils-1.3.4/vava_utils/sql/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)    14999 2023-12-21 10:22:28.000000 vavacars_data_utils-1.3.4/vava_utils/sql/sql_helper.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-03-20 08:47:38.358658 vavacars_data_utils-1.3.4/vava_utils/turkey/
--rwxrwxrwx   0 pga       (1000) pga       (1000)      148 2022-03-09 12:03:29.000000 vavacars_data_utils-1.3.4/vava_utils/turkey/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)      889 2022-03-09 12:03:29.000000 vavacars_data_utils-1.3.4/vava_utils/turkey/dates.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-03-20 08:47:38.507397 vavacars_data_utils-1.3.4/vava_utils/utils/
--rwxrwxrwx   0 pga       (1000) pga       (1000)      411 2023-07-27 10:32:52.000000 vavacars_data_utils-1.3.4/vava_utils/utils/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)      369 2022-03-09 12:03:29.000000 vavacars_data_utils-1.3.4/vava_utils/utils/callables.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     1950 2022-07-04 11:26:35.000000 vavacars_data_utils-1.3.4/vava_utils/utils/comparisons.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     1168 2023-06-15 14:28:48.000000 vavacars_data_utils-1.3.4/vava_utils/utils/naming.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)      273 2022-04-25 14:18:59.000000 vavacars_data_utils-1.3.4/vava_utils/utils/singleton.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)      734 2022-03-09 12:03:29.000000 vavacars_data_utils-1.3.4/vava_utils/utils/strings.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)      752 2024-02-19 14:35:50.000000 vavacars_data_utils-1.3.4/vava_utils/utils/utils.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-03-20 08:47:38.574896 vavacars_data_utils-1.3.4/vava_utils/vavaprice/
--rwxrwxrwx   0 pga       (1000) pga       (1000)       91 2022-03-11 15:04:33.000000 vavacars_data_utils-1.3.4/vava_utils/vavaprice/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     3225 2022-10-18 14:03:18.000000 vavacars_data_utils-1.3.4/vava_utils/vavaprice/vavaprice_helper.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-03-20 08:47:38.683168 vavacars_data_utils-1.3.4/vavacars_data_utils.egg-info/
--rwxrwxrwx   0 pga       (1000) pga       (1000)     3064 2024-03-20 08:47:37.000000 vavacars_data_utils-1.3.4/vavacars_data_utils.egg-info/PKG-INFO
--rwxrwxrwx   0 pga       (1000) pga       (1000)     1213 2024-03-20 08:47:37.000000 vavacars_data_utils-1.3.4/vavacars_data_utils.egg-info/SOURCES.txt
--rwxrwxrwx   0 pga       (1000) pga       (1000)        1 2024-03-20 08:47:37.000000 vavacars_data_utils-1.3.4/vavacars_data_utils.egg-info/dependency_links.txt
--rwxrwxrwx   0 pga       (1000) pga       (1000)      113 2024-03-20 08:47:37.000000 vavacars_data_utils-1.3.4/vavacars_data_utils.egg-info/requires.txt
--rwxrwxrwx   0 pga       (1000) pga       (1000)       16 2024-03-20 08:47:37.000000 vavacars_data_utils-1.3.4/vavacars_data_utils.egg-info/top_level.txt
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-05-22 12:31:24.319942 vavacars_data_utils-1.3.5/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     3368 2024-05-22 12:31:24.316886 vavacars_data_utils-1.3.5/PKG-INFO
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     2321 2023-06-15 14:28:48.000000 vavacars_data_utils-1.3.5/README.md
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      124 2022-03-09 12:03:29.000000 vavacars_data_utils-1.3.5/pyproject.toml
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      925 2024-05-22 12:31:24.324107 vavacars_data_utils-1.3.5/setup.cfg
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-05-22 12:31:23.435343 vavacars_data_utils-1.3.5/test/
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-05-22 12:31:23.567721 vavacars_data_utils-1.3.5/test/utils/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)        0 2022-03-09 12:03:29.000000 vavacars_data_utils-1.3.5/test/utils/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     1159 2022-03-09 12:03:29.000000 vavacars_data_utils-1.3.5/test/utils/test_strings.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-05-22 12:31:23.588470 vavacars_data_utils-1.3.5/vava_utils/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)        0 2022-03-09 12:03:29.000000 vavacars_data_utils-1.3.5/vava_utils/__init__.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-05-22 12:31:23.636555 vavacars_data_utils-1.3.5/vava_utils/azure/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       70 2022-05-04 13:49:57.000000 vavacars_data_utils-1.3.5/vava_utils/azure/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)    10204 2024-04-24 17:12:45.000000 vavacars_data_utils-1.3.5/vava_utils/azure/az_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-05-22 12:31:23.692779 vavacars_data_utils-1.3.5/vava_utils/bigquery/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       43 2023-06-15 14:28:48.000000 vavacars_data_utils-1.3.5/vava_utils/bigquery/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     1187 2023-06-15 14:28:48.000000 vavacars_data_utils-1.3.5/vava_utils/bigquery/bigquery_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-05-22 12:31:23.747252 vavacars_data_utils-1.3.5/vava_utils/camunda/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       85 2022-03-09 12:03:29.000000 vavacars_data_utils-1.3.5/vava_utils/camunda/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     4008 2023-05-16 14:47:25.000000 vavacars_data_utils-1.3.5/vava_utils/camunda/camunda_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-05-22 12:31:23.801603 vavacars_data_utils-1.3.5/vava_utils/email/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       37 2023-06-15 13:04:41.000000 vavacars_data_utils-1.3.5/vava_utils/email/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     3862 2024-04-24 17:04:24.000000 vavacars_data_utils-1.3.5/vava_utils/email/email_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-05-22 12:31:23.849265 vavacars_data_utils-1.3.5/vava_utils/salesforce/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       47 2023-06-09 14:13:08.000000 vavacars_data_utils-1.3.5/vava_utils/salesforce/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     2114 2024-03-20 08:46:56.000000 vavacars_data_utils-1.3.5/vava_utils/salesforce/salesforce_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-05-22 12:31:23.914223 vavacars_data_utils-1.3.5/vava_utils/smartiq/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      205 2022-04-25 14:18:59.000000 vavacars_data_utils-1.3.5/vava_utils/smartiq/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     7909 2022-04-25 14:18:59.000000 vavacars_data_utils-1.3.5/vava_utils/smartiq/smartiq_helper.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     9856 2022-06-16 14:27:47.000000 vavacars_data_utils-1.3.5/vava_utils/smartiq/smartiq_helper_v2.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-05-22 12:31:23.963342 vavacars_data_utils-1.3.5/vava_utils/sql/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      160 2022-06-21 13:02:18.000000 vavacars_data_utils-1.3.5/vava_utils/sql/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)    15373 2024-05-22 12:31:09.000000 vavacars_data_utils-1.3.5/vava_utils/sql/sql_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-05-22 12:31:24.004157 vavacars_data_utils-1.3.5/vava_utils/turkey/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      148 2022-03-09 12:03:29.000000 vavacars_data_utils-1.3.5/vava_utils/turkey/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      889 2022-03-09 12:03:29.000000 vavacars_data_utils-1.3.5/vava_utils/turkey/dates.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-05-22 12:31:24.163339 vavacars_data_utils-1.3.5/vava_utils/utils/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      411 2023-07-27 10:32:52.000000 vavacars_data_utils-1.3.5/vava_utils/utils/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      369 2022-03-09 12:03:29.000000 vavacars_data_utils-1.3.5/vava_utils/utils/callables.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     1950 2022-07-04 11:26:35.000000 vavacars_data_utils-1.3.5/vava_utils/utils/comparisons.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     1168 2023-06-15 14:28:48.000000 vavacars_data_utils-1.3.5/vava_utils/utils/naming.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      273 2022-04-25 14:18:59.000000 vavacars_data_utils-1.3.5/vava_utils/utils/singleton.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      734 2022-03-09 12:03:29.000000 vavacars_data_utils-1.3.5/vava_utils/utils/strings.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      752 2024-02-19 14:35:50.000000 vavacars_data_utils-1.3.5/vava_utils/utils/utils.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-05-22 12:31:24.204386 vavacars_data_utils-1.3.5/vava_utils/vavaprice/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       91 2022-03-11 15:04:33.000000 vavacars_data_utils-1.3.5/vava_utils/vavaprice/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     3225 2022-10-18 14:03:18.000000 vavacars_data_utils-1.3.5/vava_utils/vavaprice/vavaprice_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2024-05-22 12:31:24.305660 vavacars_data_utils-1.3.5/vavacars_data_utils.egg-info/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     3368 2024-05-22 12:31:23.000000 vavacars_data_utils-1.3.5/vavacars_data_utils.egg-info/PKG-INFO
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     1213 2024-05-22 12:31:23.000000 vavacars_data_utils-1.3.5/vavacars_data_utils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 pga       (1000) pga       (1000)        1 2024-05-22 12:31:23.000000 vavacars_data_utils-1.3.5/vavacars_data_utils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      194 2024-05-22 12:31:23.000000 vavacars_data_utils-1.3.5/vavacars_data_utils.egg-info/requires.txt
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       16 2024-05-22 12:31:23.000000 vavacars_data_utils-1.3.5/vavacars_data_utils.egg-info/top_level.txt
```

### Comparing `vavacars_data_utils-1.3.4/PKG-INFO` & `vavacars_data_utils-1.3.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Metadata-Version: 2.1
 Name: vavacars_data_utils
-Version: 1.3.4
+Version: 1.3.5
 Summary: Package with utils
 Home-page: https://dev.azure.com/vavacars/DataScience/_git/Data.Utils
 Author: Vavacars Data Science Team
 Author-email: acg@vava.cars
 Project-URL: Bug Tracker, https://dev.azure.com/vavacars/DataScience/_workitems/recentlyupdated/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: PyYAML>=6.0
 Requires-Dist: requests
-Requires-Dist: sqlalchemy<2.0
-Requires-Dist: redis
-Requires-Dist: msal
-Requires-Dist: pyodbc
 Requires-Dist: unidecode
-Requires-Dist: azure-communication-email
-Requires-Dist: psycopg2-binary
+Provides-Extra: bigquery
+Requires-Dist: google-cloud-bigquery; extra == "bigquery"
+Requires-Dist: google-api-core; extra == "bigquery"
+Provides-Extra: sql
+Requires-Dist: sqlalchemy<2.0; extra == "sql"
+Requires-Dist: psycopg2-binary; extra == "sql"
+Requires-Dist: pyodbc; extra == "sql"
+Requires-Dist: msal; extra == "sql"
+Provides-Extra: emai
+Requires-Dist: azure-communication-email; extra == "emai"
+Provides-Extra: azure
+Requires-Dist: azureml-core; extra == "azure"
 
 # Vavacars
 
 Vavacars utils library.
 
 ## Installation
```

### Comparing `vavacars_data_utils-1.3.4/README.md` & `vavacars_data_utils-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.3.4/setup.cfg` & `vavacars_data_utils-1.3.5/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vavacars_data_utils
-version = 1.3.4
+version = 1.3.5
 author = Vavacars Data Science Team
 author_email = acg@vava.cars
 description = Package with utils
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://dev.azure.com/vavacars/DataScience/_git/Data.Utils
 project_urls = 
@@ -18,26 +18,34 @@
 	= .
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	pandas
 	PyYAML>=6.0
 	requests
-	sqlalchemy<2.0
-	redis
-	msal
-	pyodbc
 	unidecode
-	azure-communication-email
-	psycopg2-binary
 
 [options.packages.find]
 where = .
 exclude = 
 	test
 	README.md
 	notebooks
 
+[options.extras_require]
+bigquery = 
+	google-cloud-bigquery
+	google-api-core
+sql = 
+	sqlalchemy<2.0
+	psycopg2-binary
+	pyodbc
+	msal
+emai = 
+	azure-communication-email
+azure = 
+	azureml-core
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `vavacars_data_utils-1.3.4/test/utils/test_strings.py` & `vavacars_data_utils-1.3.5/test/utils/test_strings.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.3.4/vava_utils/azure/az_helper.py` & `vavacars_data_utils-1.3.5/vava_utils/azure/az_helper.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.3.4/vava_utils/bigquery/bigquery_helper.py` & `vavacars_data_utils-1.3.5/vava_utils/bigquery/bigquery_helper.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.3.4/vava_utils/camunda/camunda_helper.py` & `vavacars_data_utils-1.3.5/vava_utils/camunda/camunda_helper.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.3.4/vava_utils/email/email_helper.py` & `vavacars_data_utils-1.3.5/vava_utils/email/email_helper.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.3.4/vava_utils/salesforce/salesforce_helper.py` & `vavacars_data_utils-1.3.5/vava_utils/salesforce/salesforce_helper.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.3.4/vava_utils/smartiq/smartiq_helper.py` & `vavacars_data_utils-1.3.5/vava_utils/smartiq/smartiq_helper.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.3.4/vava_utils/smartiq/smartiq_helper_v2.py` & `vavacars_data_utils-1.3.5/vava_utils/smartiq/smartiq_helper_v2.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.3.4/vava_utils/sql/sql_helper.py` & `vavacars_data_utils-1.3.5/vava_utils/sql/sql_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,15 @@
 
 
 def get_postgresql_helper(host, user, port, database=None, password=None, **kwargs):
     # TODO using old version of psycopg2 (new one is psycopg3) because sql_alchemy < 2 only works with old version
     engine_url = URL.create(
         drivername="postgresql+psycopg2", host=host, username=user, database=database, password=password, port=port
     )
-    engine = create_engine(
-        engine_url, pool_pre_ping=True, **kwargs
-    )
+    engine = create_engine(engine_url, pool_pre_ping=True, **kwargs)
 
     return SQL_Helper(engine, engine_type=POSTGRESQL)
 
 
 def get_mysql_helper(host, user, port, database=None, password=None, **kwargs):
     engine_url = URL.create(
         drivername="mysql+pymysql", host=host, username=user, database=database, password=password, port=port
@@ -158,26 +156,36 @@
             **kwargs: additional keyword parameters passed to pd.read_sql_query
 
         Returns:
             result (pd.DataFrame): query results in  Pandas DataFrame format
         """
         return pd.read_sql_query(text(query), self._engine, **kwargs)
 
-    def write_df(self, df: pd.DataFrame, table_name: str, chunksize: int = 1000, index: bool = False, **kwargs):
+    def write_df(
+        self, df: pd.DataFrame, table_name: str, chunksize: int = 1000, index: bool = False, if_exists="fail", **kwargs
+    ):
         """
         Store Pandas Dataframe into SQL table
 
         Args:
             df (pd.DataFrame): data to write
             table_name (str): output database table name
+            if_exists (str): action to take if table already exists
+                * fail, 
+                * replace 
+                * append 
+                * truncate: NEW, truncate table before writing, like 'replace' but keeps structure
             **kwargs: additional keyword parameters passed to df.to_sql
         """
         with self._engine.connect() as conn:
             trans = conn.begin()
             try:
+                if if_exists == "truncate": 
+                    conn.execute(f"TRUNCATE TABLE {table_name}")
+                    if_exists = "append"
                 df.to_sql(table_name.lower(), conn, chunksize=chunksize, index=index, **kwargs)
                 trans.commit()
             except Exception as ex:
                 LOGGER.warning(str(ex))
                 trans.rollback()
                 raise ex
 
@@ -209,16 +217,16 @@
                 FROM {tmp_table_name} AS tmp
                 WHERE NOT EXISTS
                 (
                     SELECT 1 FROM {table_name} 
                     WHERE {not_exists_part_cols}
                 );
             """
-            col_names = [f'[{x}]' for x in df.columns]
-            upsert_cols = [f'[{x}]' for x in upsert_cols]
+            col_names = [f"[{x}]" for x in df.columns]
+            upsert_cols = [f"[{x}]" for x in upsert_cols]
 
         elif self.engine_type == MYSQL:
             tmp_table_name = f"{table_name}_tmp_{random.randrange(0, 1000)}"
             create_sql_model = """
                 CREATE TEMPORARY TABLE IF NOT EXISTS {tmp_table_name} LIKE {table_name};
             """
             set_part_sql_model = "t.{col} = tmp.{col}"
@@ -233,16 +241,16 @@
                 FROM {tmp_table_name} AS tmp
                 WHERE NOT EXISTS
                 (
                     SELECT 1 FROM {table_name} 
                     WHERE {not_exists_part_cols}
                 );
             """
-            col_names = [f'`{x}`' for x in df.columns]
-            upsert_cols = [f'`{x}`' for x in upsert_cols]
+            col_names = [f"`{x}`" for x in df.columns]
+            upsert_cols = [f"`{x}`" for x in upsert_cols]
 
         elif self.engine_type == POSTGRESQL:
             tmp_table_name = f"{table_name}_tmp_{random.randrange(0, 1000)}"
             create_sql_model = f"""
                 CREATE TEMP TABLE {tmp_table_name} as TABLE {table_name} WITH NO DATA;
             """
             set_part_sql_model = "t.{col} = tmp.{col}"
@@ -257,16 +265,16 @@
                 FROM {tmp_table_name} AS tmp
                 WHERE NOT EXISTS
                 (
                     SELECT 1 FROM {table_name} 
                     WHERE {not_exists_part_cols}
                 );
             """
-            col_names = [f'`{x}`' for x in df.columns]
-            upsert_cols = [f'`{x}`' for x in upsert_cols]
+            col_names = [f"`{x}`" for x in df.columns]
+            upsert_cols = [f"`{x}`" for x in upsert_cols]
 
         else:
             raise NotImplementedError(f"Method not implemented for {self.engine_type} engine")
 
         try:
             # this is transactional
             with self._engine.connect() as conn:
@@ -305,18 +313,18 @@
                     insert_sql = insert_sql_model.format(
                         table_name=table_name,
                         comma_col_names=comma_col_names,
                         tmp_table_name=tmp_table_name,
                         not_exists_part_cols=not_exists_part_cols,
                     )
                     conn.execute(text(insert_sql))
-                    
+
                     # DROP tmp table
                     conn.execute(text(f"DROP TABLE {tmp_table_name};"))
-                    
+
                     trans.commit()
                 except Exception as ex:
                     LOGGER.warning(str(ex))
                     trans.rollback()
                     raise ex
         except Exception as ex:
             LOGGER.error(str(ex), exc_info=ex)
@@ -385,10 +393,9 @@
         if exists:
             self.update_row(row, keys, table_name)
         else:
             self.write_row(row, table_name)
 
         return "UPDATE" if exists else "CREATE"
 
-
     def execute(self, query: str) -> LegacyCursorResult:
-        return self._engine.execute(query)
+        return self._engine.execute(query)
```

### Comparing `vavacars_data_utils-1.3.4/vava_utils/turkey/dates.py` & `vavacars_data_utils-1.3.5/vava_utils/turkey/dates.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.3.4/vava_utils/utils/comparisons.py` & `vavacars_data_utils-1.3.5/vava_utils/utils/comparisons.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.3.4/vava_utils/utils/naming.py` & `vavacars_data_utils-1.3.5/vava_utils/utils/naming.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.3.4/vava_utils/utils/strings.py` & `vavacars_data_utils-1.3.5/vava_utils/utils/strings.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.3.4/vava_utils/utils/utils.py` & `vavacars_data_utils-1.3.5/vava_utils/utils/utils.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.3.4/vava_utils/vavaprice/vavaprice_helper.py` & `vavacars_data_utils-1.3.5/vava_utils/vavaprice/vavaprice_helper.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.3.4/vavacars_data_utils.egg-info/PKG-INFO` & `vavacars_data_utils-1.3.5/vavacars_data_utils.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Metadata-Version: 2.1
 Name: vavacars_data_utils
-Version: 1.3.4
+Version: 1.3.5
 Summary: Package with utils
 Home-page: https://dev.azure.com/vavacars/DataScience/_git/Data.Utils
 Author: Vavacars Data Science Team
 Author-email: acg@vava.cars
 Project-URL: Bug Tracker, https://dev.azure.com/vavacars/DataScience/_workitems/recentlyupdated/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: PyYAML>=6.0
 Requires-Dist: requests
-Requires-Dist: sqlalchemy<2.0
-Requires-Dist: redis
-Requires-Dist: msal
-Requires-Dist: pyodbc
 Requires-Dist: unidecode
-Requires-Dist: azure-communication-email
-Requires-Dist: psycopg2-binary
+Provides-Extra: bigquery
+Requires-Dist: google-cloud-bigquery; extra == "bigquery"
+Requires-Dist: google-api-core; extra == "bigquery"
+Provides-Extra: sql
+Requires-Dist: sqlalchemy<2.0; extra == "sql"
+Requires-Dist: psycopg2-binary; extra == "sql"
+Requires-Dist: pyodbc; extra == "sql"
+Requires-Dist: msal; extra == "sql"
+Provides-Extra: emai
+Requires-Dist: azure-communication-email; extra == "emai"
+Provides-Extra: azure
+Requires-Dist: azureml-core; extra == "azure"
 
 # Vavacars
 
 Vavacars utils library.
 
 ## Installation
```

### Comparing `vavacars_data_utils-1.3.4/vavacars_data_utils.egg-info/SOURCES.txt` & `vavacars_data_utils-1.3.5/vavacars_data_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

