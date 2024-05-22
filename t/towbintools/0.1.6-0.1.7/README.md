# Comparing `tmp/towbintools-0.1.6.tar.gz` & `tmp/towbintools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "towbintools-0.1.6.tar", last modified: Fri May 10 08:02:29 2024, max compression
+gzip compressed data, was "towbintools-0.1.7.tar", last modified: Wed May 22 08:52:05 2024, max compression
```

## Comparing `towbintools-0.1.6.tar` & `towbintools-0.1.7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.254521 towbintools-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-10 08:02:24.000000 towbintools-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-10 08:02:29.254521 towbintools-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-10 08:02:24.000000 towbintools-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 08:02:24.000000 towbintools-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 08:02:29.254521 towbintools-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.246521 towbintools-0.1.6/towbintools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.250521 towbintools-0.1.6/towbintools/classification/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/classification/classification_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.250521 towbintools-0.1.6/towbintools/data_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/data_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/data_analysis/growth_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.250521 towbintools-0.1.6/towbintools/deep_learning/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/deep_learning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.250521 towbintools-0.1.6/towbintools/deep_learning/architectures/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/deep_learning/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/deep_learning/architectures/archs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/deep_learning/architectures/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/deep_learning/deep_learning_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.250521 towbintools-0.1.6/towbintools/deep_learning/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/deep_learning/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/deep_learning/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12509 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/deep_learning/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/deep_learning/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/deep_learning/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.254521 towbintools-0.1.6/towbintools/foundation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/foundation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/foundation/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/foundation/binary_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    15736 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/foundation/detect_molts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/foundation/file_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/foundation/image_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/foundation/image_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/foundation/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/foundation/worm_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/foundation/zstack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.254521 towbintools-0.1.6/towbintools/legacy_straightening/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/legacy_straightening/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/legacy_straightening/straightening_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.254521 towbintools-0.1.6/towbintools/quantification/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/quantification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/quantification/quantification_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.254521 towbintools-0.1.6/towbintools/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/segmentation/segmentation_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.254521 towbintools-0.1.6/towbintools/straightening/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/straightening/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35283 2024-05-10 08:02:24.000000 towbintools-0.1.6/towbintools/straightening/straightening_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:02:29.254521 towbintools-0.1.6/towbintools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-10 08:02:29.000000 towbintools-0.1.6/towbintools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-10 08:02:29.000000 towbintools-0.1.6/towbintools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:02:29.000000 towbintools-0.1.6/towbintools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-10 08:02:29.000000 towbintools-0.1.6/towbintools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 08:02:29.000000 towbintools-0.1.6/towbintools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:52:05.515408 towbintools-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-22 08:52:01.000000 towbintools-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-22 08:52:05.515408 towbintools-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-22 08:52:01.000000 towbintools-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-22 08:52:01.000000 towbintools-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 08:52:05.515408 towbintools-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:52:05.511408 towbintools-0.1.7/towbintools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:52:05.511408 towbintools-0.1.7/towbintools/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17771 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/classification/classification_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:52:05.511408 towbintools-0.1.7/towbintools/data_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/data_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/data_analysis/growth_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:52:05.511408 towbintools-0.1.7/towbintools/deep_learning/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/deep_learning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:52:05.511408 towbintools-0.1.7/towbintools/deep_learning/architectures/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/deep_learning/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/deep_learning/architectures/archs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/deep_learning/architectures/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/deep_learning/deep_learning_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:52:05.511408 towbintools-0.1.7/towbintools/deep_learning/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/deep_learning/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/deep_learning/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12509 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/deep_learning/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/deep_learning/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/deep_learning/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:52:05.515408 towbintools-0.1.7/towbintools/foundation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/foundation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/foundation/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/foundation/binary_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15736 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/foundation/detect_molts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/foundation/file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/foundation/image_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/foundation/image_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/foundation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10528 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/foundation/worm_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/foundation/zstack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:52:05.515408 towbintools-0.1.7/towbintools/legacy_straightening/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/legacy_straightening/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/legacy_straightening/straightening_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:52:05.515408 towbintools-0.1.7/towbintools/quantification/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/quantification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/quantification/quantification_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:52:05.515408 towbintools-0.1.7/towbintools/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/segmentation/segmentation_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:52:05.515408 towbintools-0.1.7/towbintools/straightening/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/straightening/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35283 2024-05-22 08:52:01.000000 towbintools-0.1.7/towbintools/straightening/straightening_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:52:05.515408 towbintools-0.1.7/towbintools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-22 08:52:05.000000 towbintools-0.1.7/towbintools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-22 08:52:05.000000 towbintools-0.1.7/towbintools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 08:52:05.000000 towbintools-0.1.7/towbintools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-22 08:52:05.000000 towbintools-0.1.7/towbintools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 08:52:05.000000 towbintools-0.1.7/towbintools.egg-info/top_level.txt
```

### Comparing `towbintools-0.1.6/LICENSE` & `towbintools-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.6/PKG-INFO` & `towbintools-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: towbintools
-Version: 0.1.6
+Version: 0.1.7
 Summary: All the tools used by the Towbin Lab !
 Author-email: Sacha Psalmon <sacha.psalmon@unibe.ch>, Boris Gusev <boris.gusev@unibe.ch>
 Maintainer-email: Sacha Psalmon <sacha.psalmon@unibe.ch>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.22.4
