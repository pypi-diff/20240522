# Comparing `tmp/hikac-0.0.11.tar.gz` & `tmp/hikac-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikac-0.0.11.tar", last modified: Wed May 22 16:06:02 2024, max compression
+gzip compressed data, was "hikac-0.0.2.tar", last modified: Wed May 22 16:03:54 2024, max compression
```

## Comparing `hikac-0.0.11.tar` & `hikac-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:06:02.529400 hikac-0.0.11/
--rw-r--r--   0 yusufjon   (501) staff       (20)     1073 2024-05-22 15:25:24.000000 hikac-0.0.11/LICENSE
--rw-r--r--   0 yusufjon   (501) staff       (20)     1327 2024-05-22 16:06:02.529259 hikac-0.0.11/PKG-INFO
--rw-r--r--   0 yusufjon   (501) staff       (20)      132 2024-05-22 15:11:40.000000 hikac-0.0.11/README.md
-drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:06:02.526045 hikac-0.0.11/app/
-drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:06:02.526984 hikac-0.0.11/app/hikac/
--rw-r--r--   0 yusufjon   (501) staff       (20)       46 2024-05-22 15:22:35.000000 hikac-0.0.11/app/hikac/__init__.py
-drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:06:02.528485 hikac-0.0.11/app/hikac/src/
--rw-r--r--   0 yusufjon   (501) staff       (20)        0 2024-05-22 15:09:16.000000 hikac-0.0.11/app/hikac/src/__init__.py
--rw-r--r--   0 yusufjon   (501) staff       (20)     1743 2024-05-22 15:20:43.000000 hikac-0.0.11/app/hikac/src/hikac.py
-drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:06:02.528913 hikac-0.0.11/app/hikac/test/
--rw-r--r--   0 yusufjon   (501) staff       (20)        0 2024-05-22 15:09:16.000000 hikac-0.0.11/app/hikac/test/__init__.py
--rw-r--r--   0 yusufjon   (501) staff       (20)      166 2024-05-22 15:22:26.000000 hikac-0.0.11/app/hikac/test/test_hikac.py
-drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:06:02.528099 hikac-0.0.11/app/hikac.egg-info/
--rw-r--r--   0 yusufjon   (501) staff       (20)     1327 2024-05-22 16:06:02.000000 hikac-0.0.11/app/hikac.egg-info/PKG-INFO
--rw-r--r--   0 yusufjon   (501) staff       (20)      317 2024-05-22 16:06:02.000000 hikac-0.0.11/app/hikac.egg-info/SOURCES.txt
--rw-r--r--   0 yusufjon   (501) staff       (20)        1 2024-05-22 16:06:02.000000 hikac-0.0.11/app/hikac.egg-info/dependency_links.txt
--rw-r--r--   0 yusufjon   (501) staff       (20)       42 2024-05-22 16:06:02.000000 hikac-0.0.11/app/hikac.egg-info/requires.txt
--rw-r--r--   0 yusufjon   (501) staff       (20)        6 2024-05-22 16:06:02.000000 hikac-0.0.11/app/hikac.egg-info/top_level.txt
--rw-r--r--   0 yusufjon   (501) staff       (20)       38 2024-05-22 16:06:02.529461 hikac-0.0.11/setup.cfg
--rw-r--r--   0 yusufjon   (501) staff       (20)      838 2024-05-22 16:05:31.000000 hikac-0.0.11/setup.py
+drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:03:54.015025 hikac-0.0.2/
+-rw-r--r--   0 yusufjon   (501) staff       (20)     1073 2024-05-22 15:25:24.000000 hikac-0.0.2/LICENSE
+-rw-r--r--   0 yusufjon   (501) staff       (20)     1326 2024-05-22 16:03:54.014886 hikac-0.0.2/PKG-INFO
+-rw-r--r--   0 yusufjon   (501) staff       (20)      132 2024-05-22 15:11:40.000000 hikac-0.0.2/README.md
+drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:03:54.012545 hikac-0.0.2/app/
+drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:03:54.013198 hikac-0.0.2/app/hikac/
+-rw-r--r--   0 yusufjon   (501) staff       (20)       46 2024-05-22 15:22:35.000000 hikac-0.0.2/app/hikac/__init__.py
+drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:03:54.014208 hikac-0.0.2/app/hikac/src/
+-rw-r--r--   0 yusufjon   (501) staff       (20)        0 2024-05-22 15:09:16.000000 hikac-0.0.2/app/hikac/src/__init__.py
+-rw-r--r--   0 yusufjon   (501) staff       (20)     1743 2024-05-22 15:20:43.000000 hikac-0.0.2/app/hikac/src/hikac.py
+drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:03:54.014649 hikac-0.0.2/app/hikac/test/
+-rw-r--r--   0 yusufjon   (501) staff       (20)        0 2024-05-22 15:09:16.000000 hikac-0.0.2/app/hikac/test/__init__.py
+-rw-r--r--   0 yusufjon   (501) staff       (20)      166 2024-05-22 15:22:26.000000 hikac-0.0.2/app/hikac/test/test_hikac.py
+drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:03:54.013955 hikac-0.0.2/app/hikac.egg-info/
+-rw-r--r--   0 yusufjon   (501) staff       (20)     1326 2024-05-22 16:03:53.000000 hikac-0.0.2/app/hikac.egg-info/PKG-INFO
+-rw-r--r--   0 yusufjon   (501) staff       (20)      317 2024-05-22 16:03:53.000000 hikac-0.0.2/app/hikac.egg-info/SOURCES.txt
+-rw-r--r--   0 yusufjon   (501) staff       (20)        1 2024-05-22 16:03:53.000000 hikac-0.0.2/app/hikac.egg-info/dependency_links.txt
+-rw-r--r--   0 yusufjon   (501) staff       (20)       42 2024-05-22 16:03:53.000000 hikac-0.0.2/app/hikac.egg-info/requires.txt
+-rw-r--r--   0 yusufjon   (501) staff       (20)        6 2024-05-22 16:03:53.000000 hikac-0.0.2/app/hikac.egg-info/top_level.txt
+-rw-r--r--   0 yusufjon   (501) staff       (20)       38 2024-05-22 16:03:54.015087 hikac-0.0.2/setup.cfg
+-rw-r--r--   0 yusufjon   (501) staff       (20)      837 2024-05-22 16:03:50.000000 hikac-0.0.2/setup.py
```

### Comparing `hikac-0.0.11/LICENSE` & `hikac-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hikac-0.0.11/PKG-INFO` & `hikac-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikac
-Version: 0.0.11
+Version: 0.0.2
 Summary: A hikvision access control request manager
 Home-page: https://github.com/yusufjonc07/hikac
 Author: YusufAxmad
 Author-email: studentyusufaxmad@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hikac-0.0.11/app/hikac/src/hikac.py` & `hikac-0.0.2/app/hikac/src/hikac.py`

 * *Files identical despite different names*

### Comparing `hikac-0.0.11/app/hikac.egg-info/PKG-INFO` & `hikac-0.0.2/app/hikac.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikac
-Version: 0.0.11
+Version: 0.0.2
 Summary: A hikvision access control request manager
 Home-page: https://github.com/yusufjonc07/hikac
 Author: YusufAxmad
 Author-email: studentyusufaxmad@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hikac-0.0.11/setup.py` & `hikac-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="hikac",
-    version="0.0.11",
+    version="0.0.2",
     description="A hikvision access control request manager",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yusufjonc07/hikac",
     author="YusufAxmad",
```

