# Comparing `tmp/pysql-repo-0.7.1.tar.gz` & `tmp/pysql-repo-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysql-repo-0.7.1.tar", last modified: Wed May 22 09:02:07 2024, max compression
+gzip compressed data, was "pysql-repo-0.7.2.tar", last modified: Wed May 22 11:03:35 2024, max compression
```

## Comparing `pysql-repo-0.7.1.tar` & `pysql-repo-0.7.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:02:07.292007 pysql-repo-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)    41337 2024-05-22 09:02:07.292007 pysql-repo-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    40736 2024-05-22 09:02:00.000000 pysql-repo-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:02:07.288006 pysql-repo-0.7.1/pysql_repo/
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-22 09:02:00.000000 pysql-repo-0.7.1/pysql_repo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:02:07.292007 pysql-repo-0.7.1/pysql_repo/_constants/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-22 09:02:00.000000 pysql-repo-0.7.1/pysql_repo/_constants/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-05-22 09:02:00.000000 pysql-repo-0.7.1/pysql_repo/_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-05-22 09:02:00.000000 pysql-repo-0.7.1/pysql_repo/_database_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-22 09:02:00.000000 pysql-repo-0.7.1/pysql_repo/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    18541 2024-05-22 09:02:00.000000 pysql-repo-0.7.1/pysql_repo/_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-22 09:02:00.000000 pysql-repo-0.7.1/pysql_repo/_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    23747 2024-05-22 09:02:00.000000 pysql-repo-0.7.1/pysql_repo/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:02:07.292007 pysql-repo-0.7.1/pysql_repo/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 09:02:00.000000 pysql-repo-0.7.1/pysql_repo/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-05-22 09:02:00.000000 pysql-repo-0.7.1/pysql_repo/asyncio/async_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-22 09:02:00.000000 pysql-repo-0.7.1/pysql_repo/asyncio/async_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    19189 2024-05-22 09:02:00.000000 pysql-repo-0.7.1/pysql_repo/asyncio/async_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-22 09:02:00.000000 pysql-repo-0.7.1/pysql_repo/asyncio/async_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:02:07.292007 pysql-repo-0.7.1/pysql_repo/libs/
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-22 09:02:00.000000 pysql-repo-0.7.1/pysql_repo/libs/file_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:02:00.000000 pysql-repo-0.7.1/pysql_repo/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:02:07.292007 pysql-repo-0.7.1/pysql_repo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41337 2024-05-22 09:02:07.000000 pysql-repo-0.7.1/pysql_repo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-22 09:02:07.000000 pysql-repo-0.7.1/pysql_repo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 09:02:07.000000 pysql-repo-0.7.1/pysql_repo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 09:02:07.000000 pysql-repo-0.7.1/pysql_repo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 09:02:07.000000 pysql-repo-0.7.1/pysql_repo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 09:02:07.292007 pysql-repo-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-22 09:02:05.000000 pysql-repo-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:03:35.445509 pysql-repo-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    41337 2024-05-22 11:03:35.445509 pysql-repo-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    40736 2024-05-22 11:03:32.000000 pysql-repo-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:03:35.441509 pysql-repo-0.7.2/pysql_repo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-22 11:03:32.000000 pysql-repo-0.7.2/pysql_repo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:03:35.445509 pysql-repo-0.7.2/pysql_repo/_constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-22 11:03:32.000000 pysql-repo-0.7.2/pysql_repo/_constants/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-05-22 11:03:32.000000 pysql-repo-0.7.2/pysql_repo/_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-05-22 11:03:32.000000 pysql-repo-0.7.2/pysql_repo/_database_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-22 11:03:32.000000 pysql-repo-0.7.2/pysql_repo/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18541 2024-05-22 11:03:32.000000 pysql-repo-0.7.2/pysql_repo/_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-22 11:03:32.000000 pysql-repo-0.7.2/pysql_repo/_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23747 2024-05-22 11:03:32.000000 pysql-repo-0.7.2/pysql_repo/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:03:35.445509 pysql-repo-0.7.2/pysql_repo/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 11:03:32.000000 pysql-repo-0.7.2/pysql_repo/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-05-22 11:03:32.000000 pysql-repo-0.7.2/pysql_repo/asyncio/async_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-22 11:03:32.000000 pysql-repo-0.7.2/pysql_repo/asyncio/async_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19189 2024-05-22 11:03:32.000000 pysql-repo-0.7.2/pysql_repo/asyncio/async_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-22 11:03:32.000000 pysql-repo-0.7.2/pysql_repo/asyncio/async_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:03:35.445509 pysql-repo-0.7.2/pysql_repo/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-22 11:03:32.000000 pysql-repo-0.7.2/pysql_repo/libs/file_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:03:32.000000 pysql-repo-0.7.2/pysql_repo/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:03:35.441509 pysql-repo-0.7.2/pysql_repo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41337 2024-05-22 11:03:35.000000 pysql-repo-0.7.2/pysql_repo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-22 11:03:35.000000 pysql-repo-0.7.2/pysql_repo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:03:35.000000 pysql-repo-0.7.2/pysql_repo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 11:03:35.000000 pysql-repo-0.7.2/pysql_repo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 11:03:35.000000 pysql-repo-0.7.2/pysql_repo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 11:03:35.445509 pysql-repo-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-22 11:03:33.000000 pysql-repo-0.7.2/setup.py
```

### Comparing `pysql-repo-0.7.1/PKG-INFO` & `pysql-repo-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysql-repo
-Version: 0.7.1
+Version: 0.7.2
 Summary: A project to have a base repository class to perform select/insert/update/delete with dynamic syntax
 Home-page: https://github.com/Impro02/pysql-repo
-Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.7.1.tar.gz
+Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.7.2.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pysql-repo-0.7.1/README.md` & `pysql-repo-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.1/pysql_repo/__init__.py` & `pysql-repo-0.7.2/pysql_repo/__init__.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.1/pysql_repo/_constants/enum.py` & `pysql-repo-0.7.2/pysql_repo/_constants/enum.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.1/pysql_repo/_database.py` & `pysql-repo-0.7.2/pysql_repo/_database.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.1/pysql_repo/_database_base.py` & `pysql-repo-0.7.2/pysql_repo/_database_base.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.1/pysql_repo/_decorators.py` & `pysql-repo-0.7.2/pysql_repo/_decorators.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.1/pysql_repo/_repository.py` & `pysql-repo-0.7.2/pysql_repo/_repository.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.1/pysql_repo/_service.py` & `pysql-repo-0.7.2/pysql_repo/_service.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.1/pysql_repo/_utils.py` & `pysql-repo-0.7.2/pysql_repo/_utils.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.1/pysql_repo/asyncio/async_database.py` & `pysql-repo-0.7.2/pysql_repo/asyncio/async_database.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.1/pysql_repo/asyncio/async_decorator.py` & `pysql-repo-0.7.2/pysql_repo/asyncio/async_decorator.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.1/pysql_repo/asyncio/async_repository.py` & `pysql-repo-0.7.2/pysql_repo/asyncio/async_repository.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.1/pysql_repo/asyncio/async_service.py` & `pysql-repo-0.7.2/pysql_repo/asyncio/async_service.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.1/pysql_repo/libs/file_lib.py` & `pysql-repo-0.7.2/pysql_repo/libs/file_lib.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.1/pysql_repo.egg-info/PKG-INFO` & `pysql-repo-0.7.2/pysql_repo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysql-repo
-Version: 0.7.1
+Version: 0.7.2
 Summary: A project to have a base repository class to perform select/insert/update/delete with dynamic syntax
 Home-page: https://github.com/Impro02/pysql-repo
-Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.7.1.tar.gz
+Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.7.2.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pysql-repo-0.7.1/pysql_repo.egg-info/SOURCES.txt` & `pysql-repo-0.7.2/pysql_repo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.7.1/setup.py` & `pysql-repo-0.7.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.7.1"
+version = "0.7.2"
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="pysql-repo",
     version=version,
@@ -27,8 +27,9 @@
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
     ],
     package_data={"pysql_repo": ["py.typed"]},
+    include_package_data=True,
 )
```

