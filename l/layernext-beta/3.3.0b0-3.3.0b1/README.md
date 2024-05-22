# Comparing `tmp/layernext-beta-3.3.0b0.tar.gz` & `tmp/layernext-beta-3.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layernext-beta-3.3.0b0.tar", last modified: Wed Apr 10 05:57:14 2024, max compression
+gzip compressed data, was "layernext-beta-3.3.0b1.tar", last modified: Wed May 22 08:09:39 2024, max compression
```

## Comparing `layernext-beta-3.3.0b0.tar` & `layernext-beta-3.3.0b1.tar`

### file list

```diff
@@ -1,55 +1,53 @@
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-10 05:57:14.975846 layernext-beta-3.3.0b0/
--rw-r--r--   0 chathushka   (501) staff       (20)     1073 2023-09-11 10:46:59.000000 layernext-beta-3.3.0b0/LICENSE
--rw-r--r--   0 chathushka   (501) staff       (20)      928 2024-04-10 05:57:14.975623 layernext-beta-3.3.0b0/PKG-INFO
--rw-r--r--   0 chathushka   (501) staff       (20)      352 2023-10-18 12:39:57.000000 layernext-beta-3.3.0b0/README.md
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-10 05:57:14.958779 layernext-beta-3.3.0b0/layernext/
--rw-r--r--   0 chathushka   (501) staff       (20)   124538 2024-04-10 05:56:14.000000 layernext-beta-3.3.0b0/layernext/__init__.py
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-10 05:57:14.960695 layernext-beta-3.3.0b0/layernext/automatic_analysis/
--rw-r--r--   0 chathushka   (501) staff       (20)     8488 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/automatic_analysis/__init__.py
--rw-r--r--   0 chathushka   (501) staff       (20)     3902 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/automatic_analysis/automatic_analysis.py
--rw-r--r--   0 chathushka   (501) staff       (20)     7539 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/automatic_analysis/automatic_analysis_interface.py
--rw-r--r--   0 chathushka   (501) staff       (20)    19710 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/automatic_analysis/status_check_autoannotate_project.py
--rw-r--r--   0 chathushka   (501) staff       (20)     4927 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/automatic_analysis/support.py
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-10 05:57:14.969828 layernext-beta-3.3.0b0/layernext/datalake/
--rw-r--r--   0 chathushka   (501) staff       (20)    23794 2024-04-08 06:38:18.000000 layernext-beta-3.3.0b0/layernext/datalake/__init__.py
--rw-r--r--   0 chathushka   (501) staff       (20)    16752 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/annotation.py
--rw-r--r--   0 chathushka   (501) staff       (20)      868 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/aws_s3_client.py
--rw-r--r--   0 chathushka   (501) staff       (20)      964 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/azure_client.py
--rw-r--r--   0 chathushka   (501) staff       (20)     2307 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/constants.py
--rw-r--r--   0 chathushka   (501) staff       (20)    93969 2024-04-10 05:55:09.000000 layernext-beta-3.3.0b0/layernext/datalake/datalakeinterface.py
--rw-r--r--   0 chathushka   (501) staff       (20)        0 2023-09-11 10:46:59.000000 layernext-beta-3.3.0b0/layernext/datalake/dataset.py
--rw-r--r--   0 chathushka   (501) staff       (20)      470 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/file_trash.py
--rw-r--r--   0 chathushka   (501) staff       (20)    12275 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/file_upload.py
--rw-r--r--   0 chathushka   (501) staff       (20)      879 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/gcs_client.py
--rw-r--r--   0 chathushka   (501) staff       (20)     1642 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/ground_truth.py
--rw-r--r--   0 chathushka   (501) staff       (20)     1539 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/keys.py
--rw-r--r--   0 chathushka   (501) staff       (20)     7555 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/label.py
--rw-r--r--   0 chathushka   (501) staff       (20)     1283 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/logger.py
--rw-r--r--   0 chathushka   (501) staff       (20)     6659 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/metadata.py
--rw-r--r--   0 chathushka   (501) staff       (20)     1136 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/model_run.py
--rw-r--r--   0 chathushka   (501) staff       (20)     1166 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/mongo_json_encoder.py
--rw-r--r--   0 chathushka   (501) staff       (20)     1390 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/query.py
--rw-r--r--   0 chathushka   (501) staff       (20)      261 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/storage_client.py
--rw-r--r--   0 chathushka   (501) staff       (20)     2696 2024-04-03 07:30:54.000000 layernext-beta-3.3.0b0/layernext/datalake/storage_interface.py
--rw-r--r--   0 chathushka   (501) staff       (20)     8733 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/storage_upload.py
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-10 05:57:14.971459 layernext-beta-3.3.0b0/layernext/dataset/
--rw-r--r--   0 chathushka   (501) staff       (20)     3305 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/dataset/__init__.py
--rw-r--r--   0 chathushka   (501) staff       (20)     4561 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/dataset/dataset.py
--rw-r--r--   0 chathushka   (501) staff       (20)     9171 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/dataset/datasetinterface.py
--rw-r--r--   0 chathushka   (501) staff       (20)      431 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/dataset/logger.py
--rw-r--r--   0 chathushka   (501) staff       (20)    23610 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/dataset/sync.py
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-10 05:57:14.973453 layernext-beta-3.3.0b0/layernext/studio/
--rw-r--r--   0 chathushka   (501) staff       (20)     3661 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/studio/__init__.py
--rw-r--r--   0 chathushka   (501) staff       (20)      431 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/studio/logger.py
--rw-r--r--   0 chathushka   (501) staff       (20)     3860 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/studio/project.py
--rw-r--r--   0 chathushka   (501) staff       (20)    13127 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/studio/studiointerface.py
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-10 05:57:14.974950 layernext-beta-3.3.0b0/layernext_beta.egg-info/
--rw-r--r--   0 chathushka   (501) staff       (20)      928 2024-04-10 05:57:14.000000 layernext-beta-3.3.0b0/layernext_beta.egg-info/PKG-INFO
--rw-r--r--   0 chathushka   (501) staff       (20)     1487 2024-04-10 05:57:14.000000 layernext-beta-3.3.0b0/layernext_beta.egg-info/SOURCES.txt
--rw-r--r--   0 chathushka   (501) staff       (20)        1 2024-04-10 05:57:14.000000 layernext-beta-3.3.0b0/layernext_beta.egg-info/dependency_links.txt
--rw-r--r--   0 chathushka   (501) staff       (20)       78 2024-04-10 05:57:14.000000 layernext-beta-3.3.0b0/layernext_beta.egg-info/requires.txt
--rw-r--r--   0 chathushka   (501) staff       (20)       10 2024-04-10 05:57:14.000000 layernext-beta-3.3.0b0/layernext_beta.egg-info/top_level.txt
--rw-r--r--   0 chathushka   (501) staff       (20)       38 2024-04-10 05:57:14.975944 layernext-beta-3.3.0b0/setup.cfg
--rw-r--r--   0 chathushka   (501) staff       (20)     1950 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/setup.py
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-10 05:57:14.975132 layernext-beta-3.3.0b0/tests/
--rw-r--r--   0 chathushka   (501) staff       (20)     1043 2023-09-11 10:46:59.000000 layernext-beta-3.3.0b0/tests/test_cli.py
+drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2024-05-22 08:09:39.403265 layernext-beta-3.3.0b1/
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1073 2023-08-04 06:18:17.000000 layernext-beta-3.3.0b1/LICENSE
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      984 2024-05-22 08:09:39.403125 layernext-beta-3.3.0b1/PKG-INFO
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      352 2024-02-27 05:55:20.000000 layernext-beta-3.3.0b1/README.md
+drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2024-05-22 08:09:39.338296 layernext-beta-3.3.0b1/layernext/
+-rw-r--r--   0 channawijerathna   (501) staff       (20)   124538 2024-05-22 08:03:21.000000 layernext-beta-3.3.0b1/layernext/__init__.py
+drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2024-05-22 08:09:39.364427 layernext-beta-3.3.0b1/layernext/automatic_analysis/
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     8488 2024-02-27 05:51:55.000000 layernext-beta-3.3.0b1/layernext/automatic_analysis/__init__.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     3902 2024-02-27 05:52:03.000000 layernext-beta-3.3.0b1/layernext/automatic_analysis/automatic_analysis.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     7539 2024-02-27 05:52:00.000000 layernext-beta-3.3.0b1/layernext/automatic_analysis/automatic_analysis_interface.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)    19710 2024-02-27 05:52:06.000000 layernext-beta-3.3.0b1/layernext/automatic_analysis/status_check_autoannotate_project.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     4927 2024-02-27 05:52:09.000000 layernext-beta-3.3.0b1/layernext/automatic_analysis/support.py
+drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2024-05-22 08:09:39.374107 layernext-beta-3.3.0b1/layernext/datalake/
+-rw-r--r--   0 channawijerathna   (501) staff       (20)    23794 2024-05-10 07:36:07.000000 layernext-beta-3.3.0b1/layernext/datalake/__init__.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)    16752 2024-02-27 05:48:15.000000 layernext-beta-3.3.0b1/layernext/datalake/annotation.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      868 2024-02-27 05:48:19.000000 layernext-beta-3.3.0b1/layernext/datalake/aws_s3_client.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      964 2024-02-27 05:48:22.000000 layernext-beta-3.3.0b1/layernext/datalake/azure_client.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     2307 2024-02-27 05:48:25.000000 layernext-beta-3.3.0b1/layernext/datalake/constants.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)    93989 2024-05-22 07:56:54.000000 layernext-beta-3.3.0b1/layernext/datalake/datalakeinterface.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)        0 2024-02-27 05:50:19.000000 layernext-beta-3.3.0b1/layernext/datalake/dataset.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      470 2024-02-27 05:50:25.000000 layernext-beta-3.3.0b1/layernext/datalake/file_trash.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)    12275 2024-02-27 05:50:30.000000 layernext-beta-3.3.0b1/layernext/datalake/file_upload.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      879 2024-02-27 05:50:33.000000 layernext-beta-3.3.0b1/layernext/datalake/gcs_client.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1642 2024-02-27 05:50:43.000000 layernext-beta-3.3.0b1/layernext/datalake/ground_truth.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1539 2024-02-27 05:50:50.000000 layernext-beta-3.3.0b1/layernext/datalake/keys.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     7555 2024-02-27 05:50:54.000000 layernext-beta-3.3.0b1/layernext/datalake/label.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1283 2024-02-27 08:35:41.000000 layernext-beta-3.3.0b1/layernext/datalake/logger.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     6659 2024-02-27 05:51:27.000000 layernext-beta-3.3.0b1/layernext/datalake/metadata.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1136 2024-02-27 05:51:30.000000 layernext-beta-3.3.0b1/layernext/datalake/model_run.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1166 2024-02-27 05:51:32.000000 layernext-beta-3.3.0b1/layernext/datalake/mongo_json_encoder.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1390 2024-02-27 05:51:37.000000 layernext-beta-3.3.0b1/layernext/datalake/query.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      261 2024-02-27 05:51:39.000000 layernext-beta-3.3.0b1/layernext/datalake/storage_client.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     2696 2024-05-10 07:36:07.000000 layernext-beta-3.3.0b1/layernext/datalake/storage_interface.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     8733 2024-02-27 05:51:44.000000 layernext-beta-3.3.0b1/layernext/datalake/storage_upload.py
+drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2024-05-22 08:09:39.401010 layernext-beta-3.3.0b1/layernext/dataset/
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     3305 2024-02-27 05:52:23.000000 layernext-beta-3.3.0b1/layernext/dataset/__init__.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     4561 2024-02-27 05:52:29.000000 layernext-beta-3.3.0b1/layernext/dataset/dataset.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     9171 2024-02-27 05:52:31.000000 layernext-beta-3.3.0b1/layernext/dataset/datasetinterface.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      431 2024-02-27 05:53:12.000000 layernext-beta-3.3.0b1/layernext/dataset/logger.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)    23610 2024-02-27 05:53:09.000000 layernext-beta-3.3.0b1/layernext/dataset/sync.py
+drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2024-05-22 08:09:39.402163 layernext-beta-3.3.0b1/layernext/studio/
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     3661 2024-02-27 05:53:17.000000 layernext-beta-3.3.0b1/layernext/studio/__init__.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      431 2024-02-27 05:53:20.000000 layernext-beta-3.3.0b1/layernext/studio/logger.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     3860 2024-02-27 05:53:27.000000 layernext-beta-3.3.0b1/layernext/studio/project.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)    13127 2024-02-27 05:54:47.000000 layernext-beta-3.3.0b1/layernext/studio/studiointerface.py
+drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2024-05-22 08:09:39.402928 layernext-beta-3.3.0b1/layernext_beta.egg-info/
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      984 2024-05-22 08:09:39.000000 layernext-beta-3.3.0b1/layernext_beta.egg-info/PKG-INFO
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1469 2024-05-22 08:09:39.000000 layernext-beta-3.3.0b1/layernext_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 channawijerathna   (501) staff       (20)        1 2024-05-22 08:09:39.000000 layernext-beta-3.3.0b1/layernext_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 channawijerathna   (501) staff       (20)       78 2024-05-22 08:09:39.000000 layernext-beta-3.3.0b1/layernext_beta.egg-info/requires.txt
+-rw-r--r--   0 channawijerathna   (501) staff       (20)       10 2024-05-22 08:09:39.000000 layernext-beta-3.3.0b1/layernext_beta.egg-info/top_level.txt
+-rw-r--r--   0 channawijerathna   (501) staff       (20)       38 2024-05-22 08:09:39.403312 layernext-beta-3.3.0b1/setup.cfg
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1950 2024-02-27 05:55:14.000000 layernext-beta-3.3.0b1/setup.py
```

### Comparing `layernext-beta-3.3.0b0/LICENSE` & `layernext-beta-3.3.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/PKG-INFO` & `layernext-beta-3.3.0b1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: layernext-beta
-Version: 3.3.0b0
+Version: 3.3.0b1
 Summary: LayerNext Python SDK
