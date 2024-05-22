# Comparing `tmp/apeboiy-0.0.1.tar.gz` & `tmp/apeboiy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apeboiy-0.0.1.tar", last modified: Wed May 22 10:47:01 2024, max compression
+gzip compressed data, was "apeboiy-0.0.2.tar", last modified: Wed May 22 12:21:58 2024, max compression
```

## Comparing `apeboiy-0.0.1.tar` & `apeboiy-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 10:47:01.429191 apeboiy-0.0.1/
--rw-r--r--   0 iccy       (501) staff       (20)     1053 2024-05-22 10:25:41.000000 apeboiy-0.0.1/LICENSE
--rw-r--r--   0 iccy       (501) staff       (20)      578 2024-05-22 10:47:01.429009 apeboiy-0.0.1/PKG-INFO
--rw-r--r--   0 iccy       (501) staff       (20)      150 2024-05-22 10:25:15.000000 apeboiy-0.0.1/README.md
--rw-r--r--   0 iccy       (501) staff       (20)      508 2024-05-22 10:46:28.000000 apeboiy-0.0.1/pyproject.toml
--rw-r--r--   0 iccy       (501) staff       (20)       38 2024-05-22 10:47:01.429228 apeboiy-0.0.1/setup.cfg
-drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 10:47:01.427249 apeboiy-0.0.1/src/
-drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 10:47:01.428080 apeboiy-0.0.1/src/apeboiy/
--rw-r--r--   0 iccy       (501) staff       (20)        0 2024-05-22 10:20:04.000000 apeboiy-0.0.1/src/apeboiy/__init__.py
--rw-r--r--   0 iccy       (501) staff       (20)      115 2024-05-22 10:21:19.000000 apeboiy-0.0.1/src/apeboiy/example.py
-drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 10:47:01.428831 apeboiy-0.0.1/src/apeboiy.egg-info/
--rw-r--r--   0 iccy       (501) staff       (20)      578 2024-05-22 10:47:01.000000 apeboiy-0.0.1/src/apeboiy.egg-info/PKG-INFO
--rw-r--r--   0 iccy       (501) staff       (20)      219 2024-05-22 10:47:01.000000 apeboiy-0.0.1/src/apeboiy.egg-info/SOURCES.txt
--rw-r--r--   0 iccy       (501) staff       (20)        1 2024-05-22 10:47:01.000000 apeboiy-0.0.1/src/apeboiy.egg-info/dependency_links.txt
--rw-r--r--   0 iccy       (501) staff       (20)        8 2024-05-22 10:47:01.000000 apeboiy-0.0.1/src/apeboiy.egg-info/top_level.txt
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 12:21:58.658276 apeboiy-0.0.2/
+-rw-r--r--   0 iccy       (501) staff       (20)     1053 2024-05-22 10:25:41.000000 apeboiy-0.0.2/LICENSE
+-rw-r--r--   0 iccy       (501) staff       (20)      714 2024-05-22 12:21:58.658078 apeboiy-0.0.2/PKG-INFO
+-rw-r--r--   0 iccy       (501) staff       (20)      225 2024-05-22 10:51:09.000000 apeboiy-0.0.2/README.md
+-rw-r--r--   0 iccy       (501) staff       (20)      573 2024-05-22 12:21:55.000000 apeboiy-0.0.2/pyproject.toml
+-rw-r--r--   0 iccy       (501) staff       (20)       38 2024-05-22 12:21:58.658311 apeboiy-0.0.2/setup.cfg
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 12:21:58.656051 apeboiy-0.0.2/src/
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 12:21:58.657046 apeboiy-0.0.2/src/apeboiy/
+-rw-r--r--   0 iccy       (501) staff       (20)        0 2024-05-22 10:20:04.000000 apeboiy-0.0.2/src/apeboiy/__init__.py
+-rw-r--r--   0 iccy       (501) staff       (20)      115 2024-05-22 10:21:19.000000 apeboiy-0.0.2/src/apeboiy/example.py
+-rw-r--r--   0 iccy       (501) staff       (20)     3258 2024-05-22 12:19:49.000000 apeboiy-0.0.2/src/apeboiy/plyreader.py
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 12:21:58.657900 apeboiy-0.0.2/src/apeboiy.egg-info/
+-rw-r--r--   0 iccy       (501) staff       (20)      714 2024-05-22 12:21:58.000000 apeboiy-0.0.2/src/apeboiy.egg-info/PKG-INFO
+-rw-r--r--   0 iccy       (501) staff       (20)      278 2024-05-22 12:21:58.000000 apeboiy-0.0.2/src/apeboiy.egg-info/SOURCES.txt
+-rw-r--r--   0 iccy       (501) staff       (20)        1 2024-05-22 12:21:58.000000 apeboiy-0.0.2/src/apeboiy.egg-info/dependency_links.txt
+-rw-r--r--   0 iccy       (501) staff       (20)       31 2024-05-22 12:21:58.000000 apeboiy-0.0.2/src/apeboiy.egg-info/requires.txt
+-rw-r--r--   0 iccy       (501) staff       (20)        8 2024-05-22 12:21:58.000000 apeboiy-0.0.2/src/apeboiy.egg-info/top_level.txt
```

### Comparing `apeboiy-0.0.1/LICENSE` & `apeboiy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apeboiy-0.0.1/PKG-INFO` & `apeboiy-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: apeboiy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Shared AppleBoiy's packages.
 Author-email: AppleBoiy <contact.chaipat@gmail.com>
 Project-URL: Homepage, https://github.com/AppleBoiy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.25.1
+Requires-Dist: numpy>=1.21.0
 
 # Example Package
 
 This is a simple example package.
 
 You can read more [here.](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
+
+pypi: [pypi/AppleBoiy](https://pypi.org/manage/project/apeboiy/releases/)
```

### Comparing `apeboiy-0.0.1/src/apeboiy.egg-info/PKG-INFO` & `apeboiy-0.0.2/src/apeboiy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: apeboiy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Shared AppleBoiy's packages.
 Author-email: AppleBoiy <contact.chaipat@gmail.com>
 Project-URL: Homepage, https://github.com/AppleBoiy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.25.1
+Requires-Dist: numpy>=1.21.0
 
 # Example Package
 
 This is a simple example package.
 
 You can read more [here.](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
+
+pypi: [pypi/AppleBoiy](https://pypi.org/manage/project/apeboiy/releases/)
```

