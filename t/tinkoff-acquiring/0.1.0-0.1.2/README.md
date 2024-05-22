# Comparing `tmp/tinkoff_acquiring-0.1.0.tar.gz` & `tmp/tinkoff_acquiring-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinkoff_acquiring-0.1.0.tar", last modified: Tue May 21 21:12:10 2024, max compression
+gzip compressed data, was "tinkoff_acquiring-0.1.2.tar", last modified: Tue May 21 21:32:03 2024, max compression
```

## Comparing `tinkoff_acquiring-0.1.0.tar` & `tinkoff_acquiring-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:12:10.067566 tinkoff_acquiring-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-21 21:12:03.000000 tinkoff_acquiring-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-21 21:12:03.000000 tinkoff_acquiring-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-21 21:12:10.063566 tinkoff_acquiring-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-21 21:12:03.000000 tinkoff_acquiring-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 21:12:10.067566 tinkoff_acquiring-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-21 21:12:03.000000 tinkoff_acquiring-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:12:10.063566 tinkoff_acquiring-0.1.0/tinkoff_acquiring/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-21 21:12:03.000000 tinkoff_acquiring-0.1.0/tinkoff_acquiring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-21 21:12:03.000000 tinkoff_acquiring-0.1.0/tinkoff_acquiring/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:12:10.063566 tinkoff_acquiring-0.1.0/tinkoff_acquiring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-21 21:12:10.000000 tinkoff_acquiring-0.1.0/tinkoff_acquiring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-21 21:12:10.000000 tinkoff_acquiring-0.1.0/tinkoff_acquiring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 21:12:10.000000 tinkoff_acquiring-0.1.0/tinkoff_acquiring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 21:12:10.000000 tinkoff_acquiring-0.1.0/tinkoff_acquiring.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 21:12:10.000000 tinkoff_acquiring-0.1.0/tinkoff_acquiring.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:32:03.866172 tinkoff_acquiring-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-21 21:31:56.000000 tinkoff_acquiring-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-21 21:31:56.000000 tinkoff_acquiring-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-21 21:32:03.866172 tinkoff_acquiring-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-21 21:31:56.000000 tinkoff_acquiring-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 21:32:03.866172 tinkoff_acquiring-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-21 21:31:56.000000 tinkoff_acquiring-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:32:03.866172 tinkoff_acquiring-0.1.2/tinkoff_acquiring/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-21 21:31:56.000000 tinkoff_acquiring-0.1.2/tinkoff_acquiring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-21 21:31:56.000000 tinkoff_acquiring-0.1.2/tinkoff_acquiring/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:32:03.866172 tinkoff_acquiring-0.1.2/tinkoff_acquiring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-21 21:32:03.000000 tinkoff_acquiring-0.1.2/tinkoff_acquiring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-21 21:32:03.000000 tinkoff_acquiring-0.1.2/tinkoff_acquiring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 21:32:03.000000 tinkoff_acquiring-0.1.2/tinkoff_acquiring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 21:32:03.000000 tinkoff_acquiring-0.1.2/tinkoff_acquiring.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 21:32:03.000000 tinkoff_acquiring-0.1.2/tinkoff_acquiring.egg-info/top_level.txt
```

### Comparing `tinkoff_acquiring-0.1.0/LICENSE` & `tinkoff_acquiring-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tinkoff_acquiring-0.1.0/PKG-INFO` & `tinkoff_acquiring-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinkoff_acquiring
-Version: 0.1.0
+Version: 0.1.2
 Summary: A Python client for Tinkoff Acquiring API
 Home-page: https://github.com/sm1ky/tinkoff_acquiring
 Author: Artem
 Author-email: support@sm1ky.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,7 +23,9 @@
 ```
 
 Use python version >= 3.10
 
 Contant with me - support@sm1ky.com or t.me/sm1ky
 
 I will be very grateful to your star for this repository <3
+
+Project on PyPi - https://pypi.org/project/tinkoff-acquiring/
```

### Comparing `tinkoff_acquiring-0.1.0/setup.py` & `tinkoff_acquiring-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tinkoff_acquiring",
-    version="0.1.0",
+    version="0.1.2",
     packages=find_packages(),
     install_requires=[
         "aiohttp",
     ],
     author="Artem",
     author_email="support@sm1ky.com",
     description="A Python client for Tinkoff Acquiring API",
```

### Comparing `tinkoff_acquiring-0.1.0/tinkoff_acquiring/client.py` & `tinkoff_acquiring-0.1.2/tinkoff_acquiring/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,17 +35,18 @@
                 del params[key]
 
         params['Password'] = self.secret
         sorted_params = sorted(params.items())
         token_str = ''.join(str(value) for _, value in sorted_params)
         return hashlib.sha256(token_str.encode('utf-8')).hexdigest()
 
-    async def init_payment(self, amount, order_id, description, receipt=None, success_url: str = None, fail_url: str = None):
+    async def init_payment(self, amount: float, order_id: any, description: any, receipt=None, success_url: str = None, fail_url: str = None):
+        # Tinkoff API expects amount in kopecks, hence multiplying by 100
         params = {
-            'Amount': int(amount),
+            'Amount': int(amount * 100),  # Ensure the amount is an integer
             'OrderId': order_id,
             'Description': description,
         }
         if success_url:
             params['SuccessURL'] = success_url
         if fail_url:
             params['FailURL'] = fail_url
```

### Comparing `tinkoff_acquiring-0.1.0/tinkoff_acquiring.egg-info/PKG-INFO` & `tinkoff_acquiring-0.1.2/tinkoff_acquiring.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinkoff-acquiring
-Version: 0.1.0
+Version: 0.1.2
 Summary: A Python client for Tinkoff Acquiring API
 Home-page: https://github.com/sm1ky/tinkoff_acquiring
 Author: Artem
 Author-email: support@sm1ky.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,7 +23,9 @@
 ```
 
 Use python version >= 3.10
 
 Contant with me - support@sm1ky.com or t.me/sm1ky
 
 I will be very grateful to your star for this repository <3
+
+Project on PyPi - https://pypi.org/project/tinkoff-acquiring/
```