+Home-page: UNKNOWN
 Author: LayerNext
 Author-email: <support@layernext.ai>
+License: UNKNOWN
 Keywords: python,datalake,datasetsync,ai,annotation,layernext,layernext,machine learning
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -33,7 +36,9 @@
 api_key = 'xxxxxxxxxx'
 secret = 'xxxxxxxxxxx'
 url = 'https://api.xxxx.layernext.ai'
 
 client = layernext.LayerNextClient(api_key, secret, url)
 
 ```
+
+
```

### Comparing `layernext-beta-3.3.0b0/layernext/__init__.py` & `layernext-beta-3.3.0b1/layernext/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from deprecated import deprecated
 import uuid
 from layernext.datalake.logger import get_debug_logger
 
 # Create a package-level logger
 logger = get_debug_logger(__name__)
 
-__version__ = "3.3.0b0"
+__version__ = "3.3.0b1"
 
 
 class LayerNextClient:
     """
     Python SDK of LayerNext
     """
```

### Comparing `layernext-beta-3.3.0b0/layernext/automatic_analysis/__init__.py` & `layernext-beta-3.3.0b1/layernext/automatic_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/automatic_analysis/automatic_analysis.py` & `layernext-beta-3.3.0b1/layernext/automatic_analysis/automatic_analysis.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/automatic_analysis/automatic_analysis_interface.py` & `layernext-beta-3.3.0b1/layernext/automatic_analysis/automatic_analysis_interface.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/automatic_analysis/status_check_autoannotate_project.py` & `layernext-beta-3.3.0b1/layernext/automatic_analysis/status_check_autoannotate_project.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/automatic_analysis/support.py` & `layernext-beta-3.3.0b1/layernext/automatic_analysis/support.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/datalake/__init__.py` & `layernext-beta-3.3.0b1/layernext/datalake/__init__.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/datalake/annotation.py` & `layernext-beta-3.3.0b1/layernext/datalake/annotation.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/datalake/aws_s3_client.py` & `layernext-beta-3.3.0b1/layernext/datalake/aws_s3_client.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/datalake/azure_client.py` & `layernext-beta-3.3.0b1/layernext/datalake/azure_client.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/datalake/constants.py` & `layernext-beta-3.3.0b1/layernext/datalake/constants.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/datalake/datalakeinterface.py` & `layernext-beta-3.3.0b1/layernext/datalake/datalakeinterface.py`

 * *Files 0% similar despite different names*

```diff
@@ -2000,15 +2000,15 @@
         #     traceback.print_exc()
         #     return {"success": False, "message": "An unexpected exception occurred"}
 
     def get_metadata_details(self, object_key: dict, fields: List[str]):
         fields = json.dumps(fields)
         fields = urllib.parse.quote(fields)
         hed = {"Authorization": "Basic " + self.auth_token}
