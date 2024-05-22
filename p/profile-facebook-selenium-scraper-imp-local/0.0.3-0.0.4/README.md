# Comparing `tmp/profile_facebook_selenium_scraper_imp_local-0.0.3.tar.gz` & `tmp/profile_facebook_selenium_scraper_imp_local-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profile_facebook_selenium_scraper_imp_local-0.0.3.tar", last modified: Thu May  9 02:53:46 2024, max compression
+gzip compressed data, was "profile_facebook_selenium_scraper_imp_local-0.0.4.tar", last modified: Wed May 22 17:44:27 2024, max compression
```

## Comparing `profile_facebook_selenium_scraper_imp_local-0.0.3.tar` & `profile_facebook_selenium_scraper_imp_local-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:53:46.312955 profile_facebook_selenium_scraper_imp_local-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-09 02:53:46.312955 profile_facebook_selenium_scraper_imp_local-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-09 02:53:05.000000 profile_facebook_selenium_scraper_imp_local-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:53:46.312955 profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:53:46.312955 profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 02:53:05.000000 profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-09 02:53:05.000000 profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local/src/facebook_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    17749 2024-05-09 02:53:05.000000 profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local/src/facebook_scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:53:46.312955 profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-09 02:53:46.000000 profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-09 02:53:46.000000 profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 02:53:46.000000 profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 02:53:46.000000 profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-09 02:53:46.000000 profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-09 02:53:05.000000 profile_facebook_selenium_scraper_imp_local-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 02:53:46.312955 profile_facebook_selenium_scraper_imp_local-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-09 02:53:05.000000 profile_facebook_selenium_scraper_imp_local-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:44:26.999757 profile_facebook_selenium_scraper_imp_local-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-22 17:44:26.995757 profile_facebook_selenium_scraper_imp_local-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-22 17:43:54.000000 profile_facebook_selenium_scraper_imp_local-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:44:26.995757 profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:44:26.995757 profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:43:54.000000 profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-22 17:43:54.000000 profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local/src/facebook_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15574 2024-05-22 17:43:54.000000 profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local/src/facebook_scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:44:26.995757 profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-22 17:44:26.000000 profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-22 17:44:26.000000 profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 17:44:26.000000 profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-22 17:44:26.000000 profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-22 17:44:26.000000 profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-22 17:43:54.000000 profile_facebook_selenium_scraper_imp_local-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 17:44:26.999757 profile_facebook_selenium_scraper_imp_local-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-22 17:43:54.000000 profile_facebook_selenium_scraper_imp_local-0.0.4/setup.py
```

### Comparing `profile_facebook_selenium_scraper_imp_local-0.0.3/PKG-INFO` & `profile_facebook_selenium_scraper_imp_local-0.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: profile-facebook-selenium-scraper-imp-local
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyPI Package for Circles profile-facebook-selenium-scraper-imp-local Python
 Home-page: https://github.com/circles-zone/profile-facebook-selenium-scraper-imp-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: selenium>=4.20.0
 Requires-Dist: logger-local>=0.0.135
 Requires-Dist: profile-local>=0.0.65
 Requires-Dist: language-remote>=0.0.20
+Requires-Dist: python-sdk-remote>=0.0.75
 
 PyPI Package for Circles profile-facebook-selenium-scraper-imp-local Python
```

### Comparing `profile_facebook_selenium_scraper_imp_local-0.0.3/README.md` & `profile_facebook_selenium_scraper_imp_local-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local/src/facebook_constants.py` & `profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local/src/facebook_constants.py`

 * *Files identical despite different names*

### Comparing `profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local.egg-info/PKG-INFO` & `profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: profile-facebook-selenium-scraper-imp-local
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyPI Package for Circles profile-facebook-selenium-scraper-imp-local Python
 Home-page: https://github.com/circles-zone/profile-facebook-selenium-scraper-imp-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: selenium>=4.20.0
 Requires-Dist: logger-local>=0.0.135
 Requires-Dist: profile-local>=0.0.65
 Requires-Dist: language-remote>=0.0.20
+Requires-Dist: python-sdk-remote>=0.0.75
 
 PyPI Package for Circles profile-facebook-selenium-scraper-imp-local Python
```

### Comparing `profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local.egg-info/SOURCES.txt` & `profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `profile_facebook_selenium_scraper_imp_local-0.0.3/pyproject.toml` & `profile_facebook_selenium_scraper_imp_local-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `profile_facebook_selenium_scraper_imp_local-0.0.3/setup.py` & `profile_facebook_selenium_scraper_imp_local-0.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "profile-facebook-selenium-scraper-imp-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.3',  # https://pypi.org/project/profile-facebook-selenium-scraper-imp-local/
+    version='0.0.4',  # https://pypi.org/project/profile-facebook-selenium-scraper-imp-local/
     author="Circles",
     author_email="info@circlez.ai",
     description=f"PyPI Package for Circles {PACKAGE_NAME} Python",
     long_description=f"PyPI Package for Circles {PACKAGE_NAME} Python",
     long_description_content_type='text/markdown',
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
@@ -20,10 +20,11 @@
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'selenium>=4.20.0',
         'logger-local>=0.0.135',
         'profile-local>=0.0.65',
-        'language-remote>=0.0.20'
+        'language-remote>=0.0.20',
+        'python-sdk-remote>=0.0.75',
     ],
 )
```

