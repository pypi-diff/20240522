# Comparing `tmp/rtd-cli-0.0.2.tar.gz` & `tmp/rtd-cli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtd-cli-0.0.2.tar", last modified: Tue May 21 20:38:54 2024, max compression
+gzip compressed data, was "rtd-cli-0.0.3.tar", last modified: Tue May 21 20:44:48 2024, max compression
```

## Comparing `rtd-cli-0.0.2.tar` & `rtd-cli-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:38:54.781307 rtd-cli-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-21 20:38:54.781307 rtd-cli-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-21 20:38:44.000000 rtd-cli-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:38:54.777307 rtd-cli-0.0.2/rtd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 20:38:44.000000 rtd-cli-0.0.2/rtd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-21 20:38:44.000000 rtd-cli-0.0.2/rtd/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:38:54.781307 rtd-cli-0.0.2/rtd_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-21 20:38:54.000000 rtd-cli-0.0.2/rtd_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-21 20:38:54.000000 rtd-cli-0.0.2/rtd_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:38:54.000000 rtd-cli-0.0.2/rtd_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-21 20:38:54.000000 rtd-cli-0.0.2/rtd_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-21 20:38:54.000000 rtd-cli-0.0.2/rtd_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 20:38:54.000000 rtd-cli-0.0.2/rtd_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 20:38:54.781307 rtd-cli-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-21 20:38:44.000000 rtd-cli-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:44:48.492827 rtd-cli-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-21 20:44:48.492827 rtd-cli-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-21 20:44:38.000000 rtd-cli-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:44:48.492827 rtd-cli-0.0.3/rtd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 20:44:38.000000 rtd-cli-0.0.3/rtd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-21 20:44:38.000000 rtd-cli-0.0.3/rtd/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:44:48.492827 rtd-cli-0.0.3/rtd_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-21 20:44:48.000000 rtd-cli-0.0.3/rtd_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-21 20:44:48.000000 rtd-cli-0.0.3/rtd_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:44:48.000000 rtd-cli-0.0.3/rtd_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-21 20:44:48.000000 rtd-cli-0.0.3/rtd_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-21 20:44:48.000000 rtd-cli-0.0.3/rtd_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 20:44:48.000000 rtd-cli-0.0.3/rtd_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 20:44:48.492827 rtd-cli-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-21 20:44:38.000000 rtd-cli-0.0.3/setup.py
```

### Comparing `rtd-cli-0.0.2/PKG-INFO` & `rtd-cli-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtd-cli
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple CLI wrapper for the Readthedocs REST API
 Home-page: https://github.com/runsascoded/rtd.py
 Author: Ryan Williams
 Author-email: ryan@runsascoded.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -58,14 +58,14 @@
 limit=100
 
 keep_args=()
 for v in "${keep[@]}"; do
   keep_args+=(-e "$v")
 done
 
-rtd api "projects/$project/versions?limit=$limit&active=true&built=true"
+rtd api "projects/$project/versions?limit=$limit&active=true&built=true" \
 | jq -r '.results[] | select(.hidden | not) | .slug' \
-| grep "${keep_args[@]}" \
+| grep -v "${keep_args[@]}" \
 | xargs rtd hide -p $p
 ```
 
 [Readthedocs]: https://readthedocs.org
```

### Comparing `rtd-cli-0.0.2/README.md` & `rtd-cli-0.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -46,14 +46,14 @@
 limit=100
 
 keep_args=()
 for v in "${keep[@]}"; do
   keep_args+=(-e "$v")
 done
 
-rtd api "projects/$project/versions?limit=$limit&active=true&built=true"
+rtd api "projects/$project/versions?limit=$limit&active=true&built=true" \
 | jq -r '.results[] | select(.hidden | not) | .slug' \
-| grep "${keep_args[@]}" \
+| grep -v "${keep_args[@]}" \
 | xargs rtd hide -p $p
 ```
 
 [Readthedocs]: https://readthedocs.org
```

### Comparing `rtd-cli-0.0.2/rtd/main.py` & `rtd-cli-0.0.3/rtd/main.py`

 * *Files identical despite different names*

### Comparing `rtd-cli-0.0.2/rtd_cli.egg-info/PKG-INFO` & `rtd-cli-0.0.3/rtd_cli.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtd-cli
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple CLI wrapper for the Readthedocs REST API
 Home-page: https://github.com/runsascoded/rtd.py
 Author: Ryan Williams
 Author-email: ryan@runsascoded.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -58,14 +58,14 @@
 limit=100
 
 keep_args=()
 for v in "${keep[@]}"; do
   keep_args+=(-e "$v")
 done
 
-rtd api "projects/$project/versions?limit=$limit&active=true&built=true"
+rtd api "projects/$project/versions?limit=$limit&active=true&built=true" \
 | jq -r '.results[] | select(.hidden | not) | .slug' \
-| grep "${keep_args[@]}" \
+| grep -v "${keep_args[@]}" \
 | xargs rtd hide -p $p
 ```
 
 [Readthedocs]: https://readthedocs.org
```

### Comparing `rtd-cli-0.0.2/setup.py` & `rtd-cli-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="rtd-cli",
-    version="0.0.2",
+    version="0.0.3",
     description="Simple CLI wrapper for the Readthedocs REST API",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/runsascoded/rtd.py",
     author="Ryan Williams",
     author_email="ryan@runsascoded.com",
     install_requires=open("requirements.txt").read(),
```