-        url = f"{self.dalalake_url}/api/client/metadata/getDetails?objectKey={object_key}&fields={fields}"
+        url = f"{self.dalalake_url}/api/client/metadata/getDetails?objectKey={urllib.parse.quote(object_key)}&fields={fields}"
         res = {}
         try:
             response = requests.get(url=url, json={}, headers=hed)
             status_code = response.status_code
             res = response.json()
         except Exception as e:
             raise Exception(f"{e}")
```

### Comparing `layernext-beta-3.3.0b0/layernext/datalake/file_upload.py` & `layernext-beta-3.3.0b1/layernext/datalake/file_upload.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/datalake/gcs_client.py` & `layernext-beta-3.3.0b1/layernext/datalake/gcs_client.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/datalake/ground_truth.py` & `layernext-beta-3.3.0b1/layernext/datalake/ground_truth.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/datalake/keys.py` & `layernext-beta-3.3.0b1/layernext/datalake/keys.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/datalake/label.py` & `layernext-beta-3.3.0b1/layernext/datalake/label.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/datalake/logger.py` & `layernext-beta-3.3.0b1/layernext/datalake/logger.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/datalake/metadata.py` & `layernext-beta-3.3.0b1/layernext/datalake/metadata.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/datalake/model_run.py` & `layernext-beta-3.3.0b1/layernext/datalake/model_run.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/datalake/mongo_json_encoder.py` & `layernext-beta-3.3.0b1/layernext/datalake/mongo_json_encoder.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/datalake/query.py` & `layernext-beta-3.3.0b1/layernext/datalake/query.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/datalake/storage_interface.py` & `layernext-beta-3.3.0b1/layernext/datalake/storage_interface.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/datalake/storage_upload.py` & `layernext-beta-3.3.0b1/layernext/datalake/storage_upload.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/dataset/__init__.py` & `layernext-beta-3.3.0b1/layernext/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/dataset/dataset.py` & `layernext-beta-3.3.0b1/layernext/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/dataset/datasetinterface.py` & `layernext-beta-3.3.0b1/layernext/dataset/datasetinterface.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/dataset/sync.py` & `layernext-beta-3.3.0b1/layernext/dataset/sync.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/studio/__init__.py` & `layernext-beta-3.3.0b1/layernext/studio/__init__.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/studio/project.py` & `layernext-beta-3.3.0b1/layernext/studio/project.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext/studio/studiointerface.py` & `layernext-beta-3.3.0b1/layernext/studio/studiointerface.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.3.0b0/layernext_beta.egg-info/PKG-INFO` & `layernext-beta-3.3.0b1/layernext_beta.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: layernext-beta
-Version: 3.3.0b0
+Version: 3.3.0b1
 Summary: LayerNext Python SDK
