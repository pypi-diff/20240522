# Comparing `tmp/vantage6-algorithm-store-4.4.1.tar.gz` & `tmp/vantage6-algorithm-store-4.5.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-algorithm-store-4.4.1.tar", last modified: Wed May  8 12:54:35 2024, max compression
+gzip compressed data, was "vantage6-algorithm-store-4.5.0rc3.tar", last modified: Wed May 22 15:05:00 2024, max compression
```

## Comparing `vantage6-algorithm-store-4.4.1.tar` & `vantage6-algorithm-store-4.5.0rc3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.956863 vantage6-algorithm-store-4.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-05-08 12:54:35.956863 vantage6-algorithm-store-4.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 12:54:35.956863 vantage6-algorithm-store-4.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.948863 vantage6-algorithm-store-4.4.1/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.948863 vantage6-algorithm-store-4.4.1/vantage6/algorithm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.952863 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/__build__
--rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/default_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.952863 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/argument.py
--rw-r--r--   0 runner    (1001) docker     (127)    13848 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.952863 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/common/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/common/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/common/ui_visualization_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/developer_algorithm_association.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/review.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/role.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/role_rule_association.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/ui_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/vantage6_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.956863 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/resource/
--rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20580 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/resource/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/resource/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/resource/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.956863 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/resource/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/resource/schema/input_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/resource/schema/output_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    12971 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/resource/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     7064 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/resource/vantage6_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/resource/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-08 12:54:22.000000 vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.956863 vantage6-algorithm-store-4.4.1/vantage6_algorithm_store.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-05-08 12:54:35.000000 vantage6-algorithm-store-4.4.1/vantage6_algorithm_store.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-08 12:54:35.000000 vantage6-algorithm-store-4.4.1/vantage6_algorithm_store.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:54:35.000000 vantage6-algorithm-store-4.4.1/vantage6_algorithm_store.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-08 12:54:35.000000 vantage6-algorithm-store-4.4.1/vantage6_algorithm_store.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 12:54:35.000000 vantage6-algorithm-store-4.4.1/vantage6_algorithm_store.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:05:00.093293 vantage6-algorithm-store-4.5.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9709 2024-05-22 15:05:00.093293 vantage6-algorithm-store-4.5.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:05:00.097293 vantage6-algorithm-store-4.5.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:05:00.089293 vantage6-algorithm-store-4.5.0rc3/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:05:00.089293 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:05:00.089293 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/__build__
+-rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/default_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:05:00.093293 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13848 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:05:00.093293 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/common/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/common/ui_visualization_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/developer_algorithm_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/review.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/role_rule_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/ui_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/vantage6_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:05:00.093293 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21490 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:05:00.093293 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/schema/input_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/schema/output_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12971 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7064 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/vantage6_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-22 15:04:46.000000 vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:05:00.093293 vantage6-algorithm-store-4.5.0rc3/vantage6_algorithm_store.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9709 2024-05-22 15:05:00.000000 vantage6-algorithm-store-4.5.0rc3/vantage6_algorithm_store.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-22 15:05:00.000000 vantage6-algorithm-store-4.5.0rc3/vantage6_algorithm_store.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:05:00.000000 vantage6-algorithm-store-4.5.0rc3/vantage6_algorithm_store.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-22 15:05:00.000000 vantage6-algorithm-store-4.5.0rc3/vantage6_algorithm_store.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 15:05:00.000000 vantage6-algorithm-store-4.5.0rc3/vantage6_algorithm_store.egg-info/top_level.txt
```

### Comparing `vantage6-algorithm-store-4.4.1/PKG-INFO` & `vantage6-algorithm-store-4.5.0rc3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-algorithm-store
-Version: 4.4.1
+Version: 4.5.0rc3
 Summary: Vantage6 algorithm store
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
@@ -12,47 +12,51 @@
   <a href="https://vantage6.ai"><img src="https://github.com/IKNL/guidelines/blob/master/resources/logos/vantage6.png?raw=true" alt="vantage6" width="350"></a>
 </h1>
 
 <h3 align=center> A Privacy Enhancing Technology (PET) Operations platform</h3>
 <h3 align="center">
 
 <!-- Badges go here-->
