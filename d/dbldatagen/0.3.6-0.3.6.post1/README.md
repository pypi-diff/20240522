# Comparing `tmp/dbldatagen-0.3.6.tar.gz` & `tmp/dbldatagen-0.3.6.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbldatagen-0.3.6.tar", last modified: Sat Feb 24 02:01:00 2024, max compression
+gzip compressed data, was "dbldatagen-0.3.6.post1.tar", last modified: Wed May 22 19:35:57 2024, max compression
```

## Comparing `dbldatagen-0.3.6.tar` & `dbldatagen-0.3.6.post1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 02:01:00.783411 dbldatagen-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-02-24 02:01:00.783411 dbldatagen-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 02:01:00.779411 dbldatagen-0.3.6/dbldatagen/
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/dbldatagen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/dbldatagen/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    61096 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/dbldatagen/column_generation_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    12519 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/dbldatagen/column_spec_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    17966 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/dbldatagen/data_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)    66481 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/dbldatagen/data_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/dbldatagen/datagen_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/dbldatagen/datarange.py
--rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/dbldatagen/daterange.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 02:01:00.783411 dbldatagen-0.3.6/dbldatagen/distributions/
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/dbldatagen/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/dbldatagen/distributions/beta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/dbldatagen/distributions/data_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/dbldatagen/distributions/exponential_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/dbldatagen/distributions/gamma.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/dbldatagen/distributions/normal_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/dbldatagen/function_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/dbldatagen/html_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/dbldatagen/nrange.py
--rw-r--r--   0 runner    (1001) docker     (127)    15512 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/dbldatagen/schema_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/dbldatagen/spark_singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)    15709 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/dbldatagen/text_generator_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    41986 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/dbldatagen/text_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/dbldatagen/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 02:01:00.783411 dbldatagen-0.3.6/dbldatagen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-02-24 02:01:00.000000 dbldatagen-0.3.6/dbldatagen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-02-24 02:01:00.000000 dbldatagen-0.3.6/dbldatagen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-24 02:01:00.000000 dbldatagen-0.3.6/dbldatagen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-24 02:01:00.000000 dbldatagen-0.3.6/dbldatagen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-24 02:01:00.783411 dbldatagen-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-02-24 02:00:20.000000 dbldatagen-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:35:57.703834 dbldatagen-0.3.6.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-05-22 19:35:57.703834 dbldatagen-0.3.6.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:35:57.703834 dbldatagen-0.3.6.post1/dbldatagen/
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/dbldatagen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/dbldatagen/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61096 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/dbldatagen/column_generation_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12519 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/dbldatagen/column_spec_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20365 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/dbldatagen/data_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66481 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/dbldatagen/data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/dbldatagen/datagen_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/dbldatagen/datarange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/dbldatagen/daterange.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:35:57.703834 dbldatagen-0.3.6.post1/dbldatagen/distributions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/dbldatagen/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/dbldatagen/distributions/beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/dbldatagen/distributions/data_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/dbldatagen/distributions/exponential_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/dbldatagen/distributions/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/dbldatagen/distributions/normal_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/dbldatagen/function_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/dbldatagen/html_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/dbldatagen/nrange.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15512 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/dbldatagen/schema_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/dbldatagen/spark_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15709 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/dbldatagen/text_generator_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41986 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/dbldatagen/text_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/dbldatagen/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:35:57.703834 dbldatagen-0.3.6.post1/dbldatagen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-05-22 19:35:57.000000 dbldatagen-0.3.6.post1/dbldatagen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-22 19:35:57.000000 dbldatagen-0.3.6.post1/dbldatagen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 19:35:57.000000 dbldatagen-0.3.6.post1/dbldatagen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 19:35:57.000000 dbldatagen-0.3.6.post1/dbldatagen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-22 19:35:57.703834 dbldatagen-0.3.6.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-22 19:35:11.000000 dbldatagen-0.3.6.post1/setup.py
```

### Comparing `dbldatagen-0.3.6/CHANGELOG.md` & `dbldatagen-0.3.6.post1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 # Databricks Labs Data Generator Release Notes
 
 ## Change History
 All notable changes to the Databricks Labs Data Generator will be documented in this file.
 
