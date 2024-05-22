# Comparing `tmp/prophecy-build-tool-1.2.8.tar.gz` & `tmp/prophecy-build-tool-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophecy-build-tool-1.2.8.tar", last modified: Thu Jan 11 08:57:19 2024, max compression
+gzip compressed data, was "prophecy-build-tool-1.2.9.tar", last modified: Mon Jan 29 17:29:23 2024, max compression
```

## Comparing `prophecy-build-tool-1.2.8.tar` & `prophecy-build-tool-1.2.9.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 08:57:19.687434 prophecy-build-tool-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-01-11 08:57:19.687434 prophecy-build-tool-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-01-11 08:57:19.691434 prophecy-build-tool-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 08:57:19.679434 prophecy-build-tool-1.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 08:57:19.683434 prophecy-build-tool-1.2.8/src/pbt/
--rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 08:57:19.683434 prophecy-build-tool-1.2.8/src/pbt/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 08:57:19.683434 prophecy-build-tool-1.2.8/src/pbt/client/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/client/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/client/airflow/airflow_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/client/airflow/composer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/client/airflow/mwaa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/client/databricks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/client/nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/client/rest_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/client/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 08:57:19.683434 prophecy-build-tool-1.2.8/src/pbt/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/deployment/gems.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 08:57:19.687434 prophecy-build-tool-1.2.8/src/pbt/deployment/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/deployment/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33887 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/deployment/jobs/airflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    34619 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/deployment/jobs/databricks.py
--rw-r--r--   0 runner    (1001) docker     (127)    38283 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/deployment/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/deployment/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 08:57:19.687434 prophecy-build-tool-1.2.8/src/pbt/entities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15167 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/entities/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/pbt_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/process.py
--rw-r--r--   0 runner    (1001) docker     (127)    41311 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/prophecy_build_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 08:57:19.687434 prophecy-build-tool-1.2.8/src/pbt/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19534 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/utils/project_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/src/pbt/utils/project_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 08:57:19.687434 prophecy-build-tool-1.2.8/src/prophecy_build_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-01-11 08:57:19.000000 prophecy-build-tool-1.2.8/src/prophecy_build_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-01-11 08:57:19.000000 prophecy-build-tool-1.2.8/src/prophecy_build_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 08:57:19.000000 prophecy-build-tool-1.2.8/src/prophecy_build_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-11 08:57:19.000000 prophecy-build-tool-1.2.8/src/prophecy_build_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-01-11 08:57:19.000000 prophecy-build-tool-1.2.8/src/prophecy_build_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-11 08:57:19.000000 prophecy-build-tool-1.2.8/src/prophecy_build_tool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 08:57:19.687434 prophecy-build-tool-1.2.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/test/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/test/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-01-11 08:52:41.000000 prophecy-build-tool-1.2.8/test/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:29:23.084328 prophecy-build-tool-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-01-29 17:29:23.084328 prophecy-build-tool-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-01-29 17:29:23.088328 prophecy-build-tool-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:29:23.076327 prophecy-build-tool-1.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:29:23.080327 prophecy-build-tool-1.2.9/src/pbt/
+-rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:29:23.080327 prophecy-build-tool-1.2.9/src/pbt/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:29:23.080327 prophecy-build-tool-1.2.9/src/pbt/client/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/client/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/client/airflow/airflow_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/client/airflow/composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/client/airflow/mwaa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/client/airflow/open_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/client/databricks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/client/nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/client/rest_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/client/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:29:23.080327 prophecy-build-tool-1.2.9/src/pbt/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/deployment/gems.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:29:23.084328 prophecy-build-tool-1.2.9/src/pbt/deployment/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/deployment/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39914 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/deployment/jobs/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34619 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/deployment/jobs/databricks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43769 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/deployment/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/deployment/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:29:23.084328 prophecy-build-tool-1.2.9/src/pbt/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15167 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/entities/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/pbt_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41311 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/prophecy_build_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:29:23.084328 prophecy-build-tool-1.2.9/src/pbt/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20486 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/utils/project_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/src/pbt/utils/project_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:29:23.084328 prophecy-build-tool-1.2.9/src/prophecy_build_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-01-29 17:29:23.000000 prophecy-build-tool-1.2.9/src/prophecy_build_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-01-29 17:29:23.000000 prophecy-build-tool-1.2.9/src/prophecy_build_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 17:29:23.000000 prophecy-build-tool-1.2.9/src/prophecy_build_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-29 17:29:23.000000 prophecy-build-tool-1.2.9/src/prophecy_build_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-01-29 17:29:23.000000 prophecy-build-tool-1.2.9/src/prophecy_build_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-29 17:29:23.000000 prophecy-build-tool-1.2.9/src/prophecy_build_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 17:29:23.084328 prophecy-build-tool-1.2.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/test/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/test/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-01-29 17:24:39.000000 prophecy-build-tool-1.2.9/test/test_testing.py
```

### Comparing `prophecy-build-tool-1.2.8/LICENSE` & `prophecy-build-tool-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.2.8/PKG-INFO` & `prophecy-build-tool-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prophecy-build-tool
-Version: 1.2.8
+Version: 1.2.9
 Summary: Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the Prophecy IDE.
 Home-page: https://github.com/SimpleDataLabsInc/prophecy-build-tool
 Author: Prophecy
 Author-email: maciej@prophecy.io
 Project-URL: Bug Tracker, https://github.com/SimpleDataLabsInc/prophecy-build-tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prophecy-build-tool-1.2.8/README.md` & `prophecy-build-tool-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.2.8/setup.py` & `prophecy-build-tool-1.2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as _in:
     long_description = _in.read()
 
 setuptools.setup(
     name="prophecy-build-tool",
-    version="1.2.8",
+    version="1.2.9",
     author="Prophecy",
     author_email="maciej@prophecy.io",
     description="Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the "
                 "Prophecy IDE.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SimpleDataLabsInc/prophecy-build-tool",
```

### Comparing `prophecy-build-tool-1.2.8/src/pbt/__init__.py` & `prophecy-build-tool-1.2.9/src/pbt/__init__.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.2.8/src/pbt/client/airflow/__init__.py` & `prophecy-build-tool-1.2.9/src/pbt/client/airflow/__init__.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.2.8/src/pbt/client/airflow/composer.py` & `prophecy-build-tool-1.2.9/src/pbt/client/airflow/composer.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.2.8/src/pbt/client/airflow/mwaa.py` & `prophecy-build-tool-1.2.9/src/pbt/client/airflow/mwaa.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,37 +2,39 @@
 import datetime
 import json
 import re
 from abc import ABC
 
 import boto3
 import requests
-from tenacity import retry_if_exception_type, stop_after_attempt, wait_fixed, retry
+from tenacity import retry, retry_if_exception_type, stop_after_attempt, wait_fixed
 
 from . import AirflowRestClient
-from ...utils.exceptions import DagNotAvailableException, DagFileDeletionFailedException, DagUploadFailedException, DagListParsingFailedException
+from ...utils.exceptions import (
+    DagFileDeletionFailedException,
+    DagListParsingFailedException,
+    DagNotAvailableException,
+    DagUploadFailedException,
+)
 from ...utils.project_models import DAG
 
 
 class MWAARestClient(AirflowRestClient, ABC):
-
     def __init__(self, environment_name: str, region: str, access_key: str, secret_key: str):
         self.environment_name = environment_name
         self.aws_s3_client = boto3.client(
-            "s3",
-            region_name=region,
-            aws_access_key_id=access_key,
-            aws_secret_access_key=secret_key
+            "s3", region_name=region, aws_access_key_id=access_key, aws_secret_access_key=secret_key
         )
 
-        self.mwaa_client = boto3.client("mwaa", region_name=region, aws_access_key_id=access_key,
-                                        aws_secret_access_key=secret_key)
+        self.mwaa_client = boto3.client(
+            "mwaa", region_name=region, aws_access_key_id=access_key, aws_secret_access_key=secret_key
+        )
 
         self.environment = self.mwaa_client.get_environment(Name=environment_name)
-        self.dag_s3_path = self.environment['Environment']['DagS3Path']
+        self.dag_s3_path = self.environment["Environment"]["DagS3Path"]
         self._source_bucket = self._extract_bucket_name_from_arn()
 
     def create_secret(self, key: str, value: str) -> bool:
         return True
 
     def delete_dag_file(self, dag_id: str) -> bool:
         relative_path = f"{self.dag_s3_path}/{dag_id}.zip"
@@ -41,15 +43,16 @@
             try:
                 self._get_response("dags delete {dag_id} --yes")
                 return True
             except Exception:
                 return False
         except Exception as e:
             raise DagFileDeletionFailedException(
-                f"Error deleting file {relative_path} from bucket {self._source_bucket}", e)
+                f"Error deleting file {relative_path} from bucket {self._source_bucket}", e
+            )
 
     # todo improve both pause and unpause.
     def pause_dag(self, dag_id: str) -> DAG:
         response_as_text = self._get_response(f"dags pause {dag_id}")
         response_as_json = self._clean_response(response_as_text)
         return DAG(**response_as_json)
 
@@ -61,24 +64,26 @@
 
     def upload_dag(self, dag_id: str, file_path: str):
         relative_path = f"{self.dag_s3_path}/{dag_id}.zip"
         try:
             self.aws_s3_client.upload_file(file_path, self._source_bucket, relative_path)
         except Exception as e:
             print(f"Error uploading file {file_path} to bucket {self._source_bucket}", e)
-            raise DagUploadFailedException(
-                f"Error uploading file {file_path} to bucket {self._source_bucket}", e)
+            raise DagUploadFailedException(f"Error uploading file {file_path} to bucket {self._source_bucket}", e)
 
-    @retry(retry=retry_if_exception_type(DagNotAvailableException), stop=stop_after_attempt(20),
-           wait=wait_fixed(15),
-           reraise=True)
+    @retry(
+        retry=retry_if_exception_type(DagNotAvailableException),
+        stop=stop_after_attempt(20),
+        wait=wait_fixed(15),
+        reraise=True,
+    )
     def get_dag(self, dag_id: str) -> DAG:
         response = self._get_response("dags list -o json")
         dag_list = self._extract_and_load_list_json(response)
-        dag = next((dag for dag in dag_list if dag['dag_id'] == dag_id and dag['paused'] is not None), None)
+        dag = next((dag for dag in dag_list if dag["dag_id"] == dag_id and dag["paused"] is not None), None)
 
         if dag is not None:
             return DAG.create_from_mwaa(dag)
         else:
             raise DagNotAvailableException(f"Dag {dag_id} not found")
 
     def delete_dag(self, dag_id: str) -> str:
@@ -88,58 +93,52 @@
     def _create_cli_token(self):
         return self.mwaa_client.create_cli_token(Name=self.environment_name)
 
     def _expiry_cli_token(self):
         return ExpiringValue(lambda: self._create_cli_token(), 60 * 60 * 24)
 
     def _headers(self):
-        return {
-            "Authorization": f"Bearer {self._expiry_cli_token().get_value()['CliToken']}",
-            "User-Agent": "Prophecy"
-        }
+        return {"Authorization": f"Bearer {self._expiry_cli_token().get_value()['CliToken']}", "User-Agent": "Prophecy"}
 
     def _clean_response(self, text):
         try:
             return json.loads(text)  # Try to parse the text as JSON
         except json.JSONDecodeError:
             # If unsuccessful, perform string transformations and return the result
-            cleaned_text = "{\"" + text.strip() \
-                .replace(", ", "\", \"") \
-                .replace(": ", "\":\"") \
-                .replace(",\"", ", \"") + "\"}"
+            cleaned_text = '{"' + text.strip().replace(", ", '", "').replace(": ", '":"').replace(',"', ', "') + '"}'
             return json.loads(cleaned_text)
 
     def _execute_airflow_command(self, command: str):
         url = f"https://{self._expiry_cli_token().get_value()['WebServerHostname']}/aws_mwaa/cli"
         response = requests.post(url, headers=self._headers(), data=command)
         response.raise_for_status()  # Raise an HTTPError if the status is 4xx, 5xx
         return response.text  # Get the response body as text
 
     def _get_response(self, command: str):
         response_body = self._execute_airflow_command(command)
 
         decoded_response = json.loads(response_body)
 
-        if decoded_response.get('stdout', None) is not None:
-            return base64.b64decode(decoded_response['stdout']).decode('utf-8')
+        if decoded_response.get("stdout", None) is not None:
+            return base64.b64decode(decoded_response["stdout"]).decode("utf-8")
         else:
-            raise Exception(base64.b64decode(decoded_response['stderr']).decode('utf-8'))
+            raise Exception(base64.b64decode(decoded_response["stderr"]).decode("utf-8"))
 
     def _extract_bucket_name_from_arn(self) -> str:
         s3_arn_regex = r"arn:aws:s3:::(.+)"
 
-        match = re.match(s3_arn_regex, self.environment['Environment']['SourceBucketArn'])
+        match = re.match(s3_arn_regex, self.environment["Environment"]["SourceBucketArn"])
         if match:
             return match.group(1)  # Return the captured group
         else:
             raise ValueError(f"No match found for {self.dag_s3_path}")
 
     def _extract_and_load_list_json(self, data):
         # Using regular expression to find the JSON part
-        match = re.search(r'\[.*\]', data)
+        match = re.search(r"\[.*\]", data)
         if match:
             json_part = match.group()
             try:
                 # Parsing the JSON part
                 return json.loads(json_part)
             except json.JSONDecodeError as e:
                 print(f"Error decoding JSON: {e}")
```

### Comparing `prophecy-build-tool-1.2.8/src/pbt/client/databricks.py` & `prophecy-build-tool-1.2.9/src/pbt/client/databricks.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.2.8/src/pbt/client/nexus.py` & `prophecy-build-tool-1.2.9/src/pbt/client/nexus.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.2.8/src/pbt/client/s3.py` & `prophecy-build-tool-1.2.9/src/pbt/client/s3.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.2.8/src/pbt/deployment/__init__.py` & `prophecy-build-tool-1.2.9/src/pbt/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.2.8/src/pbt/deployment/gems.py` & `prophecy-build-tool-1.2.9/src/pbt/deployment/gems.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.2.8/src/pbt/deployment/jobs/airflow.py` & `prophecy-build-tool-1.2.9/src/pbt/deployment/jobs/airflow.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,124 +1,135 @@
 import base64
 import binascii
 import hashlib
 import os
 import zipfile
 from abc import ABC
 from concurrent.futures import ThreadPoolExecutor
-from typing import Dict, Optional, List
+from typing import Dict, List, Optional
 
 import yaml
 
 from .databricks import get_fabric_label
 from ...client.airflow.airflow_utility import create_airflow_client, get_fabric_provider_type
 from ...client.rest_client_factory import RestClientFactory
-from ...deployment import JobInfoAndOperation, OperationType, JobData, EntityIdToFabricId
+from ...deployment import EntityIdToFabricId, JobData, JobInfoAndOperation, OperationType
 from ...entities.project import Project
-from ...utility import custom_print as log, Either
+from ...utility import Either, custom_print as log
 from ...utils.constants import FABRIC_UID
-from ...utils.project_config import JobInfo, ProjectConfig, FabricInfo, update_state, await_futures_and_update_states
-from ...utils.project_models import StepMetadata, Operation, StepType, Colors
+from ...utils.project_config import FabricInfo, JobInfo, ProjectConfig, await_futures_and_update_states, update_state
+from ...utils.project_models import Colors, Operation, StepMetadata, StepType
 
 
 def generate_secure_content(content: str, salt: str) -> str:
     iterations = 10000
     key_length = 128
 
-    password = content.encode('utf-8')
-    salt_bytes = salt.encode('utf-8')
+    password = content.encode("utf-8")
+    salt_bytes = salt.encode("utf-8")
 
