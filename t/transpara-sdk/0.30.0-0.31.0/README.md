# Comparing `tmp/transpara_sdk-0.30.0.tar.gz` & `tmp/transpara_sdk-0.31.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transpara_sdk-0.30.0.tar", last modified: Wed May 22 18:04:40 2024, max compression
+gzip compressed data, was "transpara_sdk-0.31.0.tar", last modified: Wed May 22 18:16:07 2024, max compression
```

## Comparing `transpara_sdk-0.30.0.tar` & `transpara_sdk-0.31.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:04:40.873037 transpara_sdk-0.30.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2024-01-17 13:58:36.000000 transpara_sdk-0.30.0/LICENSE.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      665 2024-05-22 18:04:40.873037 transpara_sdk-0.30.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2175 2023-09-25 15:54:29.000000 transpara_sdk-0.30.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      830 2024-05-21 18:28:29.000000 transpara_sdk-0.30.0/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-22 18:04:40.873037 transpara_sdk-0.30.0/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:04:40.869037 transpara_sdk-0.30.0/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:04:40.869037 transpara_sdk-0.30.0/src/transpara/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-09-25 15:54:29.000000 transpara_sdk-0.30.0/src/transpara/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:04:40.869037 transpara_sdk-0.30.0/src/transpara/internal/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:04:40.869037 transpara_sdk-0.30.0/src/transpara/internal/extra-hooks/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      124 2024-05-21 18:17:29.000000 transpara_sdk-0.30.0/src/transpara/internal/extra-hooks/hook-opentelemetry.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10128 2024-05-22 18:04:23.000000 transpara_sdk-0.30.0/src/transpara/internal/output_tstore.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4555 2024-05-22 18:02:58.000000 transpara_sdk-0.30.0/src/transpara/internal/settings.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2755 2023-09-25 15:54:29.000000 transpara_sdk-0.30.0/src/transpara/logging_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14487 2023-09-25 15:54:29.000000 transpara_sdk-0.30.0/src/transpara/tlogging.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6838 2023-09-25 15:54:29.000000 transpara_sdk-0.30.0/src/transpara/tracing.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:04:40.869037 transpara_sdk-0.30.0/src/transpara_sdk.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      665 2024-05-22 18:04:40.000000 transpara_sdk-0.30.0/src/transpara_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      496 2024-05-22 18:04:40.000000 transpara_sdk-0.30.0/src/transpara_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-22 18:04:40.000000 transpara_sdk-0.30.0/src/transpara_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      296 2024-05-22 18:04:40.000000 transpara_sdk-0.30.0/src/transpara_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2024-05-22 18:04:40.000000 transpara_sdk-0.30.0/src/transpara_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:04:40.869037 transpara_sdk-0.30.0/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1036 2023-09-25 17:41:05.000000 transpara_sdk-0.30.0/tests/tests.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:16:07.166672 transpara_sdk-0.31.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2024-01-17 13:58:36.000000 transpara_sdk-0.31.0/LICENSE.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      665 2024-05-22 18:16:07.166672 transpara_sdk-0.31.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2175 2023-09-25 15:54:29.000000 transpara_sdk-0.31.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      830 2024-05-22 18:15:54.000000 transpara_sdk-0.31.0/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-22 18:16:07.166672 transpara_sdk-0.31.0/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:16:07.162672 transpara_sdk-0.31.0/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:16:07.162672 transpara_sdk-0.31.0/src/transpara/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-09-25 15:54:29.000000 transpara_sdk-0.31.0/src/transpara/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:16:07.166672 transpara_sdk-0.31.0/src/transpara/internal/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:16:07.166672 transpara_sdk-0.31.0/src/transpara/internal/extra-hooks/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      124 2024-05-21 18:17:29.000000 transpara_sdk-0.31.0/src/transpara/internal/extra-hooks/hook-opentelemetry.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10132 2024-05-22 18:15:38.000000 transpara_sdk-0.31.0/src/transpara/internal/output_tstore.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4555 2024-05-22 18:02:58.000000 transpara_sdk-0.31.0/src/transpara/internal/settings.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2755 2023-09-25 15:54:29.000000 transpara_sdk-0.31.0/src/transpara/logging_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14487 2023-09-25 15:54:29.000000 transpara_sdk-0.31.0/src/transpara/tlogging.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6838 2023-09-25 15:54:29.000000 transpara_sdk-0.31.0/src/transpara/tracing.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:16:07.166672 transpara_sdk-0.31.0/src/transpara_sdk.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      665 2024-05-22 18:16:07.000000 transpara_sdk-0.31.0/src/transpara_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      496 2024-05-22 18:16:07.000000 transpara_sdk-0.31.0/src/transpara_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-22 18:16:07.000000 transpara_sdk-0.31.0/src/transpara_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      296 2024-05-22 18:16:07.000000 transpara_sdk-0.31.0/src/transpara_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2024-05-22 18:16:07.000000 transpara_sdk-0.31.0/src/transpara_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:16:07.166672 transpara_sdk-0.31.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1036 2023-09-25 17:41:05.000000 transpara_sdk-0.31.0/tests/tests.py
```

### Comparing `transpara_sdk-0.30.0/LICENSE.txt` & `transpara_sdk-0.31.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.30.0/PKG-INFO` & `transpara_sdk-0.31.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transpara-sdk
-Version: 0.30.0
+Version: 0.31.0
 Summary: Transpara Python SDK
 Project-URL: homepage, https://transpara.com
 License-File: LICENSE.txt
 Requires-Dist: jsonpickle==1.4.2
 Requires-Dist: asyncio==3.4.3
 Requires-Dist: opentelemetry-api==1.20.0
 Requires-Dist: opentelemetry-sdk==1.20.0
