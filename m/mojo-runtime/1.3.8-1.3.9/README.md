# Comparing `tmp/mojo_runtime-1.3.8.tar.gz` & `tmp/mojo_runtime-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_runtime-1.3.8.tar", max compression
+gzip compressed data, was "mojo_runtime-1.3.9.tar", max compression
```

## Comparing `mojo_runtime-1.3.8.tar` & `mojo_runtime-1.3.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1083 2024-01-26 02:57:39.556318 mojo_runtime-1.3.8/LICENSE.txt
--rw-r--r--   0        0        0      121 2024-01-26 02:57:39.556444 mojo_runtime-1.3.8/README.md
--rw-r--r--   0        0        0      974 2024-03-08 14:09:58.566476 mojo_runtime-1.3.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-26 02:57:39.558145 mojo_runtime-1.3.8/source/packages/mojo/runtime/__init__.py
--rw-r--r--   0        0        0    13923 2024-01-26 02:57:39.558277 mojo_runtime-1.3.8/source/packages/mojo/runtime/activation.py
--rw-r--r--   0        0        0      816 2024-01-26 02:57:39.558430 mojo_runtime-1.3.8/source/packages/mojo/runtime/enumerations.py
--rw-r--r--   0        0        0     2134 2024-03-08 13:43:59.916182 mojo_runtime-1.3.8/source/packages/mojo/runtime/initialize.py
--rw-r--r--   0        0        0     1716 2024-01-26 02:57:39.558597 mojo_runtime-1.3.8/source/packages/mojo/runtime/integration.py
--rw-r--r--   0        0        0    10279 2024-01-26 02:57:39.558708 mojo_runtime-1.3.8/source/packages/mojo/runtime/optionoverrides.py
--rw-r--r--   0        0        0    10871 2024-02-17 00:04:03.773699 mojo_runtime-1.3.8/source/packages/mojo/runtime/paths.py
--rw-r--r--   0        0        0     1705 2024-03-08 14:09:48.553782 mojo_runtime-1.3.8/source/packages/mojo/runtime/runtimesettings.py
--rw-r--r--   0        0        0     2149 2024-01-26 02:57:39.558893 mojo_runtime-1.3.8/source/packages/mojo/runtime/variablenames.py
--rw-r--r--   0        0        0    11195 2024-03-08 13:39:40.711511 mojo_runtime-1.3.8/source/packages/mojo/runtime/variables.py
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 mojo_runtime-1.3.8/setup.py
--rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 mojo_runtime-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-26 02:57:39.556318 mojo_runtime-1.3.9/LICENSE.txt
+-rw-r--r--   0        0        0      121 2024-01-26 02:57:39.556444 mojo_runtime-1.3.9/README.md
+-rw-r--r--   0        0        0      974 2024-03-08 14:17:30.966373 mojo_runtime-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-26 02:57:39.558145 mojo_runtime-1.3.9/source/packages/mojo/runtime/__init__.py
+-rw-r--r--   0        0        0    13923 2024-01-26 02:57:39.558277 mojo_runtime-1.3.9/source/packages/mojo/runtime/activation.py
+-rw-r--r--   0        0        0      816 2024-01-26 02:57:39.558430 mojo_runtime-1.3.9/source/packages/mojo/runtime/enumerations.py
+-rw-r--r--   0        0        0     2128 2024-03-08 14:17:23.339504 mojo_runtime-1.3.9/source/packages/mojo/runtime/initialize.py
+-rw-r--r--   0        0        0     1716 2024-01-26 02:57:39.558597 mojo_runtime-1.3.9/source/packages/mojo/runtime/integration.py
+-rw-r--r--   0        0        0    10279 2024-01-26 02:57:39.558708 mojo_runtime-1.3.9/source/packages/mojo/runtime/optionoverrides.py
+-rw-r--r--   0        0        0    10871 2024-02-17 00:04:03.773699 mojo_runtime-1.3.9/source/packages/mojo/runtime/paths.py
+-rw-r--r--   0        0        0     1705 2024-03-08 14:09:48.553782 mojo_runtime-1.3.9/source/packages/mojo/runtime/runtimesettings.py
+-rw-r--r--   0        0        0     2149 2024-01-26 02:57:39.558893 mojo_runtime-1.3.9/source/packages/mojo/runtime/variablenames.py
+-rw-r--r--   0        0        0    11195 2024-03-08 13:39:40.711511 mojo_runtime-1.3.9/source/packages/mojo/runtime/variables.py
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 mojo_runtime-1.3.9/setup.py
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 mojo_runtime-1.3.9/PKG-INFO
```

### Comparing `mojo_runtime-1.3.8/LICENSE.txt` & `mojo_runtime-1.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_runtime-1.3.8/pyproject.toml` & `mojo_runtime-1.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mojo-runtime"
 description = "Automation Mojo Runtime Module (mojo-runtime)"
