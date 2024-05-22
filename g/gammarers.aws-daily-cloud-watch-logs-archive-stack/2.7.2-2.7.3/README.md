# Comparing `tmp/gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2.tar.gz` & `tmp/gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2.tar", last modified: Wed May 15 19:13:42 2024, max compression
+gzip compressed data, was "gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3.tar", last modified: Wed May 22 19:13:02 2024, max compression
```

## Comparing `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2.tar` & `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.097012 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-15 19:13:27.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 19:13:27.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-15 19:13:42.097012 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-15 19:13:27.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-15 19:13:27.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:13:42.097012 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-15 19:13:27.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.093012 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.093012 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/src/gammarers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.097012 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/
--rw-r--r--   0 runner    (1001) docker     (127)    27881 2024-05-15 19:13:27.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.097012 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-15 19:13:27.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45063 2024-05-15 19:13:27.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/_jsii/aws-daily-cloud-watch-logs-archive-stack@2.7.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:13:27.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.097012 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-15 19:13:42.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-15 19:13:42.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:13:42.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-15 19:13:42.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 19:13:42.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:13:02.900710 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-22 19:12:52.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 19:12:52.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-22 19:13:02.900710 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-22 19:12:52.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-22 19:12:52.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 19:13:02.900710 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-22 19:12:52.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:13:02.900710 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:13:02.900710 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/src/gammarers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:13:02.900710 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/
+-rw-r--r--   0 runner    (1001) docker     (127)    27881 2024-05-22 19:12:52.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:13:02.900710 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-22 19:12:52.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45062 2024-05-22 19:12:52.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/_jsii/aws-daily-cloud-watch-logs-archive-stack@2.7.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 19:12:52.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:13:02.900710 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-22 19:13:02.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-22 19:13:02.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 19:13:02.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-22 19:13:02.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 19:13:02.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/top_level.txt
```

### Comparing `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/LICENSE` & `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/PKG-INFO` & `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-daily-cloud-watch-logs-archive-stack
-Version: 2.7.2
+Version: 2.7.3
 Summary: AWS CloudWatch Logs daily archive to s3 bucket
 Home-page: https://github.com/gammarers/aws-daily-cloud-watch-logs-archive-stack.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-daily-cloud-watch-logs-archive-stack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/README.md` & `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/README.md`

 * *Files identical despite different names*

### Comparing `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/setup.py` & `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarers.aws-daily-cloud-watch-logs-archive-stack",
-    "version": "2.7.2",
+    "version": "2.7.3",
     "description": "AWS CloudWatch Logs daily archive to s3 bucket",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarers/aws-daily-cloud-watch-logs-archive-stack.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarers.aws_daily_cloud_watch_logs_archive_stack",
         "gammarers.aws_daily_cloud_watch_logs_archive_stack._jsii"
     ],
     "package_data": {
         "gammarers.aws_daily_cloud_watch_logs_archive_stack._jsii": [
-            "aws-daily-cloud-watch-logs-archive-stack@2.7.2.jsii.tgz"
+            "aws-daily-cloud-watch-logs-archive-stack@2.7.3.jsii.tgz"
         ],
         "gammarers.aws_daily_cloud_watch_logs_archive_stack": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/__init__.py` & `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/_jsii/__init__.py` & `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/_jsii/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 import aws_cdk._jsii
 import constructs._jsii
 import gammarers.aws_secure_bucket._jsii
 import gammarers.aws_secure_log_bucket._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarers/aws-daily-cloud-watch-logs-archive-stack",
-    "2.7.2",
+    "2.7.3",
     __name__[0:-6],
-    "aws-daily-cloud-watch-logs-archive-stack@2.7.2.jsii.tgz",
+    "aws-daily-cloud-watch-logs-archive-stack@2.7.3.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/PKG-INFO` & `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-daily-cloud-watch-logs-archive-stack
-Version: 2.7.2
+Version: 2.7.3
 Summary: AWS CloudWatch Logs daily archive to s3 bucket
 Home-page: https://github.com/gammarers/aws-daily-cloud-watch-logs-archive-stack.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-daily-cloud-watch-logs-archive-stack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.2/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/SOURCES.txt` & `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.3/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/SOURCES.txt
 src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/dependency_links.txt
 src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/requires.txt
 src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/top_level.txt
 src/gammarers/aws_daily_cloud_watch_logs_archive_stack/__init__.py
 src/gammarers/aws_daily_cloud_watch_logs_archive_stack/py.typed
 src/gammarers/aws_daily_cloud_watch_logs_archive_stack/_jsii/__init__.py
-src/gammarers/aws_daily_cloud_watch_logs_archive_stack/_jsii/aws-daily-cloud-watch-logs-archive-stack@2.7.2.jsii.tgz
+src/gammarers/aws_daily_cloud_watch_logs_archive_stack/_jsii/aws-daily-cloud-watch-logs-archive-stack@2.7.3.jsii.tgz
```

