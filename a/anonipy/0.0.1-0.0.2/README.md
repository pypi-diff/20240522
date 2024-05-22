# Comparing `tmp/anonipy-0.0.1.tar.gz` & `tmp/anonipy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anonipy-0.0.1.tar", last modified: Tue May 21 06:35:37 2024, max compression
+gzip compressed data, was "anonipy-0.0.2.tar", last modified: Wed May 22 07:56:32 2024, max compression
```

## Comparing `anonipy-0.0.1.tar` & `anonipy-0.0.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:35:37.373719 anonipy-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-21 06:35:33.000000 anonipy-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7563 2024-05-21 06:35:37.373719 anonipy-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-21 06:35:33.000000 anonipy-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:35:37.369719 anonipy-0.0.1/anonipy/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-21 06:35:33.000000 anonipy-0.0.1/anonipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:35:37.369719 anonipy-0.0.1/anonipy/anonymize/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-21 06:35:33.000000 anonipy-0.0.1/anonipy/anonymize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:35:37.369719 anonipy-0.0.1/anonipy/anonymize/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-21 06:35:33.000000 anonipy-0.0.1/anonipy/anonymize/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-21 06:35:33.000000 anonipy-0.0.1/anonipy/anonymize/extractors/entity_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-21 06:35:33.000000 anonipy-0.0.1/anonipy/anonymize/extractors/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:35:37.369719 anonipy-0.0.1/anonipy/anonymize/generators/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-21 06:35:33.000000 anonipy-0.0.1/anonipy/anonymize/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-21 06:35:33.000000 anonipy-0.0.1/anonipy/anonymize/generators/date_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-21 06:35:33.000000 anonipy-0.0.1/anonipy/anonymize/generators/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-21 06:35:33.000000 anonipy-0.0.1/anonipy/anonymize/generators/llm_label_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-21 06:35:33.000000 anonipy-0.0.1/anonipy/anonymize/generators/mask_label_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-21 06:35:33.000000 anonipy-0.0.1/anonipy/anonymize/generators/number_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-21 06:35:33.000000 anonipy-0.0.1/anonipy/anonymize/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-21 06:35:33.000000 anonipy-0.0.1/anonipy/anonymize/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:35:37.373719 anonipy-0.0.1/anonipy/anonymize/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-21 06:35:33.000000 anonipy-0.0.1/anonipy/anonymize/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-21 06:35:33.000000 anonipy-0.0.1/anonipy/anonymize/strategies/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-21 06:35:33.000000 anonipy-0.0.1/anonipy/anonymize/strategies/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-21 06:35:33.000000 anonipy-0.0.1/anonipy/anonymize/strategies/pseudonymization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-21 06:35:33.000000 anonipy-0.0.1/anonipy/anonymize/strategies/redaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-21 06:35:33.000000 anonipy-0.0.1/anonipy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-21 06:35:33.000000 anonipy-0.0.1/anonipy/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:35:37.373719 anonipy-0.0.1/anonipy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-21 06:35:33.000000 anonipy-0.0.1/anonipy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-21 06:35:33.000000 anonipy-0.0.1/anonipy/utils/file_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-21 06:35:33.000000 anonipy-0.0.1/anonipy/utils/language_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:35:37.373719 anonipy-0.0.1/anonipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7563 2024-05-21 06:35:37.000000 anonipy-0.0.1/anonipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-21 06:35:37.000000 anonipy-0.0.1/anonipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 06:35:37.000000 anonipy-0.0.1/anonipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-21 06:35:37.000000 anonipy-0.0.1/anonipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 06:35:37.000000 anonipy-0.0.1/anonipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-21 06:35:33.000000 anonipy-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-21 06:35:33.000000 anonipy-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-21 06:35:37.373719 anonipy-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:35:37.373719 anonipy-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:35:33.000000 anonipy-0.0.1/test/test_extractors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:35:33.000000 anonipy-0.0.1/test/test_file_system.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:35:33.000000 anonipy-0.0.1/test/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:35:33.000000 anonipy-0.0.1/test/test_language_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-21 06:35:33.000000 anonipy-0.0.1/test/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:35:33.000000 anonipy-0.0.1/test/test_strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:56:32.257749 anonipy-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-22 07:56:28.000000 anonipy-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-05-22 07:56:32.257749 anonipy-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-22 07:56:28.000000 anonipy-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:56:32.249749 anonipy-0.0.2/anonipy/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-22 07:56:28.000000 anonipy-0.0.2/anonipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:56:32.253749 anonipy-0.0.2/anonipy/anonymize/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-22 07:56:28.000000 anonipy-0.0.2/anonipy/anonymize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:56:32.253749 anonipy-0.0.2/anonipy/anonymize/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-22 07:56:28.000000 anonipy-0.0.2/anonipy/anonymize/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-22 07:56:28.000000 anonipy-0.0.2/anonipy/anonymize/extractors/entity_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-22 07:56:28.000000 anonipy-0.0.2/anonipy/anonymize/extractors/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:56:32.253749 anonipy-0.0.2/anonipy/anonymize/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-22 07:56:28.000000 anonipy-0.0.2/anonipy/anonymize/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-22 07:56:28.000000 anonipy-0.0.2/anonipy/anonymize/generators/date_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-22 07:56:28.000000 anonipy-0.0.2/anonipy/anonymize/generators/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-22 07:56:28.000000 anonipy-0.0.2/anonipy/anonymize/generators/llm_label_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-22 07:56:28.000000 anonipy-0.0.2/anonipy/anonymize/generators/mask_label_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-22 07:56:28.000000 anonipy-0.0.2/anonipy/anonymize/generators/number_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-22 07:56:28.000000 anonipy-0.0.2/anonipy/anonymize/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-22 07:56:28.000000 anonipy-0.0.2/anonipy/anonymize/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:56:32.253749 anonipy-0.0.2/anonipy/anonymize/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-22 07:56:28.000000 anonipy-0.0.2/anonipy/anonymize/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-22 07:56:28.000000 anonipy-0.0.2/anonipy/anonymize/strategies/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-22 07:56:28.000000 anonipy-0.0.2/anonipy/anonymize/strategies/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-22 07:56:28.000000 anonipy-0.0.2/anonipy/anonymize/strategies/pseudonymization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-22 07:56:28.000000 anonipy-0.0.2/anonipy/anonymize/strategies/redaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-22 07:56:28.000000 anonipy-0.0.2/anonipy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-22 07:56:28.000000 anonipy-0.0.2/anonipy/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:56:32.253749 anonipy-0.0.2/anonipy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-22 07:56:28.000000 anonipy-0.0.2/anonipy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-22 07:56:28.000000 anonipy-0.0.2/anonipy/utils/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-22 07:56:28.000000 anonipy-0.0.2/anonipy/utils/language_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:56:32.257749 anonipy-0.0.2/anonipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-05-22 07:56:32.000000 anonipy-0.0.2/anonipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-22 07:56:32.000000 anonipy-0.0.2/anonipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 07:56:32.000000 anonipy-0.0.2/anonipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-22 07:56:32.000000 anonipy-0.0.2/anonipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 07:56:32.000000 anonipy-0.0.2/anonipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-22 07:56:28.000000 anonipy-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-22 07:56:28.000000 anonipy-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-22 07:56:32.257749 anonipy-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:56:32.257749 anonipy-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:56:28.000000 anonipy-0.0.2/test/test_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:56:28.000000 anonipy-0.0.2/test/test_file_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:56:28.000000 anonipy-0.0.2/test/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:56:28.000000 anonipy-0.0.2/test/test_language_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 07:56:28.000000 anonipy-0.0.2/test/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:56:28.000000 anonipy-0.0.2/test/test_strategies.py
```

### Comparing `anonipy-0.0.1/LICENSE` & `anonipy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.1/PKG-INFO` & `anonipy-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anonipy
-Version: 0.0.1
+Version: 0.0.2
 Summary: The data anonymization package
 Author-email: Erik Novak <erik.novak@ijs.si>
 License: BSD 2-Clause License
         
         Copyright (c) 2024, Erik Novak
         All rights reserved.
         
