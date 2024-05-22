# Comparing `tmp/pgos-cli-python-sdk-v1-0.2.9.110.tar.gz` & `tmp/pgos-cli-python-sdk-v1-0.2.9.111.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgos-cli-python-sdk-v1-0.2.9.110.tar", last modified: Mon Jan  8 07:15:28 2024, max compression
+gzip compressed data, was "pgos-cli-python-sdk-v1-0.2.9.111.tar", last modified: Mon Jan  8 07:20:10 2024, max compression
```

## Comparing `pgos-cli-python-sdk-v1-0.2.9.110.tar` & `pgos-cli-python-sdk-v1-0.2.9.111.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 yilungao   (501) staff       (20)        0 2024-01-08 07:15:28.587205 pgos-cli-python-sdk-v1-0.2.9.110/
--rw-r--r--   0 yilungao   (501) staff       (20)        0 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.110/LICENSE
--rw-r--r--   0 yilungao   (501) staff       (20)      777 2024-01-08 07:15:28.586917 pgos-cli-python-sdk-v1-0.2.9.110/PKG-INFO
--rw-r--r--   0 yilungao   (501) staff       (20)      288 2023-12-15 09:07:56.000000 pgos-cli-python-sdk-v1-0.2.9.110/README.md
--rw-r--r--   0 yilungao   (501) staff       (20)      599 2024-01-08 07:15:22.000000 pgos-cli-python-sdk-v1-0.2.9.110/pyproject.toml
--rw-r--r--   0 yilungao   (501) staff       (20)       38 2024-01-08 07:15:28.587261 pgos-cli-python-sdk-v1-0.2.9.110/setup.cfg
-drwxr-xr-x   0 yilungao   (501) staff       (20)        0 2024-01-08 07:15:28.576606 pgos-cli-python-sdk-v1-0.2.9.110/src/
-drwxr-xr-x   0 yilungao   (501) staff       (20)        0 2024-01-08 07:15:28.585165 pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli/
--rw-r--r--   0 yilungao   (501) staff       (20)       74 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli/__init__.py
--rw-r--r--   0 yilungao   (501) staff       (20)     1905 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli/pgos_asset_uploader.py
--rw-r--r--   0 yilungao   (501) staff       (20)     6216 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli/pgos_backend_apis.py
--rw-r--r--   0 yilungao   (501) staff       (20)     3650 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli/pgos_cli_client.py
--rw-r--r--   0 yilungao   (501) staff       (20)     4469 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli/pgos_cli_config.py
--rw-r--r--   0 yilungao   (501) staff       (20)     5742 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli/pgos_cmdline.py
--rw-r--r--   0 yilungao   (501) staff       (20)     1619 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli/pgos_tools.py
--rw-r--r--   0 yilungao   (501) staff       (20)     8972 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli/pgos_uploader_impl_cos.py
--rw-r--r--   0 yilungao   (501) staff       (20)     4935 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli/pgos_uploader_impl_s3.py
--rw-r--r--   0 yilungao   (501) staff       (20)     1296 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli/win32_unicode_argv.py
-drwxr-xr-x   0 yilungao   (501) staff       (20)        0 2024-01-08 07:15:28.586575 pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli_python_sdk_v1.egg-info/
--rw-r--r--   0 yilungao   (501) staff       (20)      777 2024-01-08 07:15:28.000000 pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli_python_sdk_v1.egg-info/PKG-INFO
--rw-r--r--   0 yilungao   (501) staff       (20)      622 2024-01-08 07:15:28.000000 pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli_python_sdk_v1.egg-info/SOURCES.txt
--rw-r--r--   0 yilungao   (501) staff       (20)        1 2024-01-08 07:15:28.000000 pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli_python_sdk_v1.egg-info/dependency_links.txt
--rw-r--r--   0 yilungao   (501) staff       (20)       24 2024-01-08 07:15:28.000000 pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli_python_sdk_v1.egg-info/requires.txt
--rw-r--r--   0 yilungao   (501) staff       (20)        9 2024-01-08 07:15:28.000000 pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli_python_sdk_v1.egg-info/top_level.txt
-drwxr-xr-x   0 yilungao   (501) staff       (20)        0 2024-01-08 07:15:28.586148 pgos-cli-python-sdk-v1-0.2.9.110/tests/
--rw-r--r--   0 yilungao   (501) staff       (20)     3558 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.110/tests/test.py
+drwxr-xr-x   0 yilungao   (501) staff       (20)        0 2024-01-08 07:20:10.963499 pgos-cli-python-sdk-v1-0.2.9.111/
+-rw-r--r--   0 yilungao   (501) staff       (20)        0 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.111/LICENSE
+-rw-r--r--   0 yilungao   (501) staff       (20)      777 2024-01-08 07:20:10.963263 pgos-cli-python-sdk-v1-0.2.9.111/PKG-INFO
+-rw-r--r--   0 yilungao   (501) staff       (20)      288 2023-12-15 09:07:56.000000 pgos-cli-python-sdk-v1-0.2.9.111/README.md
+-rw-r--r--   0 yilungao   (501) staff       (20)      599 2024-01-08 07:20:04.000000 pgos-cli-python-sdk-v1-0.2.9.111/pyproject.toml
+-rw-r--r--   0 yilungao   (501) staff       (20)       38 2024-01-08 07:20:10.963548 pgos-cli-python-sdk-v1-0.2.9.111/setup.cfg
+drwxr-xr-x   0 yilungao   (501) staff       (20)        0 2024-01-08 07:20:10.958613 pgos-cli-python-sdk-v1-0.2.9.111/src/
+drwxr-xr-x   0 yilungao   (501) staff       (20)        0 2024-01-08 07:20:10.961845 pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli/
+-rw-r--r--   0 yilungao   (501) staff       (20)       74 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli/__init__.py
+-rw-r--r--   0 yilungao   (501) staff       (20)     1905 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli/pgos_asset_uploader.py
+-rw-r--r--   0 yilungao   (501) staff       (20)     6216 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli/pgos_backend_apis.py
+-rw-r--r--   0 yilungao   (501) staff       (20)     3650 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli/pgos_cli_client.py
+-rw-r--r--   0 yilungao   (501) staff       (20)     4469 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli/pgos_cli_config.py
+-rw-r--r--   0 yilungao   (501) staff       (20)     5742 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli/pgos_cmdline.py
+-rw-r--r--   0 yilungao   (501) staff       (20)     1619 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli/pgos_tools.py
+-rw-r--r--   0 yilungao   (501) staff       (20)     8972 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli/pgos_uploader_impl_cos.py
+-rw-r--r--   0 yilungao   (501) staff       (20)     4935 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli/pgos_uploader_impl_s3.py
+-rw-r--r--   0 yilungao   (501) staff       (20)     1296 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli/win32_unicode_argv.py
+drwxr-xr-x   0 yilungao   (501) staff       (20)        0 2024-01-08 07:20:10.962988 pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli_python_sdk_v1.egg-info/
+-rw-r--r--   0 yilungao   (501) staff       (20)      777 2024-01-08 07:20:10.000000 pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli_python_sdk_v1.egg-info/PKG-INFO
+-rw-r--r--   0 yilungao   (501) staff       (20)      622 2024-01-08 07:20:10.000000 pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli_python_sdk_v1.egg-info/SOURCES.txt
+-rw-r--r--   0 yilungao   (501) staff       (20)        1 2024-01-08 07:20:10.000000 pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli_python_sdk_v1.egg-info/dependency_links.txt
+-rw-r--r--   0 yilungao   (501) staff       (20)       24 2024-01-08 07:20:10.000000 pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli_python_sdk_v1.egg-info/requires.txt
+-rw-r--r--   0 yilungao   (501) staff       (20)        9 2024-01-08 07:20:10.000000 pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli_python_sdk_v1.egg-info/top_level.txt
+drwxr-xr-x   0 yilungao   (501) staff       (20)        0 2024-01-08 07:20:10.962731 pgos-cli-python-sdk-v1-0.2.9.111/tests/
+-rw-r--r--   0 yilungao   (501) staff       (20)     3558 2024-01-08 06:51:18.000000 pgos-cli-python-sdk-v1-0.2.9.111/tests/test.py
```

### Comparing `pgos-cli-python-sdk-v1-0.2.9.110/PKG-INFO` & `pgos-cli-python-sdk-v1-0.2.9.111/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgos-cli-python-sdk-v1
-Version: 0.2.9.110
+Version: 0.2.9.111
 Summary: PGOS commandline interface
 Author-email: yilungao <yilungao@tencent.com>
 Project-URL: Homepage, https://pgos.intlgame.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `pgos-cli-python-sdk-v1-0.2.9.110/pyproject.toml` & `pgos-cli-python-sdk-v1-0.2.9.111/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "boto3", "cos-python-sdk-v5"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pgos-cli-python-sdk-v1"
