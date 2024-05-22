# Comparing `tmp/test_nvf_builds-0.0.3.5.tar.gz` & `tmp/test_nvf_builds-0.0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_nvf_builds-0.0.3.5.tar", last modified: Tue May 21 07:43:47 2024, max compression
+gzip compressed data, was "test_nvf_builds-0.0.3.6.tar", last modified: Wed May 22 13:21:18 2024, max compression
```

## Comparing `test_nvf_builds-0.0.3.5.tar` & `test_nvf_builds-0.0.3.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.995382 test_nvf_builds-0.0.3.5/
--rw-r--r--   0 mostafa    (501) staff       (20)    11357 2024-05-07 07:57:47.000000 test_nvf_builds-0.0.3.5/LICENSE
--rw-r--r--   0 mostafa    (501) staff       (20)      480 2024-05-21 07:43:47.995312 test_nvf_builds-0.0.3.5/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)       85 2024-05-06 07:53:59.000000 test_nvf_builds-0.0.3.5/README.md
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.991580 test_nvf_builds-0.0.3.5/oasysnow/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:25.000000 test_nvf_builds-0.0.3.5/oasysnow/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.991707 test_nvf_builds-0.0.3.5/oasysnow/federated/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:50:57.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.991837 test_nvf_builds-0.0.3.5/oasysnow/federated/client/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:25:11.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/client/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.992218 test_nvf_builds-0.0.3.5/oasysnow/federated/client/filters/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:35.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/client/filters/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2484 2024-05-16 12:49:15.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/client/filters/filter_data.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2471 2024-05-06 15:57:38.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/client/filters/filter_results.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.992461 test_nvf_builds-0.0.3.5/oasysnow/federated/client/trainer/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:41.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/client/trainer/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     4653 2024-05-15 14:56:42.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/client/trainer/trainer.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.992593 test_nvf_builds-0.0.3.5/oasysnow/federated/common/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-15 14:50:33.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/common/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.992941 test_nvf_builds-0.0.3.5/oasysnow/federated/common/attestation_service/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:56:34.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/common/attestation_service/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1596 2024-05-15 14:50:41.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/common/attestation_service/server.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1324 2024-05-15 14:50:41.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/common/attestation_service/verification.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.993304 test_nvf_builds-0.0.3.5/oasysnow/federated/common/model/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:36:02.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/common/model/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1803 2024-05-15 14:55:57.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/common/model/gennet_model.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1288 2024-05-15 14:55:47.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/common/model/global_model.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.993440 test_nvf_builds-0.0.3.5/oasysnow/federated/server/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:11.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/server/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.993799 test_nvf_builds-0.0.3.5/oasysnow/federated/server/filters/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:45.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/server/filters/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2501 2024-05-15 14:51:04.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/server/filters/filter_data.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2475 2024-04-19 21:41:54.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/server/filters/filter_results.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.994127 test_nvf_builds-0.0.3.5/oasysnow/federated/server/model_runner/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:45:46.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/server/model_runner/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     4843 2024-05-15 14:56:24.000000 test_nvf_builds-0.0.3.5/oasysnow/federated/server/model_runner/model_runner.py
--rw-r--r--   0 mostafa    (501) staff       (20)       29 2024-05-15 14:24:19.000000 test_nvf_builds-0.0.3.5/requirements.txt
--rw-r--r--   0 mostafa    (501) staff       (20)      479 2024-05-21 07:43:47.995637 test_nvf_builds-0.0.3.5/setup.cfg
--rw-r--r--   0 mostafa    (501) staff       (20)      322 2024-05-06 15:10:01.000000 test_nvf_builds-0.0.3.5/setup.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-21 07:43:47.995066 test_nvf_builds-0.0.3.5/test_nvf_builds.egg-info/
--rw-r--r--   0 mostafa    (501) staff       (20)      480 2024-05-21 07:43:47.000000 test_nvf_builds-0.0.3.5/test_nvf_builds.egg-info/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)     1220 2024-05-21 07:43:47.000000 test_nvf_builds-0.0.3.5/test_nvf_builds.egg-info/SOURCES.txt
--rw-r--r--   0 mostafa    (501) staff       (20)        1 2024-05-21 07:43:47.000000 test_nvf_builds-0.0.3.5/test_nvf_builds.egg-info/dependency_links.txt
--rw-r--r--   0 mostafa    (501) staff       (20)       28 2024-05-21 07:43:47.000000 test_nvf_builds-0.0.3.5/test_nvf_builds.egg-info/requires.txt
--rw-r--r--   0 mostafa    (501) staff       (20)        9 2024-05-21 07:43:47.000000 test_nvf_builds-0.0.3.5/test_nvf_builds.egg-info/top_level.txt
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.126642 test_nvf_builds-0.0.3.6/
+-rw-r--r--   0 mostafa    (501) staff       (20)    11357 2024-05-07 07:57:47.000000 test_nvf_builds-0.0.3.6/LICENSE
+-rw-r--r--   0 mostafa    (501) staff       (20)      480 2024-05-22 13:21:18.126561 test_nvf_builds-0.0.3.6/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)       85 2024-05-06 07:53:59.000000 test_nvf_builds-0.0.3.6/README.md
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.122629 test_nvf_builds-0.0.3.6/oasysnow/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:25.000000 test_nvf_builds-0.0.3.6/oasysnow/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.122730 test_nvf_builds-0.0.3.6/oasysnow/federated/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:50:57.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.122828 test_nvf_builds-0.0.3.6/oasysnow/federated/client/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:25:11.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/client/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.123191 test_nvf_builds-0.0.3.6/oasysnow/federated/client/filters/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:35.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/client/filters/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2484 2024-05-16 12:49:15.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/client/filters/filter_data.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2471 2024-05-06 15:57:38.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/client/filters/filter_results.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.123413 test_nvf_builds-0.0.3.6/oasysnow/federated/client/trainer/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:41.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/client/trainer/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     4653 2024-05-15 14:56:42.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/client/trainer/trainer.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.123567 test_nvf_builds-0.0.3.6/oasysnow/federated/common/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-15 14:50:33.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/common/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.123887 test_nvf_builds-0.0.3.6/oasysnow/federated/common/attestation_service/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:56:34.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/common/attestation_service/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1596 2024-05-15 14:50:41.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/common/attestation_service/server.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1324 2024-05-15 14:50:41.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/common/attestation_service/verification.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.124290 test_nvf_builds-0.0.3.6/oasysnow/federated/common/model/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:36:02.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/common/model/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1803 2024-05-15 14:55:57.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/common/model/gennet_model.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1288 2024-05-15 14:55:47.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/common/model/global_model.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.124437 test_nvf_builds-0.0.3.6/oasysnow/federated/server/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:11.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/server/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.124817 test_nvf_builds-0.0.3.6/oasysnow/federated/server/filters/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:45.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/server/filters/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2501 2024-05-15 14:51:04.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/server/filters/filter_data.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2475 2024-04-19 21:41:54.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/server/filters/filter_results.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.125087 test_nvf_builds-0.0.3.6/oasysnow/federated/server/model_runner/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:45:46.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/server/model_runner/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     4843 2024-05-15 14:56:24.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/server/model_runner/model_runner.py
+-rw-r--r--   0 mostafa    (501) staff       (20)       29 2024-05-15 14:24:19.000000 test_nvf_builds-0.0.3.6/requirements.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)      479 2024-05-22 13:21:18.126897 test_nvf_builds-0.0.3.6/setup.cfg
+-rw-r--r--   0 mostafa    (501) staff       (20)      322 2024-05-06 15:10:01.000000 test_nvf_builds-0.0.3.6/setup.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.126320 test_nvf_builds-0.0.3.6/test_nvf_builds.egg-info/
+-rw-r--r--   0 mostafa    (501) staff       (20)      480 2024-05-22 13:21:18.000000 test_nvf_builds-0.0.3.6/test_nvf_builds.egg-info/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)     1220 2024-05-22 13:21:18.000000 test_nvf_builds-0.0.3.6/test_nvf_builds.egg-info/SOURCES.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)        1 2024-05-22 13:21:18.000000 test_nvf_builds-0.0.3.6/test_nvf_builds.egg-info/dependency_links.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)       28 2024-05-22 13:21:18.000000 test_nvf_builds-0.0.3.6/test_nvf_builds.egg-info/requires.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)        9 2024-05-22 13:21:18.000000 test_nvf_builds-0.0.3.6/test_nvf_builds.egg-info/top_level.txt
```

### Comparing `test_nvf_builds-0.0.3.5/LICENSE` & `test_nvf_builds-0.0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.5/oasysnow/federated/client/filters/filter_data.py` & `test_nvf_builds-0.0.3.6/oasysnow/federated/client/filters/filter_data.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.5/oasysnow/federated/client/filters/filter_results.py` & `test_nvf_builds-0.0.3.6/oasysnow/federated/client/filters/filter_results.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.5/oasysnow/federated/client/trainer/trainer.py` & `test_nvf_builds-0.0.3.6/oasysnow/federated/client/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.5/oasysnow/federated/common/attestation_service/server.py` & `test_nvf_builds-0.0.3.6/oasysnow/federated/common/attestation_service/server.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.5/oasysnow/federated/common/attestation_service/verification.py` & `test_nvf_builds-0.0.3.6/oasysnow/federated/common/attestation_service/verification.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.5/oasysnow/federated/common/model/gennet_model.py` & `test_nvf_builds-0.0.3.6/oasysnow/federated/common/model/gennet_model.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.5/oasysnow/federated/common/model/global_model.py` & `test_nvf_builds-0.0.3.6/oasysnow/federated/common/model/global_model.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.5/oasysnow/federated/server/filters/filter_data.py` & `test_nvf_builds-0.0.3.6/oasysnow/federated/server/filters/filter_data.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.5/oasysnow/federated/server/filters/filter_results.py` & `test_nvf_builds-0.0.3.6/oasysnow/federated/server/filters/filter_results.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.5/oasysnow/federated/server/model_runner/model_runner.py` & `test_nvf_builds-0.0.3.6/oasysnow/federated/server/model_runner/model_runner.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.5/test_nvf_builds.egg-info/SOURCES.txt` & `test_nvf_builds-0.0.3.6/test_nvf_builds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