+Home-page: UNKNOWN
 Author: LayerNext
 Author-email: <support@layernext.ai>
+License: UNKNOWN
 Keywords: python,datalake,datasetsync,ai,annotation,layernext,layernext,machine learning
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -33,7 +36,9 @@
 api_key = 'xxxxxxxxxx'
 secret = 'xxxxxxxxxxx'
 url = 'https://api.xxxx.layernext.ai'
 
 client = layernext.LayerNextClient(api_key, secret, url)
 
 ```
+
+
```

### Comparing `layernext-beta-3.3.0b0/layernext_beta.egg-info/SOURCES.txt` & `layernext-beta-3.3.0b1/layernext_beta.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,9 +37,8 @@
 layernext/studio/logger.py
 layernext/studio/project.py
 layernext/studio/studiointerface.py
 layernext_beta.egg-info/PKG-INFO
 layernext_beta.egg-info/SOURCES.txt
 layernext_beta.egg-info/dependency_links.txt
 layernext_beta.egg-info/requires.txt
-layernext_beta.egg-info/top_level.txt
-tests/test_cli.py
+layernext_beta.egg-info/top_level.txt
```

### Comparing `layernext-beta-3.3.0b0/setup.py` & `layernext-beta-3.3.0b1/setup.py`

 * *Files identical despite different names*