-version = "0.2.9.110"
+version = "0.2.9.111"
 
 authors = [
   { name="yilungao", email="yilungao@tencent.com" },
 ]
 description = "PGOS commandline interface"
 
 readme = "README.md"
```

### Comparing `pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli/pgos_asset_uploader.py` & `pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli/pgos_asset_uploader.py`

 * *Files identical despite different names*

### Comparing `pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli/pgos_backend_apis.py` & `pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli/pgos_backend_apis.py`

 * *Files identical despite different names*

### Comparing `pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli/pgos_cli_client.py` & `pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli/pgos_cli_client.py`

 * *Files identical despite different names*

### Comparing `pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli/pgos_cli_config.py` & `pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli/pgos_cli_config.py`

 * *Files identical despite different names*

### Comparing `pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli/pgos_cmdline.py` & `pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli/pgos_cmdline.py`

 * *Files identical despite different names*

### Comparing `pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli/pgos_tools.py` & `pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli/pgos_tools.py`

 * *Files identical despite different names*

### Comparing `pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli/pgos_uploader_impl_cos.py` & `pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli/pgos_uploader_impl_cos.py`

 * *Files identical despite different names*

### Comparing `pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli/pgos_uploader_impl_s3.py` & `pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli/pgos_uploader_impl_s3.py`

 * *Files identical despite different names*

### Comparing `pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli/win32_unicode_argv.py` & `pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli/win32_unicode_argv.py`

 * *Files identical despite different names*

### Comparing `pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli_python_sdk_v1.egg-info/PKG-INFO` & `pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli_python_sdk_v1.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgos-cli-python-sdk-v1
-Version: 0.2.9.110
+Version: 0.2.9.111
 Summary: PGOS commandline interface
 Author-email: yilungao <yilungao@tencent.com>
 Project-URL: Homepage, https://pgos.intlgame.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `pgos-cli-python-sdk-v1-0.2.9.110/src/pgos_cli_python_sdk_v1.egg-info/SOURCES.txt` & `pgos-cli-python-sdk-v1-0.2.9.111/src/pgos_cli_python_sdk_v1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pgos-cli-python-sdk-v1-0.2.9.110/tests/test.py` & `pgos-cli-python-sdk-v1-0.2.9.111/tests/test.py`

 * *Files identical despite different names*