-    derived_key = hashlib.pbkdf2_hmac('sha256', password, salt_bytes, iterations, dklen=key_length // 8)
+    derived_key = hashlib.pbkdf2_hmac("sha256", password, salt_bytes, iterations, dklen=key_length // 8)
     hash_bytes = binascii.hexlify(derived_key)
 
-    return base64.b64encode(hash_bytes).decode('utf-8').replace('\\W+', '_')
+    return base64.b64encode(hash_bytes).decode("utf-8").replace("\\W+", "_")
 
 
 def calculate_checksum(input_str, salt=None):
     salt = salt or "better_salt_than_never"
 
     md = hashlib.sha256()
-    input_bytes = input_str.encode('utf-8')
-    salt_bytes = salt.encode('utf-8')
+    input_bytes = input_str.encode("utf-8")
+    salt_bytes = salt.encode("utf-8")
 
     md.update(input_bytes)
     md.update(salt_bytes)
 
     digest_bytes = md.digest()
 
-    return ''.join(f'{byte:02x}' for byte in digest_bytes)
+    return "".join(f"{byte:02x}" for byte in digest_bytes)
 
 
 def does_dag_file_exist(rdc: Dict[str, str]) -> bool:
-    return rdc is not None and 'dag.py' in rdc
+    return rdc is not None and "dag.py" in rdc
 
 
 def filter_job_files(rdc: Dict[str, str]):
-    filtered_files = {file_name: file_content for file_name, file_content in rdc.items()
-                      if
-                      file_name == 'dag.py' or '__init__.py' or file_name == 'prophecy-job.json' or
-                      'tasks/' in file_name}
+    filtered_files = {
+        file_name: file_content
+        for file_name, file_content in rdc.items()
+        if file_name == "dag.py" or "__init__.py" or file_name == "prophecy-job.json" or "tasks/" in file_name
+    }
     k = sorted(filtered_files.items())
     return k
 
 
 def sanitize_job(job_id) -> str:
-    return ('_' if job_id is None else job_id).split('/')[-1].replace('\\W', '_')
+    return ("_" if job_id is None else job_id).split("/")[-1].replace("\\W", "_")
 
 
 def get_zipped_dag_name(dag_name: str):
     return f"/tmp/{dag_name}.zip"
 
 
 def zip_folder(rdc: dict, output_path):
-    with zipfile.ZipFile(output_path, 'w', zipfile.ZIP_STORED) as zipf:
+    with zipfile.ZipFile(output_path, "w", zipfile.ZIP_STORED) as zipf:
         for path, content in rdc.items():
             zipf.writestr(path, content)
 
 
 class AirflowJob(JobData, ABC):
-
-    def __init__(self, job_pbt: dict, prophecy_job_yaml: str, rdc: Dict[str, str], rdc_with_placeholder: Dict[str, str],
-                 sha: Optional[str], fabric_override: Optional[str] = None):
+    def __init__(
+        self,
+        job_pbt: dict,
+        prophecy_job_yaml: str,
+        rdc: Dict[str, str],
+        rdc_with_placeholder: Dict[str, str],
+        sha: Optional[str],
+        fabric_override: Optional[str] = None,
+    ):
         self.job_pbt = job_pbt
         self.prophecy_job_yaml = prophecy_job_yaml
         self.rdc = rdc
         self.rdc_with_placeholder = rdc_with_placeholder
         self.sha = sha
         self.fabric_override = fabric_override
 
         self.prophecy_job_json_dict = self._initialize_prophecy_job_json()
 
     @property
     def name(self):
-        return self.job_pbt.get('name', None)
+        return self.job_pbt.get("name", None)
 
     @property
     def is_valid_job(self):
         prophecy_job_yaml_dict = self.prophecy_job_json_dict
 
-        return self.job_pbt is not None and self.prophecy_job_yaml is not None and self.rdc is not None and \
-            prophecy_job_yaml_dict.get('metainfo', {}).get('fabricId', None) is not None
+        return (
+            self.job_pbt is not None
+            and self.prophecy_job_yaml is not None
+            and self.rdc is not None
+            and prophecy_job_yaml_dict.get("metainfo", {}).get("fabricId", None) is not None
+        )
 
     # we can't use pbt file because it doesn't have fabric per pipeline which airflow jobs supports
     @property
     def pipeline_and_fabric_ids(self) -> List[EntityIdToFabricId]:
         pipeline_and_fabric_ids = []
         prophecy_job_yaml_dict = self.prophecy_job_json_dict
 
         if self.job_pbt is not None and self.prophecy_job_yaml is not None and self.rdc is not None:
-            for process_id, process in prophecy_job_yaml_dict.get('processes', {}).items():
-                properties = process.get('properties', {})
+            for process_id, process in prophecy_job_yaml_dict.get("processes", {}).items():
+                properties = process.get("properties", {})
 
-                cluster_size = properties.get('clusterSize', None)
-                pipeline_id = properties.get('pipelineId', {})
+                cluster_size = properties.get("clusterSize", None)
+                pipeline_id = properties.get("pipelineId", {})
 
                 if cluster_size is not None:
                     # shady stuff but can't help
-                    pipeline_and_fabric_ids.append(EntityIdToFabricId(pipeline_id, cluster_size.split('/')[0]))
+                    pipeline_and_fabric_ids.append(EntityIdToFabricId(pipeline_id, cluster_size.split("/")[0]))
 
         return pipeline_and_fabric_ids
 
     def validate_prophecy_managed_checksum(self, salt: str):
         file_joiner: str = "$$$"
         # always use rdc_with_placeholder to calculate checksum
         content = file_joiner.join(content for (name, content) in filter_job_files(self.rdc_with_placeholder))
@@ -127,39 +138,39 @@
 
     @property
     def job_files(self):
         return filter_job_files(self.rdc)
 
     @property
     def dag_name(self):
-        return self.prophecy_job_json_dict.get('metainfo', {}).get('dagName', None)
+        return self.prophecy_job_json_dict.get("metainfo", {}).get("dagName", None)
 
     @property
     def is_disabled(self):
-        return self.prophecy_job_json_dict.get("metainfo", {}).get('enabled', False) is False
+        return self.prophecy_job_json_dict.get("metainfo", {}).get("enabled", False) is False
 
     @property
     def is_enabled(self):
-        return self.prophecy_job_json_dict.get("metainfo", {}).get('enabled', False) is True
+        return self.prophecy_job_json_dict.get("metainfo", {}).get("enabled", False) is True
 
     @property
     def fabric_id(self):
         if self.fabric_override is not None and len(self.fabric_override) > 0:
             return self.fabric_override
         else:
             fabric_id = self.job_pbt.get(FABRIC_UID)
             return str(fabric_id) if fabric_id is not None else None
 
     @property
     def pipelines(self):
-        return self.job_pbt.get('pipelines', [])
+        return self.job_pbt.get("pipelines", [])
 
     @property
     def has_dbt_component(self):
-        return any(value.get('component', None) == 'dbt' for value in self.prophecy_job_json_dict['processes'].values())
+        return any(value.get("component", None) == "dbt" for value in self.prophecy_job_json_dict["processes"].values())
 
     def _initialize_prophecy_job_json(self) -> dict:
         try:
             return yaml.unsafe_load(self.prophecy_job_yaml)
         except Exception as e:
             log("Error while loading prophecy job yaml", e)
             return {}
@@ -179,16 +190,19 @@
         self._fabrics_config = project_config.fabric_config
 
         self._airflow_clients = {}
         self.deployment_run_override_config = project_config.configs_override
         self._rest_client_factory = RestClientFactory.get_instance(RestClientFactory, self._fabrics_config)
         self._airflow_jobs: Dict[str, AirflowJob] = self._initialize_airflow_jobs()
 
-        (self.valid_airflow_jobs, self._invalid_airflow_jobs,
-         self._airflow_jobs_without_code) = self._initialize_valid_airflow_jobs()
+        (
+            self.valid_airflow_jobs,
+            self._invalid_airflow_jobs,
+            self._airflow_jobs_without_code,
+        ) = self._initialize_valid_airflow_jobs()
 
         self.prophecy_managed_dbt_jobs: Dict[str, AirflowJob] = self._initialize_prophecy_managed_dbt_jobs()
 
     def get_airflow_client(self, fabric_id):
         return self._rest_client_factory.airflow_client(fabric_id)
 
     def summary(self):
@@ -205,88 +219,101 @@
     @property
     def _operation_to_step_id(self):
         return {
             Operation.Remove: self._REMOVE_JOBS_STEP_ID,
             Operation.Add: self._ADD_JOBS_STEP_ID,
             Operation.Pause: self._PAUSE_JOBS_STEP_ID,
             Operation.Rename: self._RENAME_JOBS_STEP_ID,
-            Operation.Skipped: self._SKIP_JOBS_STEP_ID
+            Operation.Skipped: self._SKIP_JOBS_STEP_ID,
         }
 
     def headers(self):
         job_types = {
             Operation.Remove: self._list_remove_jobs(),
             Operation.Add: self._add_jobs(),
             Operation.Pause: self._pause_jobs(),
             Operation.Rename: self._rename_jobs(),
-            Operation.Skipped: self._skip_jobs()
+            Operation.Skipped: self._skip_jobs(),
         }
 
         all_headers = []
 
         for job_action, jobs in job_types.items():
             if jobs:
                 len_jobs = len(jobs)
-                job_header_suffix = f'{len_jobs} Airflow job' if len_jobs == 1 else f'{len_jobs} Airflow jobs'
+                job_header_suffix = f"{len_jobs} Airflow job" if len_jobs == 1 else f"{len_jobs} Airflow jobs"
                 step_id = self._operation_to_step_id[job_action]
                 all_headers.append(
-                    StepMetadata(step_id, f"{job_action.value} {job_header_suffix}",
-                                 job_action, StepType.Job)
+                    StepMetadata(step_id, f"{job_action.value} {job_header_suffix}", job_action, StepType.Job)
                 )
 
         return all_headers
 
     def deploy(self):
         if len(self.headers()) > 0:
             log(f"{Colors.OKBLUE}\n\nDeploying airflow jobs{Colors.ENDC}\n")
 
-        responses = self._deploy_remove_jobs() + self._deploy_pause_jobs() + \
-            self._deploy_add_jobs() + self._deploy_rename_jobs()
+        responses = (
+            self._deploy_remove_jobs()
+            + self._deploy_pause_jobs()
+            + self._deploy_add_jobs()
+            + self._deploy_rename_jobs()
+        )
 
         self._deploy_skipped_jobs()
 
         return responses
 
     def _initialize_airflow_jobs(self):
         jobs = {}
 
         for job_id, parsed_job in self._project.jobs.items():
 
             fabric_override = self.deployment_run_override_config.find_fabric_override_for_job(job_id)
             fabric_override = str(fabric_override) if fabric_override is not None else None
 
-            job_fabric = parsed_job.get('fabricUID', None)
+            job_fabric = parsed_job.get("fabricUID", None)
             job_fabric = str(job_fabric) if job_fabric is not None else None
 
-            does_fabric_exist = self._fabrics_config.get_fabric(
-                job_fabric) is not None or self._fabrics_config.get_fabric(fabric_override) is not None
+            does_fabric_exist = (
+                self._fabrics_config.get_fabric(job_fabric) is not None
+                or self._fabrics_config.get_fabric(fabric_override) is not None
+            )
 
-            if 'Databricks' not in parsed_job.get('scheduler', None) and \
-                    self.deployment_run_override_config.is_job_to_run(job_id) and does_fabric_exist:
+            if (
+                "Databricks" not in parsed_job.get("scheduler", None)
+                and self.deployment_run_override_config.is_job_to_run(job_id)
+                and does_fabric_exist
+            ):
 
                 rdc_with_placeholders = self._project.load_airflow_folder_with_placeholder(job_id)
                 rdc = self._project.load_airflow_folder(job_id)
 
                 aspects = self._project.load_airflow_aspect(job_id)
 
                 prophecy_job_json = None
                 sha = None
 
-                if rdc is not None and 'prophecy-job.json' in rdc:
-                    prophecy_job_json = rdc.get('prophecy-job.json', None)
+                if rdc is not None and "prophecy-job.json" in rdc:
+                    prophecy_job_json = rdc.get("prophecy-job.json", None)
 
                 if aspects is not None:
                     try:
-                        sha = yaml.safe_load(aspects).get('sha', None)
+                        sha = yaml.safe_load(aspects).get("sha", None)
                     except Exception as e:
                         log("Error while loading prophecy job yaml", e)
 
-                jobs[job_id] = AirflowJob(parsed_job, prophecy_job_json, rdc, rdc_with_placeholders, sha,
-                                          fabric_override=self.deployment_run_override_config.find_fabric_override_for_job(
-                                              job_id))
+                jobs[job_id] = AirflowJob(
+                    parsed_job,
+                    prophecy_job_json,
+                    rdc,
+                    rdc_with_placeholders,
+                    sha,
+                    fabric_override=self.deployment_run_override_config.find_fabric_override_for_job(job_id),
+                )
 
         return jobs
 
     def _initialize_valid_airflow_jobs(self):
         valid_airflow_jobs = {}
         invalid_airflow_jobs = {}
         airflow_jobs_without_code = {}
@@ -303,41 +330,43 @@
             else:
                 airflow_jobs_without_code[job_id] = job_data
 
         return valid_airflow_jobs, invalid_airflow_jobs, airflow_jobs_without_code
 
     def _validate_airflow_job(self, job_id: str, job_data: AirflowJob):
 
-        is_prophecy_managed_fabric = self._fabrics_config.is_prophecy_managed(
-            job_data.fabric_id)
+        is_prophecy_managed_fabric = self._fabrics_config.is_prophecy_managed(job_data.fabric_id)
         rdc = job_data.rdc
 
         if does_dag_file_exist(rdc) is False:
             return Either(
-                left=Exception(f"Please open the Job `{job_id}` in editor, check diagnostic errors and release again."))
+                left=Exception(f"Please open the Job `{job_id}` in editor, check diagnostic errors and release again.")
+            )
 
         elif is_prophecy_managed_fabric:
             if job_data.validate_prophecy_managed_checksum(self._project_config.system_config.prophecy_salt):
                 return Either(right=job_data.job_files)
 
             else:
-                return Either(left=Exception(
-                    f"Job `{job_id}` has been externally edited. Please open the Job in editor and release again."))
+                return Either(
+                    left=Exception(
+                        f"Job `{job_id}` has been externally edited. Please open the Job in editor and release again."
+                    )
+                )
         else:
             return Either(right=rdc)
 
     # we won't be able to completely validated the prophecy_job_json structure to prophecy_job.json.
     def _initialize_prophecy_managed_dbt_jobs(self) -> Dict[str, AirflowJob]:
         prophecy_managed_dbt_jobs = {}
 
         for job_id, job_data in self.valid_airflow_jobs.items():
 
             is_job_enabled = job_data.is_enabled
-            is_prophecy_managed_fabric = self._fabrics_config.is_prophecy_managed(
-                job_data.fabric_id)
+            is_prophecy_managed_fabric = self._fabrics_config.is_prophecy_managed(job_data.fabric_id)
 
             if is_job_enabled and is_prophecy_managed_fabric and job_data.has_dbt_component:
                 prophecy_managed_dbt_jobs[job_id] = job_data
 
         return prophecy_managed_dbt_jobs
 
     def _list_remove_jobs(self) -> List[JobInfo]:
@@ -352,60 +381,71 @@
         return await_futures_and_update_states(futures, self._operation_to_step_id[Operation.Remove])
 
     def _remove_job(self, job_info: JobInfo):
         client = self.get_airflow_client(job_info.fabric_id)
 
         try:
             client.delete_dag_file(job_info.external_job_id)
-            log(f"Successfully deleted job {job_info.external_job_id} from job_id {job_info.id}",
-                step_id=self._REMOVE_JOBS_STEP_ID)
+            log(
+                f"Successfully deleted job {job_info.external_job_id} from job_id {job_info.id}",
+                step_id=self._REMOVE_JOBS_STEP_ID,
+            )
             return Either(right=JobInfoAndOperation(job_info, OperationType.DELETED))
 
         except Exception as e:
-            log(f"Error while deleting job {job_info.external_job_id} from job_id {job_info.id}, Please delete the Dag manually from Dag location if required.",
+            log(
+                f"Error while deleting job {job_info.external_job_id} from job_id {job_info.id}, Please delete the Dag manually from Dag location if required.",
                 exception=e,
-                step_id=self._REMOVE_JOBS_STEP_ID)
+                step_id=self._REMOVE_JOBS_STEP_ID,
+            )
             return Either(right=JobInfoAndOperation(job_info, OperationType.DELETED))
 
-    '''
+    """
         Compare what exists in state config to what exists in code.
-     '''
+     """
 
     def _jobs_to_be_deleted(self) -> List[JobInfo]:
         all_jobs = {**self.valid_airflow_jobs, **self._invalid_airflow_jobs, **self._airflow_jobs_without_code}
         return [
-            airflow_job for airflow_job in self._jobs_state.airflow_jobs
+            airflow_job
+            for airflow_job in self._jobs_state.airflow_jobs
             if not any(
                 airflow_job.id == job_id
-                for job_id in list(all_jobs.keys())  # check from available airflow jobs.
-            ) and self._fabrics_config.get_fabric(airflow_job.fabric_id) is not None
+                for job_id in list(all_jobs.keys())
+                # check from available airflow jobs.
+            )
+            and self._fabrics_config.get_fabric(airflow_job.fabric_id) is not None
         ]
 
-    '''
+    """
         There exist a job in folder whose fabric id is different from the one in state config.
         folder can only have one job with a given job id.
-    '''
+    """
 
     def _jobs_with_fabric_changed(self) -> List[JobInfo]:
 
         return [
-            airflow_job for airflow_job in self._jobs_state.airflow_jobs
+            airflow_job
+            for airflow_job in self._jobs_state.airflow_jobs
             if any(
                 airflow_job.id == job_id and airflow_job.fabric_id != job_data.fabric_id
-                for job_id, job_data in self.valid_airflow_jobs.items()  # Check only from valid airflow jobs.
+                for job_id, job_data in self.valid_airflow_jobs.items()
+                # Check only from valid airflow jobs.
             )
         ]
 
     def _rename_jobs(self) -> List[JobInfo]:
         return [
-            airflow_job for airflow_job in self._jobs_state.airflow_jobs
-
+            airflow_job
+            for airflow_job in self._jobs_state.airflow_jobs
             if any(
-                airflow_job.id == job_id and airflow_job.fabric_id == job_data.fabric_id and
-                job_data.is_enabled and airflow_job.external_job_id != job_data.dag_name
+                airflow_job.id == job_id
+                and airflow_job.fabric_id == job_data.fabric_id
+                and job_data.is_enabled
+                and airflow_job.external_job_id != job_data.dag_name
                 for job_id, job_data in self.valid_airflow_jobs.items()
             )
         ]
 
     def _all_removed_airflow_jobs(self) -> List[JobInfo]:
         return self._rename_jobs() + self._jobs_with_fabric_changed() + self._jobs_to_be_deleted()
 
@@ -415,37 +455,33 @@
     def _pause_jobs(self) -> Dict[str, JobInfo]:
         old_enabled_job = {job.id: job for job in self._jobs_state.airflow_jobs if job.is_paused is False}
 
         old_enabled_job_which_are_disabled_in_new = {
             job_id: job_info
             for job_id, job_info in old_enabled_job.items()
             if any(
-                job_id == _id and job_info.fabric_id == job_data.fabric_id and job_data.is_disabled  # disabled in new
+                job_id == _id and job_info.fabric_id == job_data.fabric_id and job_data.is_disabled
+                # disabled in new
                 for _id, job_data in self.valid_airflow_jobs.items()
             )
         }
 
         jobs_not_in_removed_jobs = {
             job_id: job_info
             for job_id, job_info in old_enabled_job_which_are_disabled_in_new.items()
-            if not self._all_removed_airflow_jobs() and not any(
-                airflow_job.id == job_id
-                for airflow_job in self._all_removed_airflow_jobs()
-            )
+            if not self._all_removed_airflow_jobs()
+            and not any(airflow_job.id == job_id for airflow_job in self._all_removed_airflow_jobs())
         }
 
         return jobs_not_in_removed_jobs
 
     # always add new jobs only if they are enabled.
     # this is equivalent to refresh because airflow merge based on it's dag_name.
     def _add_jobs(self) -> Dict[str, AirflowJob]:
-        return {
-            job_id: job_data for job_id, job_data in self.valid_airflow_jobs.items()
-            if job_data.is_enabled is True
-        }
+        return {job_id: job_data for job_id, job_data in self.valid_airflow_jobs.items() if job_data.is_enabled is True}
 
     def _deploy_add_jobs(self):
         futures = []
 
         with ThreadPoolExecutor(max_workers=10) as executor:
             for job_id, job_data in self._add_jobs().items():
                 futures.append(executor.submit(lambda j_id=job_id, j_data=job_data: self._add_job(j_id, j_data)))
@@ -462,68 +498,93 @@
         fabric_name = fabric_config.name if fabric_config is not None else None
 
         fabric_label = get_fabric_label(fabric_name, job_data.fabric_id)
         try:
             client.upload_dag(dag_name, zipped_dag_name)
             try:
                 client.unpause_dag(dag_name)
-                log(f"{Colors.OKGREEN}Successfully un-paused dag:{dag_name} for job:{job_id} and fabric:{fabric_label}{Colors.ENDC}",
-                    step_id=self._ADD_JOBS_STEP_ID)
+                log(
+                    f"{Colors.OKGREEN}Successfully un-paused dag:{dag_name} for job:{job_id} and fabric:{fabric_label}{Colors.ENDC}",
+                    step_id=self._ADD_JOBS_STEP_ID,
+                )
             except Exception as e:
-                log(f"{Colors.FAIL}Failed to un-pause dag with name:{dag_name} for job:{job_id} and fabric:{fabric_label}{Colors.ENDC}",
-                    exception=e, step_id=self._ADD_JOBS_STEP_ID)
+                log(
+                    f"{Colors.FAIL}Failed to un-pause dag with name:{dag_name} for job:{job_id} and fabric:{fabric_label}{Colors.ENDC}",
+                    exception=e,
+                    step_id=self._ADD_JOBS_STEP_ID,
+                )
 
                 return Either(left=e)
 
-            log(f"{Colors.OKGREEN}Successfully added job:{dag_name} for job_id:{job_id} on fabric:{fabric_label}{Colors.ENDC}",
-                step_id=self._ADD_JOBS_STEP_ID)
+            log(
+                f"{Colors.OKGREEN}Successfully added job:{dag_name} for job_id:{job_id} on fabric:{fabric_label}{Colors.ENDC}",
+                step_id=self._ADD_JOBS_STEP_ID,
+            )
 
-            job_info = JobInfo.create_job(job_data.name, job_id, job_data.fabric_id, dag_name,
-                                          self._project.release_tag,
-                                          job_data.is_disabled,
-                                          get_fabric_provider_type(job_data.fabric_id, self._project_config))
+            job_info = JobInfo.create_job(
+                job_data.name,
+                job_id,
+                job_data.fabric_id,
+                dag_name,
+                self._project.release_tag,
+                job_data.is_disabled,
+                get_fabric_provider_type(job_data.fabric_id, self._project_config),
+            )
 
             return Either(right=JobInfoAndOperation(job_info, OperationType.CREATED))
         except Exception as e:
-            log(f"{Colors.FAIL}Failed to upload_dag for job_id:{job_id} with dag_name {dag_name}{Colors.ENDC}", e,
-                step_id=self._ADD_JOBS_STEP_ID)
+            log(
+                f"{Colors.FAIL}Failed to upload_dag for job_id:{job_id} with dag_name {dag_name}{Colors.ENDC}",
+                e,
+                step_id=self._ADD_JOBS_STEP_ID,
+            )
             return Either(left=e)
 
     def _deploy_skipped_jobs(self):
         for job_id, message in self._skip_jobs().items():
-            log(f"Skipping job_id: {job_id} encountered some error ", exception=message.left,
-                step_id=self._SKIP_JOBS_STEP_ID)
+            log(
+                f"Skipping job_id: {job_id} encountered some error ",
+                exception=message.left,
+                step_id=self._SKIP_JOBS_STEP_ID,
+            )
         if len(self._skip_jobs()) > 0:
             update_state([Either(right=True)], self._operation_to_step_id[Operation.Skipped])
 
     def _skip_jobs(self):
-        return {job_id: self._validate_airflow_job(job_id, job_data)
-                for job_id, job_data in self._airflow_jobs.items()
-                if self._validate_airflow_job(job_id, job_data).is_left}
+        return {
+            job_id: self._validate_airflow_job(job_id, job_data)
+            for job_id, job_data in self._airflow_jobs.items()
+            if self._validate_airflow_job(job_id, job_data).is_left
+        }
 
     def _deploy_rename_jobs(self):
         futures = []
         with ThreadPoolExecutor(max_workers=10) as executor:
             for job_info in self._rename_jobs():
                 futures.append(executor.submit(lambda j_info=job_info: self._delete_job_for_renamed_job(j_info)))
 
         return await_futures_and_update_states(futures, self._operation_to_step_id[Operation.Rename])
 
     def _delete_job_for_renamed_job(self, jobs_info: JobInfo):
         try:
             client = create_airflow_client(jobs_info.fabric_id, self._project_config)
             client.delete_dag(sanitize_job(jobs_info.external_job_id))
 
-            log(f"{Colors.OKGREEN}Successfully deleted dag for job_id: {jobs_info.id}{Colors.ENDC}",
-                step_id=self._RENAME_JOBS_STEP_ID)
+            log(
+                f"{Colors.OKGREEN}Successfully deleted dag for job_id: {jobs_info.id}{Colors.ENDC}",
+                step_id=self._RENAME_JOBS_STEP_ID,
+            )
 
             return Either(right=JobInfoAndOperation(jobs_info, OperationType.DELETED))
         except Exception as e:
-            log(f"{Colors.WARNING}Failed to delete dag for job_id: {jobs_info.id} with job name {jobs_info.external_job_id} in fabric {jobs_info.fabric_id}, Please delete the Dag manually from Dag location if required.{Colors.ENDC}",
-                exception=e, step_id=self._RENAME_JOBS_STEP_ID)
+            log(
+                f"{Colors.WARNING}Failed to delete dag for job_id: {jobs_info.id} with job name {jobs_info.external_job_id} in fabric {jobs_info.fabric_id}, Please delete the Dag manually from Dag location if required.{Colors.ENDC}",
+                exception=e,
+                step_id=self._RENAME_JOBS_STEP_ID,
+            )
             return Either(right=JobInfoAndOperation(jobs_info, OperationType.DELETED))
 
     def _deploy_pause_jobs(self):
         futures = []
         with ThreadPoolExecutor(max_workers=10) as executor:
             for job_id, job_data in self._pause_jobs().items():
                 futures.append(executor.submit(lambda j_id=job_id, j_data=job_data: self._pause_job(j_id, j_data)))
@@ -537,29 +598,32 @@
             dag_name = job_info.external_job_id
         else:
             dag_name = sanitize_job(job_id)
 
         job_info.pause(True)
         try:
             client.pause_dag(dag_name)
-            log(f"{Colors.OKGREEN}Successfully paused job {dag_name} for job_id {job_id}{Colors.ENDC}",
-                step_id=self._PAUSE_JOBS_STEP_ID)
+            log(
+                f"{Colors.OKGREEN}Successfully paused job {dag_name} for job_id {job_id}{Colors.ENDC}",
+                step_id=self._PAUSE_JOBS_STEP_ID,
+            )
             return Either(right=JobInfoAndOperation(job_info, OperationType.REFRESH))
         except Exception as e:
-            log(f"{Colors.WARNING}Failed to pause_dag for job_id: {job_id} with dag_name {dag_name}{Colors.ENDC}",
+            log(
+                f"{Colors.WARNING}Failed to pause_dag for job_id: {job_id} with dag_name {dag_name}{Colors.ENDC}",
                 exception=e,
-                step_id=self._PAUSE_JOBS_STEP_ID)
+                step_id=self._PAUSE_JOBS_STEP_ID,
+            )
             return Either(right=JobInfoAndOperation(job_info, OperationType.REFRESH))
 
 
 class AirflowGitSecrets:
     _AIRFLOW_GIT_SECRETS_STEP_ID = "airflow-git-secrets"
 
-    def __init__(self, project: Project, airflow_jobs: AirflowJobDeployment,
-                 project_config: ProjectConfig):
+    def __init__(self, project: Project, airflow_jobs: AirflowJobDeployment, project_config: ProjectConfig):
         self.project = project
         self.airflow_jobs = airflow_jobs
         self.project_config = project_config
         self.deployment_state = project_config.jobs_state
         self.fabric_config = project_config.fabric_config
 
     def summary(self) -> List[str]:
@@ -575,16 +639,21 @@
                     summary.append(f"Creating git secrets for project {project_id} ")
 
         return summary
 
     def headers(self) -> List[StepMetadata]:
         if len(self.airflow_jobs.prophecy_managed_dbt_jobs) > 0:
             return [
-                StepMetadata(self._AIRFLOW_GIT_SECRETS_STEP_ID, "Create git secrets for airflow jobs", Operation.Build,
-                             StepType.AirflowGitSecrets)]
+                StepMetadata(
+                    self._AIRFLOW_GIT_SECRETS_STEP_ID,
+                    "Create git secrets for airflow jobs",
+                    Operation.Build,
+                    StepType.AirflowGitSecrets,
+                )
+            ]
         else:
             return []
 
     def deploy(self):
 
         futures = []
 
@@ -597,48 +666,58 @@
 
             with ThreadPoolExecutor(max_workers=10) as executor:
                 for project_git_tokens in self.fabric_config.project_git_tokens:
                     git_tokens = project_git_tokens.git_token
                     project_id = project_git_tokens.project_id
 
                     if len(git_tokens) == 0:
-                        log(f"{Colors.WARNING}No git tokens found for project_id: {project_id}, Ignoring{Colors.ENDC}",
-                            step_id=self._AIRFLOW_GIT_SECRETS_STEP_ID)
+                        log(
+                            f"{Colors.WARNING}No git tokens found for project_id: {project_id}, Ignoring{Colors.ENDC}",
+                            step_id=self._AIRFLOW_GIT_SECRETS_STEP_ID,
+                        )
 
                     else:
                         futures.append(
                             executor.submit(
                                 lambda p_id=project_id, j_data=job_data, token=git_tokens: self._create_git_secrets(
-                                    p_id, j_data, token)))
+                                    p_id, j_data, token
+                                )
+                            )
+                        )
 
             return await_futures_and_update_states(futures, self._AIRFLOW_GIT_SECRETS_STEP_ID)
         else:
             # log("No dbt jobs found, Ignoring", step_id=self._AIRFLOW_GIT_SECRETS_STEP_ID)
             return []
 
     def _create_git_secrets(self, project_id, job_data, git_tokens):
         # todo fix this
-        execution_db_suffix = os.getenv('EXECUTION_DB_SUFFIX', 'dev')
+        execution_db_suffix = os.getenv("EXECUTION_DB_SUFFIX", "dev")
         client = self.airflow_jobs.get_airflow_client(job_data.fabric_id)
         try:
             client.create_secret(
-                generate_secure_content(f'{execution_db_suffix}_{project_id}', 'gitSecretSalt'), git_tokens)
-            log(f'{Colors.OKGREEN}Successfully created git secrets for project {project_id}{Colors.ENDC}',
-                step_id=self._AIRFLOW_GIT_SECRETS_STEP_ID)
+                generate_secure_content(f"{execution_db_suffix}_{project_id}", "gitSecretSalt"), git_tokens
+            )
+            log(
+                f"{Colors.OKGREEN}Successfully created git secrets for project {project_id}{Colors.ENDC}",
+                step_id=self._AIRFLOW_GIT_SECRETS_STEP_ID,
+            )
 
         except Exception as e:
-            log(f'{Colors.WARNING}Failed in creating git secrets for project {project_id}{Colors.ENDC}', exception=e,
-                step_id=self._AIRFLOW_GIT_SECRETS_STEP_ID)
+            log(
+                f"{Colors.WARNING}Failed in creating git secrets for project {project_id}{Colors.ENDC}",
+                exception=e,
+                step_id=self._AIRFLOW_GIT_SECRETS_STEP_ID,
+            )
 
 
 class EMRPipelineConfigurations:
     _STEP_ID = "EMR_pipeline_configurations"
 
-    def __init__(self, project: Project, airflow_jobs: AirflowJobDeployment,
-                 project_config: ProjectConfig):
+    def __init__(self, project: Project, airflow_jobs: AirflowJobDeployment, project_config: ProjectConfig):
         self.airflow_jobs = airflow_jobs
         self.pipeline_configurations = project.pipeline_configurations
         self.project_config = project_config
         self.project = project
         self._jobs_state = project_config.jobs_state
         self._fabric_config = project_config.fabric_config
         self._rest_client_factory = RestClientFactory.get_instance(RestClientFactory, self._fabric_config)
@@ -653,40 +732,51 @@
                 summary.append(f"Uploading pipeline emr-configurations for pipeline {ids}")
 
         return summary
 
     def headers(self) -> List[StepMetadata]:
         all_configs = [value for sublist in self.pipeline_configurations.values() for value in sublist]
         if len(all_configs) > 0 and len(self._emr_fabrics()) > 0:
-            return [StepMetadata(self._STEP_ID,
-                                 f"Upload {len(all_configs)} pipeline emr-configurations",
-                                 Operation.Upload, StepType.PipelineConfiguration)]
+            return [
+                StepMetadata(
+                    self._STEP_ID,
+                    f"Upload {len(all_configs)} pipeline emr-configurations",
+                    Operation.Upload,
+                    StepType.PipelineConfiguration,
+                )
+            ]
         else:
             return []
 
     def deploy(self):
 
         futures = []
 
         with ThreadPoolExecutor(max_workers=10) as executor:
             if len(self.headers()) > 0:
                 log(f"\n\n{Colors.OKBLUE}Uploading EMR pipeline configurations {Colors.ENDC}\n\n")
 
             def execute_job(_fabric_info, _config_content, _config_path):
-                futures.append(executor.submit(
-                    lambda f_info=_fabric_info, conf_content=_config_content, conf_path=_config_path:
-                    self._upload_configuration(f_info, conf_content, conf_path)))
+                futures.append(
+                    executor.submit(
+                        lambda f_info=_fabric_info, conf_content=_config_content, conf_path=_config_path: self._upload_configuration(
+                            f_info, conf_content, conf_path
+                        )
+                    )
+                )
 
             for pipeline_id, configurations in self.pipeline_configurations.items():
 
                 path = self.project_config.system_config.get_s3_base_path()
-                pipeline_path = f'{path}/{self.project.project_id}/{self.project.release_version}/configurations/{pipeline_id}'
+                pipeline_path = (
+                    f"{path}/{self.project.project_id}/{self.project.release_version}/configurations/{pipeline_id}"
+                )
 
                 for configuration_name, configuration_content in configurations.items():
-                    configuration_path = f'{pipeline_path}/{configuration_name}.jsn'
+                    configuration_path = f"{pipeline_path}/{configuration_name}.jsn"
 
                     for fabric_info in self._fabric_config.emr_fabrics():
 
                         if fabric_info.emr is not None:
                             execute_job(fabric_info, configuration_content, configuration_path)
 
         return await_futures_and_update_states(futures, self._STEP_ID)
@@ -695,31 +785,34 @@
         upload_path = f"{fabric_info.emr.bare_path_prefix()}/{configuration_path}"
         emr_info = fabric_info.emr
 
         try:
             client = self._rest_client_factory.s3_client(str(fabric_info.id))
             client.upload_content(emr_info.bare_bucket(), upload_path, configuration_content)
 
-            log(f"{Colors.OKGREEN}Uploaded pipeline configuration on path {upload_path} on fabric {fabric_info.id}{Colors.ENDC}",
-                step_id=self._STEP_ID)
+            log(
+                f"{Colors.OKGREEN}Uploaded pipeline configuration on path {upload_path} on fabric {fabric_info.id}{Colors.ENDC}",
+                step_id=self._STEP_ID,
+            )
 
             return Either(right=True)
 
         except Exception as e:
-            log(f"{Colors.FAIL}Failed to upload pipeline configuration for path {upload_path} for fabric {fabric_info.id}{Colors.ENDC}",
+            log(
+                f"{Colors.FAIL}Failed to upload pipeline configuration for path {upload_path} for fabric {fabric_info.id}{Colors.ENDC}",
                 exception=e,
-                step_id=self._STEP_ID)
+                step_id=self._STEP_ID,
+            )
             return Either(left=e)
 
 
 class DataprocPipelineConfigurations:
     _STEP_ID = "DATAPROC_pipeline_configurations"
 
-    def __init__(self, project: Project, airflow_jobs: AirflowJobDeployment,
-                 project_config: ProjectConfig):
+    def __init__(self, project: Project, airflow_jobs: AirflowJobDeployment, project_config: ProjectConfig):
         self.airflow_jobs = airflow_jobs
         self.pipeline_configurations = project.pipeline_configurations
         self.project = project
         self.project_config = project_config
         self._deployment_state = project_config.jobs_state
         self._fabric_config = project_config.fabric_config
         self._rest_client_factory = RestClientFactory.get_instance(RestClientFactory, self._fabric_config)
@@ -734,37 +827,48 @@
                 summary.append(f"Uploading pipeline dataproc-configurations for pipeline {ids}")
 
         return summary
 
     def headers(self) -> List[StepMetadata]:
         all_configs = [value for sublist in self.pipeline_configurations.values() for value in sublist]
         if len(all_configs) > 0 and len(self._dataproc_fabrics()) > 0:
-            return [StepMetadata(self._STEP_ID,
-                                 f"Upload {len(all_configs)} pipeline dataproc-configurations",
-                                 Operation.Upload, StepType.PipelineConfiguration)]
+            return [
+                StepMetadata(
+                    self._STEP_ID,
+                    f"Upload {len(all_configs)} pipeline dataproc-configurations",
+                    Operation.Upload,
+                    StepType.PipelineConfiguration,
+                )
+            ]
         else:
             return []
 
     def deploy(self):
         futures = []
 
         with ThreadPoolExecutor(max_workers=10) as executor:
             if len(self.headers()) > 0:
                 log(f"\n\n{Colors.OKBLUE} Uploading dataproc configurations {Colors.ENDC}\n\n")
 
             def execute_job(fabric_info, configuration_content, configuration_path):
-                futures.append(executor.submit(
-                    lambda f_info=fabric_info, conf_content=configuration_content, conf_path=configuration_path:
-                    self._upload_configuration(f_info, conf_content, conf_path)))
+                futures.append(
+                    executor.submit(
+                        lambda f_info=fabric_info, conf_content=configuration_content, conf_path=configuration_path: self._upload_configuration(
+                            f_info, conf_content, conf_path
+                        )
+                    )
+                )
 
             for pipeline_id, configurations in self.pipeline_configurations.items():
                 path = self.project_config.system_config.get_s3_base_path()
-                pipeline_path = f'{path}/{self.project.project_id}/{self.project.release_version}/configurations/{pipeline_id}'
+                pipeline_path = (
+                    f"{path}/{self.project.project_id}/{self.project.release_version}/configurations/{pipeline_id}"
+                )
                 for configuration_name, configuration_content in configurations.items():
-                    configuration_path = f'{pipeline_path}/{configuration_name}.jsn'
+                    configuration_path = f"{pipeline_path}/{configuration_name}.jsn"
 
                     for fabric_info in self._fabric_config.dataproc_fabrics():
 
                         if fabric_info.dataproc is not None:
                             execute_job(fabric_info, configuration_content, configuration_path)
 
         return await_futures_and_update_states(futures, self._STEP_ID)
@@ -772,17 +876,121 @@
     def _upload_configuration(self, fabric_info: FabricInfo, configuration_content, configuration_path):
         upload_path = f"{fabric_info.dataproc.bare_path_prefix()}/{configuration_path}"
         dataproc_info = fabric_info.dataproc
         try:
             client = self._rest_client_factory.dataproc_client(str(fabric_info.id))
             client.put_object(dataproc_info.bare_bucket(), upload_path, configuration_content)
 
-            log(f"{Colors.OKGREEN}Uploaded pipeline configuration on path {upload_path}{Colors.ENDC}",
-                step_id=self._STEP_ID)
+            log(
+                f"{Colors.OKGREEN}Uploaded pipeline configuration on path {upload_path}{Colors.ENDC}",
+                step_id=self._STEP_ID,
+            )
+
+            return Either(right=True)
+
+        except Exception as e:
+            log(
+                f"{Colors.FAIL}Failed to upload pipeline configuration for path {upload_path} for fabric {fabric_info.id}{Colors.ENDC}",
+                exception=e,
+                step_id=self._STEP_ID,
+            )
+            return Either(left=e)
+
+
+class SparkSubmitPipelineConfigurations:
+    _STEP_ID = "SPARK_SUBMIT_pipeline_configurations"
+
+    def __init__(self, project: Project, airflow_jobs: AirflowJobDeployment, project_config: ProjectConfig):
+        self.airflow_jobs = airflow_jobs
+        self.pipeline_configurations = project.pipeline_configurations
+        self.project = project
+        self.project_config = project_config
+        self._deployment_state = project_config.jobs_state
+        self._fabric_config = project_config.fabric_config
+        self._rest_client_factory = RestClientFactory.get_instance(RestClientFactory, self._fabric_config)
+
+    def _spark_submit_fabrics(self):
+        return self._fabric_config.airflow_open_source_fabrics()
+
+    def summary(self) -> List[str]:
+        summary = []
+        for ids in self.pipeline_configurations.keys():
+            if len(self._spark_submit_fabrics()) > 0:
+                summary.append(f"Uploading pipeline spark-submit-configurations for pipeline {ids}")
+
+        return summary
+
+    def headers(self) -> List[StepMetadata]:
+        all_configs = [value for sublist in self.pipeline_configurations.values() for value in sublist]
+        if len(all_configs) > 0 and len(self._spark_submit_fabrics()) > 0:
+            return [
+                StepMetadata(
+                    self._STEP_ID,
+                    f"Upload {len(all_configs)} pipeline spark-submit-configurations",
+                    Operation.Upload,
+                    StepType.PipelineConfiguration,
+                )
+            ]
+        else:
+            return []
+
+    def deploy(self):
+        futures = []
+
+        with ThreadPoolExecutor(max_workers=10) as executor:
+            if len(self.headers()) > 0:
+                log(f"\n\n{Colors.OKBLUE} Uploading spark-submit configurations {Colors.ENDC}\n\n")
+
+            def execute_job(
+                fabric_info, configuration_relative_directory, configuration_file_name, configuration_content
+            ):
+                futures.append(
+                    executor.submit(
+                        lambda f_info=fabric_info, conf_content=configuration_content, conf_path=f"{configuration_relative_directory}/{configuration_file_name}": self._upload_configuration(
+                            f_info, configuration_relative_directory, configuration_file_name, configuration_content
+                        )
+                    )
+                )
+
+            for pipeline_id, configurations in self.pipeline_configurations.items():
+                path = self.project_config.system_config.get_hdfs_base_path()
+                pipeline_path = (
+                    f"{path}/{self.project.project_id}/{self.project.release_version}/configurations/{pipeline_id}"
+                )
+                for configuration_name, configuration_content in configurations.items():
+                    configuration_file_name = f"{configuration_name}.jsn"
+                    configuration_relative_directory = pipeline_path
+
+                    for fabric_info in self._spark_submit_fabrics():
+
+                        if fabric_info.airflow_oss is not None:
+                            execute_job(
+                                fabric_info,
+                                configuration_relative_directory,
+                                configuration_file_name,
+                                configuration_content,
+                            )
+
+        return await_futures_and_update_states(futures, self._STEP_ID)
+
+    def _upload_configuration(
+        self, fabric_info: FabricInfo, configuration_relative_directory, configuration_file_name, configuration_content
+    ):
+        upload_directory = f"{fabric_info.airflow_oss.location}/{configuration_relative_directory}"
+        try:
+            client = self._rest_client_factory.open_source_hdfs_client(str(fabric_info.id))
+            client.put_object(upload_directory, configuration_file_name, configuration_content)
+
+            log(
+                f"{Colors.OKGREEN}Uploaded pipeline configuration on path {upload_directory}{Colors.ENDC}",
+                step_id=self._STEP_ID,
+            )
 
             return Either(right=True)
 
         except Exception as e:
-            log(f"{Colors.FAIL}Failed to upload pipeline configuration for path {upload_path} for fabric {fabric_info.id}{Colors.ENDC}",
+            log(
+                f"{Colors.FAIL}Failed to upload pipeline configuration for path {upload_directory} for fabric {fabric_info.id}{Colors.ENDC}",
                 exception=e,
-                step_id=self._STEP_ID)
+                step_id=self._STEP_ID,
+            )
             return Either(left=e)
```

### Comparing `prophecy-build-tool-1.2.8/src/pbt/deployment/jobs/databricks.py` & `prophecy-build-tool-1.2.9/src/pbt/deployment/jobs/databricks.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.2.8/src/pbt/deployment/pipeline.py` & `prophecy-build-tool-1.2.9/src/pbt/deployment/pipeline.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,48 +3,57 @@
 import re
 import subprocess
 import sys
 import tempfile
 import threading
 from abc import ABC, abstractmethod
 from concurrent.futures import ThreadPoolExecutor, as_completed
-from typing import Optional, List, Dict
+from typing import Dict, List, Optional
 
 from requests import HTTPError
 
 from . import JobData
 from ..client.nexus import NexusClient
 from ..client.rest_client_factory import RestClientFactory
 from ..deployment.jobs.airflow import AirflowJobDeployment
 from ..deployment.jobs.databricks import DatabricksJobsDeployment, get_fabric_label
 from ..entities.project import Project, is_cross_project_pipeline
-from ..utility import custom_print as log, Either, is_online_mode
+from ..utility import Either, custom_print as log, is_online_mode
 from ..utils.constants import SCALA_LANGUAGE
 from ..utils.exceptions import ProjectBuildFailedException
-from ..utils.project_config import ProjectConfig, EMRInfo, DataprocInfo, DeploymentMode
-from ..utils.project_models import StepMetadata, Operation, StepType, Status, LogLevel, Colors
+from ..utils.project_config import DataprocInfo, DeploymentMode, EMRInfo, OpenSourceAirflowInfo, ProjectConfig
+from ..utils.project_models import Colors, LogLevel, Operation, Status, StepMetadata, StepType
 
 
 def get_package_name(project_language: str, pipeline_name: str):
     if project_language == SCALA_LANGUAGE:
-        return f'{pipeline_name}.jar'
+        return f"{pipeline_name}.jar"
     else:
-        # todo combine in a single regex
-        regex_match = r"[^\w\d.]+"
-        underscore_regex = r"(_)\1+"
-        result = re.sub(regex_match, "_", pipeline_name)
-        result = re.sub(underscore_regex, "_", result)
-        return f'{result}-1.0-py3-none-any.whl'
+        result = python_pipeline_name(pipeline_name)
+        return f"{result}-1.0-py3-none-any.whl"
+
+
+def python_pipeline_name(pipeline_name: str):
+    # todo combine in a single regex
+    regex_match = r"[^\w\d.]+"
+    underscore_regex = r"(_)\1+"
+    result = re.sub(regex_match, "_", pipeline_name)
+    return re.sub(underscore_regex, "_", result)
 
 
 class PipelineDeployment:
-    def __init__(self, project: Project, databricks_jobs: DatabricksJobsDeployment,
-                 airflow_jobs: AirflowJobDeployment,
-                 project_config: ProjectConfig, job_ids: Optional[List[str]] = None,
-                 pipelines_to_build: Optional[List[str]] = None):
+    def __init__(
+        self,
+        project: Project,
+        databricks_jobs: DatabricksJobsDeployment,
+        airflow_jobs: AirflowJobDeployment,
+        project_config: ProjectConfig,
+        job_ids: Optional[List[str]] = None,
+        pipelines_to_build: Optional[List[str]] = None,
+    ):
 
         self.job_ids = job_ids
         self.pipelines_to_build = pipelines_to_build
 
         self.databricks_jobs = databricks_jobs
         self.airflow_jobs = airflow_jobs
 
@@ -54,55 +63,63 @@
         self.are_tests_enabled = project_config.configs_override.tests_enabled
 
         self.pipeline_id_to_local_path = {}
         self.has_pipelines = False  # in case deployment doesn't have any pipelines.
 
     @property
     def _all_jobs(self) -> Dict[str, JobData]:
-        return {
-            **self.databricks_jobs.valid_databricks_jobs,
-            **self.airflow_jobs.valid_airflow_jobs
-        }
+        return {**self.databricks_jobs.valid_databricks_jobs, **self.airflow_jobs.valid_airflow_jobs}
 
     def summary(self):
 
         summary = []
         for pipeline_id, pipeline_name in self._pipeline_components_from_jobs().items():
             summary.append(f"Pipeline {pipeline_id} will be build and uploaded.")
         return summary
 
     def headers(self):
         headers = []
         for pipeline_id, pipeline_name in self._pipeline_components_from_jobs().items():
-            headers.append(StepMetadata(pipeline_id, f"Build {pipeline_name} pipeline",
-                                        Operation.Build, StepType.Pipeline))
+            headers.append(
+                StepMetadata(pipeline_id, f"Build {pipeline_name} pipeline", Operation.Build, StepType.Pipeline)
+            )
         return headers
 
     def _build_and_upload_online(self, pipeline_jobs):
         responses = []
         max_workers = os.getenv("PBT_MAX_WORKERS", 2)
         with ThreadPoolExecutor(max_workers=max_workers) as executor:
-            futures = {executor.submit(self.build_and_upload_pipeline, pipeline_id, pipeline_name): (
-                pipeline_id, pipeline_name) for pipeline_id, pipeline_name in pipeline_jobs}
+            futures = {
+                executor.submit(self.build_and_upload_pipeline, pipeline_id, pipeline_name): (
+                    pipeline_id,
+                    pipeline_name,
+                )
+                for pipeline_id, pipeline_name in pipeline_jobs
+            }
 
             for future in as_completed(futures):
                 responses.append(future.result())
         return responses
 
     def _build_and_upload_offline(self, pipeline_jobs):
         responses = []
         for index, (pipeline_id, pipeline_name) in enumerate(pipeline_jobs, start=1):
             try:
-                log(f"{Colors.OKBLUE}\nBuilding pipeline {pipeline_id} [{index}/{len(pipeline_jobs)}]{Colors.ENDC}\n\n",
-                    indent=1)
+                log(
+                    f"{Colors.OKBLUE}\nBuilding pipeline {pipeline_id} [{index}/{len(pipeline_jobs)}]{Colors.ENDC}\n\n",
+                    indent=1,
+                )
                 response = self.build_and_upload_pipeline(pipeline_id, pipeline_name)
                 responses.append(response)
             except Exception as exc:
-                log(f"{Colors.FAIL}Pipeline {pipeline_id} generated an exception: {exc}{Colors.ENDC}",
-                    step_id=pipeline_id, indent=1)
+                log(
+                    f"{Colors.FAIL}Pipeline {pipeline_id} generated an exception: {exc}{Colors.ENDC}",
+                    step_id=pipeline_id,
+                    indent=1,
+                )
         return responses
 
     def build_and_upload(self):
         use_threads = is_online_mode()
 
         if len(self._pipeline_components_from_jobs().items()) > 0:
             log(f"\n\n{Colors.OKCYAN}Building {len(self._pipeline_to_list_fabrics)} Pipelines {Colors.ENDC}\n")
@@ -115,36 +132,41 @@
         else:
             return self._build_and_upload_offline(pipelines_from_job)
 
     def build_and_upload_pipeline(self, pipeline_id, pipeline_name):
         log(step_id=pipeline_id, step_status=Status.RUNNING)
 
         all_available_fabrics = set(self.project_config.fabric_config.list_all_fabrics())
-        relevant_fabrics_for_pipeline = [fabric for fabric in self._pipeline_to_list_fabrics.get(pipeline_id) if
-                                         fabric in all_available_fabrics]
-
-        pipeline_builder = PackageBuilderAndUploader(self.project, pipeline_id, pipeline_name,
-                                                     self.project_config,
-                                                     are_tests_enabled=self.are_tests_enabled,
-                                                     fabrics=relevant_fabrics_for_pipeline)
+        relevant_fabrics_for_pipeline = [
+            fabric for fabric in self._pipeline_to_list_fabrics.get(pipeline_id) if fabric in all_available_fabrics
+        ]
+
+        pipeline_builder = PackageBuilderAndUploader(
+            self.project,
+            pipeline_id,
+            pipeline_name,
+            self.project_config,
+            are_tests_enabled=self.are_tests_enabled,
+            fabrics=relevant_fabrics_for_pipeline,
+        )
         return pipeline_builder.build_and_upload_pipeline()
 
     def deploy(self):
         return self.build_and_upload()
 
     def validate(self, treat_warning_as_errors: bool = False):
         all_pipelines = self._pipeline_components_from_jobs()
         log(f"{Colors.OKBLUE} Validating pipelines {Colors.ENDC}")
 
         overall_validate_status = True
 
         for pipeline_id, pipeline_name in all_pipelines.items():
             log(f"\n\nValidating pipeline {pipeline_name} \n")
             rdc = self.project.load_pipeline_folder(pipeline_id)
-            workflow = rdc.get('.prophecy/workflow.latest.json', None)
+            workflow = rdc.get(".prophecy/workflow.latest.json", None)
 
             num_errors = 0
             num_warnings = 0
 
             if workflow is None:
                 log(f"\n{Colors.FAIL}Empty Pipeline Found: {pipeline_name}!{Colors.ENDC}")
             else:
@@ -174,63 +196,82 @@
         log(f"{Colors.OKBLUE}Testing pipelines{Colors.ENDC}")
 
         responses = {}
         for pipeline_id, pipeline_name in self._pipeline_components_from_jobs().items():
             log(f"{Colors.OKGREEN} Testing pipeline `{pipeline_id}` {Colors.ENDC}", step_id=pipeline_id)
             log(step_id=pipeline_id, step_status=Status.RUNNING)
 
-            pipeline_builder = PackageBuilderAndUploader(self.project, pipeline_id, pipeline_name,
-                                                         self.project_config,
-                                                         are_tests_enabled=True,
-                                                         fabrics=self._pipeline_to_list_fabrics.get(pipeline_id))
+            pipeline_builder = PackageBuilderAndUploader(
+                self.project,
+                pipeline_id,
+                pipeline_name,
+                self.project_config,
+                are_tests_enabled=True,
+                fabrics=self._pipeline_to_list_fabrics.get(pipeline_id),
+            )
             return_code = pipeline_builder.test()
             responses[pipeline_id] = return_code
         for pipeline_id, return_code in responses.items():
             if return_code in (0, 5):
                 log(f"{Colors.OKGREEN} Pipeline test succeeded : `{pipeline_id}` {Colors.ENDC}")
             else:
                 log(f"{Colors.FAIL} Pipeline test failed : `{pipeline_id}`  {Colors.ENDC}")
 
     def build(self, pipeline_names: str = "", ignore_build_errors: bool = False, ignore_parse_errors: bool = False):
         # these can be names and ids.
         all_pipeline_ids = self._pipeline_to_list_fabrics_full_deployment.keys()
-        pipeline_ids_to_name = {pipeline_id: self.project.get_pipeline_name(pipeline_id) for pipeline_id in
-                                all_pipeline_ids if self.project.get_pipeline_name(pipeline_id) is not None}
+        pipeline_ids_to_name = {
+            pipeline_id: self.project.get_pipeline_name(pipeline_id)
+            for pipeline_id in all_pipeline_ids
+            if self.project.get_pipeline_name(pipeline_id) is not None
+        }
 
         if pipeline_names is not None and len(pipeline_names) > 0:
             pipelines_set = {pipeline for pipeline in pipeline_names.split(",")}
-            pipeline_ids_to_name = {pipeline_id: pipeline_name for pipeline_id, pipeline_name in
-                                    pipeline_ids_to_name.items()
-                                    if pipeline_name in pipelines_set}
-
-            pipelines_to_skip_build = {pipeline_id: pipeline_name for pipeline_id, pipeline_name in
-                                       pipeline_ids_to_name.items()
-                                       if pipeline_name not in pipelines_set}
+            pipeline_ids_to_name = {
+                pipeline_id: pipeline_name
+                for pipeline_id, pipeline_name in pipeline_ids_to_name.items()
+                if pipeline_name in pipelines_set
+            }
+
+            pipelines_to_skip_build = {
+                pipeline_id: pipeline_name
+                for pipeline_id, pipeline_name in pipeline_ids_to_name.items()
+                if pipeline_name not in pipelines_set
+            }
 
             if len(pipelines_to_skip_build) > 0:
-                log(f"{Colors.WARNING}Skipping build for pipelines {pipelines_to_skip_build}, Please check the ids/names of provided pipelines {Colors.ENDC}")
+                log(
+                    f"{Colors.WARNING}Skipping build for pipelines {pipelines_to_skip_build}, Please check the ids/names of provided pipelines {Colors.ENDC}"
+                )
 
         log(f"\n\n{Colors.OKBLUE}Building pipelines {len(pipeline_ids_to_name)}{Colors.ENDC}\n")
 
         build_errors = False
         for index, (pipeline_id, pipeline_name) in enumerate(pipeline_ids_to_name.items(), start=1):
-            log(f"\n\n{Colors.OKGREEN}Building pipeline `{pipeline_name}`:[{index}/{len(pipeline_ids_to_name)}] {Colors.ENDC}\n",
-                indent=1)
+            log(
+                f"\n\n{Colors.OKGREEN}Building pipeline `{pipeline_name}`:[{index}/{len(pipeline_ids_to_name)}] {Colors.ENDC}\n",
+                indent=1,
+            )
             log(step_id=pipeline_id, step_status=Status.RUNNING)
 
             code = self.project.load_pipeline_folder(pipeline_id)
 
             if (len(code) == 0) and ignore_parse_errors:
                 log(f"{Colors.WARNING}Pipeline `{pipeline_name}` code is not present {Colors.ENDC}", indent=2)
                 pass
 
-            pipeline_builder = PackageBuilderAndUploader(self.project, pipeline_id, pipeline_name,
-                                                         self.project_config,
-                                                         are_tests_enabled=False,
-                                                         fabrics=self._pipeline_to_list_fabrics.get(pipeline_id))
+            pipeline_builder = PackageBuilderAndUploader(
+                self.project,
+                pipeline_id,
+                pipeline_name,
+                self.project_config,
+                are_tests_enabled=False,
+                fabrics=self._pipeline_to_list_fabrics.get(pipeline_id),
+            )
             try:
                 build_success = pipeline_builder.build(ignore_build_errors) == 0
             except ProjectBuildFailedException:
                 build_success = False
 
             if build_success:
                 build_errors = True
@@ -270,16 +311,15 @@
         return pipelines_to_fabrics
 
     @property
     def _pipeline_to_list_fabrics(self) -> Dict[str, List[str]]:
         if self.deployment_mode == DeploymentMode.SelectiveJob:
             return self._pipeline_to_list_fabrics_selective_job
         elif not is_online_mode():
-            return {**self._pipeline_to_list_fabrics_full_deployment,
-                    **self._pipeline_to_list_fabrics_selective_job}
+            return {**self._pipeline_to_list_fabrics_full_deployment, **self._pipeline_to_list_fabrics_selective_job}
         else:
             return self._pipeline_to_list_fabrics_full_deployment
 
     def _pipeline_components_from_jobs(self):
         pipeline_components = {}
 
         for pipeline_id in list(self._pipeline_to_list_fabrics.keys()):
@@ -288,38 +328,44 @@
 
         return pipeline_components
 
 
 # look at the nexus client, download the jar in target folder or dist folder and return or
 # if it's not present in nexus, then build the jar upload to nexus and return it back.
 class PackageBuilderAndUploader:
-
-    def __init__(self, project: Project, pipeline_id: str, pipeline_name: str,
-                 project_config: ProjectConfig = None, are_tests_enabled: bool = False, fabrics: List = []):
+    def __init__(
+        self,
+        project: Project,
+        pipeline_id: str,
+        pipeline_name: str,
+        project_config: ProjectConfig = None,
+        are_tests_enabled: bool = False,
+        fabrics: List = [],
+    ):
 
         self._pipeline_id = pipeline_id
         self._pipeline_name = pipeline_name
         self._are_tests_enabled = are_tests_enabled
         self._project = project
         self._project_langauge = project.project_language
         self._base_path = project.load_pipeline_base_path(pipeline_id)
         self._project_config = project_config
         self.fabrics = fabrics
-        self.pipeline_upload_manager = PipelineUploadManager(self._project, self._project_config, self._pipeline_id,
-                                                             self._pipeline_name,
-                                                             self.fabrics)
+        self.pipeline_upload_manager = PipelineUploadManager(
+            self._project, self._project_config, self._pipeline_id, self._pipeline_name, self.fabrics
+        )
 
     def _initialize_temp_folder(self):
         rdc = self._project.load_pipeline_folder(self._pipeline_id)
 
         temp_dir = tempfile.mkdtemp()
         for file_name, file_content in rdc.items():
             file_path = os.path.join(temp_dir, file_name)
             os.makedirs(os.path.dirname(file_path), exist_ok=True)
-            with open(file_path, 'w') as f:
+            with open(file_path, "w") as f:
                 f.write(file_content)
         self._base_path = temp_dir
 
     def test(self):
 
         if self._project_langauge == SCALA_LANGUAGE:
             return self.mvn_test()
@@ -349,82 +395,96 @@
 
             if self._project_langauge == SCALA_LANGUAGE:
                 self.mvn_build()
             else:
                 self.wheel_build()
 
             path = Project.get_pipeline_whl_or_jar(self._base_path)
-            log(f"{Colors.OKGREEN}Pipeline package built successfully, with path {path}{Colors.ENDC}\n",
-                step_id=self._pipeline_id, indent=2)
+            log(
+                f"{Colors.OKGREEN}Pipeline package built successfully, with path {path}{Colors.ENDC}\n",
+                step_id=self._pipeline_id,
+                indent=2,
+            )
 
             if self._project_config.system_config.nexus is not None:
                 log("Trying to upload pipeline package to nexus.", self._pipeline_id)
                 self._uploading_to_nexus(path)
 
             log(f"Uploading pipeline {self._pipeline_id} from path {path}", indent=2)
 
             return self._upload_pipeline(path)
 
         except Exception as e:
-            log(message=f"{Colors.FAIL}Failed to build the pipeline package.{Colors.ENDC}", exception=e,
-                step_id=self._pipeline_id, indent=1)
+            log(
+                message=f"{Colors.FAIL}Failed to build the pipeline package.{Colors.ENDC}",
+                exception=e,
+                step_id=self._pipeline_id,
+                indent=1,
+            )
             log(step_id=self._pipeline_id, step_status=Status.FAILED)
             return Either(left=e)
 
     def _upload_pipeline(self, path: str) -> Either:
         return self.pipeline_upload_manager.upload_pipeline(path)
 
     def _download_pipeline_from_nexus(self) -> Optional[Either]:
         if self._project_config.system_config.nexus is not None:
-            log("Project has nexus configured, trying to download the pipeline package.", step_id=self._pipeline_id,
-                indent=2)
+            log(
+                "Project has nexus configured, trying to download the pipeline package.",
+                step_id=self._pipeline_id,
+                indent=2,
+            )
             return self._download_from_nexus()
         else:
             # log("Project does not have nexus configured, building the pipeline package.", step_id=self._pipeline_id, indent=2)
             return None
 
     def _uploading_to_nexus(self, upload_path):
         try:
             client = NexusClient.initialize_nexus_client(self._project_config)
-            client.upload_file(upload_path, self._project.project_id,
-                               self._pipeline_id, self._project.release_version,
-                               self._get_package_name())
+            client.upload_file(
+                upload_path,
+                self._project.project_id,
+                self._pipeline_id,
+                self._project.release_version,
+                self._get_package_name(),
+            )
             log("Pipeline uploaded to nexus.", step_id=self._pipeline_id)
         except Exception as e:
             log("Failed to upload pipeline to nexus", e, self._pipeline_id)
 
     def _download_from_nexus(self):
         try:
             client = NexusClient.initialize_nexus_client(self._project_config)
             package_name = self._get_package_name()
-            response = client.download_file(package_name,
-                                            self._project.project_id,
-                                            self._project.release_version,
-                                            self._pipeline_id)
+            response = client.download_file(
+                package_name, self._project.project_id, self._project.release_version, self._pipeline_id
+            )
             log("Pipeline downloaded from nexus.", step_id=self._pipeline_id)
             return Either(right=response)
         except Exception as e:
             log("Failed to download pipeline from nexus", e, self._pipeline_id)
             return Either(left=e)
 
     def _get_package_name(self):
         if self._project_langauge == SCALA_LANGUAGE:
-            return f'{self._pipeline_name}.jar'
+            return f"{self._pipeline_name}.jar"
         else:
             # todo combine in a single regex
             regex_match = r"[^\w\d.]+"
             underscore_regex = r"(_)\1+"
             result = re.sub(regex_match, "_", self._pipeline_name)
             result = re.sub(underscore_regex, "_", result)
-            return f'{result}-1.0-py3-none-any.whl'
+            return f"{result}-1.0-py3-none-any.whl"
 
     def mvn_build(self, ignore_build_errors: bool = False):
         mvn = "mvn"
-        command = [mvn, "package", "-DskipTests"] if not self._are_tests_enabled else [mvn, "package",
-                                                                                       "-Dfabric=default"]
+        command = (
+            [mvn, "package", "-DskipTests"] if not self._are_tests_enabled else [mvn, "package", "-Dfabric=default"]
+        )
 
         log(f"Running mvn command {command}", step_id=self._pipeline_id, indent=2)
 
         return self._build(command, ignore_build_errors)
 
     def mvn_test(self):
         mvn = "mvn"
@@ -457,42 +517,42 @@
     # maybe we can try another iteration with yield ?
     def _build(self, command: list, ignore_build_errors: bool = False):
         env = dict(os.environ)
 
         # Set the MAVEN_OPTS variable
         env["MAVEN_OPTS"] = "-Xmx1024m -XX:MaxPermSize=512m -Xss32m"
 
-        if env.get('FABRIC_NAME', None) is None:
+        if env.get("FABRIC_NAME", None) is None:
             env["FABRIC_NAME"] = "default"  # for python test runs.
 
-        log(f"Running command {command} on path {self._base_path}",
-            step_id=self._pipeline_id, indent=2)
-        process = subprocess.Popen(command, shell=False, stdout=subprocess.PIPE, stderr=subprocess.PIPE, env=env,
-                                   cwd=self._base_path)
+        log(f"Running command {command} on path {self._base_path}", step_id=self._pipeline_id, indent=2)
+        process = subprocess.Popen(
+            command, shell=False, stdout=subprocess.PIPE, stderr=subprocess.PIPE, env=env, cwd=self._base_path
+        )
 
         def log_output(pipe, log_function):
             while True:
                 # Read line from stdout or stderr, break if EOF
                 output = pipe.readline()
                 if process.poll() is not None and not output:
                     break
                 # Decode line and print it
                 response = output.decode().strip()
 
                 # stripping unnecessary logs
-                if not re.search(r'Progress \(\d+\):', response) and len(response) != 0 and response != '\n':
+                if not re.search(r"Progress \(\d+\):", response) and len(response) != 0 and response != "\n":
                     log_function(response)
 
         # Create threads to read and log stdout and stderr simultaneously
-        stdout_thread = threading.Thread(target=log_output,
-                                         args=(
-                                             process.stdout, lambda msg: log(msg, step_id=self._pipeline_id, indent=2)))
-        stderr_thread = threading.Thread(target=log_output,
-                                         args=(
-                                             process.stderr, lambda msg: log(msg, step_id=self._pipeline_id, indent=2)))
+        stdout_thread = threading.Thread(
+            target=log_output, args=(process.stdout, lambda msg: log(msg, step_id=self._pipeline_id, indent=2))
+        )
+        stderr_thread = threading.Thread(
+            target=log_output, args=(process.stderr, lambda msg: log(msg, step_id=self._pipeline_id, indent=2))
+        )
 
         # Start threads
         stdout_thread.start()
         stderr_thread.start()
 
         # Wait for both threads to finish
         stdout_thread.join()
@@ -508,27 +568,33 @@
         else:
             log(f"Build failed with exit code {return_code}", step_id=self._pipeline_id, indent=2)
             raise ProjectBuildFailedException(f"Build failed with exit code {return_code}")
 
         return return_code
 
 
+# Create for Synapse / Azure
 class PipelineUploader(ABC):
-
     @abstractmethod
     def upload_pipeline(self, path: str):
         pass
 
     def exists(self) -> bool:
         pass
 
 
 class PipelineUploadManager(PipelineUploader, ABC):
-    def __init__(self, project: Project, project_config: ProjectConfig, pipeline_id: str, pipeline_name: str,
-                 all_fabrics: List[str]):
+    def __init__(
+        self,
+        project: Project,
+        project_config: ProjectConfig,
+        pipeline_id: str,
+        pipeline_name: str,
+        all_fabrics: List[str],
+    ):
         self.project = project
         self.project_config = project_config
         self.pipeline_id = pipeline_id
         self.pipeline_name = pipeline_name
         self.all_fabrics = all_fabrics
 
     def upload_pipeline(self, from_path: str):
@@ -542,15 +608,16 @@
                 # scala based pipeline
                 file_name = file_name_with_extension.replace("-1.0.jar", ".jar")
             else:
                 # python based pipeline they are correctly generated.
                 file_name = file_name_with_extension
 
             subscribed_project_id, subscribed_project_release_version, path = is_cross_project_pipeline(
-                self.pipeline_id)
+                self.pipeline_id
+            )
 
             if subscribed_project_id is not None:
                 to_path = f"{subscribed_project_id}/{subscribed_project_release_version}"
             else:
                 to_path = f"{self.project.project_id}/{self.project.release_version}"
 
             responses = []
@@ -558,101 +625,189 @@
             for fabric_id in self.all_fabrics:
                 try:
                     fabric_info = self.project_config.fabric_config.get_fabric(fabric_id)
                     fabric_name = fabric_info.name
                     db_info = fabric_info.databricks
                     emr_info = fabric_info.emr
                     dataproc_info = fabric_info.dataproc
+                    oss_info = fabric_info.airflow_oss
 
                     if db_info is not None:
-                        pipeline_uploader = DatabricksPipelineUploader(self.project, self.project_config,
-                                                                       self.pipeline_id, to_path, from_path,
-                                                                       file_name,
-                                                                       fabric_id, fabric_name)
+                        pipeline_uploader = DatabricksPipelineUploader(
+                            self.project,
+                            self.project_config,
+                            self.pipeline_id,
+                            to_path,
+                            from_path,
+                            file_name,
+                            fabric_id,
+                            fabric_name,
+                        )
 
                     elif emr_info is not None:
-                        pipeline_uploader = EMRPipelineUploader(self.project, self.project_config,
-                                                                self.pipeline_id, from_path, to_path,
-                                                                file_name, fabric_id, fabric_name, emr_info)
+                        pipeline_uploader = EMRPipelineUploader(
+                            self.project,
+                            self.project_config,
+                            self.pipeline_id,
+                            from_path,
+                            to_path,
+                            file_name,
+                            fabric_id,
+                            fabric_name,
+                            emr_info,
+                        )
 
                     elif dataproc_info is not None:
-                        pipeline_uploader = DataprocPipelineUploader(self.project, self.project_config,
-                                                                     self.pipeline_id, from_path, to_path,
-                                                                     file_name, fabric_id, fabric_name, dataproc_info)
+                        pipeline_uploader = DataprocPipelineUploader(
+                            self.project,
+                            self.project_config,
+                            self.pipeline_id,
+                            from_path,
+                            to_path,
+                            file_name,
+                            fabric_id,
+                            fabric_name,
+                            dataproc_info,
+                        )
+
+                    elif oss_info is not None:
+                        pipeline_uploader = HdfsPipelineUploader(
+                            self.project,
+                            self.project_config,
+                            self.pipeline_id,
+                            from_path,
+                            to_path,
+                            file_name,
+                            fabric_id,
+                            fabric_name,
+                            oss_info,
+                        )
+
                     else:
-                        log(f"{Colors.WARNING}Fabric id `{fabric_id}` with name `{fabric_name}` is not supported for pipeline upload{Colors.ENDC}",
-                            step_id=self.pipeline_id, )
+                        log(
+                            f"{Colors.WARNING}Fabric id `{fabric_id}` with name `{fabric_name}` is not supported for pipeline upload{Colors.ENDC}",
+                            step_id=self.pipeline_id,
+                        )
                         pipeline_uploader = DummyPipelineUploader()
 
                     responses.append(pipeline_uploader.upload_pipeline(""))
 
                 except Exception as e:
-                    log(f"{Colors.FAIL}Error while uploading pipeline {self.pipeline_id} for fabric {fabric_id}{Colors.ENDC}",
-                        step_id=self.pipeline_id, exception=e, level=LogLevel.TRACE, indent=2)
+                    log(
+                        f"{Colors.FAIL}Error while uploading pipeline {self.pipeline_id} for fabric {fabric_id}{Colors.ENDC}",
+                        step_id=self.pipeline_id,
+                        exception=e,
+                        level=LogLevel.TRACE,
+                        indent=2,
+                    )
                     log(step_status=Status.FAILED, step_id=self.pipeline_id)
                     responses.append(Either(left=e))
 
             if all([response.is_right for response in responses]):
                 log(step_status=Status.SUCCEEDED, step_id=self.pipeline_id)
                 return Either(right=True)
             else:
                 log(step_status=Status.FAILED, step_id=self.pipeline_id)
                 return Either(left=responses)
 
         except Exception as e:
-            log(f"{Colors.FAIL}Error while uploading pipeline {self.pipeline_id}{Colors.ENDC}",
+            log(
+                f"{Colors.FAIL}Error while uploading pipeline {self.pipeline_id}{Colors.ENDC}",
                 step_id=self.pipeline_id,
-                exception=e, indent=2)
+                exception=e,
+                indent=2,
+            )
             log(step_status=Status.FAILED, step_id=self.pipeline_id)
             return Either(left=e)
 
     def exists(self) -> bool:
         response = True
         file_name = get_package_name(self.project.project_language, self.pipeline_name)
 
         subscribed_project_id, subscribed_project_release_version, path = self.project.is_cross_project_pipeline(
-            self.pipeline_id)
+            self.pipeline_id
+        )
 
         if subscribed_project_id is not None:
             to_path = f"{subscribed_project_id}/{subscribed_project_release_version}"
         else:
             to_path = f"{self.project.project_id}/{self.project.release_version}"
 
         for fabric_id in self.all_fabrics:
             fabric_info = self.project_config.fabric_config.get_fabric(fabric_id)
             fabric_name = fabric_info.name
             db_info = fabric_info.databricks
             emr_info = fabric_info.emr
             dataproc_info = fabric_info.dataproc
+            oss_info = fabric_info.airflow_oss
 
             if db_info is not None:
-                pipeline_uploader = DatabricksPipelineUploader(self.project, self.project_config,
-                                                               self.pipeline_id, to_path, "", file_name,
-                                                               fabric_id, fabric_name)
+                pipeline_uploader = DatabricksPipelineUploader(
+                    self.project, self.project_config, self.pipeline_id, to_path, "", file_name, fabric_id, fabric_name
+                )
 
             elif emr_info is not None:
-                pipeline_uploader = EMRPipelineUploader(self.project, self.project_config,
-                                                        self.pipeline_id, to_path, "", file_name, fabric_id,
-                                                        fabric_name, emr_info)
+                pipeline_uploader = EMRPipelineUploader(
+                    self.project,
+                    self.project_config,
+                    self.pipeline_id,
+                    to_path,
+                    "",
+                    file_name,
+                    fabric_id,
+                    fabric_name,
+                    emr_info,
+                )
 
             elif dataproc_info is not None:
-                pipeline_uploader = DataprocPipelineUploader(self.project, self.project_config,
-                                                             self.pipeline_id, to_path, "", file_name,
-                                                             fabric_id, fabric_name, dataproc_info)
+                pipeline_uploader = DataprocPipelineUploader(
+                    self.project,
+                    self.project_config,
+                    self.pipeline_id,
+                    to_path,
+                    "",
+                    file_name,
+                    fabric_id,
+                    fabric_name,
+                    dataproc_info,
+                )
+
+            elif oss_info is not None:
+                pipeline_uploader = HdfsPipelineUploader(
+                    self.project,
+                    self.project_config,
+                    self.pipeline_id,
+                    to_path,
+                    "",
+                    file_name,
+                    fabric_id,
+                    fabric_name,
+                    dataproc_info,
+                )
             else:
                 pipeline_uploader = DummyPipelineUploader()
 
             response = response and pipeline_uploader.exists()
 
         return response
 
 
 class EMRPipelineUploader(PipelineUploader, ABC):
-    def __init__(self, project: Project, project_config: ProjectConfig, pipeline_id: str,
-                 from_path: str, to_path: str, file_name: str, fabric_id: str, fabric_name: str, emr_info: EMRInfo):
+    def __init__(
+        self,
+        project: Project,
+        project_config: ProjectConfig,
+        pipeline_id: str,
+        from_path: str,
+        to_path: str,
+        file_name: str,
+        fabric_id: str,
+        fabric_name: str,
+        emr_info: EMRInfo,
+    ):
         self.project = project
         self.project_config = project_config
         self.pipeline_id = pipeline_id
 
         self.from_path = from_path
         self.to_path = to_path
         self.file_name = file_name
@@ -660,48 +815,69 @@
         self.fabric_name = fabric_name
 
         self.emr_info = emr_info
         self.file_name = file_name
 
         self.rest_client_factory = RestClientFactory.get_instance(RestClientFactory, project_config.fabric_config)
         self.base_path = self.project_config.system_config.get_s3_base_path()
-        self.upload_path = f"{self.emr_info.bare_path_prefix()}/{self.base_path}/{self.to_path}/pipeline/{self.file_name}".lstrip(
-            "/")
+        self.upload_path = (
+            f"{self.emr_info.bare_path_prefix()}/{self.base_path}/{self.to_path}/pipeline/{self.file_name}".lstrip("/")
+        )
 
     def upload_pipeline(self, path: str):
 
         try:
             client = self.rest_client_factory.s3_client(self.fabric_id)
             client.upload_file(self.emr_info.bare_bucket(), self.upload_path, self.from_path)
 
-            log(f"{Colors.OKGREEN}Uploaded pipeline to s3, from path {self.from_path} to path {self.upload_path} for fabric {self.fabric_name}{Colors.ENDC}",
-                step_id=self.pipeline_id, indent=2)
+            log(
+                f"{Colors.OKGREEN}Uploaded pipeline to s3, from path {self.from_path} to path {self.upload_path} for fabric {self.fabric_name}{Colors.ENDC}",
+                step_id=self.pipeline_id,
+                indent=2,
+            )
 
             if self.project.project_language == "python":
                 content = self.project.get_py_pipeline_main_file(self.pipeline_id)
                 pipeline_name = self.pipeline_id.split("/")[1]
                 launcher_path = f"{self.emr_info.bare_path_prefix()}/{self.base_path}/{self.to_path}/pipeline/{pipeline_name}/launcher.py".lstrip(
-                    '/')
+                    "/"
+                )
                 client.upload_content(self.emr_info.bare_bucket(), launcher_path, content)
 
-                log(f"{Colors.OKGREEN}Uploading py pipeline launcher to to-path {launcher_path} for fabric {self.fabric_name}{Colors.ENDC}",
-                    step_id=self.pipeline_id, indent=2)
+                log(
+                    f"{Colors.OKGREEN}Uploading py pipeline launcher to to-path {launcher_path} for fabric {self.fabric_name}{Colors.ENDC}",
+                    step_id=self.pipeline_id,
+                    indent=2,
+                )
             return Either(right=True)
         except Exception as e:
-            log(f"{Colors.WARNING}Unknown Exception while uploading pipeline to emr, from-path {self.from_path} to path {self.upload_path} for fabric {self.fabric_name}, Ignoring{Colors.ENDC}",
-                exception=e, step_id=self.pipeline_id, indent=2)
+            log(
+                f"{Colors.WARNING}Unknown Exception while uploading pipeline to emr, from-path {self.from_path} to path {self.upload_path} for fabric {self.fabric_name}, Ignoring{Colors.ENDC}",
+                exception=e,
+                step_id=self.pipeline_id,
+                indent=2,
+            )
             return Either(right=True)
 
     def exists(self) -> bool:
         return False
 
 
 class DatabricksPipelineUploader(PipelineUploader, ABC):
-    def __init__(self, project: Project, project_config: ProjectConfig, pipeline_id: str,
-                 to_path: str, file_path: str, file_name: str, fabric_id: str, fabric_name: str):
+    def __init__(
+        self,
+        project: Project,
+        project_config: ProjectConfig,
+        pipeline_id: str,
+        to_path: str,
+        file_path: str,
+        file_name: str,
+        fabric_id: str,
+        fabric_name: str,
+    ):
         self.project = project
         self.project_config = project_config
         self.file_name = file_name
         self.file_path = file_path
         self.pipeline_id = pipeline_id
         self.to_path = to_path
         self.fabric_id = fabric_id
@@ -712,98 +888,208 @@
         self.base_path = self.project_config.system_config.get_dbfs_base_path()
         self.upload_path = f"{self.base_path}/{self.to_path}/pipeline/{self.file_name}"
 
     def upload_pipeline(self, path: str) -> Either:
         try:
             client = self.rest_client_factory.databricks_client(self.fabric_id)
             client.upload_src_path(self.file_path, self.upload_path)
-            log(f"Uploading pipeline to databricks from-path `{self.file_path}` to path `{self.upload_path}` for fabric `{self.fabric_label}`",
-                step_id=self.pipeline_id, indent=2)
+            log(
+                f"Uploading pipeline to databricks from-path `{self.file_path}` to path `{self.upload_path}` for fabric `{self.fabric_label}`",
+                step_id=self.pipeline_id,
+                indent=2,
+            )
 
             return Either(right=True)
 
         except HTTPError as e:
-            response = e.response.content.decode('utf-8')
+            response = e.response.content.decode("utf-8")
             log(step_id=self.pipeline_id, message=response)
 
             if e.response.status_code == 401 or e.response.status_code == 403:
-                log(f'{Colors.WARNING}Error on uploading pipeline to databricks from path {self.file_path} to path {self.upload_path} for fabric {self.fabric_label}, but ignoring{Colors.ENDC}',
-                    exception=e, step_id=self.pipeline_id, indent=2)
+                log(
+                    f"{Colors.WARNING}Error on uploading pipeline to databricks from path {self.file_path} to path {self.upload_path} for fabric {self.fabric_label}, but ignoring{Colors.ENDC}",
+                    exception=e,
+                    step_id=self.pipeline_id,
+                    indent=2,
+                )
                 return Either(right=True)
             else:
-                log(f"{Colors.FAIL}HttpError on uploading pipeline to databricks from-path {self.file_path} to path {self.upload_path} for fabric {self.fabric_label}{Colors.ENDC}",
-                    exception=e, step_id=self.pipeline_id, indent=2)
+                log(
+                    f"{Colors.FAIL}HttpError on uploading pipeline to databricks from-path {self.file_path} to path {self.upload_path} for fabric {self.fabric_label}{Colors.ENDC}",
+                    exception=e,
+                    step_id=self.pipeline_id,
+                    indent=2,
+                )
                 return Either(left=e)
 
         except Exception as e:
-            log(f"{Colors.FAIL}Unknown Exception on uploading pipeline to databricks from-path {self.file_path} to path {self.upload_path} for fabric {self.fabric_label}, ignoring exception{Colors.ENDC}",
-                exception=e, step_id=self.pipeline_id, indent=2)
+            log(
+                f"{Colors.FAIL}Unknown Exception on uploading pipeline to databricks from-path {self.file_path} to path {self.upload_path} for fabric {self.fabric_label}, ignoring exception{Colors.ENDC}",
+                exception=e,
+                step_id=self.pipeline_id,
+                indent=2,
+            )
             return Either(right=True)
 
     def exists(self) -> bool:
         try:
             log(f"Checking if path {self.upload_path} already exists.", self.pipeline_id, indent=2)
             client = self.rest_client_factory.databricks_client(self.fabric_id)
             return client.path_exist(self.upload_path)
         except Exception as e:
-            log(f"{Colors.WARNING} Failed checking path {self.upload_path}{Colors.ENDC}", step_id=self.pipeline_id,
+            log(
+                f"{Colors.WARNING} Failed checking path {self.upload_path}{Colors.ENDC}",
+                step_id=self.pipeline_id,
                 exception=e,
-                indent=2)
+                indent=2,
+            )
             return False
 
 
 class DummyPipelineUploader(PipelineUploader, ABC):
-
     def upload_pipeline(self, path: str):
         return Either(right=True)
 
     def exists(self) -> bool:
         return True
 
 
 class DataprocPipelineUploader(PipelineUploader, ABC):
-    def __init__(self, project: Project, project_config: ProjectConfig, pipeline_id: str,
-                 from_path: str, to_path: str, file_name: str, fabric_id: str, fabric_name: str,
-                 dataproc_info: DataprocInfo):
+    def __init__(
+        self,
+        project: Project,
+        project_config: ProjectConfig,
+        pipeline_id: str,
+        from_path: str,
+        to_path: str,
+        file_name: str,
+        fabric_id: str,
+        fabric_name: str,
+        dataproc_info: DataprocInfo,
+    ):
         self.project = project
         self.project_config = project_config
         self.pipeline_id = pipeline_id
 
         self.from_path = from_path
         self.to_path = to_path
         self.fabric_id = fabric_id
         self.fabric_name = fabric_name
         self.fabric_label = get_fabric_label(fabric_name, fabric_id)
 
         self.dataproc_info = dataproc_info
         self.file_name = file_name
         self.rest_client_factory = RestClientFactory.get_instance(RestClientFactory, project_config.fabric_config)
         self.base_path = self.project_config.system_config.get_s3_base_path()
-        self.upload_path = f"{self.dataproc_info.bare_path_prefix()}/{self.base_path}/{self.to_path}/pipeline/{self.file_name}".lstrip(
-            "/")
+        self.upload_path = (
+            f"{self.dataproc_info.bare_path_prefix()}/{self.base_path}/{self.to_path}/pipeline/{self.file_name}".lstrip(
+                "/"
+            )
+        )
 
     def upload_pipeline(self, path: str):
         try:
-            client = self.rest_client_factory.dataproc_client(self.fabric_name)
+            client = self.rest_client_factory.dataproc_client(self.fabric_id)
             client.put_object_from_file(self.dataproc_info.bare_bucket(), self.upload_path, self.from_path)
 
-            log(f"{Colors.OKGREEN}Uploaded pipeline to data-proc, from-path {self.from_path} to to-path {self.upload_path} for fabric {self.fabric_label}{Colors.ENDC}",
-                step_id=self.pipeline_id, indent=2)
+            log(
+                f"{Colors.OKGREEN}Uploaded pipeline to data-proc, from-path {self.from_path} to to-path {self.upload_path} for fabric {self.fabric_label}{Colors.ENDC}",
+                step_id=self.pipeline_id,
+                indent=2,
+            )
 
             if self.project.project_language == "python":
                 content = self.project.get_py_pipeline_main_file(self.pipeline_id)
-                pipeline_name = self.pipeline_id.split("/")[1]
+                pipeline_name = python_pipeline_name(self.pipeline_id.split("/")[1])
                 launcher_path = f"{self.dataproc_info.bare_path_prefix()}/{self.base_path}/{self.to_path}/pipeline/{pipeline_name}/launcher.py".lstrip(
-                    '/')
+                    "/"
+                )
                 client.put_object(self.dataproc_info.bare_bucket(), launcher_path, content)
 
-                log(f"{Colors.OKGREEN}Uploading py pipeline launcher to to-path {launcher_path} and bucket {self.dataproc_info.bare_bucket()} for fabric {self.fabric_label}{Colors.ENDC}",
-                    step_id=self.pipeline_id, indent=2)
+                log(
+                    f"{Colors.OKGREEN}Uploading py pipeline launcher to to-path {launcher_path} and bucket {self.dataproc_info.bare_bucket()} for fabric {self.fabric_label}{Colors.ENDC}",
+                    step_id=self.pipeline_id,
+                    indent=2,
+                )
             return Either(right=True)
 
         except Exception as e:
-            log(f"{Colors.WARNING}Unknown Exception while uploading pipeline to data-proc, from-path {self.from_path} to to-path {self.upload_path} for fabric {self.fabric_label}, ignoring exception{Colors.ENDC}",
-                exception=e, step_id=self.pipeline_id, indent=2)
+            log(
+                f"{Colors.WARNING}Unknown Exception while uploading pipeline to data-proc, from-path {self.from_path} to to-path {self.upload_path} for fabric {self.fabric_label}, ignoring exception{Colors.ENDC}",
+                exception=e,
+                step_id=self.pipeline_id,
+                indent=2,
+            )
+            return Either(right=True)
+
+    def exists(self) -> bool:
+        return True
+
+
+class HdfsPipelineUploader(PipelineUploader, ABC):
+    def __init__(
+        self,
+        project: Project,
+        project_config: ProjectConfig,
+        pipeline_id: str,
+        from_path: str,
+        to_path: str,
+        file_name: str,
+        fabric_id: str,
+        fabric_name: str,
+        oss_info: OpenSourceAirflowInfo,
+    ):
+        self.project = project
+        self.project_config = project_config
+        self.pipeline_id = pipeline_id
+
+        self.from_path = from_path
+        self.to_path = to_path
+        self.fabric_id = fabric_id
+        self.fabric_name = fabric_name
+        self.fabric_label = get_fabric_label(fabric_name, fabric_id)
+
+        self.oss_info = oss_info
+        self.file_name = file_name
+        self.rest_client_factory = RestClientFactory.get_instance(RestClientFactory, project_config.fabric_config)
+        self.prophecy_base_path = self.project_config.system_config.get_hdfs_base_path()
+        self.root_location = self.oss_info.location.rstrip("/")
+        self.upload_directory = f"{self.root_location}/{self.prophecy_base_path}/{self.to_path}/pipeline"
+
+    def upload_pipeline(self, path: str):
+        try:
+            client = self.rest_client_factory.open_source_hdfs_client(self.fabric_id)
+            client.put_object_from_file(self.upload_directory, self.file_name, self.from_path)
+
+            log(
+                f"{Colors.OKGREEN}Uploaded pipeline to HDFS, from-path {self.from_path} to-path {self.upload_directory} for fabric {self.fabric_label}{Colors.ENDC}",
+                step_id=self.pipeline_id,
+                indent=2,
+            )
+
+            if self.project.project_language == "python":
+                content = self.project.get_py_pipeline_main_file(self.pipeline_id)
+                pipeline_name = python_pipeline_name(self.pipeline_id.split("/")[1])
+                launcher_file_name = "launcher.py"
+                launcher_directory = (
+                    f"{self.root_location}/{self.prophecy_base_path}/{self.to_path}/pipeline/{pipeline_name}"
+                )
+                client.put_object(launcher_directory, launcher_file_name, content)
+
+                log(
+                    f"{Colors.OKGREEN}Uploading py pipeline launcher to to-path {launcher_directory} for fabric {self.fabric_label}{Colors.ENDC}",
+                    step_id=self.pipeline_id,
+                    indent=2,
+                )
+            return Either(right=True)
+
+        except Exception as e:
+            log(
+                f"{Colors.WARNING}Unknown Exception while uploading pipeline to data-proc, from-path {self.from_path} to to-path {self.upload_directory} for fabric {self.fabric_label}, ignoring exception{Colors.ENDC}",
+                exception=e,
+                step_id=self.pipeline_id,
+                indent=2,
+            )
             return Either(right=True)
 
     def exists(self) -> bool:
         return True
```

### Comparing `prophecy-build-tool-1.2.8/src/pbt/deployment/project.py` & `prophecy-build-tool-1.2.9/src/pbt/deployment/project.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,76 +1,96 @@
 import copy
 import os
 from typing import List
 
 import yaml
 
 from .gems import GemsDeployment
-from ..deployment.jobs.airflow import AirflowJobDeployment, AirflowGitSecrets, EMRPipelineConfigurations, \
-    DataprocPipelineConfigurations
-from ..deployment.jobs.databricks import DatabricksJobsDeployment, ScriptComponents, PipelineConfigurations, \
-    DBTComponents
+from ..deployment.jobs.airflow import (
+    AirflowGitSecrets,
+    AirflowJobDeployment,
+    DataprocPipelineConfigurations,
+    EMRPipelineConfigurations,
+    SparkSubmitPipelineConfigurations,
+)
+from ..deployment.jobs.databricks import (
+    DBTComponents,
+    DatabricksJobsDeployment,
+    PipelineConfigurations,
+    ScriptComponents,
+)
 from ..deployment.pipeline import PipelineDeployment
 from ..entities.project import Project
-from ..utility import custom_print as log, Either, is_online_mode
+from ..utility import Either, custom_print as log, is_online_mode
 from ..utility import remove_null_items_recursively
 from ..utils.constants import NEW_JOB_STATE_FILE
 from ..utils.project_config import ProjectConfig
-from ..utils.project_models import StepMetadata, Operation, StepType, Status, Colors
+from ..utils.project_models import Colors, Operation, Status, StepMetadata, StepType
 
 
 class ProjectDeployment:
     def __init__(self, project: Project, project_config: ProjectConfig):
         self.project = project
         self.project_config = project_config
 
         self._databricks_jobs = DatabricksJobsDeployment(project, project_config)
         self._airflow_jobs = AirflowJobDeployment(project, project_config)
 
         self._script_component = ScriptComponents(project, self._databricks_jobs, project_config)
-        self._pipeline_configurations = PipelineConfigurations(project, self._databricks_jobs,
-                                                               project_config)
+        self._pipeline_configurations = PipelineConfigurations(project, self._databricks_jobs, project_config)
+        self._spark_submit_pipeline_configurations = SparkSubmitPipelineConfigurations(
+            project, self._airflow_jobs, project_config
+        )
         self._emr_pipeline_configurations = EMRPipelineConfigurations(project, self._airflow_jobs, project_config)
 
-        self._dataproc_pipeline_configurations = DataprocPipelineConfigurations(project, self._airflow_jobs,
-                                                                                project_config)
+        self._dataproc_pipeline_configurations = DataprocPipelineConfigurations(
+            project, self._airflow_jobs, project_config
+        )
 
         self._dbt_component = DBTComponents(project, self._databricks_jobs, project_config)
         self._airflow_git_secrets = AirflowGitSecrets(project, self._airflow_jobs, project_config)
 
-        self._pipelines = PipelineDeployment(project, self._databricks_jobs, self._airflow_jobs,
-                                             project_config)
+        self._pipelines = PipelineDeployment(project, self._databricks_jobs, self._airflow_jobs, project_config)
 
         # add gems Deployment.
         self._gems = GemsDeployment(project, project_config)
 
     def headers(self):
-        summary = self._gems.summary() + self._script_component.summary() + \
-                  self._dbt_component.summary() + self._airflow_git_secrets.summary() + \
-                  self._pipeline_configurations.summary() + self._emr_pipeline_configurations.summary() + \
-                  self._dataproc_pipeline_configurations.summary() + self._pipelines.summary() + \
-                  self._databricks_jobs.summary() + self._airflow_jobs.summary()
+        summary = (
+            self._gems.summary()
+            + self._script_component.summary()
+            + self._dbt_component.summary()
+            + self._airflow_git_secrets.summary()
+            + self._pipeline_configurations.summary()
+            + self._spark_submit_pipeline_configurations.summary()
+            + self._emr_pipeline_configurations.summary()
+            + self._dataproc_pipeline_configurations.summary()
+            + self._pipelines.summary()
+            + self._databricks_jobs.summary()
+            + self._airflow_jobs.summary()
+        )
 
         if len(summary) == 0:
             summary = ["No Job and pipelines to build"]
 
         summary_header = [StepMetadata("Summary", "Summary", Operation.Build, StepType.Summary)]
 
         header_components = (
             summary_header,
             self._gems.headers(),
             self._script_component.headers(),
             self._dbt_component.headers(),
             self._airflow_git_secrets.headers(),
             self._pipeline_configurations.headers(),
+            self._spark_submit_pipeline_configurations.headers(),
             self._emr_pipeline_configurations.headers(),
             self._dataproc_pipeline_configurations.headers(),
             self._pipelines.headers(),
             self._databricks_jobs.headers(),
-            self._airflow_jobs.headers()
+            self._airflow_jobs.headers(),
         )
 
         headers = sum(header_components, [])
 
         # 1st steps have to be summary
         for header in headers:
             log(step_id=header.id, step_metadata=header)
@@ -84,15 +104,17 @@
 
     def build(self, pipelines, ignore_build_errors, ignore_parse_errors):
         self._pipelines.build(pipelines, ignore_build_errors, ignore_parse_errors)
 
     def validate(self, treat_warning_as_errors):
         self._pipelines.validate(treat_warning_as_errors)
 
-    def test(self, ):
+    def test(
+        self,
+    ):
         self._pipelines.test()
 
     def _deploy_gems(self):
         gems_responses = self._gems.deploy()
 
         if gems_responses is not None and any(response.is_left for response in gems_responses):
             raise Exception("Gems deployment failed.")
@@ -109,37 +131,48 @@
         if dbt_responses is not None and any(response.is_left for response in dbt_responses):
             raise Exception("DBT deployment failed.")
 
     def _deploy_airflow_git_secrets(self):
         airflow_git_secrets_responses = self._airflow_git_secrets.deploy()
 
         if airflow_git_secrets_responses is not None and any(
-                response.is_left for response in airflow_git_secrets_responses):
+            response.is_left for response in airflow_git_secrets_responses
+        ):
             raise Exception("Airflow git secrets deployment failed.")
 
     def _deploy_pipeline_configs(self):
         pipeline_config_responses = self._pipeline_configurations.deploy()
 
         if pipeline_config_responses is not None and any(response.is_left for response in pipeline_config_responses):
             raise Exception("Pipeline config deployment failed.")
 
     def _deploy_emr_pipeline_config(self):
         emr_pipeline_config_responses = self._emr_pipeline_configurations.deploy()
 
         if emr_pipeline_config_responses is not None and any(
-                response.is_left for response in emr_pipeline_config_responses):
+            response.is_left for response in emr_pipeline_config_responses
+        ):
             raise Exception("EMR pipeline config deployment failed.")
 
     def _deploy_dataproc_pipeline_config(self):
         dataproc_pipeline_config_responses = self._dataproc_pipeline_configurations.deploy()
 
         if dataproc_pipeline_config_responses is not None and any(
-                response.is_left for response in dataproc_pipeline_config_responses):
+            response.is_left for response in dataproc_pipeline_config_responses
+        ):
             raise Exception("Dataproc pipeline config deployment failed.")
 
+    def _deploy_spark_submit_pipeline_config(self):
+        spark_submit_pipeline_config_responses = self._spark_submit_pipeline_configurations.deploy()
+
+        if spark_submit_pipeline_config_responses is not None and any(
+                response.is_left for response in spark_submit_pipeline_config_responses
+        ):
+            raise Exception("Spark Submit pipeline config deployment failed.")
+
     def _deploy_pipelines(self):
         pipeline_responses = self._pipelines.deploy()
 
         if pipeline_responses is not None and any(response.is_left for response in pipeline_responses):
             raise Exception("Pipeline deployment failed.")
 
     def _deploy_databricks_jobs(self) -> List[Either]:
@@ -156,14 +189,15 @@
         if is_online_mode():
             self._deploy_gems()
 
         self._deploy_scripts()
         self._deploy_dbt_components()
         self._deploy_airflow_git_secrets()
         self._deploy_pipeline_configs()
+        self._deploy_spark_submit_pipeline_config()
         self._deploy_emr_pipeline_config()
         self._deploy_dataproc_pipeline_config()
 
         if not self.project_config.skip_builds:
             self._deploy_pipelines()
         else:
             log("\nSkipping pipeline deployment as skip_builds is set to true.\n")
@@ -182,15 +216,15 @@
         if not os.path.exists(base_path):
             os.makedirs(base_path)
 
         if self.project_config.based_on_file or self.project_config.migrate:
             path = os.path.join(base_path, NEW_JOB_STATE_FILE)
             yaml_str = yaml.dump(data=remove_null_items_recursively(new_state_config.dict()))
 
-            with open(path, 'w') as file:
+            with open(path, "w") as file:
                 file.write(yaml_str)
 
         # Only fail when there is a failure in jobs deployment.
         if databricks_responses is not None and any(response.is_left for response in databricks_responses):
             for response in databricks_responses:
                 if response.is_left:
                     print(response.left)
@@ -201,27 +235,30 @@
 
         log(f"\n\n{Colors.OKCYAN}Deployment completed successfully.\n{Colors.ENDC}")
 
         if self.project_config.migrate:
             log(f"\n\n{Colors.OKCYAN}Migrating project to new version. \n{Colors.ENDC}")
             try:
                 fabric_config_str = yaml.dump(
-                    data=remove_null_items_recursively(self.project_config.fabric_config_without_conf_replace.dict()))
+                    data=remove_null_items_recursively(self.project_config.fabric_config_without_conf_replace.dict())
+                )
                 system_config_str = yaml.dump(
-                    data=remove_null_items_recursively(self.project_config.system_config.dict()))
+                    data=remove_null_items_recursively(self.project_config.system_config.dict())
+                )
                 config_override_str = yaml.dump(
-                    data=remove_null_items_recursively(self.project_config.configs_override.dict()))
+                    data=remove_null_items_recursively(self.project_config.configs_override.dict())
+                )
 
-                with open(os.path.join(base_path, "fabrics.yml"), 'w') as file:
+                with open(os.path.join(base_path, "fabrics.yml"), "w") as file:
                     file.write(fabric_config_str)
 
-                with open(os.path.join(base_path, "system.yml"), 'w') as file:
+                with open(os.path.join(base_path, "system.yml"), "w") as file:
                     file.write(system_config_str)
 
-                with open(os.path.join(base_path, "override.yml"), 'w') as file:
+                with open(os.path.join(base_path, "override.yml"), "w") as file:
                     file.write(config_override_str)
 
                 log(f"\n\n{Colors.OKCYAN}Successfully migrated project to new version.\n{Colors.ENDC}")
             except Exception as e:
                 log(f"\n\n{Colors.FAIL}Failed to migrate project to new version.\n{Colors.ENDC}", e)
                 if os.path.isdir(base_path):
                     os.rmdir(base_path)
```

### Comparing `prophecy-build-tool-1.2.8/src/pbt/entities/project.py` & `prophecy-build-tool-1.2.9/src/pbt/entities/project.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.2.8/src/pbt/pbt_cli.py` & `prophecy-build-tool-1.2.9/src/pbt/pbt_cli.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.2.8/src/pbt/process.py` & `prophecy-build-tool-1.2.9/src/pbt/process.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.2.8/src/pbt/prophecy_build_tool.py` & `prophecy-build-tool-1.2.9/src/pbt/prophecy_build_tool.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.2.8/src/pbt/utility.py` & `prophecy-build-tool-1.2.9/src/pbt/utility.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.2.8/src/pbt/utils/constants.py` & `prophecy-build-tool-1.2.9/src/pbt/utils/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,10 +33,12 @@
 
 FABRIC_ID = "fabric_id"
 FABRIC_UID = "fabricUID"
 SECRET_SCOPE = "secret_scope"
 
 DBFS_FILE_STORE = "dbfs:/FileStore"
 S3_FILE_STORE = "s3://"
+HDFS_FILE_STORE = "hdfs://"
+LOCAL_FILE_STORE = "/"
 PROPHECY_ARTIFACTS = "prophecy/artifacts"
 
 NEW_JOB_STATE_FILE = "new_state.yml"
```

### Comparing `prophecy-build-tool-1.2.8/src/pbt/utils/exceptions.py` & `prophecy-build-tool-1.2.9/src/pbt/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.2.8/src/pbt/utils/project_config.py` & `prophecy-build-tool-1.2.9/src/pbt/utils/project_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 from asyncio import Future
 from concurrent.futures import as_completed
 from typing import List, Optional
 
 from pydantic import BaseModel
 from pydantic_yaml import parse_yaml_raw_as
 
-from .constants import PROPHECY_ARTIFACTS, DBFS_FILE_STORE
+from .constants import DBFS_FILE_STORE, PROPHECY_ARTIFACTS
 from .exceptions import ConfigFileNotFoundException
 from .project_models import Status
-from ..deployment import OperationType, JobInfoAndOperation
+from ..deployment import JobInfoAndOperation, OperationType
 from ..entities.project import Project
 from ..utility import Either, custom_print as log, is_online_mode
 
 
 class SchedulerType(enum.Enum):
     Composer = "Composer"
     MWAA = "MWAA"
     Databricks = "Databricks"
     Prophecy = "Prophecy"
     EMR = "EMR"
+    OpenSource = "OpenSource"
 
     @staticmethod
     def from_type(provider_type: str):
         return SchedulerType[provider_type]
 
 
 class FabricType(enum.Enum):
@@ -34,14 +35,15 @@
     Sql = "Sql"
     Airflow = "Airflow"
 
 
 class FabricProviderType(enum.Enum):
     Composer = "Composer"
     MWAA = "MWAA"
+    OpenSource = "OpenSource"
     Databricks = "Databricks"
     Prophecy = "Prophecy"
     EMR = "EMR"
     Dataproc = "Dataproc"
 
 
 class DeploymentMode(enum.Enum):
@@ -114,14 +116,25 @@
     access_key: str
     secret_key: str
     airflow_url: str
     dag_location: str
     environment_name: str
 
 
+class OpenSourceAirflowInfo(BaseModel):
+    airflow_url: str
+    airflow_username: str
+    airflow_password: str
+    uploader_url: str
+    uploader_username: str
+    uploader_password: str
+    dag_location: str
+    location: str
+
+
 # catpure the group.
 pattern = r"{{(\w+)}}"
 
 
 class DatabricksInfo(BaseModel):
     url: str
     token: str
@@ -143,22 +156,28 @@
 class FabricInfo(BaseModel):
     id: str
     name: str
     type: Optional[FabricType]  # sql/ databricks/ airflow
     provider: Optional[FabricProviderType]  # composer/mwaa/prophecy/databricks/dataproc
     composer: Optional[ComposerInfo] = None
     mwaa: Optional[MwaaInfo] = None
+    airflow_oss: Optional[OpenSourceAirflowInfo] = None
     databricks: Optional[DatabricksInfo] = None
     emr: Optional[EMRInfo] = None
     dataproc: Optional[DataprocInfo] = None
 
     @staticmethod
     def create_db_fabric(id: str, host: str, token: str):
-        return FabricInfo(id=id, name="", type=FabricType.Spark, provider=FabricProviderType.Databricks,
-                          databricks=DatabricksInfo.create(host, token))
+        return FabricInfo(
+            id=id,
+            name="",
+            type=FabricType.Spark,
+            provider=FabricProviderType.Databricks,
+            databricks=DatabricksInfo.create(host, token),
+        )
 
     def resolve(self):
         if self.databricks is not None:
             self.databricks.resolve()
 
         return self
 
@@ -173,30 +192,44 @@
     skip_processing: Optional[bool] = False  # this is useful in case when we deploy from older release tags.
     release_tag: Optional[str] = None
 
     def update_release_tag(self, release_tag):
         self.release_tag = release_tag
 
     def is_job_same_as(self, job_info) -> bool:
-        return self.external_job_id == job_info.external_job_id and self.fabric_id == job_info.fabric_id and \
-            self.id == job_info.id and self.name == job_info.name and self.type == job_info.type
+        return (
+            self.external_job_id == job_info.external_job_id
+            and self.fabric_id == job_info.fabric_id
+            and self.id == job_info.id
+            and self.name == job_info.name
+            and self.type == job_info.type
+        )
 
     def pause(self, flag: bool):
         self.is_paused = flag
 
     @staticmethod
-    def create_job(name: str, id: str, fabric_id: str, external_job_id: str, release_tag: str,
-                   is_paused: bool = False, fabric_provider_type: str = "Databricks"):
-        return JobInfo(name=name,
-                       type=SchedulerType.from_type(fabric_provider_type),
-                       id=id,
-                       fabric_id=fabric_id,
-                       external_job_id=external_job_id,
-                       release_tag=release_tag,
-                       is_paused=is_paused)
+    def create_job(
+        name: str,
+        id: str,
+        fabric_id: str,
+        external_job_id: str,
+        release_tag: str,
+        is_paused: bool = False,
+        fabric_provider_type: str = "Databricks",
+    ):
+        return JobInfo(
+            name=name,
+            type=SchedulerType.from_type(fabric_provider_type),
+            id=id,
+            fabric_id=fabric_id,
+            external_job_id=external_job_id,
+            release_tag=release_tag,
+            is_paused=is_paused,
+        )
 
 
 class ProjectAndGitTokens(BaseModel):
     project_id: str
     git_token: str = ""
 
 
@@ -211,41 +244,54 @@
     def get_fabric(self, fabric_id: str) -> Optional[FabricInfo]:
         return next((fabric for fabric in self.fabrics if fabric.id == fabric_id), None)
 
     def does_fabric_exist(self, fabric_id: str) -> bool:
         return self.get_fabric(fabric_id) is not None
 
     def git_token_for_project(self, project_id: str) -> Optional[str]:
-        return next((entity.git_token for entity in self.project_git_tokens if entity.project_id == project_id),
-                    None)
+        return next((entity.git_token for entity in self.project_git_tokens if entity.project_id == project_id), None)
 
     def is_prophecy_managed(self, fabric_id: str) -> bool:
         if self.get_fabric(fabric_id) is not None:
             fabric_info = self.get_fabric(fabric_id)
             return fabric_info.type == FabricType.Airflow and fabric_info.provider == FabricProviderType.Prophecy
 
         return False
 
     def is_fabric_emr_fabric(self, fabric_id: str) -> bool:
-        return any((fabric for fabric in self.fabrics if
-                    fabric.id == fabric_id and fabric.provider == FabricProviderType.EMR))
+        return any(
+            (fabric for fabric in self.fabrics if fabric.id == fabric_id and fabric.provider == FabricProviderType.EMR)
+        )
 
     def db_fabrics(self) -> List[str]:
         return [fabric.id for fabric in self.fabrics if fabric.provider == FabricProviderType.Databricks]
 
     def is_databricks_fabric(self, fabric_id: str) -> bool:
         return fabric_id in self.db_fabrics()
 
     def emr_fabrics(self) -> List[FabricInfo]:
-        return [fabric for fabric in self.fabrics if
-                (fabric.type == FabricType.Spark and fabric.provider == FabricProviderType.EMR)]
+        return [
+            fabric
+            for fabric in self.fabrics
+            if (fabric.type == FabricType.Spark and fabric.provider == FabricProviderType.EMR)
+        ]
 
     def dataproc_fabrics(self) -> List[FabricInfo]:
-        return [fabric for fabric in self.fabrics if
-                (fabric.type == FabricType.Spark and fabric.provider == FabricProviderType.Dataproc)]
+        return [
+            fabric
+            for fabric in self.fabrics
+            if (fabric.type == FabricType.Spark and fabric.provider == FabricProviderType.Dataproc)
+        ]
+
+    def airflow_open_source_fabrics(self) -> List[FabricInfo]:
+        return [
+            fabric
+            for fabric in self.fabrics
+            if (fabric.type == FabricType.Airflow and fabric.provider == FabricProviderType.OpenSource)
+        ]
 
     def list_all_fabrics(self) -> List[str]:
         return [fabric.id for fabric in self.fabrics]
 
     def filter_provided_fabrics(self, fabric_ids: str):
         if fabric_ids is not None and len(fabric_ids) > 0:
             fabrics = set(fabric_ids.split(","))
@@ -271,33 +317,29 @@
         return [job for job in self.jobs_to_process if job.type == SchedulerType.Databricks]
 
     @property
     def airflow_jobs(self) -> List[JobInfo]:
         return [job for job in self.jobs_to_process if job.type != SchedulerType.Databricks]
 
     def contains_job(self, job_id: str, fabric_uid: str) -> bool:
-        return any(
-            job.id == job_id and job.fabric_id == fabric_uid for job in self.jobs_to_process)
+        return any(job.id == job_id and job.fabric_id == fabric_uid for job in self.jobs_to_process)
 
     def all_jobs_for_id(self, job_id: str) -> List[JobInfo]:
         return [job for job in self.jobs_to_process if job.id == job_id]
 
     def job_for_id_and_fabric(self, job_id: str, fabric_id: str) -> Optional[JobInfo]:
-        return next(
-            (job for job in self.all_jobs_for_id(job_id) if job.fabric_id == fabric_id), None)
+        return next((job for job in self.all_jobs_for_id(job_id) if job.fabric_id == fabric_id), None)
 
     def filter_job(self, job_info) -> List[JobInfo]:
-        return [job for job in self.jobs if
-                not (job.id == job_info.id and job.fabric_id == job_info.fabric_id)]
+        return [job for job in self.jobs if not (job.id == job_info.id and job.fabric_id == job_info.fabric_id)]
 
     def update_state(self, jobs_responses: List[Either]):
-        filtered_response: List[JobInfoAndOperation] = [response.right for
-                                                        response
-                                                        in jobs_responses if
-                                                        response.is_right]
+        filtered_response: List[JobInfoAndOperation] = [
+            response.right for response in jobs_responses if response.is_right
+        ]
         # Important to do all operations in this order,
         # first we delete
         # then we refresh
         # then we create
 
         for job_response in filtered_response:
             job_info = job_response.job_info
@@ -348,18 +390,15 @@
 class ConfigsOverride(BaseModel):
     tests_enabled: Optional[bool] = False
     mode: Optional[DeploymentMode] = DeploymentMode.FullProject
     jobs_and_fabric: Optional[List[JobAndFabric]] = None
 
     def find_fabric_override_for_job(self, job_id: str) -> Optional[str]:
         if self.mode == DeploymentMode.SelectiveJob:
-            return next(
-                (entity.fabric_id for entity in self.jobs_and_fabric if entity.job_id == job_id),
-                None
-            )
+            return next((entity.fabric_id for entity in self.jobs_and_fabric if entity.job_id == job_id), None)
         return None
 
     def is_job_to_run(self, job_id) -> bool:
         if self.mode == DeploymentMode.SelectiveJob:
             return any(job_and_fabric.job_id == job_id for job_and_fabric in self.jobs_and_fabric)
         return True
 
@@ -383,48 +422,61 @@
     url: str
     username: str
     password: str
     repository: str
 
 
 class SystemConfig(BaseModel):
-    customer_name: Optional[str] = 'dev'
-    control_plane_name: Optional[str] = 'execution'
-    prophecy_salt: Optional[str] = 'execution'
+    customer_name: Optional[str] = "dev"
+    control_plane_name: Optional[str] = "execution"
+    prophecy_salt: Optional[str] = "execution"
     nexus: Optional[NexusConfig] = None
 
     def get_dbfs_base_path(self):
-        return f'{DBFS_FILE_STORE}/{PROPHECY_ARTIFACTS}/{self.customer_name}/{self.control_plane_name}'
+        return f"{DBFS_FILE_STORE}/{PROPHECY_ARTIFACTS}/{self.customer_name}/{self.control_plane_name}"
 
     def get_s3_base_path(self):
         return f"{PROPHECY_ARTIFACTS}/{self.customer_name}/{self.control_plane_name}"
 
+    def get_hdfs_base_path(self):
+        return f"{PROPHECY_ARTIFACTS}/{self.customer_name}/{self.control_plane_name}"
+
     @staticmethod
     def empty():
         return SystemConfig()
 
 
 def load_jobs_state(job_state_path: str, is_based_on_file: bool = True):
     if job_state_path is not None and len(job_state_path) > 0 and is_based_on_file and os.path.exists(job_state_path):
         with open(job_state_path, "r") as job_state:
             return parse_yaml_raw_as(JobsState, job_state.read())
     else:
         raise ConfigFileNotFoundException("Job state config path is not provided")
 
 
 def load_system_config(system_config_path: str, is_based_on_file: bool = True):
-    if system_config_path is not None and len(system_config_path) > 0 and is_based_on_file and os.path.exists(system_config_path):
+    if (
+        system_config_path is not None
+        and len(system_config_path) > 0
+        and is_based_on_file
+        and os.path.exists(system_config_path)
+    ):
         with open(system_config_path, "r") as system_config:
             return parse_yaml_raw_as(SystemConfig, system_config.read())
     else:
         raise ConfigFileNotFoundException("System config path is not provided")
 
 
 def load_configs_override(configs_override_path, is_based_on_file: bool = True):
-    if configs_override_path is not None and len(configs_override_path) > 0 and is_based_on_file and os.path.exists(configs_override_path):
+    if (
+        configs_override_path is not None
+        and len(configs_override_path) > 0
+        and is_based_on_file
+        and os.path.exists(configs_override_path)
+    ):
         with open(configs_override_path, "r") as config_override:
             return parse_yaml_raw_as(ConfigsOverride, config_override.read())
     else:
         return ConfigsOverride.empty()
 
 
 def load_fabric_config(fabric_config_path):
@@ -432,53 +484,71 @@
         with open(fabric_config_path, "r") as fabric_config:
             return parse_yaml_raw_as(FabricConfig, fabric_config.read())
     else:
         raise ConfigFileNotFoundException("Fabric config path is not provided")
 
 
 class ProjectConfig:
-    def __init__(self, jobs_state: JobsState, fabric_config: FabricConfig, system_config: SystemConfig,
-                 config_override: ConfigsOverride, based_on_file: bool = True, skip_builds: bool = False,
-                 migrate: bool = False, conf_folder: str = ""):
+    def __init__(
+        self,
+        jobs_state: JobsState,
+        fabric_config: FabricConfig,
+        system_config: SystemConfig,
+        config_override: ConfigsOverride,
+        based_on_file: bool = True,
+        skip_builds: bool = False,
+        migrate: bool = False,
+        conf_folder: str = "",
+    ):
         self.jobs_state = jobs_state
         self.system_config = system_config
         self.configs_override = config_override
         self.based_on_file = based_on_file
         self.skip_builds = skip_builds
         self.migrate = migrate
         self.conf_folder = conf_folder
         self.fabric_config_without_conf_replace = copy.deepcopy(fabric_config)
         self.fabric_config = fabric_config.resolve_env_vars()
 
     @staticmethod
-    def from_path(project: Project, job_state_path: str, system_config_path: str, configs_override_path: str,
-                  fabric_config_path: str, fabric_ids: str, job_ids: str, skip_build: bool, conf_folder: str,
-                  migrate: bool):
+    def from_path(
+        project: Project,
+        job_state_path: str,
+        system_config_path: str,
+        configs_override_path: str,
+        fabric_config_path: str,
+        fabric_ids: str,
+        job_ids: str,
+        skip_build: bool,
+        conf_folder: str,
+        migrate: bool,
+    ):
 
         is_based_on_file = conf_folder != "" and len(conf_folder) > 0
 
         if is_online_mode() and len(conf_folder) > 0:
             jobs = load_jobs_state(job_state_path)
             fabrics = load_fabric_config(fabric_config_path)
             system = load_system_config(system_config_path)
             configs = load_configs_override(configs_override_path)
             return ProjectConfig(jobs, fabrics, system, configs, skip_builds=skip_build)
 
         else:
 
             if not is_based_on_file:
                 # only cli case for databricks/ fabrics
-                host = os.environ.get("DATABRICKS_HOST", 'test')
-                token = os.environ.get("DATABRICKS_TOKEN", 'test')
+                host = os.environ.get("DATABRICKS_HOST", "test")
+                token = os.environ.get("DATABRICKS_TOKEN", "test")
                 if not fabric_ids:
                     allowed_fabrics = project.fabrics()
                 else:
                     allowed_fabrics = fabric_ids.split(",")
-                fabric_list = [FabricInfo.create_db_fabric(id=fabric, host=host, token=token) for fabric in
-                               allowed_fabrics]
+                fabric_list = [
+                    FabricInfo.create_db_fabric(id=fabric, host=host, token=token) for fabric in allowed_fabrics
+                ]
                 fabrics_config = FabricConfig(fabrics=fabric_list)
 
             else:
                 # most important files.
                 # fabrics
                 fabrics_config = load_fabric_config(fabric_config_path)
                 fabrics_config.filter_provided_fabrics(fabric_ids)
@@ -507,29 +577,46 @@
                 configs = ConfigsOverride.empty()
                 configs.mode = DeploymentMode.FullProject  # only build what's needed.
                 if len(job_ids) != 0:
                     allowed_jobs = job_ids.split(",")
                     configs.jobs_and_fabric = [JobAndFabric.create(f"jobs/{job}", "") for job in allowed_jobs]
                     configs.mode = DeploymentMode.SelectiveJob
 
-            return ProjectConfig(jobs, fabrics_config, system, configs, based_on_file=is_based_on_file,
-                                 skip_builds=skip_build, migrate=migrate)
+            return ProjectConfig(
+                jobs,
+                fabrics_config,
+                system,
+                configs,
+                based_on_file=is_based_on_file,
+                skip_builds=skip_build,
+                migrate=migrate,
+            )
 
     # best used when invoking from execution.
     @classmethod
-    def from_conf_folder(cls, project: Project, conf_folder, fabric_ids: str, job_ids: str, skip_builds: bool,
-                         migrate: bool):
+    def from_conf_folder(
+        cls, project: Project, conf_folder, fabric_ids: str, job_ids: str, skip_builds: bool, migrate: bool
+    ):
         jobs_state = os.path.join(conf_folder, "state.yml")
         system_config = os.path.join(conf_folder, "system.yml")
         config_override = os.path.join(conf_folder, "override.yml")
         fabric_config = os.path.join(conf_folder, "fabrics.yml")
 
-        return ProjectConfig.from_path(project, jobs_state, system_config, config_override, fabric_config, fabric_ids,
-                                       job_ids,
-                                       skip_builds, conf_folder, migrate)
+        return ProjectConfig.from_path(
+            project,
+            jobs_state,
+            system_config,
+            config_override,
+            fabric_config,
+            fabric_ids,
+            job_ids,
+            skip_builds,
+            conf_folder,
+            migrate,
+        )
 
 
 def await_futures_and_update_states(futures: List[Future], step_id: str):
     responses = []
 
     for future in as_completed(futures):
         responses.append(future.result())
```

### Comparing `prophecy-build-tool-1.2.8/src/pbt/utils/project_models.py` & `prophecy-build-tool-1.2.9/src/pbt/utils/project_models.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.2.8/src/prophecy_build_tool.egg-info/PKG-INFO` & `prophecy-build-tool-1.2.9/src/prophecy_build_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prophecy-build-tool
-Version: 1.2.8
+Version: 1.2.9
 Summary: Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the Prophecy IDE.
 Home-page: https://github.com/SimpleDataLabsInc/prophecy-build-tool
 Author: Prophecy
 Author-email: maciej@prophecy.io
 Project-URL: Bug Tracker, https://github.com/SimpleDataLabsInc/prophecy-build-tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prophecy-build-tool-1.2.8/src/prophecy_build_tool.egg-info/SOURCES.txt` & `prophecy-build-tool-1.2.9/src/prophecy_build_tool.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 src/pbt/client/nexus.py
 src/pbt/client/rest_client_factory.py
 src/pbt/client/s3.py
 src/pbt/client/airflow/__init__.py
 src/pbt/client/airflow/airflow_utility.py
 src/pbt/client/airflow/composer.py
 src/pbt/client/airflow/mwaa.py
+src/pbt/client/airflow/open_source.py
 src/pbt/deployment/__init__.py
 src/pbt/deployment/gems.py
 src/pbt/deployment/pipeline.py
 src/pbt/deployment/project.py
 src/pbt/deployment/jobs/__init__.py
 src/pbt/deployment/jobs/airflow.py
 src/pbt/deployment/jobs/databricks.py
```

### Comparing `prophecy-build-tool-1.2.8/test/test_build.py` & `prophecy-build-tool-1.2.9/test/test_build.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.2.8/test/test_deploy.py` & `prophecy-build-tool-1.2.9/test/test_deploy.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.2.8/test/test_testing.py` & `prophecy-build-tool-1.2.9/test/test_testing.py`

 * *Files identical despite different names*