+
+### Version 0.3.6 Post 1
+
+#### Changed
+* Updated docs for complex data types / JSON to correct code examples
+* Updated license file in public docs
+
+#### Fixed 
+* Fixed scenario where `DataAnalyzer` is used on dataframe containing a column named `summary`
+
+
 ### Version 0.3.6
 
 #### Changed
 * Updated readme to include details on which versions of Databricks runtime support Unity Catalog `shared` access mode.
 * Updated code to use default parallelism of 200 when using a shared Spark session
 * Updated code to use Spark's SQL function `element_at` instead of array indexing due to incompatibility
```

### Comparing `dbldatagen-0.3.6/CONTRIBUTING.md` & `dbldatagen-0.3.6.post1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/LICENSE` & `dbldatagen-0.3.6.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/PKG-INFO` & `dbldatagen-0.3.6.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbldatagen
-Version: 0.3.6
+Version: 0.3.6.post1
 Summary: Databricks Labs -  PySpark Synthetic Data Generator
 Home-page: https://github.com/databrickslabs/data-generator
 Author: Ronan Stokes, Databricks
 License: Databricks License
 Project-URL: Databricks Labs, https://www.databricks.com/learn/labs
 Project-URL: Documentation, https://databrickslabs.github.io/dbldatagen/public_docs/index.html
 Classifier: Programming Language :: Python :: 3
