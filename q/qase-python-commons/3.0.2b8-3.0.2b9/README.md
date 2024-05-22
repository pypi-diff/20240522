# Comparing `tmp/qase_python_commons-3.0.2b8.tar.gz` & `tmp/qase_python_commons-3.0.2b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase_python_commons-3.0.2b8.tar", last modified: Mon May 20 09:23:05 2024, max compression
+gzip compressed data, was "qase_python_commons-3.0.2b9.tar", last modified: Wed May 22 13:49:47 2024, max compression
```

## Comparing `qase_python_commons-3.0.2b8.tar` & `qase_python_commons-3.0.2b9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:05.374483 qase_python_commons-3.0.2b8/
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-20 09:23:05.370483 qase_python_commons-3.0.2b8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 09:23:05.374483 qase_python_commons-3.0.2b8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:05.362483 qase_python_commons-3.0.2b8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:05.362483 qase_python_commons-3.0.2b8/src/qase/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:05.366483 qase_python_commons-3.0.2b8/src/qase/commons/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:05.366483 qase_python_commons-3.0.2b8/src/qase/commons/client/
--rw-r--r--   0 runner    (1001) docker     (127)    11038 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/client/api_v1_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/client/api_v2_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/client/base_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:05.366483 qase_python_commons-3.0.2b8/src/qase/commons/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/exceptions/reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:05.366483 qase_python_commons-3.0.2b8/src/qase/commons/models/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/models/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/models/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/models/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/models/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/models/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/models/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/models/step.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/models/suite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:05.370483 qase_python_commons-3.0.2b8/src/qase/commons/profilers/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/profilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/profilers/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/profilers/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/profilers/sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:05.370483 qase_python_commons-3.0.2b8/src/qase/commons/reporters/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/reporters/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/reporters/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/reporters/testops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:05.370483 qase_python_commons-3.0.2b8/src/qase/commons/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/validators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:05.370483 qase_python_commons-3.0.2b8/src/qase_python_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-20 09:23:05.000000 qase_python_commons-3.0.2b8/src/qase_python_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-20 09:23:05.000000 qase_python_commons-3.0.2b8/src/qase_python_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 09:23:05.000000 qase_python_commons-3.0.2b8/src/qase_python_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-20 09:23:05.000000 qase_python_commons-3.0.2b8/src/qase_python_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-20 09:23:05.000000 qase_python_commons-3.0.2b8/src/qase_python_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:49:47.591179 qase_python_commons-3.0.2b9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-22 13:49:47.587179 qase_python_commons-3.0.2b9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:49:47.591179 qase_python_commons-3.0.2b9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:49:47.583179 qase_python_commons-3.0.2b9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:49:47.579179 qase_python_commons-3.0.2b9/src/qase/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:49:47.583179 qase_python_commons-3.0.2b9/src/qase/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:49:47.583179 qase_python_commons-3.0.2b9/src/qase/commons/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    11038 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/client/api_v1_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/client/api_v2_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/client/base_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:49:47.583179 qase_python_commons-3.0.2b9/src/qase/commons/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/exceptions/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:49:47.587179 qase_python_commons-3.0.2b9/src/qase/commons/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/models/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/models/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/models/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/models/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/models/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/models/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/models/suite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:49:47.587179 qase_python_commons-3.0.2b9/src/qase/commons/profilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/profilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/profilers/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/profilers/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/profilers/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:49:47.587179 qase_python_commons-3.0.2b9/src/qase/commons/reporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/reporters/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/reporters/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/reporters/testops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:49:47.587179 qase_python_commons-3.0.2b9/src/qase/commons/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-22 13:49:42.000000 qase_python_commons-3.0.2b9/src/qase/commons/validators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:49:47.587179 qase_python_commons-3.0.2b9/src/qase_python_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-22 13:49:47.000000 qase_python_commons-3.0.2b9/src/qase_python_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-22 13:49:47.000000 qase_python_commons-3.0.2b9/src/qase_python_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:49:47.000000 qase_python_commons-3.0.2b9/src/qase_python_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-22 13:49:47.000000 qase_python_commons-3.0.2b9/src/qase_python_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 13:49:47.000000 qase_python_commons-3.0.2b9/src/qase_python_commons.egg-info/top_level.txt
```

### Comparing `qase_python_commons-3.0.2b8/PKG-INFO` & `qase_python_commons-3.0.2b9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-python-commons
-Version: 3.0.2b8
+Version: 3.0.2b9
 Summary: A library for Qase TestOps and Qase Report
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `qase_python_commons-3.0.2b8/pyproject.toml` & `qase_python_commons-3.0.2b9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qase-python-commons"
-version = "3.0.2b8"
+version = "3.0.2b9"
 description = "A library for Qase TestOps and Qase Report"
 readme = "README.md"
 authors = [{name = "Qase Team", email = "support@qase.io"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
```