+
 [![Release](https://github.com/vantage6/vantage6/actions/workflows/release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/release.yml)
 [![PyPI vantage6](https://badge.fury.io/py/vantage6.svg)](https://badge.fury.io/py/vantage6)
 [![Unittests](https://github.com/vantage6/vantage6/actions/workflows/unit_tests.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/unit_tests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/vantage6/vantage6/badge.svg?branch=main)](https://coveralls.io/github/vantage6/vantage6?branch=main)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/2e60ac3b3f284620805f7399cba317be)](https://www.codacy.com/gh/vantage6/vantage6/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=vantage6/vantage6&amp;utm_campaign=Badge_Grade)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7382602.svg)](https://doi.org/10.5281/zenodo.7382602)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/2e60ac3b3f284620805f7399cba317be)](https://app.codacy.com/gh/vantage6/vantage6/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![DOI](https://zenodo.org/badge/492818831.svg)](https://zenodo.org/badge/latestdoi/492818831)
+
 </h3>
 
 <p align="center">
   <a href="#books-quickstart">Quickstart</a> •
   <a href="#project-structure">Project structure</a> •
   <a href="#gift_heart-join-the-community">Join the community</a> •
   <a href="#black_nib-references">References</a>
 </p>
 
+---
 
------------------------------------------------------------------------------------------------------
 This repository is contains all the **vantage6** infrastructure source code. The **vantage6** technology enables to manage and deploy privacy enhancing technologies like Federated Learning (FL) and Multi-Party Computation (MPC). Please visit our [website (vantage6.ai)](https://vantage6.ai) to learn more!
 
 You can find more (user) documentation at [readthedocs (docs.vantage6.ai)](https://docs.vantage6.ai). If you have any questions, suggestions or just want to chat about federated learning: join our [Discord (https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel.
 
 ## Infrastructure overview
 
 ![Vantage6 architecture overview](docs/images/overview-infrastructure.png)
 
-*A High level overview of the vantage6 infrastructure. Vantage6 has both a client-server and peer-to-peer architecture. The client is used by the researcher to create (PET) computation requests. It is also used to manage users, organizations and collaborations. The server contains users, organizations, collaborations, tasks and their results. It provides a central access point for both the clients and nodes. The nodes have access to privacy sensitive data and handle computation requests retrieved from the server. Computation request are executed as separate containers on the node. These containers are connected to containers at other nodes by a VPN network.*
+_A High level overview of the vantage6 infrastructure. Vantage6 has both a client-server and peer-to-peer architecture. The client is used by the researcher to create (PET) computation requests. It is also used to manage users, organizations and collaborations. The server contains users, organizations, collaborations, tasks and their results. It provides a central access point for both the clients and nodes. The nodes have access to privacy sensitive data and handle computation requests retrieved from the server. Computation request are executed as separate containers on the node. These containers are connected to containers at other nodes by a VPN network._
 
 ## :books: Quickstart
 
 ### Requirements
+
 The **vantage6** infrastructure is delivered in Docker images. To run these images, you need to have [Docker](https://docs.docker.com/get-docker/) installed. To install the latest version of the vantage6 CLI, you need to have [Python](https://www.python.org/downloads/), we recommend using an environment manager like [mini-conda](https://docs.conda.io/en/latest/miniconda.html).
 
 Install the latest version of the vantage6 CLI by using:
+
 ```bash
 pip install vantage6
 ```
 
 This install the `v6` commands, which allows you to manage your nodes and servers. To view all available options, run:
 
 ```bash
@@ -79,16 +83,16 @@
 
 # View server logs
 v6 server attach
 ```
 
 From here you can use the [vantage6-client](https://pypi.org/project/vantage6-client) to interact with the server. The demo network has a pre-configured organization with the following credentials:
 
-* Username: `org_1-admin`
-* Password: `password`
+- Username: `org_1-admin`
+- Password: `password`
 
 For example, you can create a new organization by running:
 
 ```python
 from vantage6.client import Client
 
 client = Client('http://127.0.0.1', 5000, '/api', log_level='debug')
@@ -106,69 +110,74 @@
 ```
 
 You can find more (user) documentation at [readthedocs (docs.vantage6.ai)](https://docs.vantage6.ai)
 
 ## Project structure
 
 ### PYPI packages
+
 This repository is home to 6 PyPi packages:
 
-* [vantage6](https://pypi.org/project/vantage6) -> _CLI for managing node and server instances_
-* [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client for interacting with the vantage6-server_
-* [vantage6-algorithm-tools](https://pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate algorithm development_
-* [vantage6-node](https://pypi.org/project/vantage6-node) -> _Node application package_
-* [vantage6-server](https://pypi.org/project/vantage6-server) -> _Server application package_
-* [vantage6-algorithm-store](https://pypi.org/project/vantage6-algorithm-store) -> _Algorithm store application package_
-* [vantage6-common](https://pypi.org/project/vantage6-common) -> _Package with common vantage6 functions_
-* [vantage6-backend-common](https://pypi.org/project/vantage6-backend-common) -> _Package with functions common to central server and algorithm store_
+- [vantage6](https://pypi.org/project/vantage6) -> _CLI for managing node and server instances_
+- [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client for interacting with the vantage6-server_
+- [vantage6-algorithm-tools](https://pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate algorithm development_
+- [vantage6-node](https://pypi.org/project/vantage6-node) -> _Node application package_
+- [vantage6-server](https://pypi.org/project/vantage6-server) -> _Server application package_
+- [vantage6-algorithm-store](https://pypi.org/project/vantage6-algorithm-store) -> _Algorithm store application package_
+- [vantage6-common](https://pypi.org/project/vantage6-common) -> _Package with common vantage6 functions_
+- [vantage6-backend-common](https://pypi.org/project/vantage6-backend-common) -> _Package with functions common to central server and algorithm store_
 
 **Note that when using vantage6 you do not install the _server_ and _node_ packages. These are delivered to you in Docker images.**
 
 This repository also hosts the code for the vantage6 user interface (UI). The UI
 is an Angular web application that can be used to interact with the vantage6 server
 easily.
 
 ### Docker images
+
 The vantage6 infrastructure is delivered in Docker images. All Docker images are stored in our private [Harbor](https://goharbor.io/) registry. The most important images are:
 
-* `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application Docker image_
-* `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server application Docker image_
-* `harbor2.vantage6.ai/infrastructure/ui:VERSION` -> _User interface Docker image_
-* `harbor2.vantage6.ai/infrastructure/algorithm-store:VERSION` -> _Algorithm store Docker image_
+- `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application Docker image_
+- `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server application Docker image_
+- `harbor2.vantage6.ai/infrastructure/ui:VERSION` -> _User interface Docker image_
+- `harbor2.vantage6.ai/infrastructure/algorithm-store:VERSION` -> _Algorithm store Docker image_
 
 with `VERSION` being the full semantic version of the vantage6 infrastructure, e.g. `4.0.0` or `4.1.0rc0`.
 
 Several other images are used to support the infrastructure:
 
-* `harbor2.vantage6.ai/infrastructure/infrastructure-base:VERSION` -> _Base image for the infrastructure_
-* `harbor2.vantage6.ai/infrastructure/squid:VERSION` -> _Squid proxy image used for the whitelisting service_
-* `harbor2.vantage6.ai/infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_
-* `harbor2.vantage6.ai/infrastructure/vpn-client` -> _VPN image used to connect to the VPN_
-* `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN image used for initialization_
-* `harbor2.vantage6.ai/infrastructure/ssh-tunnel` -> _SSH tunnel image used for connecting algorithms to external services_
+- `harbor2.vantage6.ai/infrastructure/infrastructure-base:VERSION` -> _Base image for the infrastructure_
+- `harbor2.vantage6.ai/infrastructure/squid:VERSION` -> _Squid proxy image used for the whitelisting service_
+- `harbor2.vantage6.ai/infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_
+- `harbor2.vantage6.ai/infrastructure/vpn-client` -> _VPN image used to connect to the VPN_
+- `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN image used for initialization_
+- `harbor2.vantage6.ai/infrastructure/ssh-tunnel` -> _SSH tunnel image used for connecting algorithms to external services_
 
 And finally there are some images released for algorithm development:
 
-* `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base image for algorithm development_
-* `harbor2.vantage6.ai/infrastructure/algorithm-ohdsi-base:MAJOR.MINOR` -> _Extended algorithm base image for OHDSI algorithm development_
+- `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base image for algorithm development_
+- `harbor2.vantage6.ai/infrastructure/algorithm-ohdsi-base:MAJOR.MINOR` -> _Extended algorithm base image for OHDSI algorithm development_
 
 ## :gift_heart: Join the community!
+
 We hope to continue developing, improving, and supporting **vantage6** with the help of the federated learning community. If you are interested in contributing, first of all, thank you! Second, please take a look at our [contributing guidelines](https://docs.vantage6.ai/en/main/devops/contribute.html)
 
 <a href="https://github.com/vantage6/vantage6/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=vantage6/vantage6" />
 </a>
 
 ## :black_nib: References
+
 If you are using **vantage6**, please cite this repository as well as the accompanying papers as follows:
 
-> * F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6. Available at https://doi.org/10.5281/zenodo.7221216. Accessed on MONTH, 20XX.
-> * A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse. VANTAGE6: an open source priVAcy preserviNg federaTed leArninG infrastructurE for Secure Insight eXchange. AMIA Annual Symposium Proceedings, 2020, p. 870-877. [[BibTeX](https://arturomoncadatorres.com/bibtex/moncada-torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)]
-> * D. Smits\*, B. van Beusekom\*, F. Martin, L. Veen, G. Geleijnse, A. Moncada-Torres, An Improved Infrastructure for Privacy-Preserving Analysis of Patient Data, Proceedings of the International Conference of Informatics, Management, and Technology in Healthcare (ICIMTH), vol. 25, 2022, p. 144-147. [[BibTeX](https://arturomoncadatorres.com/bibtex/smits2022improved.txt), [PDF](https://ebooks.iospress.nl/volumearticle/60190)]
+> - F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6. Available at https://doi.org/10.5281/zenodo.7221216. Accessed on MONTH, 20XX.
+> - A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse. VANTAGE6: an open source priVAcy preserviNg federaTed leArninG infrastructurE for Secure Insight eXchange. AMIA Annual Symposium Proceedings, 2020, p. 870-877. [[BibTeX](https://arturomoncadatorres.com/bibtex/moncada-torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)]
+> - D. Smits\*, B. van Beusekom\*, F. Martin, L. Veen, G. Geleijnse, A. Moncada-Torres, An Improved Infrastructure for Privacy-Preserving Analysis of Patient Data, Proceedings of the International Conference of Informatics, Management, and Technology in Healthcare (ICIMTH), vol. 25, 2022, p. 144-147. [[BibTeX](https://arturomoncadatorres.com/bibtex/smits2022improved.txt), [PDF](https://ebooks.iospress.nl/volumearticle/60190)]
+
+---
 
------------------------------------------------------------------------------------------------------
 <p align="center">
   <a href="https://vantage6.ai">vantage6.ai</a> •
   <a href="https://discord.gg/yAyFf6Y">Discord</a> •
   <a href="https://vantage6.discourse.group/">Discourse</a> •
   <a href="https://docs.vantage6.ai">User documentation</a> •
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-algorithm-store Version: 4.4.1 Summary:
+Metadata-Version: 2.1 Name: vantage6-algorithm-store Version: 4.5.0rc3 Summary:
 Vantage6 algorithm store Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10 Description-Content-Type: text/markdown Provides-Extra:
 dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
@@ -10,38 +10,37 @@
 rreelleeaassee..yymmll)) [[!![[PPyyPPII vvaannttaaggee66]]((hhttttppss::////bbaaddggee..ffuurryy..iioo//ppyy//vvaannttaaggee66..ssvvgg))]]((hhttttppss::////
 bbaaddggee..ffuurryy..iioo//ppyy//vvaannttaaggee66)) [[!![[UUnniitttteessttss]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//
    aaccttiioonnss//wwoorrkkfflloowwss//uunniitt__tteessttss..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//
     vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//uunniitt__tteessttss..yymmll)) [[!![[CCoovveerraaggee SSttaattuuss]]((hhttttppss::////
  ccoovveerraallllss..iioo//rreeppooss//ggiitthhuubb//vvaannttaaggee66//vvaannttaaggee66//bbaaddggee..ssvvgg??bbrraanncchh==mmaaiinn))]]((hhttttppss::////
  ccoovveerraallllss..iioo//ggiitthhuubb//vvaannttaaggee66//vvaannttaaggee66??bbrraanncchh==mmaaiinn)) [[!![[CCooddaaccyy BBaaddggee]]((hhttttppss::////
 aapppp..ccooddaaccyy..ccoomm//pprroojjeecctt//bbaaddggee//GGrraaddee//22ee6600aacc33bb33ff228844662200880055ff77339999ccbbaa331177bbee))]]((hhttttppss::////
-                     wwwwww..ccooddaaccyy..ccoomm//gghh//vvaannttaaggee66//vvaannttaaggee66//
-   ddaasshhbbooaarrdd??uuttmm__ssoouurrccee==ggiitthhuubb..ccoomm&&uuttmm__mmeeddiiuumm==rreeffeerrrraall&&uuttmm__ccoonntteenntt==vvaannttaaggee66//
-   vvaannttaaggee66&&uuttmm__ccaammppaaiiggnn==BBaaddggee__GGrraaddee)) [[!![[DDOOII]]((hhttttppss::////zzeennooddoo..oorrgg//bbaaddggee//DDOOII//
-   1100..55228811//zzeennooddoo..77338822660022..ssvvgg))]]((hhttttppss::////ddooii..oorrgg//1100..55228811//zzeennooddoo..77338822660022)) ********
+                     aapppp..ccooddaaccyy..ccoomm//gghh//vvaannttaaggee66//vvaannttaaggee66//
+ddaasshhbbooaarrdd??uuttmm__ssoouurrccee==gghh&&uuttmm__mmeeddiiuumm==rreeffeerrrraall&&uuttmm__ccoonntteenntt==&&uuttmm__ccaammppaaiiggnn==BBaaddggee__ggrraaddee))
+  [[!![[DDOOII]]((hhttttppss::////zzeennooddoo..oorrgg//bbaaddggee//449922881188883311..ssvvgg))]]((hhttttppss::////zzeennooddoo..oorrgg//bbaaddggee//
+                           llaatteessttddooii//449922881188883311)) ********
     _Q_u_i_c_k_s_t_a_r_t â¢ _P_r_o_j_e_c_t_ _s_t_r_u_c_t_u_r_e â¢ _J_o_i_n_ _t_h_e_ _c_o_m_m_u_n_i_t_y â¢ _R_e_f_e_r_e_n_c_e_s
--------------------------------------------------------------------------------
----------------------- This repository is contains all the **vantage6**
-infrastructure source code. The **vantage6** technology enables to manage and
-deploy privacy enhancing technologies like Federated Learning (FL) and Multi-
-Party Computation (MPC). Please visit our [website (vantage6.ai)](https://
-vantage6.ai) to learn more! You can find more (user) documentation at
-[readthedocs (docs.vantage6.ai)](https://docs.vantage6.ai). If you have any
-questions, suggestions or just want to chat about federated learning: join our
-[Discord (https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel. ##
+--- This repository is contains all the **vantage6** infrastructure source
+code. The **vantage6** technology enables to manage and deploy privacy
+enhancing technologies like Federated Learning (FL) and Multi-Party Computation
+(MPC). Please visit our [website (vantage6.ai)](https://vantage6.ai) to learn
+more! You can find more (user) documentation at [readthedocs
+(docs.vantage6.ai)](https://docs.vantage6.ai). If you have any questions,
+suggestions or just want to chat about federated learning: join our [Discord
+(https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel. ##
 Infrastructure overview ![Vantage6 architecture overview](docs/images/overview-
-infrastructure.png) *A High level overview of the vantage6 infrastructure.
+infrastructure.png) _A High level overview of the vantage6 infrastructure.
 Vantage6 has both a client-server and peer-to-peer architecture. The client is
 used by the researcher to create (PET) computation requests. It is also used to
 manage users, organizations and collaborations. The server contains users,
 organizations, collaborations, tasks and their results. It provides a central
 access point for both the clients and nodes. The nodes have access to privacy
 sensitive data and handle computation requests retrieved from the server.
 Computation request are executed as separate containers on the node. These
-containers are connected to containers at other nodes by a VPN network.* ## :
+containers are connected to containers at other nodes by a VPN network._ ## :
 books: Quickstart ### Requirements The **vantage6** infrastructure is delivered
 in Docker images. To run these images, you need to have [Docker](https://
 docs.docker.com/get-docker/) installed. To install the latest version of the
 vantage6 CLI, you need to have [Python](https://www.python.org/downloads/), we
 recommend using an environment manager like [mini-conda](https://docs.conda.io/
 en/latest/miniconda.html). Install the latest version of the vantage6 CLI by
 using: ```bash pip install vantage6 ``` This install the `v6` commands, which
@@ -50,75 +49,74 @@
 using: ```bash v6 dev create-demo-network ``` This creates a local network with
 a server and two nodes. You can start the network by running: ```bash v6 dev
 start-demo-network ``` This will start the server and nodes in the background.
 You can view the logs by running: ```bash # View node logs v6 node attach #
 View server logs v6 server attach ``` From here you can use the [vantage6-
 client](https://pypi.org/project/vantage6-client) to interact with the server.
 The demo network has a pre-configured organization with the following
-credentials: * Username: `org_1-admin` * Password: `password` For example, you
+credentials: - Username: `org_1-admin` - Password: `password` For example, you
 can create a new organization by running: ```python from vantage6.client import
 Client client = Client('http://127.0.0.1', 5000, '/api', log_level='debug')
 client.authenticate('org_1-admin', 'password') client.setup_encryption(None)
 client.organization.create( name='My organization', address1='My address',
 address2='My address', zipcode='1234AB', country='The Netherlands', domain='my-
 organization.com' ) ``` You can find more (user) documentation at [readthedocs
 (docs.vantage6.ai)](https://docs.vantage6.ai) ## Project structure ### PYPI
-packages This repository is home to 6 PyPi packages: * [vantage6](https://
-pypi.org/project/vantage6) -> _CLI for managing node and server instances_ *
+packages This repository is home to 6 PyPi packages: - [vantage6](https://
+pypi.org/project/vantage6) -> _CLI for managing node and server instances_ -
 [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client
-for interacting with the vantage6-server_ * [vantage6-algorithm-tools](https://
+for interacting with the vantage6-server_ - [vantage6-algorithm-tools](https://
 pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate
-algorithm development_ * [vantage6-node](https://pypi.org/project/vantage6-
-node) -> _Node application package_ * [vantage6-server](https://pypi.org/
-project/vantage6-server) -> _Server application package_ * [vantage6-algorithm-
+algorithm development_ - [vantage6-node](https://pypi.org/project/vantage6-
+node) -> _Node application package_ - [vantage6-server](https://pypi.org/
+project/vantage6-server) -> _Server application package_ - [vantage6-algorithm-
 store](https://pypi.org/project/vantage6-algorithm-store) -> _Algorithm store
-application package_ * [vantage6-common](https://pypi.org/project/vantage6-
-common) -> _Package with common vantage6 functions_ * [vantage6-backend-common]
+application package_ - [vantage6-common](https://pypi.org/project/vantage6-
+common) -> _Package with common vantage6 functions_ - [vantage6-backend-common]
 (https://pypi.org/project/vantage6-backend-common) -> _Package with functions
 common to central server and algorithm store_ **Note that when using vantage6
 you do not install the _server_ and _node_ packages. These are delivered to you
 in Docker images.** This repository also hosts the code for the vantage6 user
 interface (UI). The UI is an Angular web application that can be used to
 interact with the vantage6 server easily. ### Docker images The vantage6
 infrastructure is delivered in Docker images. All Docker images are stored in
 our private [Harbor](https://goharbor.io/) registry. The most important images
-are: * `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application
-Docker image_ * `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server
-application Docker image_ * `harbor2.vantage6.ai/infrastructure/ui:VERSION` -
-> _User interface Docker image_ * `harbor2.vantage6.ai/infrastructure/
+are: - `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application
+Docker image_ - `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server
+application Docker image_ - `harbor2.vantage6.ai/infrastructure/ui:VERSION` -
+> _User interface Docker image_ - `harbor2.vantage6.ai/infrastructure/
 algorithm-store:VERSION` -> _Algorithm store Docker image_ with `VERSION` being
 the full semantic version of the vantage6 infrastructure, e.g. `4.0.0` or
-`4.1.0rc0`. Several other images are used to support the infrastructure: *
+`4.1.0rc0`. Several other images are used to support the infrastructure: -
 `harbor2.vantage6.ai/infrastructure/infrastructure-base:VERSION` -> _Base image
-for the infrastructure_ * `harbor2.vantage6.ai/infrastructure/squid:VERSION` -
-> _Squid proxy image used for the whitelisting service_ * `harbor2.vantage6.ai/
-infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_ *
+for the infrastructure_ - `harbor2.vantage6.ai/infrastructure/squid:VERSION` -
+> _Squid proxy image used for the whitelisting service_ - `harbor2.vantage6.ai/
+infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_ -
 `harbor2.vantage6.ai/infrastructure/vpn-client` -> _VPN image used to connect
-to the VPN_ * `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN
-image used for initialization_ * `harbor2.vantage6.ai/infrastructure/ssh-
+to the VPN_ - `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN
+image used for initialization_ - `harbor2.vantage6.ai/infrastructure/ssh-
 tunnel` -> _SSH tunnel image used for connecting algorithms to external
 services_ And finally there are some images released for algorithm development:
-* `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base
-image for algorithm development_ * `harbor2.vantage6.ai/infrastructure/
+- `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base
+image for algorithm development_ - `harbor2.vantage6.ai/infrastructure/
 algorithm-ohdsi-base:MAJOR.MINOR` -> _Extended algorithm base image for OHDSI
 algorithm development_ ## :gift_heart: Join the community! We hope to continue
 developing, improving, and supporting **vantage6** with the help of the
 federated learning community. If you are interested in contributing, first of
 all, thank you! Second, please take a look at our [contributing guidelines]
 (https://docs.vantage6.ai/en/main/devops/contribute.html) _[_h_t_t_p_s_:_/_/
 _c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_v_a_n_t_a_g_e_6_/_v_a_n_t_a_g_e_6_]## :black_nib: References If you are
 using **vantage6**, please cite this repository as well as the accompanying
-papers as follows: > * F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6.
+papers as follows: > - F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6.
 Available at https://doi.org/10.5281/zenodo.7221216. Accessed on MONTH, 20XX. >
-* A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse.
+- A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse.
 VANTAGE6: an open source priVAcy preserviNg federaTed leArninG infrastructurE
 for Secure Insight eXchange. AMIA Annual Symposium Proceedings, 2020, p. 870-
 877. [[BibTeX](https://arturomoncadatorres.com/bibtex/moncada-
-torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)] > * D. Smits\*,
+torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)] > - D. Smits\*,
 B. van Beusekom\*, F. Martin, L. Veen, G. Geleijnse, A. Moncada-Torres, An
 Improved Infrastructure for Privacy-Preserving Analysis of Patient Data,
 Proceedings of the International Conference of Informatics, Management, and
 Technology in Healthcare (ICIMTH), vol. 25, 2022, p. 144-147. [[BibTeX](https:/
 /arturomoncadatorres.com/bibtex/smits2022improved.txt), [PDF](https://
-ebooks.iospress.nl/volumearticle/60190)] --------------------------------------
----------------------------------------------------------------
+ebooks.iospress.nl/volumearticle/60190)] ---
        _v_a_n_t_a_g_e_6_._a_i â¢ _D_i_s_c_o_r_d â¢ _D_i_s_c_o_u_r_s_e â¢ _U_s_e_r_ _d_o_c_u_m_e_n_t_a_t_i_o_n â¢
```

### Comparing `vantage6-algorithm-store-4.4.1/setup.py` & `vantage6-algorithm-store-4.5.0rc3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     long_description_content_type="text/markdown",
     url="https://github.com/vantage6/vantage6",
     packages=find_namespace_packages(),
     python_requires=">=3.10",
     install_requires=[
         "flasgger==0.9.5",
         "flask==2.2.5",
-        "Flask-Cors==3.0.10",
+        "Flask-Cors==4.0.1",
         "Flask-Principal==0.4.0",
         "flask-marshmallow==0.15.0",
         "Flask-RESTful==0.3.10",
         "gevent==23.9.1",
         "jsonschema==4.21.1",
         "marshmallow==3.19.0",
         "requests==2.31.0",
```

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/__init__.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
             It is important to close the db session to avoid having dangling
             sessions.
             """
             if error.code == 404:
                 log.debug("404 error for route '%s'", _get_request_path(request))
             else:
                 log.warning("HTTP Exception occured during request")
-                log.debug("%s", traceback.format_exc())
+                log.warning("%s", traceback.format_exc())
             DatabaseSessionManager.clear_session()
             return error.get_response()
 
         @self.app.errorhandler(Exception)
         def error2_remove_db_session(error):
             """In case an exception occurs during the request.
 
@@ -285,15 +285,15 @@
 
         # add whitelisted server and root user from config file if they do not exist
         if root_user := self.ctx.config.get("root_user", {}):
             whitelisted_uri = root_user.get("v6_server_uri")
             root_username = root_user.get("username")
             if whitelisted_uri and root_username:
                 if not (v6_server := db.Vantage6Server.get_by_url(whitelisted_uri)):
-                    log.debug("This server will be whitelisted: %s", whitelisted_uri)
+                    log.info("This server will be whitelisted: %s", whitelisted_uri)
                     v6_server = db.Vantage6Server(url=whitelisted_uri)
                     v6_server.save()
 
                 # if the user does not exist already, add it
                 if not db.User.get_by_server(
                     username=root_username, v6_server_id=v6_server.id
                 ):
```

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/_version.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/_version.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, "__build__")) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = (4, 4, 1, "final", __build__, 0)
+version_info = (4, 5, 0, "candidate", __build__, 0)
 
 # Module version stage suffix map
 _specifier_ = {"alpha": "a", "beta": "b", "candidate": "rc", "final": ""}
 version = f"{version_info[0]}.{version_info[1]}.{version_info[2]}"
 pre_release = (
     ""
     if version_info[3] == "final"
```

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/db.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     Function,
     Permission,
     Role,
     Rule,
     User,
     Review,
     Vantage6Server,
+    role_rule_association,
 )
 from vantage6.common import logger_name
 from vantage6.common.globals import STRING_ENCODING
 
 
 module_name = logger_name(__name__)
 log = logging.getLogger(module_name)
```

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/default_roles.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/default_roles.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/globals.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/__init__.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/algorithm.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/algorithm.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/argument.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/argument.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/base.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/base.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/common/enums.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/common/enums.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/common/ui_visualization_schemas.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/common/ui_visualization_schemas.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/database.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/database.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/function.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/function.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/permission.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/permission.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 Permission = Table(
     "Permission",
     Base.metadata,
     Column("user_id", Integer, ForeignKey("user.id")),
     Column("role_id", Integer, ForeignKey("role.id")),
 )
 
+# TODO when this is activated, also include the changes in the rule endpoints (e.g.
+# where there is a filter by user)
 # TODO: integrate this with the Permission model from the v6 server
 # UserPermission = Table(
 #     'UserPermission',
 #     Base.metadata,
 #     Column('rule_id', Integer, ForeignKey('rule.id')),
 #     Column('user_id', Integer, ForeignKey('user.id'))
 # )
```

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/review.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/review.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/role.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/role.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/role_rule_association.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/role_rule_association.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/rule.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/rule.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/ui_visualization.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/ui_visualization.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/user.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/user.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/model/vantage6_server.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/model/vantage6_server.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/permission.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/permission.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/resource/__init__.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/resource/algorithm.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
             "name",
             "description",
             "image",
             "partitioning",
             "vantage6_version",
         ]:
             if (value := request.args.get(field)) is not None:
-                q = q.filter(getattr(db_Algorithm, field).like(f"%{value}%"))
+                q = q.filter(getattr(db_Algorithm, field).like(value))
 
         # paginate results
         try:
             page = Pagination.from_query(q, request, db.Algorithm)
         except (ValueError, AttributeError) as e:
             return {"msg": str(e)}, HTTPStatus.BAD_REQUEST
 
@@ -496,14 +496,33 @@
                                 type: string
                                 description: Description of the argument
                               type:
                                 type: string
                                 description: Type of argument. Can be 'string',
                                   'integer', 'float', 'boolean', 'json',
                                   'column', 'organizations' or 'organization'
+                        ui_visualizations:
+                          type: array
+                          description: List of visualizations that are available in
+                            the algorithm
+                          items:
+                            properties:
+                              name:
+                                type: string
+                                description: Name of the visualization
+                              description:
+                                type: string
+                                description: Description of the visualization
+                              type:
+                                type: string
+                                description: Type of visualization.
+                              schema:
+                                type: object
+                                description: Schema that describes the visualization.
+
 
         responses:
           201:
             description: Algorithm created successfully
           400:
             description: Invalid input
           401:
```

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/resource/role.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/role.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/resource/rule.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/vantage6_server.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,217 +1,242 @@
 import logging
 
-from http import HTTPStatus
-from flask.globals import request
-from flask import g
+from flask import g, request
 from flask_restful import Api
-from sqlalchemy import or_
-
+from http import HTTPStatus
 from vantage6.common import logger_name
-from vantage6.algorithm.store import db
-from vantage6.algorithm.store.resource import (
-    AlgorithmStoreResources,
-    with_authentication,
+from vantage6.algorithm.store.resource.schema.input_schema import (
+    Vantage6ServerInputSchema,
+)
+from vantage6.algorithm.store.resource.schema.output_schema import (
+    Vantage6ServerOutputSchema,
 )
-from vantage6.algorithm.store.resource.schema.output_schema import RuleOutputSchema
-from vantage6.backend.common.resource.pagination import Pagination
+from vantage6.algorithm.store.model.vantage6_server import (
+    Vantage6Server as db_Vantage6Server,
+)
+from vantage6.algorithm.store.resource import with_authentication
+
+# TODO move to common / refactor
+from vantage6.algorithm.store.resource import AlgorithmStoreResources
 
 
 module_name = logger_name(__name__)
 log = logging.getLogger(module_name)
-rule_schema = RuleOutputSchema()
 
 
 def setup(api: Api, api_base: str, services: dict) -> None:
     """
-    Setup the rule resource.
+    Setup the version resource.
 
     Parameters
     ----------
     api : Api
         Flask restful api instance
     api_base : str
         Base url of the api
     services : dict
         Dictionary with services required for the resource endpoints
     """
     path = "/".join([api_base, module_name])
-    log.info(f'Setting up "{path}" and subdirectories')
+    log.info('Setting up "%s" and subdirectories', path)
+
+    api.add_resource(
+        Vantage6Servers,
+        api_base + "/vantage6-server",
+        endpoint="server_without_id",
+        methods=("GET", "POST"),
+        resource_class_kwargs=services,
+    )
 
     api.add_resource(
-        Rules,
-        path,
-        endpoint="rule_without_id",
-        methods=("GET",),
+        Vantage6Server,
+        api_base + "/vantage6-server/<int:id>",
+        endpoint="server_with_id",
+        methods=("GET", "DELETE"),
         resource_class_kwargs=services,
     )
-    # api.add_resource(
-    #     Rule,
-    #     path + "/<int:id>",
-    #     endpoint="rule_with_id",
-    #     methods=("GET",),
-    #     resource_class_kwargs=services,
-    # )
+
+
+v6_server_input_schema = Vantage6ServerInputSchema()
+v6_server_output_schema = Vantage6ServerOutputSchema()
 
 
 # ------------------------------------------------------------------------------
 # Resources / API's
 # ------------------------------------------------------------------------------
-class Rules(AlgorithmStoreResources):
+class Vantage6Servers(AlgorithmStoreResources):
+    """Resource for /algorithm"""
+
     @with_authentication()
     def get(self):
-        """List algorithm store rules
+        """List whitelisted vantage6 servers
         ---
-        description: >-
-            List of all available rules at the algorithm store. The user must be
-            authenticated, but does not require any additional permissions to
-            view the rules.
+        description: Return a list of vantage6 servers that are whitelisted
+          in this algorithm store instance.
 
         parameters:
-            - in: query
-              name: name
-              schema:
-                type: string
-              description: Filter by name of the rule
-            - in: query
-              name: operation
-              schema:
-                type: string
-              description: Get rules for a specific type of operation
-            - in: query
-              name: role_id
-              schema:
-                type: integer
-              description: Get rules for a specific role
-            - in: query
-              name: page
-              schema:
-                type: integer
-              description: Page number for pagination (default=1)
-            - in: query
-              name: per_page
-              schema:
-                type: integer
-              description: Number of items per page (default=10)
-            - in: query
-              name: sort
-              schema:
-                type: string
-              description: >-
-                Sort by one or more fields, separated by a comma. Use a minus
-                sign (-) in front of the field to sort in descending order.
-            - in: query
-              name: no_pagination
-              schema:
-                type: int
-              description: >-
-                If set to 1, pagination is disabled and all items are returned.
+          - in: query
+            name: url
+            schema:
+              type: string
+            description: Filter on algorithm name using the SQL operator LIKE.
 
         responses:
           200:
-            description: Ok
+            description: OK
           400:
-            description: Improper values for pagination or sorting parameters
+            description: Invalid input
+          401:
+            description: Unauthorized
 
         security:
-            - bearerAuth: []
+          - bearerAuth: []
 
-        tags: ["Rule"]
+        tags: ["Vantage6 Server"]
         """
-        q = g.session.query(db.Rule)
-
+        # TODO add pagination
+        # TODO extend filtering
         args = request.args
+        q = g.session.query(db_Vantage6Server)
+
+        if "url" in args:
+            q = q.filter(db_Vantage6Server.url.like(args["url"]))
+
+        servers = q.all()
+        return v6_server_output_schema.dump(servers, many=True), HTTPStatus.OK
+
+    # Note: this endpoint is not authenticated, because it is used by the
+    # vantage6 server to whitelist itself.
+    def post(self):
+        """Create new whitelisted vantage6 server
+        ---
+        description: >-
+          Whitelist a new vantage6 server in this algorithm store instance.
+
+        requestBody:
+          content:
+            application/json:
+              schema:
+                properties:
+                  url:
+                    type: string
+                    description: URL of the vantage6 server
+                  force:
+                    type: boolean
+                    description: Force creation of the vantage6 server. If a
+
+        responses:
+          201:
+            description: Algorithm created successfully
+          400:
+            description: Invalid input
+          401:
+            description: Unauthorized
+
+        security:
+          - bearerAuth: []
+
+        tags: ["Vantage6 Server"]
+        """
+        data = request.get_json()
+
+        # validate the request body
+        errors = v6_server_input_schema.validate(data)
+        if errors:
+            return {
+                "msg": "Request body is incorrect",
+                "errors": errors,
+            }, HTTPStatus.BAD_REQUEST
+
+        # issue a warning if someone tries to whitelist localhost
+        force = data.get("force", False)
+        # TODO make function in common to test for localhost
+        if not force and ("localhost" in data["url"] or "127.0.0.1" in data["url"]):
+            return {
+                "msg": "You are trying to whitelist a localhost address for a "
+                "vantage6 server. This is not secure and should only be "
+                "done for development servers. If you are sure you want to "
+                "whitelist localhost, please specify the 'force' parameter in"
+                " the request body."
+            }, HTTPStatus.BAD_REQUEST
+
+        # delete any existing record with the same url to prevent duplicates
+        existing_server = db_Vantage6Server.get_by_url(data["url"])
+        if existing_server:
+            existing_server.delete()
+
+        # create the whitelisted server record
+        server = db_Vantage6Server(url=data["url"])
+        server.save()
+
+        return v6_server_output_schema.dump(server, many=False), HTTPStatus.CREATED
+
+
+class Vantage6Server(AlgorithmStoreResources):
+    """Resource for /algorithm/<id>"""
+
+    @with_authentication()
+    def get(self, id):
+        """Get specific whitelisted vantage6 server
+        ---
+        description: Return an vantage6 server specified by ID.
+
+        parameters:
+          - in: path
+            name: id
+            schema:
+              type: integer
+            description: ID of the algorithm
+
+        responses:
+          200:
+            description: OK
+          401:
+            description: Unauthorized
+          404:
+            description: Algorithm not found
+
+        security:
+          - bearerAuth: []
+
+        tags: ["Vantage6 Server"]
+        """
+        server = db_Vantage6Server.get(id)
+        if not server:
+            return {"msg": "Vantage6 server not found"}, HTTPStatus.NOT_FOUND
+
+        return v6_server_output_schema.dump(server, many=False), HTTPStatus.OK
+
+    @with_authentication()
+    def delete(self, id):
+        """Delete whitelist vantage6 server
+        ---
+        description: Delete a whitelisted vantage6 server specified by ID.
+
+        parameters:
+          - in: path
+            name: id
+            schema:
+              type: integer
+            description: ID of the algorithm
+
+        responses:
+          200:
+            description: OK
+          401:
+            description: Unauthorized
+          404:
+            description: Algorithm not found
+
+        security:
+          - bearerAuth: []
+
+        tags: ["Vantage6 Server"]
+        """
+        server = db_Vantage6Server.get(id)
+        if not server:
+            return {"msg": "Vantage6 server not found"}, HTTPStatus.NOT_FOUND
 
-        # filter by any field of this endpoint
-        for param in ["name", "operation"]:
-            if param in args:
-                q = q.filter(getattr(db.Rule, param) == args[param])
-
-        # find roles containing a specific rule
-        if "role_id" in args:
-            role = db.Role.get(args["role_id"])
-            if not role:
-                return {
-                    "msg": f'Role with id={args["role_id"]} does not exist!'
-                }, HTTPStatus.BAD_REQUEST
-            q = (
-                q.join(db.role_rule_association)
-                .join(db.Role)
-                .filter(db.Role.id == args["role_id"])
-            )
-
-        # TODO implement user_id filter - should also take server into account
-        # # find all rules of a specific user. This is done by first joining all
-        # # tables to find all rules originating from a user's roles. Then, we
-        # # do an outer join to find all rules that are directly assigned to the
-        # # user.
-        # if "user_id" in args:
-        #     user = db.User.get(args["user_id"])
-        #     if not user:
-        #         return {
-        #             "msg": f'User with id={args["user_id"]} does not exist!'
-        #         }, HTTPStatus.BAD_REQUEST
-        #     q = (
-        #         q.join(db.role_rule_association)
-        #         .join(db.Role)
-        #         .join(db.Permission)
-        #         .join(db.User)
-        #         .outerjoin(db.UserPermission, db.Rule.id == db.UserPermission.c.rule_id)
-        #         .filter(
-        #             or_(
-        #                 db.User.id == args["user_id"],
-        #                 db.UserPermission.c.user_id == args["user_id"],
-        #             )
-        #         )
-        #     )
-
-        # check if pagination is disabled
-        paginate = True
-        if "no_pagination" in args and args["no_pagination"] == "1":
-            paginate = False
-
-        # paginate results
-        try:
-            page = Pagination.from_query(q, request, db.Rule, paginate=paginate)
-        except (ValueError, AttributeError) as e:
-            return {"msg": str(e)}, HTTPStatus.BAD_REQUEST
-
-        # model serialization
-        return self.response(page, rule_schema)
-
-
-# class Rule(ServicesResources):
-#     @with_user
-#     def get(self, id):
-#         """Returns a specific rule
-#         ---
-#         description: >-
-#             Get a rule by it's id. The user must be authenticated, but does
-#             not require any additional permissions to view rules.\n
-
-#             Accesible to users.
-
-#         parameters:
-#         - in: path
-#           name: id
-#           schema:
-#               type: integer
-#           minimum: 1
-#           description: rule_id
-#           required: true
-
-#         responses:
-#           200:
-#             description: Ok
-#           404:
-#             description: Rule not found
-
-#         security:
-#             - bearerAuth: []
-
-#         tags: ["Rule"]
-#         """
-#         rule = db.Rule.get(id)
-#         if not rule:
-#             return {"msg": f"Rule id={id} not found!"}, HTTPStatus.NOT_FOUND
+        url = server.url
+        server.delete()
 
-#         return rule_schema.dump(rule, many=False), HTTPStatus.OK
+        return {"msg": f"Server '{url}' was successfully deleted"}, HTTPStatus.OK
```

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/resource/schema/input_schema.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/schema/input_schema.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/resource/schema/output_schema.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/schema/output_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,30 +69,28 @@
 
 class AlgorithmOutputSchema(HATEOASModelSchema):
     """Marshmallow output schema to serialize the Algorithm model"""
 
     class Meta:
         model = Algorithm
 
-    functions = fields.Nested("FunctionOutputSchema", many=True, exclude=["id"])
+    functions = fields.Nested("FunctionOutputSchema", many=True)
 
 
 class FunctionOutputSchema(HATEOASModelSchema):
     """Marshmallow output schema to serialize the Function model"""
 
     class Meta:
         model = Function
 
     type_ = fields.String(data_key="type")
 
-    databases = fields.Nested("DatabaseOutputSchema", many=True, exclude=["id"])
-    arguments = fields.Nested("ArgumentOutputSchema", many=True, exclude=["id"])
-    ui_visualizations = fields.Nested(
-        "UIVisualizationOutputSchema", many=True, exclude=["id"]
-    )
+    databases = fields.Nested("DatabaseOutputSchema", many=True)
+    arguments = fields.Nested("ArgumentOutputSchema", many=True)
+    ui_visualizations = fields.Nested("UIVisualizationOutputSchema", many=True)
 
 
 class DatabaseOutputSchema(HATEOASModelSchema):
     """Marshmallow output schema to serialize the Database model"""
 
     class Meta:
         model = Database
```

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/resource/user.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/user.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.4.1/vantage6/algorithm/store/resource/version.py` & `vantage6-algorithm-store-4.5.0rc3/vantage6/algorithm/store/resource/version.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.4.1/vantage6_algorithm_store.egg-info/PKG-INFO` & `vantage6-algorithm-store-4.5.0rc3/vantage6_algorithm_store.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-algorithm-store
-Version: 4.4.1
+Version: 4.5.0rc3
 Summary: Vantage6 algorithm store
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
@@ -12,47 +12,51 @@
   <a href="https://vantage6.ai"><img src="https://github.com/IKNL/guidelines/blob/master/resources/logos/vantage6.png?raw=true" alt="vantage6" width="350"></a>
 </h1>
 
 <h3 align=center> A Privacy Enhancing Technology (PET) Operations platform</h3>
 <h3 align="center">
 
 <!-- Badges go here-->
+
 [![Release](https://github.com/vantage6/vantage6/actions/workflows/release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/release.yml)
 [![PyPI vantage6](https://badge.fury.io/py/vantage6.svg)](https://badge.fury.io/py/vantage6)
 [![Unittests](https://github.com/vantage6/vantage6/actions/workflows/unit_tests.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/unit_tests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/vantage6/vantage6/badge.svg?branch=main)](https://coveralls.io/github/vantage6/vantage6?branch=main)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/2e60ac3b3f284620805f7399cba317be)](https://www.codacy.com/gh/vantage6/vantage6/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=vantage6/vantage6&amp;utm_campaign=Badge_Grade)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7382602.svg)](https://doi.org/10.5281/zenodo.7382602)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/2e60ac3b3f284620805f7399cba317be)](https://app.codacy.com/gh/vantage6/vantage6/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![DOI](https://zenodo.org/badge/492818831.svg)](https://zenodo.org/badge/latestdoi/492818831)
+
 </h3>
 
 <p align="center">
   <a href="#books-quickstart">Quickstart</a> •
   <a href="#project-structure">Project structure</a> •
   <a href="#gift_heart-join-the-community">Join the community</a> •
   <a href="#black_nib-references">References</a>
 </p>
 
+---
 
------------------------------------------------------------------------------------------------------
 This repository is contains all the **vantage6** infrastructure source code. The **vantage6** technology enables to manage and deploy privacy enhancing technologies like Federated Learning (FL) and Multi-Party Computation (MPC). Please visit our [website (vantage6.ai)](https://vantage6.ai) to learn more!
 
 You can find more (user) documentation at [readthedocs (docs.vantage6.ai)](https://docs.vantage6.ai). If you have any questions, suggestions or just want to chat about federated learning: join our [Discord (https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel.
 
 ## Infrastructure overview
 
 ![Vantage6 architecture overview](docs/images/overview-infrastructure.png)
 
-*A High level overview of the vantage6 infrastructure. Vantage6 has both a client-server and peer-to-peer architecture. The client is used by the researcher to create (PET) computation requests. It is also used to manage users, organizations and collaborations. The server contains users, organizations, collaborations, tasks and their results. It provides a central access point for both the clients and nodes. The nodes have access to privacy sensitive data and handle computation requests retrieved from the server. Computation request are executed as separate containers on the node. These containers are connected to containers at other nodes by a VPN network.*
+_A High level overview of the vantage6 infrastructure. Vantage6 has both a client-server and peer-to-peer architecture. The client is used by the researcher to create (PET) computation requests. It is also used to manage users, organizations and collaborations. The server contains users, organizations, collaborations, tasks and their results. It provides a central access point for both the clients and nodes. The nodes have access to privacy sensitive data and handle computation requests retrieved from the server. Computation request are executed as separate containers on the node. These containers are connected to containers at other nodes by a VPN network._
 
 ## :books: Quickstart
 
 ### Requirements
+
 The **vantage6** infrastructure is delivered in Docker images. To run these images, you need to have [Docker](https://docs.docker.com/get-docker/) installed. To install the latest version of the vantage6 CLI, you need to have [Python](https://www.python.org/downloads/), we recommend using an environment manager like [mini-conda](https://docs.conda.io/en/latest/miniconda.html).
 
 Install the latest version of the vantage6 CLI by using:
+
 ```bash
 pip install vantage6
 ```
 
 This install the `v6` commands, which allows you to manage your nodes and servers. To view all available options, run:
 
 ```bash
@@ -79,16 +83,16 @@
 
 # View server logs
 v6 server attach
 ```
 
 From here you can use the [vantage6-client](https://pypi.org/project/vantage6-client) to interact with the server. The demo network has a pre-configured organization with the following credentials:
 
-* Username: `org_1-admin`
-* Password: `password`
+- Username: `org_1-admin`
+- Password: `password`
 
 For example, you can create a new organization by running:
 
 ```python
 from vantage6.client import Client
 
 client = Client('http://127.0.0.1', 5000, '/api', log_level='debug')
@@ -106,69 +110,74 @@
 ```
 
 You can find more (user) documentation at [readthedocs (docs.vantage6.ai)](https://docs.vantage6.ai)
 
 ## Project structure
 
 ### PYPI packages
+
 This repository is home to 6 PyPi packages:
 
-* [vantage6](https://pypi.org/project/vantage6) -> _CLI for managing node and server instances_
-* [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client for interacting with the vantage6-server_
-* [vantage6-algorithm-tools](https://pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate algorithm development_
-* [vantage6-node](https://pypi.org/project/vantage6-node) -> _Node application package_
-* [vantage6-server](https://pypi.org/project/vantage6-server) -> _Server application package_
-* [vantage6-algorithm-store](https://pypi.org/project/vantage6-algorithm-store) -> _Algorithm store application package_
-* [vantage6-common](https://pypi.org/project/vantage6-common) -> _Package with common vantage6 functions_
-* [vantage6-backend-common](https://pypi.org/project/vantage6-backend-common) -> _Package with functions common to central server and algorithm store_
+- [vantage6](https://pypi.org/project/vantage6) -> _CLI for managing node and server instances_
+- [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client for interacting with the vantage6-server_
+- [vantage6-algorithm-tools](https://pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate algorithm development_
+- [vantage6-node](https://pypi.org/project/vantage6-node) -> _Node application package_
+- [vantage6-server](https://pypi.org/project/vantage6-server) -> _Server application package_
+- [vantage6-algorithm-store](https://pypi.org/project/vantage6-algorithm-store) -> _Algorithm store application package_
+- [vantage6-common](https://pypi.org/project/vantage6-common) -> _Package with common vantage6 functions_
+- [vantage6-backend-common](https://pypi.org/project/vantage6-backend-common) -> _Package with functions common to central server and algorithm store_
 
 **Note that when using vantage6 you do not install the _server_ and _node_ packages. These are delivered to you in Docker images.**
 
 This repository also hosts the code for the vantage6 user interface (UI). The UI
 is an Angular web application that can be used to interact with the vantage6 server
 easily.
 
 ### Docker images
+
 The vantage6 infrastructure is delivered in Docker images. All Docker images are stored in our private [Harbor](https://goharbor.io/) registry. The most important images are:
 
-* `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application Docker image_
-* `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server application Docker image_
-* `harbor2.vantage6.ai/infrastructure/ui:VERSION` -> _User interface Docker image_
-* `harbor2.vantage6.ai/infrastructure/algorithm-store:VERSION` -> _Algorithm store Docker image_
+- `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application Docker image_
+- `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server application Docker image_
+- `harbor2.vantage6.ai/infrastructure/ui:VERSION` -> _User interface Docker image_
+- `harbor2.vantage6.ai/infrastructure/algorithm-store:VERSION` -> _Algorithm store Docker image_
 
 with `VERSION` being the full semantic version of the vantage6 infrastructure, e.g. `4.0.0` or `4.1.0rc0`.
 
 Several other images are used to support the infrastructure:
 
-* `harbor2.vantage6.ai/infrastructure/infrastructure-base:VERSION` -> _Base image for the infrastructure_
-* `harbor2.vantage6.ai/infrastructure/squid:VERSION` -> _Squid proxy image used for the whitelisting service_
-* `harbor2.vantage6.ai/infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_
-* `harbor2.vantage6.ai/infrastructure/vpn-client` -> _VPN image used to connect to the VPN_
-* `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN image used for initialization_
-* `harbor2.vantage6.ai/infrastructure/ssh-tunnel` -> _SSH tunnel image used for connecting algorithms to external services_
+- `harbor2.vantage6.ai/infrastructure/infrastructure-base:VERSION` -> _Base image for the infrastructure_
+- `harbor2.vantage6.ai/infrastructure/squid:VERSION` -> _Squid proxy image used for the whitelisting service_
+- `harbor2.vantage6.ai/infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_
+- `harbor2.vantage6.ai/infrastructure/vpn-client` -> _VPN image used to connect to the VPN_
+- `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN image used for initialization_
+- `harbor2.vantage6.ai/infrastructure/ssh-tunnel` -> _SSH tunnel image used for connecting algorithms to external services_
 
 And finally there are some images released for algorithm development:
 
-* `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base image for algorithm development_
-* `harbor2.vantage6.ai/infrastructure/algorithm-ohdsi-base:MAJOR.MINOR` -> _Extended algorithm base image for OHDSI algorithm development_
+- `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base image for algorithm development_
+- `harbor2.vantage6.ai/infrastructure/algorithm-ohdsi-base:MAJOR.MINOR` -> _Extended algorithm base image for OHDSI algorithm development_
 
 ## :gift_heart: Join the community!
+
 We hope to continue developing, improving, and supporting **vantage6** with the help of the federated learning community. If you are interested in contributing, first of all, thank you! Second, please take a look at our [contributing guidelines](https://docs.vantage6.ai/en/main/devops/contribute.html)
 
 <a href="https://github.com/vantage6/vantage6/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=vantage6/vantage6" />
 </a>
 
 ## :black_nib: References
+
 If you are using **vantage6**, please cite this repository as well as the accompanying papers as follows:
 
-> * F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6. Available at https://doi.org/10.5281/zenodo.7221216. Accessed on MONTH, 20XX.
-> * A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse. VANTAGE6: an open source priVAcy preserviNg federaTed leArninG infrastructurE for Secure Insight eXchange. AMIA Annual Symposium Proceedings, 2020, p. 870-877. [[BibTeX](https://arturomoncadatorres.com/bibtex/moncada-torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)]
-> * D. Smits\*, B. van Beusekom\*, F. Martin, L. Veen, G. Geleijnse, A. Moncada-Torres, An Improved Infrastructure for Privacy-Preserving Analysis of Patient Data, Proceedings of the International Conference of Informatics, Management, and Technology in Healthcare (ICIMTH), vol. 25, 2022, p. 144-147. [[BibTeX](https://arturomoncadatorres.com/bibtex/smits2022improved.txt), [PDF](https://ebooks.iospress.nl/volumearticle/60190)]
+> - F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6. Available at https://doi.org/10.5281/zenodo.7221216. Accessed on MONTH, 20XX.
+> - A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse. VANTAGE6: an open source priVAcy preserviNg federaTed leArninG infrastructurE for Secure Insight eXchange. AMIA Annual Symposium Proceedings, 2020, p. 870-877. [[BibTeX](https://arturomoncadatorres.com/bibtex/moncada-torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)]
+> - D. Smits\*, B. van Beusekom\*, F. Martin, L. Veen, G. Geleijnse, A. Moncada-Torres, An Improved Infrastructure for Privacy-Preserving Analysis of Patient Data, Proceedings of the International Conference of Informatics, Management, and Technology in Healthcare (ICIMTH), vol. 25, 2022, p. 144-147. [[BibTeX](https://arturomoncadatorres.com/bibtex/smits2022improved.txt), [PDF](https://ebooks.iospress.nl/volumearticle/60190)]
+
+---
 
------------------------------------------------------------------------------------------------------
 <p align="center">
   <a href="https://vantage6.ai">vantage6.ai</a> •
   <a href="https://discord.gg/yAyFf6Y">Discord</a> •
   <a href="https://vantage6.discourse.group/">Discourse</a> •
   <a href="https://docs.vantage6.ai">User documentation</a> •
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-algorithm-store Version: 4.4.1 Summary:
+Metadata-Version: 2.1 Name: vantage6-algorithm-store Version: 4.5.0rc3 Summary:
 Vantage6 algorithm store Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10 Description-Content-Type: text/markdown Provides-Extra:
 dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
@@ -10,38 +10,37 @@
 rreelleeaassee..yymmll)) [[!![[PPyyPPII vvaannttaaggee66]]((hhttttppss::////bbaaddggee..ffuurryy..iioo//ppyy//vvaannttaaggee66..ssvvgg))]]((hhttttppss::////
 bbaaddggee..ffuurryy..iioo//ppyy//vvaannttaaggee66)) [[!![[UUnniitttteessttss]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//
    aaccttiioonnss//wwoorrkkfflloowwss//uunniitt__tteessttss..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//
     vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//uunniitt__tteessttss..yymmll)) [[!![[CCoovveerraaggee SSttaattuuss]]((hhttttppss::////
  ccoovveerraallllss..iioo//rreeppooss//ggiitthhuubb//vvaannttaaggee66//vvaannttaaggee66//bbaaddggee..ssvvgg??bbrraanncchh==mmaaiinn))]]((hhttttppss::////
  ccoovveerraallllss..iioo//ggiitthhuubb//vvaannttaaggee66//vvaannttaaggee66??bbrraanncchh==mmaaiinn)) [[!![[CCooddaaccyy BBaaddggee]]((hhttttppss::////
 aapppp..ccooddaaccyy..ccoomm//pprroojjeecctt//bbaaddggee//GGrraaddee//22ee6600aacc33bb33ff228844662200880055ff77339999ccbbaa331177bbee))]]((hhttttppss::////
-                     wwwwww..ccooddaaccyy..ccoomm//gghh//vvaannttaaggee66//vvaannttaaggee66//
-   ddaasshhbbooaarrdd??uuttmm__ssoouurrccee==ggiitthhuubb..ccoomm&&uuttmm__mmeeddiiuumm==rreeffeerrrraall&&uuttmm__ccoonntteenntt==vvaannttaaggee66//
-   vvaannttaaggee66&&uuttmm__ccaammppaaiiggnn==BBaaddggee__GGrraaddee)) [[!![[DDOOII]]((hhttttppss::////zzeennooddoo..oorrgg//bbaaddggee//DDOOII//
-   1100..55228811//zzeennooddoo..77338822660022..ssvvgg))]]((hhttttppss::////ddooii..oorrgg//1100..55228811//zzeennooddoo..77338822660022)) ********
+                     aapppp..ccooddaaccyy..ccoomm//gghh//vvaannttaaggee66//vvaannttaaggee66//
+ddaasshhbbooaarrdd??uuttmm__ssoouurrccee==gghh&&uuttmm__mmeeddiiuumm==rreeffeerrrraall&&uuttmm__ccoonntteenntt==&&uuttmm__ccaammppaaiiggnn==BBaaddggee__ggrraaddee))
+  [[!![[DDOOII]]((hhttttppss::////zzeennooddoo..oorrgg//bbaaddggee//449922881188883311..ssvvgg))]]((hhttttppss::////zzeennooddoo..oorrgg//bbaaddggee//
+                           llaatteessttddooii//449922881188883311)) ********
     _Q_u_i_c_k_s_t_a_r_t â¢ _P_r_o_j_e_c_t_ _s_t_r_u_c_t_u_r_e â¢ _J_o_i_n_ _t_h_e_ _c_o_m_m_u_n_i_t_y â¢ _R_e_f_e_r_e_n_c_e_s
--------------------------------------------------------------------------------
----------------------- This repository is contains all the **vantage6**
-infrastructure source code. The **vantage6** technology enables to manage and
-deploy privacy enhancing technologies like Federated Learning (FL) and Multi-
-Party Computation (MPC). Please visit our [website (vantage6.ai)](https://
-vantage6.ai) to learn more! You can find more (user) documentation at
-[readthedocs (docs.vantage6.ai)](https://docs.vantage6.ai). If you have any
-questions, suggestions or just want to chat about federated learning: join our
-[Discord (https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel. ##
+--- This repository is contains all the **vantage6** infrastructure source
+code. The **vantage6** technology enables to manage and deploy privacy
+enhancing technologies like Federated Learning (FL) and Multi-Party Computation
+(MPC). Please visit our [website (vantage6.ai)](https://vantage6.ai) to learn
+more! You can find more (user) documentation at [readthedocs
+(docs.vantage6.ai)](https://docs.vantage6.ai). If you have any questions,
+suggestions or just want to chat about federated learning: join our [Discord
+(https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel. ##
 Infrastructure overview ![Vantage6 architecture overview](docs/images/overview-
-infrastructure.png) *A High level overview of the vantage6 infrastructure.
+infrastructure.png) _A High level overview of the vantage6 infrastructure.
 Vantage6 has both a client-server and peer-to-peer architecture. The client is
 used by the researcher to create (PET) computation requests. It is also used to
 manage users, organizations and collaborations. The server contains users,
 organizations, collaborations, tasks and their results. It provides a central
 access point for both the clients and nodes. The nodes have access to privacy
 sensitive data and handle computation requests retrieved from the server.
 Computation request are executed as separate containers on the node. These
-containers are connected to containers at other nodes by a VPN network.* ## :
+containers are connected to containers at other nodes by a VPN network._ ## :
 books: Quickstart ### Requirements The **vantage6** infrastructure is delivered
 in Docker images. To run these images, you need to have [Docker](https://
 docs.docker.com/get-docker/) installed. To install the latest version of the
 vantage6 CLI, you need to have [Python](https://www.python.org/downloads/), we
 recommend using an environment manager like [mini-conda](https://docs.conda.io/
 en/latest/miniconda.html). Install the latest version of the vantage6 CLI by
 using: ```bash pip install vantage6 ``` This install the `v6` commands, which
@@ -50,75 +49,74 @@
 using: ```bash v6 dev create-demo-network ``` This creates a local network with
 a server and two nodes. You can start the network by running: ```bash v6 dev
 start-demo-network ``` This will start the server and nodes in the background.
 You can view the logs by running: ```bash # View node logs v6 node attach #
 View server logs v6 server attach ``` From here you can use the [vantage6-
 client](https://pypi.org/project/vantage6-client) to interact with the server.
 The demo network has a pre-configured organization with the following
-credentials: * Username: `org_1-admin` * Password: `password` For example, you
+credentials: - Username: `org_1-admin` - Password: `password` For example, you
 can create a new organization by running: ```python from vantage6.client import
 Client client = Client('http://127.0.0.1', 5000, '/api', log_level='debug')
 client.authenticate('org_1-admin', 'password') client.setup_encryption(None)
 client.organization.create( name='My organization', address1='My address',
 address2='My address', zipcode='1234AB', country='The Netherlands', domain='my-
 organization.com' ) ``` You can find more (user) documentation at [readthedocs
 (docs.vantage6.ai)](https://docs.vantage6.ai) ## Project structure ### PYPI
-packages This repository is home to 6 PyPi packages: * [vantage6](https://
-pypi.org/project/vantage6) -> _CLI for managing node and server instances_ *
+packages This repository is home to 6 PyPi packages: - [vantage6](https://
+pypi.org/project/vantage6) -> _CLI for managing node and server instances_ -
 [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client
-for interacting with the vantage6-server_ * [vantage6-algorithm-tools](https://
+for interacting with the vantage6-server_ - [vantage6-algorithm-tools](https://
 pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate
-algorithm development_ * [vantage6-node](https://pypi.org/project/vantage6-
-node) -> _Node application package_ * [vantage6-server](https://pypi.org/
-project/vantage6-server) -> _Server application package_ * [vantage6-algorithm-
+algorithm development_ - [vantage6-node](https://pypi.org/project/vantage6-
+node) -> _Node application package_ - [vantage6-server](https://pypi.org/
+project/vantage6-server) -> _Server application package_ - [vantage6-algorithm-
 store](https://pypi.org/project/vantage6-algorithm-store) -> _Algorithm store
-application package_ * [vantage6-common](https://pypi.org/project/vantage6-
-common) -> _Package with common vantage6 functions_ * [vantage6-backend-common]
+application package_ - [vantage6-common](https://pypi.org/project/vantage6-
+common) -> _Package with common vantage6 functions_ - [vantage6-backend-common]
 (https://pypi.org/project/vantage6-backend-common) -> _Package with functions
 common to central server and algorithm store_ **Note that when using vantage6
 you do not install the _server_ and _node_ packages. These are delivered to you
 in Docker images.** This repository also hosts the code for the vantage6 user
 interface (UI). The UI is an Angular web application that can be used to
 interact with the vantage6 server easily. ### Docker images The vantage6
 infrastructure is delivered in Docker images. All Docker images are stored in
 our private [Harbor](https://goharbor.io/) registry. The most important images
-are: * `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application
-Docker image_ * `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server
-application Docker image_ * `harbor2.vantage6.ai/infrastructure/ui:VERSION` -
-> _User interface Docker image_ * `harbor2.vantage6.ai/infrastructure/
+are: - `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application
+Docker image_ - `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server
+application Docker image_ - `harbor2.vantage6.ai/infrastructure/ui:VERSION` -
+> _User interface Docker image_ - `harbor2.vantage6.ai/infrastructure/
 algorithm-store:VERSION` -> _Algorithm store Docker image_ with `VERSION` being
 the full semantic version of the vantage6 infrastructure, e.g. `4.0.0` or
-`4.1.0rc0`. Several other images are used to support the infrastructure: *
+`4.1.0rc0`. Several other images are used to support the infrastructure: -
 `harbor2.vantage6.ai/infrastructure/infrastructure-base:VERSION` -> _Base image
-for the infrastructure_ * `harbor2.vantage6.ai/infrastructure/squid:VERSION` -
-> _Squid proxy image used for the whitelisting service_ * `harbor2.vantage6.ai/
-infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_ *
+for the infrastructure_ - `harbor2.vantage6.ai/infrastructure/squid:VERSION` -
+> _Squid proxy image used for the whitelisting service_ - `harbor2.vantage6.ai/
+infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_ -
 `harbor2.vantage6.ai/infrastructure/vpn-client` -> _VPN image used to connect
-to the VPN_ * `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN
-image used for initialization_ * `harbor2.vantage6.ai/infrastructure/ssh-
+to the VPN_ - `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN
+image used for initialization_ - `harbor2.vantage6.ai/infrastructure/ssh-
 tunnel` -> _SSH tunnel image used for connecting algorithms to external
 services_ And finally there are some images released for algorithm development:
-* `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base
-image for algorithm development_ * `harbor2.vantage6.ai/infrastructure/
+- `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base
+image for algorithm development_ - `harbor2.vantage6.ai/infrastructure/
 algorithm-ohdsi-base:MAJOR.MINOR` -> _Extended algorithm base image for OHDSI
 algorithm development_ ## :gift_heart: Join the community! We hope to continue
 developing, improving, and supporting **vantage6** with the help of the
 federated learning community. If you are interested in contributing, first of
 all, thank you! Second, please take a look at our [contributing guidelines]
 (https://docs.vantage6.ai/en/main/devops/contribute.html) _[_h_t_t_p_s_:_/_/
 _c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_v_a_n_t_a_g_e_6_/_v_a_n_t_a_g_e_6_]## :black_nib: References If you are
 using **vantage6**, please cite this repository as well as the accompanying
-papers as follows: > * F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6.
+papers as follows: > - F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6.
 Available at https://doi.org/10.5281/zenodo.7221216. Accessed on MONTH, 20XX. >
-* A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse.
+- A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse.
 VANTAGE6: an open source priVAcy preserviNg federaTed leArninG infrastructurE
 for Secure Insight eXchange. AMIA Annual Symposium Proceedings, 2020, p. 870-
 877. [[BibTeX](https://arturomoncadatorres.com/bibtex/moncada-
-torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)] > * D. Smits\*,
+torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)] > - D. Smits\*,
 B. van Beusekom\*, F. Martin, L. Veen, G. Geleijnse, A. Moncada-Torres, An
 Improved Infrastructure for Privacy-Preserving Analysis of Patient Data,
 Proceedings of the International Conference of Informatics, Management, and
 Technology in Healthcare (ICIMTH), vol. 25, 2022, p. 144-147. [[BibTeX](https:/
 /arturomoncadatorres.com/bibtex/smits2022improved.txt), [PDF](https://
-ebooks.iospress.nl/volumearticle/60190)] --------------------------------------
----------------------------------------------------------------
+ebooks.iospress.nl/volumearticle/60190)] ---
        _v_a_n_t_a_g_e_6_._a_i â¢ _D_i_s_c_o_r_d â¢ _D_i_s_c_o_u_r_s_e â¢ _U_s_e_r_ _d_o_c_u_m_e_n_t_a_t_i_o_n â¢
```

### Comparing `vantage6-algorithm-store-4.4.1/vantage6_algorithm_store.egg-info/SOURCES.txt` & `vantage6-algorithm-store-4.5.0rc3/vantage6_algorithm_store.egg-info/SOURCES.txt`

 * *Files identical despite different names*