@@ -20,14 +20,15 @@
 
 <!-- Top bar will be removed from PyPi packaged versions -->
 
 [![build](https://github.com/databrickslabs/dbldatagen/workflows/build/badge.svg?branch=master)](https://github.com/databrickslabs/dbldatagen/actions?query=workflow%3Abuild+branch%3Amaster)
 [![PyPi package](https://img.shields.io/pypi/v/dbldatagen?color=green)](https://pypi.org/project/dbldatagen/)
 [![codecov](https://codecov.io/gh/databrickslabs/dbldatagen/branch/master/graph/badge.svg)](https://codecov.io/gh/databrickslabs/dbldatagen)
 [![PyPi downloads](https://img.shields.io/pypi/dm/dbldatagen?label=PyPi%20Downloads)](https://pypistats.org/packages/dbldatagen)
+[![lines of code](https://tokei.rs/b1/github/databrickslabs/dbldatagen)]([https://codecov.io/github/databrickslabs/dbldatagen](https://github.com/databrickslabs/dbldatagen))
 
 <!-- 
 [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/databrickslabs/dbldatagen.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/databrickslabs/dbldatagen/context:python)
 [![downloads](https://img.shields.io/github/downloads/databrickslabs/dbldatagen/total.svg)](https://hanadigital.github.io/grev/?user=databrickslabs&repo=dbldatagen)
 -->
 
 ## Project Description
@@ -71,15 +72,15 @@
 ## Documentation
 
 Please refer to the [online documentation](https://databrickslabs.github.io/dbldatagen/public_docs/index.html) for 
 details of use and many examples.
 
 Release notes and details of the latest changes for this specific release
 can be found in the GitHub repository
-[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.6/CHANGELOG.md)
+[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.6post1/CHANGELOG.md)
 
 # Installation
 
 Use `pip install dbldatagen` to install the PyPi package.
 
 Within a Databricks notebook, invoke the following in a notebook cell
 ```commandline
```

### Comparing `dbldatagen-0.3.6/PULL_REQUEST_TEMPLATE.md` & `dbldatagen-0.3.6.post1/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/README.md` & `dbldatagen-0.3.6.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 [Tutorial](tutorial) 
 <!-- Dont remove: end exclude package -->
 
 [![build](https://github.com/databrickslabs/dbldatagen/workflows/build/badge.svg?branch=master)](https://github.com/databrickslabs/dbldatagen/actions?query=workflow%3Abuild+branch%3Amaster)
 [![PyPi package](https://img.shields.io/pypi/v/dbldatagen?color=green)](https://pypi.org/project/dbldatagen/)
 [![codecov](https://codecov.io/gh/databrickslabs/dbldatagen/branch/master/graph/badge.svg)](https://codecov.io/gh/databrickslabs/dbldatagen)
 [![PyPi downloads](https://img.shields.io/pypi/dm/dbldatagen?label=PyPi%20Downloads)](https://pypistats.org/packages/dbldatagen)
+[![lines of code](https://tokei.rs/b1/github/databrickslabs/dbldatagen)]([https://codecov.io/github/databrickslabs/dbldatagen](https://github.com/databrickslabs/dbldatagen))
 
 <!-- 
 [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/databrickslabs/dbldatagen.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/databrickslabs/dbldatagen/context:python)
 [![downloads](https://img.shields.io/github/downloads/databrickslabs/dbldatagen/total.svg)](https://hanadigital.github.io/grev/?user=databrickslabs&repo=dbldatagen)
 -->
 
 ## Project Description
@@ -59,15 +60,15 @@
 ## Documentation
 
 Please refer to the [online documentation](https://databrickslabs.github.io/dbldatagen/public_docs/index.html) for 
 details of use and many examples.
 
 Release notes and details of the latest changes for this specific release
 can be found in the GitHub repository
-[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.6/CHANGELOG.md)
+[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.6post1/CHANGELOG.md)
 
 # Installation
 
 Use `pip install dbldatagen` to install the PyPi package.
 
 Within a Databricks notebook, invoke the following in a notebook cell
 ```commandline
```

### Comparing `dbldatagen-0.3.6/dbldatagen/__init__.py` & `dbldatagen-0.3.6.post1/dbldatagen/__init__.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/dbldatagen/_version.py` & `dbldatagen-0.3.6.post1/dbldatagen/_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     major, minor, patch, release, build = r.match(version).groups()
     version_info = VersionInfo(major, minor, patch, release, build)
     logger = logging.getLogger(__name__)
     logger.info("Version : %s", version_info)
     return version_info
 
 
-__version__ = "0.3.6"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
+__version__ = "0.3.6post1"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
 __version_info__ = get_version(__version__)
 
 
 def _get_spark_version(sparkVersion):
     try:
         r = re.compile(r'(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>.*)')
         major, minor, patch, release = r.match(sparkVersion).groups()
```

### Comparing `dbldatagen-0.3.6/dbldatagen/column_generation_spec.py` & `dbldatagen-0.3.6.post1/dbldatagen/column_generation_spec.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/dbldatagen/column_spec_options.py` & `dbldatagen-0.3.6.post1/dbldatagen/column_spec_options.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/dbldatagen/data_analyzer.py` & `dbldatagen-0.3.6.post1/dbldatagen/data_analyzer.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,30 +3,36 @@
 #
 
 """
 This module defines the ``DataAnalyzer`` class.
 
 This code is experimental and both APIs and code generated is liable to change in future versions.
 """
-from pyspark.sql.types import LongType, FloatType, IntegerType, StringType, DoubleType, BooleanType, ShortType, \
-    TimestampType, DateType, DecimalType, ByteType, BinaryType, StructType, ArrayType, DataType
+import logging
 
 import pyspark.sql as ssql
-import pyspark.sql.functions as F
+from pyspark.sql.types import LongType, FloatType, IntegerType, StringType, DoubleType, BooleanType, ShortType, \
+    TimestampType, DateType, DecimalType, ByteType, BinaryType, StructType, ArrayType, DataType
 
-from .utils import strip_margins
 from .spark_singleton import SparkSingleton
+from .utils import strip_margins
+
+SUMMARY_FIELD_NAME = "summary"
+SUMMARY_FIELD_NAME_RENAMED = "__summary__"
+DATA_SUMMARY_FIELD_NAME = "__data_summary__"
 
 
 class DataAnalyzer:
     """This class is used to analyze an existing data set to assist in generating a test data set with similar
     characteristics, and to generate code from existing schemas and data
 
     :param df: Spark dataframe to analyze
     :param sparkSession: Spark session instance to use when performing spark operations
+    :param debug: If True, additional debug information is logged
+    :param verbose: If True, additional information is logged
 
     .. warning::
        Experimental
 
     """
     _DEFAULT_GENERATED_NAME = "synthetic_data"
 
@@ -39,29 +45,48 @@
                         |#   Github project - [https://github.com/databrickslabs/dbldatagen]
                         |#""", '|')
 
     _GENERATED_FROM_SCHEMA_COMMENT = strip_margins("""
                         |# Column definitions are stubs only - modify to generate correct data  
                         |#""", '|')
 
-    def __init__(self, df=None, sparkSession=None):
+    def __init__(self, df=None, sparkSession=None, debug=False, verbose=False):
         """ Constructor:
         :param df: Dataframe to analyze
         :param sparkSession: Spark session to use
         """
+        # set up logging
+        self.verbose = verbose
+        self.debug = debug
+
+        self._setupLogger()
+
         assert df is not None, "dataframe must be supplied"
 
         self._df = df
 
         if sparkSession is None:
             sparkSession = SparkSingleton.getLocalInstance()
 
         self._sparkSession = sparkSession
         self._dataSummary = None
 
+    def _setupLogger(self):
+        """Set up logging
+
+        This will set the logger at warning, info or debug levels depending on the instance construction parameters
+        """
+        self.logger = logging.getLogger("DataAnalyzer")
+        if self.debug:
+            self.logger.setLevel(logging.DEBUG)
+        elif self.verbose:
+            self.logger.setLevel(logging.INFO)
+        else:
+            self.logger.setLevel(logging.WARNING)
+
     def _displayRow(self, row):
         """Display details for row"""
         results = []
         row_key_pairs = row.asDict()
         for x in row_key_pairs:
             results.append(f"{x}: {row[x]}")
 
@@ -91,14 +116,39 @@
         if dfSummary is not None:
             dfResult = dfSummary.union(dfData.selectExpr(*exprs).limit(rowLimit))
         else:
             dfResult = dfData.selectExpr(*exprs).limit(rowLimit)
 
         return dfResult
 
+    def _get_dataframe_describe_stats(self, df):
+        """ Get summary statistics for dataframe handling renaming of summary field if necessary"""
+        print("schema", df.schema)
+
+        src_fields = [fld.name for fld in df.schema.fields]
+        print("src_fields", src_fields)
+        renamed_summary = False
+
+        # get summary statistics handling the case where a field named 'summary' exists
+        # if the `summary` field name exists, we'll rename it to avoid a conflict
+        if SUMMARY_FIELD_NAME in src_fields:
+            renamed_summary = True
+            df = df.withColumnRenamed(SUMMARY_FIELD_NAME, SUMMARY_FIELD_NAME_RENAMED)
+
+        # The dataframe describe method produces a field named `summary`. We'll rename this to avoid conflict with
+        # any natural fields using the same name.
+        summary_df = df.describe().withColumnRenamed(SUMMARY_FIELD_NAME, DATA_SUMMARY_FIELD_NAME)
+
+        # if we renamed a field called `summary` in the data, we'll rename it back.
+        # The data summary field produced by the describe method has already been renamed so there will be no conflict.
+        if renamed_summary:
+            summary_df = summary_df.withColumnRenamed(SUMMARY_FIELD_NAME_RENAMED, SUMMARY_FIELD_NAME)
+
+        return summary_df
+
     def summarizeToDF(self):
         """ Generate summary analysis of data set as dataframe
 
         :return: Summary results as dataframe
 
         The resulting dataframe can be displayed with the ``display`` function in a notebook environment
         or with the ``show`` method.
@@ -150,19 +200,20 @@
 
         dfDataSummary = self._addMeasureToSummary(
             'max',
             fieldExprs=[f"string(max({dtype[0]})) as {dtype[0]}" for dtype in dtypes],
             dfData=self._df,
             dfSummary=dfDataSummary)
 
-        descriptionDf = self._df.describe().where("summary in ('mean', 'stddev')")
+        descriptionDf = (self._get_dataframe_describe_stats(self._df)
+                         .where(f"{DATA_SUMMARY_FIELD_NAME} in ('mean', 'stddev')"))
         describeData = descriptionDf.collect()
 
         for row in describeData:
-            measure = row['summary']
+            measure = row[DATA_SUMMARY_FIELD_NAME]
 
             values = {k[0]: '' for k in dtypes}
 
             row_key_pairs = row.asDict()
             for k1 in row_key_pairs:
                 values[k1] = str(row[k1])
 
@@ -397,15 +448,20 @@
 
         :param suppressOutput: Suppress printing of generated code if True
         :param name: Optional name for data generator
         :return: String containing skeleton code
 
         """
         assert self._df is not None
-        assert type(self._df) is ssql.DataFrame, "sourceDf must be a valid Pyspark dataframe"
+
+        if not isinstance(self._df, ssql.DataFrame):
+            self.logger.warning(strip_margins(
+                """The parameter `sourceDf` should be a valid Pyspark dataframe.
+                   |Note this warning may false due to use of remote connection to a Spark cluster""",
+                '|'))
 
         if self._dataSummary is None:
             df_summary = self.summarizeToDF()
 
             self._dataSummary = {}
             for row in df_summary.collect():
                 row_key_pairs = row.asDict()
```

### Comparing `dbldatagen-0.3.6/dbldatagen/data_generator.py` & `dbldatagen-0.3.6.post1/dbldatagen/data_generator.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/dbldatagen/datagen_constants.py` & `dbldatagen-0.3.6.post1/dbldatagen/datagen_constants.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/dbldatagen/datarange.py` & `dbldatagen-0.3.6.post1/dbldatagen/datarange.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/dbldatagen/daterange.py` & `dbldatagen-0.3.6.post1/dbldatagen/daterange.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/dbldatagen/distributions/__init__.py` & `dbldatagen-0.3.6.post1/dbldatagen/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/dbldatagen/distributions/beta.py` & `dbldatagen-0.3.6.post1/dbldatagen/distributions/beta.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/dbldatagen/distributions/data_distribution.py` & `dbldatagen-0.3.6.post1/dbldatagen/distributions/data_distribution.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/dbldatagen/distributions/exponential_distribution.py` & `dbldatagen-0.3.6.post1/dbldatagen/distributions/exponential_distribution.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/dbldatagen/distributions/gamma.py` & `dbldatagen-0.3.6.post1/dbldatagen/distributions/gamma.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/dbldatagen/distributions/normal_distribution.py` & `dbldatagen-0.3.6.post1/dbldatagen/distributions/normal_distribution.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/dbldatagen/function_builder.py` & `dbldatagen-0.3.6.post1/dbldatagen/function_builder.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/dbldatagen/html_utils.py` & `dbldatagen-0.3.6.post1/dbldatagen/html_utils.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/dbldatagen/nrange.py` & `dbldatagen-0.3.6.post1/dbldatagen/nrange.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/dbldatagen/schema_parser.py` & `dbldatagen-0.3.6.post1/dbldatagen/schema_parser.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/dbldatagen/spark_singleton.py` & `dbldatagen-0.3.6.post1/dbldatagen/spark_singleton.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/dbldatagen/text_generator_plugins.py` & `dbldatagen-0.3.6.post1/dbldatagen/text_generator_plugins.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/dbldatagen/text_generators.py` & `dbldatagen-0.3.6.post1/dbldatagen/text_generators.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/dbldatagen/utils.py` & `dbldatagen-0.3.6.post1/dbldatagen/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     Define a deprecated decorator without dependencies on 3rd party libraries
 
     Note there is a 3rd party library called `deprecated` that provides this feature but goal is to only have
     dependencies on packages already used in the Databricks runtime
     """
 
     # create closure around function that follows use of the decorator
-
     def deprecated_decorator(func):
         @functools.wraps(func)
         def deprecated_func(*args, **kwargs):
             warnings.warn(f"`{func.__name__}` is a deprecated function or method. \n{message}",
                           category=DeprecationWarning, stacklevel=1)
             warnings.simplefilter('default', DeprecationWarning)
             return func(*args, **kwargs)
@@ -286,15 +285,14 @@
     It will handle multiple matches performing splits on each match.
 
     For example, the following code will produce the results below:
 
     x = ['id', 'city_name', 'id', 'city_id', 'city_pop', 'id', 'city_id', 'city_pop','city_id', 'city_pop','id']
     splitListOnCondition(x, lambda el: el == 'id')
 
-
     Result:
     `[['id'], ['city_name'], ['id'], ['city_id', 'city_pop'],
       ['id'], ['city_id', 'city_pop', 'city_id', 'city_pop'], ['id']]`
 
     :arg lst: list of items to perform condition matches against
     :arg cond: lambda function or function taking single argument and returning True or False
     :returns: list of sublists
```

### Comparing `dbldatagen-0.3.6/dbldatagen.egg-info/PKG-INFO` & `dbldatagen-0.3.6.post1/dbldatagen.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbldatagen
-Version: 0.3.6
+Version: 0.3.6.post1
 Summary: Databricks Labs -  PySpark Synthetic Data Generator
 Home-page: https://github.com/databrickslabs/data-generator
 Author: Ronan Stokes, Databricks
 License: Databricks License
 Project-URL: Databricks Labs, https://www.databricks.com/learn/labs
 Project-URL: Documentation, https://databrickslabs.github.io/dbldatagen/public_docs/index.html
 Classifier: Programming Language :: Python :: 3
@@ -20,14 +20,15 @@
 
 <!-- Top bar will be removed from PyPi packaged versions -->
 
 [![build](https://github.com/databrickslabs/dbldatagen/workflows/build/badge.svg?branch=master)](https://github.com/databrickslabs/dbldatagen/actions?query=workflow%3Abuild+branch%3Amaster)
 [![PyPi package](https://img.shields.io/pypi/v/dbldatagen?color=green)](https://pypi.org/project/dbldatagen/)
 [![codecov](https://codecov.io/gh/databrickslabs/dbldatagen/branch/master/graph/badge.svg)](https://codecov.io/gh/databrickslabs/dbldatagen)
 [![PyPi downloads](https://img.shields.io/pypi/dm/dbldatagen?label=PyPi%20Downloads)](https://pypistats.org/packages/dbldatagen)
+[![lines of code](https://tokei.rs/b1/github/databrickslabs/dbldatagen)]([https://codecov.io/github/databrickslabs/dbldatagen](https://github.com/databrickslabs/dbldatagen))
 
 <!-- 
 [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/databrickslabs/dbldatagen.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/databrickslabs/dbldatagen/context:python)
 [![downloads](https://img.shields.io/github/downloads/databrickslabs/dbldatagen/total.svg)](https://hanadigital.github.io/grev/?user=databrickslabs&repo=dbldatagen)
 -->
 
 ## Project Description
@@ -71,15 +72,15 @@
 ## Documentation
 
 Please refer to the [online documentation](https://databrickslabs.github.io/dbldatagen/public_docs/index.html) for 
 details of use and many examples.
 
 Release notes and details of the latest changes for this specific release
 can be found in the GitHub repository
-[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.6/CHANGELOG.md)
+[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.6post1/CHANGELOG.md)
 
 # Installation
 
 Use `pip install dbldatagen` to install the PyPi package.
 
 Within a Databricks notebook, invoke the following in a notebook cell
 ```commandline
```

### Comparing `dbldatagen-0.3.6/dbldatagen.egg-info/SOURCES.txt` & `dbldatagen-0.3.6.post1/dbldatagen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.6/setup.py` & `dbldatagen-0.3.6.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     The Databricks Labs Data Generator can generate realistic synthetic data sets at scale for testing, 
     benchmarking, environment validation and other purposes.
     """
 
 setuptools.setup(
     name="dbldatagen",
-    version="0.3.6",
+    version="0.3.6post1",
     author="Ronan Stokes, Databricks",
     description="Databricks Labs -  PySpark Synthetic Data Generator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/databrickslabs/data-generator",
     project_urls={
         "Databricks Labs": "https://www.databricks.com/learn/labs",
```