```

### Comparing `transpara_sdk-0.30.0/README.md` & `transpara_sdk-0.31.0/README.md`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.30.0/pyproject.toml` & `transpara_sdk-0.31.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 author = "Transpara"
 author_email = "arturo.aguilar@transpara.com"
 
 [project]
 name = "transpara-sdk"
-version = "0.30.0"
+version = "0.31.0"
 description = "Transpara Python SDK"
 dependencies = [
     "jsonpickle==1.4.2",
     "asyncio==3.4.3",
     "opentelemetry-api==1.20.0",
     "opentelemetry-sdk==1.20.0",
     "opentelemetry-exporter-otlp==1.20.0",
```

### Comparing `transpara_sdk-0.30.0/src/transpara/internal/output_tstore.py` & `transpara_sdk-0.31.0/src/transpara/internal/output_tstore.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,17 +287,17 @@
 #     assert output_tstore.q.qsize() == 5
 
 
 if __name__ == "__main__":
     #test_line()
     if sys.platform == 'win32':
         from dotenv import load_dotenv
-        import os
+        #import os
         asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy()) 
         load_dotenv()
-        script_dir = os.path.dirname(os.path.abspath(__file__))
-        os.chdir(script_dir)
-        print(f"Current working directory: {os.getcwd()}")
+        #script_dir = os.path.dirname(os.path.abspath(__file__))
+        #os.chdir(script_dir)
+        #print(f"Current working directory: {os.getcwd()}")
 
     asyncio.run(run_all())
```

### Comparing `transpara_sdk-0.30.0/src/transpara/internal/settings.py` & `transpara_sdk-0.31.0/src/transpara/internal/settings.py`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.30.0/src/transpara/logging_config.py` & `transpara_sdk-0.31.0/src/transpara/logging_config.py`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.30.0/src/transpara/tlogging.py` & `transpara_sdk-0.31.0/src/transpara/tlogging.py`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.30.0/src/transpara/tracing.py` & `transpara_sdk-0.31.0/src/transpara/tracing.py`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.30.0/src/transpara_sdk.egg-info/PKG-INFO` & `transpara_sdk-0.31.0/src/transpara_sdk.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transpara-sdk
-Version: 0.30.0
+Version: 0.31.0
 Summary: Transpara Python SDK
 Project-URL: homepage, https://transpara.com
 License-File: LICENSE.txt
 Requires-Dist: jsonpickle==1.4.2
 Requires-Dist: asyncio==3.4.3
 Requires-Dist: opentelemetry-api==1.20.0
 Requires-Dist: opentelemetry-sdk==1.20.0
```

### Comparing `transpara_sdk-0.30.0/tests/tests.py` & `transpara_sdk-0.31.0/tests/tests.py`

 * *Files identical despite different names*