@@ -73,21 +73,21 @@
 
 <p align="center">
   <i>Data anonymization package, supporting different anonymization strategies</i>
 </p>
 
 <p align="center">
   <a href="https://github.com/eriknovak/anonipy/actions/workflows/unittests.yaml" target="_blank">
-    <img src="https://github.com/eriknovak/anonipy/actions/workflows/unittests.yaml/badge.svg" alt="Test">
+    <img src="https://github.com/eriknovak/anonipy/actions/workflows/unittests.yaml/badge.svg" alt="Test" />
   </a>
   <a href="https://pypi.org/project/anonipy" target="_blank">
-    <img src="https://img.shields.io/pypi/v/anonipy?color=%2334D058&amp;label=pypi%20package" alt="Package version">
+    <img src="https://img.shields.io/pypi/v/anonipy?color=%2334D058&amp;label=pypi%20package" alt="Package version" />
   </a>
   <a href="https://pypi.org/project/anonipy" target="_blank">
-    <img src="https://img.shields.io/pypi/pyversions/anonipy.svg?color=%2334D058" alt="Supported Python versions">
+    <img src="https://img.shields.io/pypi/pyversions/anonipy.svg?color=%2334D058" alt="Supported Python versions" />
   </a>
 </p>
 
 
 ---
 
 **Documentation:** [https://eriknovak.github.io/anonipy](https://eriknovak.github.io/anonipy)
```

### Comparing `anonipy-0.0.1/README.md` & `anonipy-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 <p align="center">
   <i>Data anonymization package, supporting different anonymization strategies</i>
 </p>
 
 <p align="center">
   <a href="https://github.com/eriknovak/anonipy/actions/workflows/unittests.yaml" target="_blank">
-    <img src="https://github.com/eriknovak/anonipy/actions/workflows/unittests.yaml/badge.svg" alt="Test">
+    <img src="https://github.com/eriknovak/anonipy/actions/workflows/unittests.yaml/badge.svg" alt="Test" />
   </a>
   <a href="https://pypi.org/project/anonipy" target="_blank">
-    <img src="https://img.shields.io/pypi/v/anonipy?color=%2334D058&amp;label=pypi%20package" alt="Package version">
+    <img src="https://img.shields.io/pypi/v/anonipy?color=%2334D058&amp;label=pypi%20package" alt="Package version" />
   </a>
   <a href="https://pypi.org/project/anonipy" target="_blank">
-    <img src="https://img.shields.io/pypi/pyversions/anonipy.svg?color=%2334D058" alt="Supported Python versions">
+    <img src="https://img.shields.io/pypi/pyversions/anonipy.svg?color=%2334D058" alt="Supported Python versions" />
   </a>
 </p>
 
 
 ---
 
 **Documentation:** [https://eriknovak.github.io/anonipy](https://eriknovak.github.io/anonipy)
```

### Comparing `anonipy-0.0.1/anonipy/anonymize/extractors/entity_extractor.py` & `anonipy-0.0.2/anonipy/anonymize/extractors/entity_extractor.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.1/anonipy/anonymize/generators/date_generator.py` & `anonipy-0.0.2/anonipy/anonymize/generators/date_generator.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.1/anonipy/anonymize/generators/llm_label_generator.py` & `anonipy-0.0.2/anonipy/anonymize/generators/llm_label_generator.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.1/anonipy/anonymize/generators/mask_label_generator.py` & `anonipy-0.0.2/anonipy/anonymize/generators/mask_label_generator.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.1/anonipy/anonymize/generators/number_generator.py` & `anonipy-0.0.2/anonipy/anonymize/generators/number_generator.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.1/anonipy/anonymize/regex.py` & `anonipy-0.0.2/anonipy/anonymize/regex.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.1/anonipy/anonymize/strategies/masking.py` & `anonipy-0.0.2/anonipy/anonymize/strategies/masking.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.1/anonipy/anonymize/strategies/pseudonymization.py` & `anonipy-0.0.2/anonipy/anonymize/strategies/pseudonymization.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.1/anonipy/anonymize/strategies/redaction.py` & `anonipy-0.0.2/anonipy/anonymize/strategies/redaction.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.1/anonipy/utils/language_detector.py` & `anonipy-0.0.2/anonipy/utils/language_detector.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.1/anonipy.egg-info/PKG-INFO` & `anonipy-0.0.2/anonipy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anonipy
-Version: 0.0.1
+Version: 0.0.2
 Summary: The data anonymization package
 Author-email: Erik Novak <erik.novak@ijs.si>
 License: BSD 2-Clause License
         
         Copyright (c) 2024, Erik Novak
         All rights reserved.
         
@@ -73,21 +73,21 @@
 
 <p align="center">
   <i>Data anonymization package, supporting different anonymization strategies</i>
 </p>
 
 <p align="center">
   <a href="https://github.com/eriknovak/anonipy/actions/workflows/unittests.yaml" target="_blank">
-    <img src="https://github.com/eriknovak/anonipy/actions/workflows/unittests.yaml/badge.svg" alt="Test">
+    <img src="https://github.com/eriknovak/anonipy/actions/workflows/unittests.yaml/badge.svg" alt="Test" />
   </a>
   <a href="https://pypi.org/project/anonipy" target="_blank">
-    <img src="https://img.shields.io/pypi/v/anonipy?color=%2334D058&amp;label=pypi%20package" alt="Package version">
+    <img src="https://img.shields.io/pypi/v/anonipy?color=%2334D058&amp;label=pypi%20package" alt="Package version" />
   </a>
   <a href="https://pypi.org/project/anonipy" target="_blank">
-    <img src="https://img.shields.io/pypi/pyversions/anonipy.svg?color=%2334D058" alt="Supported Python versions">
+    <img src="https://img.shields.io/pypi/pyversions/anonipy.svg?color=%2334D058" alt="Supported Python versions" />
   </a>
 </p>
 
 
 ---
 
 **Documentation:** [https://eriknovak.github.io/anonipy](https://eriknovak.github.io/anonipy)
```

### Comparing `anonipy-0.0.1/anonipy.egg-info/SOURCES.txt` & `anonipy-0.0.2/anonipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.1/pyproject.toml` & `anonipy-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
-version = "0.0.1"
+version = "0.0.2"
 name = "anonipy"
 description = "The data anonymization package"
 authors=[{ name = "Erik Novak", email = "erik.novak@ijs.si" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 dynamic = ["dependencies"]
 classifiers = [
```

