# Comparing `tmp/contact_profile_local-0.0.8.tar.gz` & `tmp/contact_profile_local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_profile_local-0.0.8.tar", last modified: Wed May  8 19:04:14 2024, max compression
+gzip compressed data, was "contact_profile_local-0.0.9.tar", last modified: Wed May  8 19:56:10 2024, max compression
```

## Comparing `contact_profile_local-0.0.8.tar` & `contact_profile_local-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:04:14.658355 contact_profile_local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-08 19:04:14.654355 contact_profile_local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 19:03:41.000000 contact_profile_local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:04:14.654355 contact_profile_local-0.0.8/contact_profile_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:04:14.654355 contact_profile_local-0.0.8/contact_profile_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:03:41.000000 contact_profile_local-0.0.8/contact_profile_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-05-08 19:03:41.000000 contact_profile_local-0.0.8/contact_profile_local/src/contact_profiles_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-08 19:03:41.000000 contact_profile_local-0.0.8/contact_profile_local/src/contact_profiles_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:04:14.654355 contact_profile_local-0.0.8/contact_profile_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-08 19:04:14.000000 contact_profile_local-0.0.8/contact_profile_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-08 19:04:14.000000 contact_profile_local-0.0.8/contact_profile_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 19:04:14.000000 contact_profile_local-0.0.8/contact_profile_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-08 19:04:14.000000 contact_profile_local-0.0.8/contact_profile_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 19:04:14.000000 contact_profile_local-0.0.8/contact_profile_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-08 19:03:41.000000 contact_profile_local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 19:04:14.658355 contact_profile_local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-08 19:03:41.000000 contact_profile_local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:56:10.262792 contact_profile_local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-08 19:56:10.262792 contact_profile_local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 19:55:39.000000 contact_profile_local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:56:10.258792 contact_profile_local-0.0.9/contact_profile_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:56:10.262792 contact_profile_local-0.0.9/contact_profile_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:55:39.000000 contact_profile_local-0.0.9/contact_profile_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-05-08 19:55:39.000000 contact_profile_local-0.0.9/contact_profile_local/src/contact_profiles_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-08 19:55:39.000000 contact_profile_local-0.0.9/contact_profile_local/src/contact_profiles_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:56:10.262792 contact_profile_local-0.0.9/contact_profile_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-08 19:56:10.000000 contact_profile_local-0.0.9/contact_profile_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-08 19:56:10.000000 contact_profile_local-0.0.9/contact_profile_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 19:56:10.000000 contact_profile_local-0.0.9/contact_profile_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-08 19:56:10.000000 contact_profile_local-0.0.9/contact_profile_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 19:56:10.000000 contact_profile_local-0.0.9/contact_profile_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-08 19:55:39.000000 contact_profile_local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 19:56:10.262792 contact_profile_local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-08 19:55:39.000000 contact_profile_local-0.0.9/setup.py
```

### Comparing `contact_profile_local-0.0.8/PKG-INFO` & `contact_profile_local-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-profile-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles contact-profile-local Python
 Home-page: https://github.com/circles-zone/contact-profile-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `contact_profile_local-0.0.8/contact_profile_local/src/contact_profiles_local.py` & `contact_profile_local-0.0.9/contact_profile_local/src/contact_profiles_local.py`

 * *Files identical despite different names*

### Comparing `contact_profile_local-0.0.8/contact_profile_local/src/contact_profiles_local_constants.py` & `contact_profile_local-0.0.9/contact_profile_local/src/contact_profiles_local_constants.py`

 * *Files identical despite different names*

### Comparing `contact_profile_local-0.0.8/contact_profile_local.egg-info/PKG-INFO` & `contact_profile_local-0.0.9/contact_profile_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-profile-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles contact-profile-local Python
 Home-page: https://github.com/circles-zone/contact-profile-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `contact_profile_local-0.0.8/setup.py` & `contact_profile_local-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "contact-profile-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.8',  # https://pypi.org/project/contact-profile-local/
+    version='0.0.9',  # https://pypi.org/project/contact-profile-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles contact-profile-local Python",
     long_description="PyPI Package for Circles contact-profile-local Python",
     long_description_content_type='text/markdown',
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

