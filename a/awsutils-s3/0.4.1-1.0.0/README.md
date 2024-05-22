# Comparing `tmp/awsutils-s3-0.4.1.tar.gz` & `tmp/awsutils-s3-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsutils-s3-0.4.1.tar", last modified: Fri May 17 18:33:48 2024, max compression
+gzip compressed data, was "awsutils-s3-1.0.0.tar", last modified: Wed May 22 19:01:04 2024, max compression
```

## Comparing `awsutils-s3-0.4.1.tar` & `awsutils-s3-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:33:48.318579 awsutils-s3-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 18:33:41.000000 awsutils-s3-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-17 18:33:48.318579 awsutils-s3-0.4.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:33:48.314579 awsutils-s3-0.4.1/awsutils/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-17 18:33:41.000000 awsutils-s3-0.4.1/awsutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:33:48.318579 awsutils-s3-0.4.1/awsutils/s3/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-17 18:33:41.000000 awsutils-s3-0.4.1/awsutils/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-17 18:33:41.000000 awsutils-s3-0.4.1/awsutils/s3/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 18:33:41.000000 awsutils-s3-0.4.1/awsutils/s3/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-17 18:33:41.000000 awsutils-s3-0.4.1/awsutils/s3/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    13300 2024-05-17 18:33:41.000000 awsutils-s3-0.4.1/awsutils/s3/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-17 18:33:41.000000 awsutils-s3-0.4.1/awsutils/s3/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:33:48.318579 awsutils-s3-0.4.1/awsutils_s3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-17 18:33:48.000000 awsutils-s3-0.4.1/awsutils_s3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-17 18:33:48.000000 awsutils-s3-0.4.1/awsutils_s3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 18:33:48.000000 awsutils-s3-0.4.1/awsutils_s3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-17 18:33:48.000000 awsutils-s3-0.4.1/awsutils_s3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 18:33:48.000000 awsutils-s3-0.4.1/awsutils_s3.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-17 18:33:48.000000 awsutils-s3-0.4.1/awsutils_s3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 18:33:48.000000 awsutils-s3-0.4.1/awsutils_s3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 18:33:48.318579 awsutils-s3-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-17 18:33:41.000000 awsutils-s3-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:04.752072 awsutils-s3-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 19:00:56.000000 awsutils-s3-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-22 19:01:04.752072 awsutils-s3-1.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:04.752072 awsutils-s3-1.0.0/awsutils/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 19:00:56.000000 awsutils-s3-1.0.0/awsutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:04.752072 awsutils-s3-1.0.0/awsutils/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-22 19:00:56.000000 awsutils-s3-1.0.0/awsutils/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-22 19:00:56.000000 awsutils-s3-1.0.0/awsutils/s3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 19:00:56.000000 awsutils-s3-1.0.0/awsutils/s3/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-22 19:00:56.000000 awsutils-s3-1.0.0/awsutils/s3/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13300 2024-05-22 19:00:56.000000 awsutils-s3-1.0.0/awsutils/s3/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-22 19:00:56.000000 awsutils-s3-1.0.0/awsutils/s3/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:04.752072 awsutils-s3-1.0.0/awsutils_s3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-22 19:01:04.000000 awsutils-s3-1.0.0/awsutils_s3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-22 19:01:04.000000 awsutils-s3-1.0.0/awsutils_s3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 19:01:04.000000 awsutils-s3-1.0.0/awsutils_s3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 19:01:04.000000 awsutils-s3-1.0.0/awsutils_s3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 19:01:04.000000 awsutils-s3-1.0.0/awsutils_s3.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-22 19:01:04.000000 awsutils-s3-1.0.0/awsutils_s3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 19:01:04.000000 awsutils-s3-1.0.0/awsutils_s3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 19:01:04.752072 awsutils-s3-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-22 19:00:56.000000 awsutils-s3-1.0.0/setup.py
```

### Comparing `awsutils-s3-0.4.1/awsutils/s3/__main__.py` & `awsutils-s3-1.0.0/awsutils/s3/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 def print_output(event, bucket=None, local_path=None, remote_path=None):
     string = '{0}: {1} => {2}' if not event.lower().startswith('download') else '{0}: {2} to {1}'
     print(string.format(event, local_path, os.path.join(bucket_uri(bucket), remote_path if remote_path else '')))
 
 
 def upload(bucket=None, local_path=None, remote_path=None):
     """Upload a file or folder to an AWS S3 bucket."""
-    S3(str(bucket), quiet=False).upload(local_path=local_path, remote_path=remote_path)
+    return S3(str(bucket), quiet=False).upload(local_path=local_path, remote_path=remote_path)
 
 
 def download(bucket=None, local_path=None, remote_path=None, recursive=False):
     """Download a file or folder to an AWS S3 bucket."""
-    S3(str(bucket), quiet=False).download(local_path=local_path, remote_path=remote_path, recursive=recursive)
+    return S3(str(bucket), quiet=False).download(local_path=local_path, remote_path=remote_path, recursive=recursive)
 
 
 def sync(bucket=None, local_path=None, remote_path=None, delete=False, remote_source=False):
     """Sync files or folders to an AWS S3 bucket."""
-    S3(str(bucket), quiet=False).sync(local_path=local_path, remote_path=remote_path, delete=delete,
-                                      remote_source=remote_source)
+    return S3(str(bucket), quiet=False).sync(local_path=local_path, remote_path=remote_path, delete=delete,
+                                             remote_source=remote_source)
 
 
 def main():
     # Declare argparse argument descriptions
     usage = 'AWS S3 command-line-interface wrapper.'
     description = 'Execute AWS S3 commands.'
     helpers = {
```

### Comparing `awsutils-s3-0.4.1/awsutils/s3/commands.py` & `awsutils-s3-1.0.0/awsutils/s3/commands.py`

 * *Files identical despite different names*

### Comparing `awsutils-s3-0.4.1/awsutils/s3/s3.py` & `awsutils-s3-1.0.0/awsutils/s3/s3.py`

 * *Files identical despite different names*

### Comparing `awsutils-s3-0.4.1/awsutils/s3/url.py` & `awsutils-s3-1.0.0/awsutils/s3/url.py`

 * *Files identical despite different names*

### Comparing `awsutils-s3-0.4.1/setup.py` & `awsutils-s3-1.0.0/setup.py`

 * *Files identical despite different names*