-version = "1.3.8"
+version = "1.3.9"
 authors = [
     "Myron Walker <myron.walker@gmail.com>"
 ]
 readme = "README.md"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `mojo_runtime-1.3.8/source/packages/mojo/runtime/activation.py` & `mojo_runtime-1.3.9/source/packages/mojo/runtime/activation.py`

 * *Files identical despite different names*

### Comparing `mojo_runtime-1.3.8/source/packages/mojo/runtime/enumerations.py` & `mojo_runtime-1.3.9/source/packages/mojo/runtime/enumerations.py`

 * *Files identical despite different names*

### Comparing `mojo_runtime-1.3.8/source/packages/mojo/runtime/initialize.py` & `mojo_runtime-1.3.9/source/packages/mojo/runtime/initialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     # enter into an automation process, whether via a test runner, terminal, or debugging a single
     # file that we properly parse arguments and settings and launch the automation process
     # consistently.
     
 
     MOJO_RUNTIME_STATE.INITIALIZED = True
 
-    establish_runtime_settings(name=name, home_directory=home_dir, logger_name=logger_name, default_configuration=default_configuration, service_name=service_name)
+    establish_runtime_settings(name=name, home_dir=home_dir, logger_name=logger_name, default_configuration=default_configuration, service_name=service_name)
     
     from mojo.runtime.variables import resolve_runtime_variables
 
     # The runtime variables can tell us where to find extensions, so we must resolve the runtime
     # varaibles before attempting to resolve any extension factories.
     resolve_runtime_variables()
```

### Comparing `mojo_runtime-1.3.8/source/packages/mojo/runtime/integration.py` & `mojo_runtime-1.3.9/source/packages/mojo/runtime/integration.py`

 * *Files identical despite different names*

### Comparing `mojo_runtime-1.3.8/source/packages/mojo/runtime/optionoverrides.py` & `mojo_runtime-1.3.9/source/packages/mojo/runtime/optionoverrides.py`

 * *Files identical despite different names*

### Comparing `mojo_runtime-1.3.8/source/packages/mojo/runtime/paths.py` & `mojo_runtime-1.3.9/source/packages/mojo/runtime/paths.py`

 * *Files identical despite different names*

### Comparing `mojo_runtime-1.3.8/source/packages/mojo/runtime/runtimesettings.py` & `mojo_runtime-1.3.9/source/packages/mojo/runtime/runtimesettings.py`

 * *Files identical despite different names*

### Comparing `mojo_runtime-1.3.8/source/packages/mojo/runtime/variablenames.py` & `mojo_runtime-1.3.9/source/packages/mojo/runtime/variablenames.py`

 * *Files identical despite different names*

### Comparing `mojo_runtime-1.3.8/source/packages/mojo/runtime/variables.py` & `mojo_runtime-1.3.9/source/packages/mojo/runtime/variables.py`

 * *Files identical despite different names*

### Comparing `mojo_runtime-1.3.8/setup.py` & `mojo_runtime-1.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'mojo-config>=1.3.10,<1.4.0',
  'mojo-errors>=1.3.0,<1.4.0',
  'mojo-extension>=1.3.12,<1.4.0',
  'mojo-xmodules>=1.3.0,<1.4.0']
 
 setup_kwargs = {
     'name': 'mojo-runtime',
-    'version': '1.3.8',
+    'version': '1.3.9',
     'description': 'Automation Mojo Runtime Module (mojo-runtime)',
     'long_description': '# Contextualize\nA package used to create a global context that allows for the distribution of options and configuration.\n',
     'author': 'Myron Walker',
     'author_email': 'myron.walker@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'http://automationmojo.com',
```

### Comparing `mojo_runtime-1.3.8/PKG-INFO` & `mojo_runtime-1.3.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mojo-runtime
-Version: 1.3.8
+Version: 1.3.9
 Summary: Automation Mojo Runtime Module (mojo-runtime)
 Home-page: http://automationmojo.com
 License: LICENSE.txt
 Keywords: python
 Author: Myron Walker
 Author-email: myron.walker@gmail.com
 Requires-Python: >=3.8,<4.0
```