### Comparing `qase_python_commons-3.0.2b8/src/qase/commons/client/api_v1_client.py` & `qase_python_commons-3.0.2b9/src/qase/commons/client/api_v1_client.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b8/src/qase/commons/client/api_v2_client.py` & `qase_python_commons-3.0.2b9/src/qase/commons/client/api_v2_client.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b8/src/qase/commons/client/base_api_client.py` & `qase_python_commons-3.0.2b9/src/qase/commons/client/base_api_client.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b8/src/qase/commons/config.py` & `qase_python_commons-3.0.2b9/src/qase/commons/config.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b8/src/qase/commons/loader.py` & `qase_python_commons-3.0.2b9/src/qase/commons/loader.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b8/src/qase/commons/logger.py` & `qase_python_commons-3.0.2b9/src/qase/commons/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,10 +23,10 @@
                 f.write(log)
 
     def log_debug(self, message: str):
         if self.debug:
             self.log(message, 'debug')
 
     @staticmethod
-    def _get_timestamp(format: str = "%Y%m%d_%H:%M:%S"):
+    def _get_timestamp(format: str = "%Y%m%d_%H_%M_%S"):
         now = datetime.datetime.now()
         return now.strftime(format)
```

### Comparing `qase_python_commons-3.0.2b8/src/qase/commons/models/attachment.py` & `qase_python_commons-3.0.2b9/src/qase/commons/models/attachment.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b8/src/qase/commons/models/result.py` & `qase_python_commons-3.0.2b9/src/qase/commons/models/result.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b8/src/qase/commons/models/run.py` & `qase_python_commons-3.0.2b9/src/qase/commons/models/run.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b8/src/qase/commons/models/runtime.py` & `qase_python_commons-3.0.2b9/src/qase/commons/models/runtime.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b8/src/qase/commons/models/step.py` & `qase_python_commons-3.0.2b9/src/qase/commons/models/step.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b8/src/qase/commons/profilers/network.py` & `qase_python_commons-3.0.2b9/src/qase/commons/profilers/network.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b8/src/qase/commons/profilers/sleep.py` & `qase_python_commons-3.0.2b9/src/qase/commons/profilers/sleep.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b8/src/qase/commons/reporters/core.py` & `qase_python_commons-3.0.2b9/src/qase/commons/reporters/core.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b8/src/qase/commons/reporters/report.py` & `qase_python_commons-3.0.2b9/src/qase/commons/reporters/report.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b8/src/qase/commons/reporters/testops.py` & `qase_python_commons-3.0.2b9/src/qase/commons/reporters/testops.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b8/src/qase/commons/utils.py` & `qase_python_commons-3.0.2b9/src/qase/commons/utils.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b8/src/qase_python_commons.egg-info/PKG-INFO` & `qase_python_commons-3.0.2b9/src/qase_python_commons.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-python-commons
-Version: 3.0.2b8
+Version: 3.0.2b9
 Summary: A library for Qase TestOps and Qase Report
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `qase_python_commons-3.0.2b8/src/qase_python_commons.egg-info/SOURCES.txt` & `qase_python_commons-3.0.2b9/src/qase_python_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

