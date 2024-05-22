# Comparing `tmp/opensearch-rest-resources-0.0.8.tar.gz` & `tmp/opensearch-rest-resources-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensearch-rest-resources-0.0.8.tar", last modified: Fri Apr  5 11:12:20 2024, max compression
+gzip compressed data, was "opensearch-rest-resources-0.0.9.tar", last modified: Mon Apr  8 09:54:25 2024, max compression
```

## Comparing `opensearch-rest-resources-0.0.8.tar` & `opensearch-rest-resources-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:12:20.200490 opensearch-rest-resources-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-05 11:12:10.000000 opensearch-rest-resources-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 11:12:10.000000 opensearch-rest-resources-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-05 11:12:20.196490 opensearch-rest-resources-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-05 11:12:10.000000 opensearch-rest-resources-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-05 11:12:10.000000 opensearch-rest-resources-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 11:12:20.200490 opensearch-rest-resources-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-05 11:12:10.000000 opensearch-rest-resources-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:12:20.196490 opensearch-rest-resources-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:12:20.196490 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources/
--rw-r--r--   0 runner    (1001) docker     (127)    54134 2024-04-05 11:12:10.000000 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:12:20.196490 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-05 11:12:10.000000 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    85850 2024-04-05 11:12:10.000000 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources/_jsii/opensearch-rest-resources@0.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 11:12:10.000000 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:12:20.196490 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-05 11:12:20.000000 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-05 11:12:20.000000 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 11:12:20.000000 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-05 11:12:20.000000 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 11:12:20.000000 opensearch-rest-resources-0.0.8/src/opensearch_rest_resources.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:54:25.472117 opensearch-rest-resources-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-08 09:54:14.000000 opensearch-rest-resources-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 09:54:14.000000 opensearch-rest-resources-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-08 09:54:25.472117 opensearch-rest-resources-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-08 09:54:14.000000 opensearch-rest-resources-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-08 09:54:14.000000 opensearch-rest-resources-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 09:54:25.472117 opensearch-rest-resources-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-08 09:54:14.000000 opensearch-rest-resources-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:54:25.468117 opensearch-rest-resources-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:54:25.472117 opensearch-rest-resources-0.0.9/src/opensearch_rest_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    54134 2024-04-08 09:54:14.000000 opensearch-rest-resources-0.0.9/src/opensearch_rest_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:54:25.472117 opensearch-rest-resources-0.0.9/src/opensearch_rest_resources/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-08 09:54:14.000000 opensearch-rest-resources-0.0.9/src/opensearch_rest_resources/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85857 2024-04-08 09:54:14.000000 opensearch-rest-resources-0.0.9/src/opensearch_rest_resources/_jsii/opensearch-rest-resources@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:54:14.000000 opensearch-rest-resources-0.0.9/src/opensearch_rest_resources/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:54:25.472117 opensearch-rest-resources-0.0.9/src/opensearch_rest_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-08 09:54:25.000000 opensearch-rest-resources-0.0.9/src/opensearch_rest_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-08 09:54:25.000000 opensearch-rest-resources-0.0.9/src/opensearch_rest_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:54:25.000000 opensearch-rest-resources-0.0.9/src/opensearch_rest_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 09:54:25.000000 opensearch-rest-resources-0.0.9/src/opensearch_rest_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 09:54:25.000000 opensearch-rest-resources-0.0.9/src/opensearch_rest_resources.egg-info/top_level.txt
```

### Comparing `opensearch-rest-resources-0.0.8/LICENSE` & `opensearch-rest-resources-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `opensearch-rest-resources-0.0.8/PKG-INFO` & `opensearch-rest-resources-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensearch-rest-resources
-Version: 0.0.8
+Version: 0.0.9
 Summary: Manage OpenSearch REST resources from AWS CDK.
 Home-page: https://github.com/tmokmss/opensearch-rest-resources.git
 Author: tmokmss<tomookam@live.jp>
 License: MIT
 Project-URL: Source, https://github.com/tmokmss/opensearch-rest-resources.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `opensearch-rest-resources-0.0.8/README.md` & `opensearch-rest-resources-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-rest-resources-0.0.8/setup.py` & `opensearch-rest-resources-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "opensearch-rest-resources",
-    "version": "0.0.8",
+    "version": "0.0.9",
     "description": "Manage OpenSearch REST resources from AWS CDK.",
     "license": "MIT",
     "url": "https://github.com/tmokmss/opensearch-rest-resources.git",
     "long_description_content_type": "text/markdown",
     "author": "tmokmss<tomookam@live.jp>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "opensearch_rest_resources",
         "opensearch_rest_resources._jsii"
     ],
     "package_data": {
         "opensearch_rest_resources._jsii": [
-            "opensearch-rest-resources@0.0.8.jsii.tgz"
+            "opensearch-rest-resources@0.0.9.jsii.tgz"
         ],
         "opensearch_rest_resources": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `opensearch-rest-resources-0.0.8/src/opensearch_rest_resources/__init__.py` & `opensearch-rest-resources-0.0.9/src/opensearch_rest_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-rest-resources-0.0.8/src/opensearch_rest_resources.egg-info/PKG-INFO` & `opensearch-rest-resources-0.0.9/src/opensearch_rest_resources.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensearch-rest-resources
-Version: 0.0.8
+Version: 0.0.9
 Summary: Manage OpenSearch REST resources from AWS CDK.
 Home-page: https://github.com/tmokmss/opensearch-rest-resources.git
 Author: tmokmss<tomookam@live.jp>
 License: MIT
 Project-URL: Source, https://github.com/tmokmss/opensearch-rest-resources.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `opensearch-rest-resources-0.0.8/src/opensearch_rest_resources.egg-info/SOURCES.txt` & `opensearch-rest-resources-0.0.9/src/opensearch_rest_resources.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/opensearch_rest_resources/py.typed
 src/opensearch_rest_resources.egg-info/PKG-INFO
 src/opensearch_rest_resources.egg-info/SOURCES.txt
 src/opensearch_rest_resources.egg-info/dependency_links.txt
 src/opensearch_rest_resources.egg-info/requires.txt
 src/opensearch_rest_resources.egg-info/top_level.txt
 src/opensearch_rest_resources/_jsii/__init__.py
-src/opensearch_rest_resources/_jsii/opensearch-rest-resources@0.0.8.jsii.tgz
+src/opensearch_rest_resources/_jsii/opensearch-rest-resources@0.0.9.jsii.tgz
```

