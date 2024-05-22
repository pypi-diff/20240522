# Comparing `tmp/iRe.py-0.1.1.tar.gz` & `tmp/iRe.py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iRe.py-0.1.1.tar", last modified: Mon May 13 02:10:44 2024, max compression
+gzip compressed data, was "iRe.py-0.2.0.tar", last modified: Wed May 22 04:44:00 2024, max compression
```

## Comparing `iRe.py-0.1.1.tar` & `iRe.py-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 02:10:44.586588 iRe.py-0.1.1/
--rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-13 02:10:29.000000 iRe.py-0.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      920 2024-05-13 02:10:44.585589 iRe.py-0.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      514 2024-05-13 02:10:29.000000 iRe.py-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 02:10:44.584589 iRe.py-0.1.1/iRe.py.egg-info/
--rw-r--r--   0 root         (0) root         (0)      920 2024-05-13 02:10:44.000000 iRe.py-0.1.1/iRe.py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      237 2024-05-13 02:10:44.000000 iRe.py-0.1.1/iRe.py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 02:10:44.000000 iRe.py-0.1.1/iRe.py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      195 2024-05-13 02:10:44.000000 iRe.py-0.1.1/iRe.py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2024-05-13 02:10:44.000000 iRe.py-0.1.1/iRe.py.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 02:10:44.585589 iRe.py-0.1.1/ire/
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-13 02:10:29.000000 iRe.py-0.1.1/ire/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2024-05-13 02:10:29.000000 iRe.py-0.1.1/ire/dvc.py
--rw-rw-rw-   0 root         (0) root         (0)     2613 2024-05-13 02:10:29.000000 iRe.py-0.1.1/ire/git.py
--rw-rw-rw-   0 root         (0) root         (0)     6447 2024-05-13 02:10:29.000000 iRe.py-0.1.1/ire/ire.py
--rw-rw-rw-   0 root         (0) root         (0)     1747 2024-05-13 02:10:29.000000 iRe.py-0.1.1/ire/utils.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 02:10:44.586588 iRe.py-0.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-13 02:10:29.000000 iRe.py-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 04:44:00.702634 iRe.py-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-22 04:43:45.000000 iRe.py-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      920 2024-05-22 04:44:00.701634 iRe.py-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      514 2024-05-22 04:43:45.000000 iRe.py-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 04:44:00.700634 iRe.py-0.2.0/iRe.py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      920 2024-05-22 04:44:00.000000 iRe.py-0.2.0/iRe.py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      247 2024-05-22 04:44:00.000000 iRe.py-0.2.0/iRe.py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 04:44:00.000000 iRe.py-0.2.0/iRe.py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      195 2024-05-22 04:44:00.000000 iRe.py-0.2.0/iRe.py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-05-22 04:44:00.000000 iRe.py-0.2.0/iRe.py.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 04:44:00.701634 iRe.py-0.2.0/ire/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-05-22 04:43:45.000000 iRe.py-0.2.0/ire/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2024-05-22 04:43:45.000000 iRe.py-0.2.0/ire/dvc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2613 2024-05-22 04:43:45.000000 iRe.py-0.2.0/ire/git.py
+-rw-rw-rw-   0 root         (0) root         (0)    10790 2024-05-22 04:43:45.000000 iRe.py-0.2.0/ire/ire.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2024-05-22 04:43:45.000000 iRe.py-0.2.0/ire/md.py
+-rw-rw-rw-   0 root         (0) root         (0)     1747 2024-05-22 04:43:45.000000 iRe.py-0.2.0/ire/utils.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 04:44:00.702634 iRe.py-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-22 04:43:45.000000 iRe.py-0.2.0/setup.py
```

### Comparing `iRe.py-0.1.1/LICENSE` & `iRe.py-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iRe.py-0.1.1/PKG-INFO` & `iRe.py-0.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iRe.py
-Version: 0.1.1
+Version: 0.2.0
 Summary: Export tables and plots from Jupyter notebooks, along with metadata for embedding interactive tables in downstream apps.
 Home-page: https://gitlab.com/runsascoded/ire/py
 Author: Ryan Williams
 Author-email: ryan@runsascoded.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: plotly
```

### Comparing `iRe.py-0.1.1/README.md` & `iRe.py-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `iRe.py-0.1.1/iRe.py.egg-info/PKG-INFO` & `iRe.py-0.2.0/iRe.py.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iRe.py
-Version: 0.1.1
+Version: 0.2.0
 Summary: Export tables and plots from Jupyter notebooks, along with metadata for embedding interactive tables in downstream apps.
 Home-page: https://gitlab.com/runsascoded/ire/py
 Author: Ryan Williams
 Author-email: ryan@runsascoded.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: plotly
```

### Comparing `iRe.py-0.1.1/ire/dvc.py` & `iRe.py-0.2.0/ire/dvc.py`

 * *Files identical despite different names*

### Comparing `iRe.py-0.1.1/ire/git.py` & `iRe.py-0.2.0/ire/git.py`

 * *Files identical despite different names*

### Comparing `iRe.py-0.1.1/ire/utils.py` & `iRe.py-0.2.0/ire/utils.py`

 * *Files identical despite different names*

### Comparing `iRe.py-0.1.1/setup.py` & `iRe.py-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="iRe.py",
-    version="0.1.1",
+    version="0.2.0",
     description="Export tables and plots from Jupyter notebooks, along with metadata for embedding interactive tables in downstream apps.",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=open("requirements.txt", "r").read(),
     extras_require={
         "plotly": "plotly",
```

