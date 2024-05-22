# Comparing `tmp/nowcasting_datamodel-1.5.8.tar.gz` & `tmp/nowcasting_datamodel-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowcasting_datamodel-1.5.8.tar", last modified: Tue Aug 15 11:08:03 2023, max compression
+gzip compressed data, was "nowcasting_datamodel-1.5.9.tar", last modified: Thu Aug 17 07:00:16 2023, max compression
```

## Comparing `nowcasting_datamodel-1.5.8.tar` & `nowcasting_datamodel-1.5.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 11:08:03.544475 nowcasting_datamodel-1.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-08-15 11:08:03.544475 nowcasting_datamodel-1.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/diagram_pv.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 11:08:03.540475 nowcasting_datamodel-1.5.8/nowcasting_datamodel/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9987 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/fake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 11:08:03.540475 nowcasting_datamodel-1.5.8/nowcasting_datamodel/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/migrations/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 11:08:03.544475 nowcasting_datamodel-1.5.8/nowcasting_datamodel/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/models/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/models/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    19379 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/models/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/models/gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/models/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/national.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 11:08:03.544475 nowcasting_datamodel-1.5.8/nowcasting_datamodel/read/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/read/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 11:08:03.544475 nowcasting_datamodel-1.5.8/nowcasting_datamodel/read/blend/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/read/blend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/read/blend/blend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12284 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/read/blend/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/read/blend/weights.py
--rw-r--r--   0 runner    (1001) docker     (123)    24306 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/read/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/read/read_gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/read/read_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/read/read_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/read/read_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 11:08:03.544475 nowcasting_datamodel-1.5.8/nowcasting_datamodel/save/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/save/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/save/adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/save/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/save/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 11:08:03.540475 nowcasting_datamodel-1.5.8/nowcasting_datamodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-08-15 11:08:03.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-08-15 11:08:03.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-15 11:08:03.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-15 11:08:03.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-15 11:08:03.000000 nowcasting_datamodel-1.5.8/nowcasting_datamodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-15 11:08:03.544475 nowcasting_datamodel-1.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 11:08:03.544475 nowcasting_datamodel-1.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/tests/test_databaseconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/tests/test_fake_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/tests/test_national.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-15 11:07:52.000000 nowcasting_datamodel-1.5.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 07:00:16.138833 nowcasting_datamodel-1.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-08-17 07:00:16.138833 nowcasting_datamodel-1.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/diagram_pv.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 07:00:16.134833 nowcasting_datamodel-1.5.9/nowcasting_datamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9987 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/fake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 07:00:16.134833 nowcasting_datamodel-1.5.9/nowcasting_datamodel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/migrations/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 07:00:16.138833 nowcasting_datamodel-1.5.9/nowcasting_datamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/models/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/models/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19379 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/models/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/models/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/models/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/national.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 07:00:16.138833 nowcasting_datamodel-1.5.9/nowcasting_datamodel/read/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/read/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 07:00:16.138833 nowcasting_datamodel-1.5.9/nowcasting_datamodel/read/blend/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/read/blend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/read/blend/blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12284 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/read/blend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/read/blend/weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24306 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/read/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/read/read_gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/read/read_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/read/read_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/read/read_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 07:00:16.138833 nowcasting_datamodel-1.5.9/nowcasting_datamodel/save/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/save/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/save/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/save/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/save/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 07:00:16.134833 nowcasting_datamodel-1.5.9/nowcasting_datamodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-08-17 07:00:16.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-08-17 07:00:16.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-17 07:00:16.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-17 07:00:16.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-17 07:00:16.000000 nowcasting_datamodel-1.5.9/nowcasting_datamodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-17 07:00:16.138833 nowcasting_datamodel-1.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 07:00:16.138833 nowcasting_datamodel-1.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/tests/test_databaseconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/tests/test_fake_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/tests/test_national.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-17 07:00:01.000000 nowcasting_datamodel-1.5.9/tests/test_utils.py
```

### Comparing `nowcasting_datamodel-1.5.8/PKG-INFO` & `nowcasting_datamodel-1.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting_datamodel
-Version: 1.5.8
+Version: 1.5.9
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.5.8/README.md` & `nowcasting_datamodel-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/diagram.png` & `nowcasting_datamodel-1.5.9/diagram.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/diagram_pv.png` & `nowcasting_datamodel-1.5.9/diagram_pv.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/connection.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/connection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/fake.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/migrations/app.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/migrations/app.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/models/__init__.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/models/api.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/models/api.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/models/convert.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/models/convert.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/models/forecast.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/models/forecast.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/models/gsp.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/models/gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/models/metric.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/models/metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/models/models.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/models/models.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/models/pv.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/models/pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/models/utils.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/models/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/national.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/read/blend/blend.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/read/blend/blend.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/read/blend/utils.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/read/blend/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/read/blend/weights.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/read/blend/weights.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/read/read.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/read/read.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/read/read_gsp.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/read/read_gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/read/read_metric.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/read/read_metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/read/read_pv.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/read/read_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/read/read_user.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/read/read_user.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/save/adjust.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/save/adjust.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/save/save.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/save/save.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/save/update.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/save/update.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel/utils.py` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel.egg-info/PKG-INFO` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting-datamodel
-Version: 1.5.8
+Version: 1.5.9
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.5.8/nowcasting_datamodel.egg-info/SOURCES.txt` & `nowcasting_datamodel-1.5.9/nowcasting_datamodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/setup.py` & `nowcasting_datamodel-1.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/tests/test_databaseconnection.py` & `nowcasting_datamodel-1.5.9/tests/test_databaseconnection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/tests/test_fake.py` & `nowcasting_datamodel-1.5.9/tests/test_fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/tests/test_fake_pv.py` & `nowcasting_datamodel-1.5.9/tests/test_fake_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/tests/test_national.py` & `nowcasting_datamodel-1.5.9/tests/test_national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.5.8/tests/test_utils.py` & `nowcasting_datamodel-1.5.9/tests/test_utils.py`

 * *Files identical despite different names*