```

### Comparing `towbintools-0.1.6/README.md` & `towbintools-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.6/pyproject.toml` & `towbintools-0.1.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "towbintools"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   {name="Sacha Psalmon", email="sacha.psalmon@unibe.ch" },
   {name="Boris Gusev", email="boris.gusev@unibe.ch" }
 ]
 maintainers = [
     {name = "Sacha Psalmon", email="sacha.psalmon@unibe.ch"},
 ]
```

### Comparing `towbintools-0.1.6/towbintools/data_analysis/growth_rate.py` & `towbintools-0.1.7/towbintools/data_analysis/growth_rate.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.6/towbintools/deep_learning/architectures/archs.py` & `towbintools-0.1.7/towbintools/deep_learning/architectures/archs.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.6/towbintools/deep_learning/architectures/models.py` & `towbintools-0.1.7/towbintools/deep_learning/architectures/models.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.6/towbintools/deep_learning/deep_learning_tools.py` & `towbintools-0.1.7/towbintools/deep_learning/deep_learning_tools.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.6/towbintools/deep_learning/utils/augmentation.py` & `towbintools-0.1.7/towbintools/deep_learning/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.6/towbintools/deep_learning/utils/dataset.py` & `towbintools-0.1.7/towbintools/deep_learning/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.6/towbintools/deep_learning/utils/loss.py` & `towbintools-0.1.7/towbintools/deep_learning/utils/loss.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.6/towbintools/foundation/backbone.py` & `towbintools-0.1.7/towbintools/foundation/backbone.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.6/towbintools/foundation/binary_image.py` & `towbintools-0.1.7/towbintools/foundation/binary_image.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.6/towbintools/foundation/detect_molts.py` & `towbintools-0.1.7/towbintools/foundation/detect_molts.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.6/towbintools/foundation/file_handling.py` & `towbintools-0.1.7/towbintools/foundation/file_handling.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.6/towbintools/foundation/image_handling.py` & `towbintools-0.1.7/towbintools/foundation/image_handling.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.6/towbintools/foundation/image_quality.py` & `towbintools-0.1.7/towbintools/foundation/image_quality.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.6/towbintools/foundation/utils.py` & `towbintools-0.1.7/towbintools/foundation/utils.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.6/towbintools/foundation/zstack.py` & `towbintools-0.1.7/towbintools/foundation/zstack.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.6/towbintools/legacy_straightening/straightening_tools.py` & `towbintools-0.1.7/towbintools/legacy_straightening/straightening_tools.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.6/towbintools/quantification/quantification_tools.py` & `towbintools-0.1.7/towbintools/quantification/quantification_tools.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.6/towbintools/segmentation/segmentation_tools.py` & `towbintools-0.1.7/towbintools/segmentation/segmentation_tools.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.6/towbintools/straightening/straightening_tools.py` & `towbintools-0.1.7/towbintools/straightening/straightening_tools.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.6/towbintools.egg-info/PKG-INFO` & `towbintools-0.1.7/towbintools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: towbintools
-Version: 0.1.6
+Version: 0.1.7
 Summary: All the tools used by the Towbin Lab !
 Author-email: Sacha Psalmon <sacha.psalmon@unibe.ch>, Boris Gusev <boris.gusev@unibe.ch>
 Maintainer-email: Sacha Psalmon <sacha.psalmon@unibe.ch>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.22.4
```

### Comparing `towbintools-0.1.6/towbintools.egg-info/SOURCES.txt` & `towbintools-0.1.7/towbintools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

