# Comparing `tmp/tc-neo4j-lib-1.0.2.tar.gz` & `tmp/tc_neo4j_lib-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tc-neo4j-lib-1.0.2.tar", last modified: Tue Dec 19 12:17:59 2023, max compression
+gzip compressed data, was "tc_neo4j_lib-2.0.0.tar", last modified: Wed May 22 16:10:05 2024, max compression
```

## Comparing `tc-neo4j-lib-1.0.2.tar` & `tc_neo4j_lib-2.0.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 12:17:59.049162 tc-neo4j-lib-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-12-19 12:17:59.049162 tc-neo4j-lib-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      627 2023-12-19 12:17:51.000000 tc-neo4j-lib-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 12:17:59.049162 tc-neo4j-lib-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      512 2023-12-19 12:17:51.000000 tc-neo4j-lib-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 12:17:59.045163 tc-neo4j-lib-1.0.2/tc_neo4j_lib/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-19 12:17:51.000000 tc-neo4j-lib-1.0.2/tc_neo4j_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4961 2023-12-19 12:17:51.000000 tc-neo4j-lib-1.0.2/tc_neo4j_lib/neo4j_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 12:17:59.049162 tc-neo4j-lib-1.0.2/tc_neo4j_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-12-19 12:17:59.000000 tc-neo4j-lib-1.0.2/tc_neo4j_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      397 2023-12-19 12:17:59.000000 tc-neo4j-lib-1.0.2/tc_neo4j_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 12:17:59.000000 tc-neo4j-lib-1.0.2/tc_neo4j_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-12-19 12:17:59.000000 tc-neo4j-lib-1.0.2/tc_neo4j_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-19 12:17:59.000000 tc-neo4j-lib-1.0.2/tc_neo4j_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 12:17:59.045163 tc-neo4j-lib-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 12:17:51.000000 tc-neo4j-lib-1.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 12:17:59.045163 tc-neo4j-lib-1.0.2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 12:17:51.000000 tc-neo4j-lib-1.0.2/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2023-12-19 12:17:51.000000 tc-neo4j-lib-1.0.2/tests/integration/test_neo4j_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 12:17:59.049162 tc-neo4j-lib-1.0.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 12:17:51.000000 tc-neo4j-lib-1.0.2/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2023-12-19 12:17:51.000000 tc-neo4j-lib-1.0.2/tests/unit/test_set_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:10:05.345095 tc_neo4j_lib-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-22 16:10:05.345095 tc_neo4j_lib-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-22 16:09:54.000000 tc_neo4j_lib-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:10:05.345095 tc_neo4j_lib-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-22 16:09:54.000000 tc_neo4j_lib-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:10:05.345095 tc_neo4j_lib-2.0.0/tc_neo4j_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-22 16:09:54.000000 tc_neo4j_lib-2.0.0/tc_neo4j_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-22 16:09:54.000000 tc_neo4j_lib-2.0.0/tc_neo4j_lib/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-22 16:09:54.000000 tc_neo4j_lib-2.0.0/tc_neo4j_lib/neo4j_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-22 16:09:54.000000 tc_neo4j_lib-2.0.0/tc_neo4j_lib/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:10:05.345095 tc_neo4j_lib-2.0.0/tc_neo4j_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-22 16:10:05.000000 tc_neo4j_lib-2.0.0/tc_neo4j_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-22 16:10:05.000000 tc_neo4j_lib-2.0.0/tc_neo4j_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:10:05.000000 tc_neo4j_lib-2.0.0/tc_neo4j_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-22 16:10:05.000000 tc_neo4j_lib-2.0.0/tc_neo4j_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-22 16:10:05.000000 tc_neo4j_lib-2.0.0/tc_neo4j_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:10:05.345095 tc_neo4j_lib-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:09:54.000000 tc_neo4j_lib-2.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:10:05.345095 tc_neo4j_lib-2.0.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:09:54.000000 tc_neo4j_lib-2.0.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-22 16:09:54.000000 tc_neo4j_lib-2.0.0/tests/integration/test_run_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:10:05.345095 tc_neo4j_lib-2.0.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:09:54.000000 tc_neo4j_lib-2.0.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-22 16:09:54.000000 tc_neo4j_lib-2.0.0/tests/unit/test_credentials.py
```

### Comparing `tc-neo4j-lib-1.0.2/PKG-INFO` & `tc_neo4j_lib-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-neo4j-lib
-Version: 1.0.2
+Version: 2.0.0
 Summary: A neo4j shared library to use across togethercrew python projects.
 Author: Mohammad Amin Dadgar, TogetherCrew
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Requires-Dist: numpy>=1.24.1
 Requires-Dist: pytest<8.0.0,>=7.2.0
 Requires-Dist: pytest-cov<6.0.0,>=4.0.0
```

### Comparing `tc-neo4j-lib-1.0.2/README.md` & `tc_neo4j_lib-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `tc-neo4j-lib-1.0.2/setup.py` & `tc_neo4j_lib-2.0.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 
 setup(
     name="tc-neo4j-lib",
-    version="1.0.2",
+    version="2.0.0",
     author="Mohammad Amin Dadgar, TogetherCrew",
     maintainer="Mohammad Amin Dadgar",
     maintainer_email="dadgaramin96@gmail.com",
     packages=find_packages(),
     description="A neo4j shared library to use across togethercrew python projects.",
     long_description=open("README.md").read(),
     install_requires=requirements,
```

### Comparing `tc-neo4j-lib-1.0.2/tc_neo4j_lib.egg-info/PKG-INFO` & `tc_neo4j_lib-2.0.0/tc_neo4j_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-neo4j-lib
-Version: 1.0.2
+Version: 2.0.0
 Summary: A neo4j shared library to use across togethercrew python projects.
 Author: Mohammad Amin Dadgar, TogetherCrew
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Requires-Dist: numpy>=1.24.1
 Requires-Dist: pytest<8.0.0,>=7.2.0
 Requires-Dist: pytest-cov<6.0.0,>=4.0.0
```

