# Comparing `tmp/transpara_sdk-0.29.0.tar.gz` & `tmp/transpara_sdk-0.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transpara_sdk-0.29.0.tar", last modified: Wed Apr 24 21:07:54 2024, max compression
+gzip compressed data, was "transpara_sdk-0.30.0.tar", last modified: Wed May 22 18:04:40 2024, max compression
```

## Comparing `transpara_sdk-0.29.0.tar` & `transpara_sdk-0.30.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 21:07:54.908192 transpara_sdk-0.29.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2024-01-17 13:58:36.000000 transpara_sdk-0.29.0/LICENSE.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      480 2024-04-24 21:07:54.908192 transpara_sdk-0.29.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2175 2023-09-25 15:54:29.000000 transpara_sdk-0.29.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      693 2024-04-24 21:07:34.000000 transpara_sdk-0.29.0/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-24 21:07:54.908192 transpara_sdk-0.29.0/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 21:07:54.908192 transpara_sdk-0.29.0/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 21:07:54.908192 transpara_sdk-0.29.0/src/transpara/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-09-25 15:54:29.000000 transpara_sdk-0.29.0/src/transpara/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 21:07:54.908192 transpara_sdk-0.29.0/src/transpara/internal/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3439 2024-04-24 21:07:21.000000 transpara_sdk-0.29.0/src/transpara/internal/settings.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2755 2023-09-25 15:54:29.000000 transpara_sdk-0.29.0/src/transpara/logging_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14487 2023-09-25 15:54:29.000000 transpara_sdk-0.29.0/src/transpara/tlogging.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6838 2023-09-25 15:54:29.000000 transpara_sdk-0.29.0/src/transpara/tracing.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 21:07:54.908192 transpara_sdk-0.29.0/src/transpara_sdk.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      480 2024-04-24 21:07:54.000000 transpara_sdk-0.29.0/src/transpara_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      399 2024-04-24 21:07:54.000000 transpara_sdk-0.29.0/src/transpara_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-24 21:07:54.000000 transpara_sdk-0.29.0/src/transpara_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2024-04-24 21:07:54.000000 transpara_sdk-0.29.0/src/transpara_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2024-04-24 21:07:54.000000 transpara_sdk-0.29.0/src/transpara_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 21:07:54.908192 transpara_sdk-0.29.0/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1036 2023-09-25 17:41:05.000000 transpara_sdk-0.29.0/tests/tests.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:04:40.873037 transpara_sdk-0.30.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2024-01-17 13:58:36.000000 transpara_sdk-0.30.0/LICENSE.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      665 2024-05-22 18:04:40.873037 transpara_sdk-0.30.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2175 2023-09-25 15:54:29.000000 transpara_sdk-0.30.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      830 2024-05-21 18:28:29.000000 transpara_sdk-0.30.0/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-22 18:04:40.873037 transpara_sdk-0.30.0/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:04:40.869037 transpara_sdk-0.30.0/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:04:40.869037 transpara_sdk-0.30.0/src/transpara/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-09-25 15:54:29.000000 transpara_sdk-0.30.0/src/transpara/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:04:40.869037 transpara_sdk-0.30.0/src/transpara/internal/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:04:40.869037 transpara_sdk-0.30.0/src/transpara/internal/extra-hooks/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      124 2024-05-21 18:17:29.000000 transpara_sdk-0.30.0/src/transpara/internal/extra-hooks/hook-opentelemetry.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10128 2024-05-22 18:04:23.000000 transpara_sdk-0.30.0/src/transpara/internal/output_tstore.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4555 2024-05-22 18:02:58.000000 transpara_sdk-0.30.0/src/transpara/internal/settings.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2755 2023-09-25 15:54:29.000000 transpara_sdk-0.30.0/src/transpara/logging_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14487 2023-09-25 15:54:29.000000 transpara_sdk-0.30.0/src/transpara/tlogging.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6838 2023-09-25 15:54:29.000000 transpara_sdk-0.30.0/src/transpara/tracing.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:04:40.869037 transpara_sdk-0.30.0/src/transpara_sdk.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      665 2024-05-22 18:04:40.000000 transpara_sdk-0.30.0/src/transpara_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      496 2024-05-22 18:04:40.000000 transpara_sdk-0.30.0/src/transpara_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-22 18:04:40.000000 transpara_sdk-0.30.0/src/transpara_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      296 2024-05-22 18:04:40.000000 transpara_sdk-0.30.0/src/transpara_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2024-05-22 18:04:40.000000 transpara_sdk-0.30.0/src/transpara_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:04:40.869037 transpara_sdk-0.30.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1036 2023-09-25 17:41:05.000000 transpara_sdk-0.30.0/tests/tests.py
```

### Comparing `transpara_sdk-0.29.0/LICENSE.txt` & `transpara_sdk-0.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.29.0/README.md` & `transpara_sdk-0.30.0/README.md`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.29.0/pyproject.toml` & `transpara_sdk-0.30.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 [metadata]
 author = "Transpara"
 author_email = "arturo.aguilar@transpara.com"
 
 [project]
 name = "transpara-sdk"
-version = "0.29.0"
+version = "0.30.0"
 description = "Transpara Python SDK"
 dependencies = [
     "jsonpickle==1.4.2",
     "asyncio==3.4.3",
     "opentelemetry-api==1.20.0",
     "opentelemetry-sdk==1.20.0",
     "opentelemetry-exporter-otlp==1.20.0",
     "opentelemetry-exporter-otlp-proto-http==1.20.0",
     "pydantic==2.7.0",
-    "requests==2.26.0"
+    "requests==2.26.0",
+    "pytest-dotenv>=0.5.2",
+    "httpx>=0.25.1",
+    "tenacity>=8.2.2",
+    "asyncio>=3.4.3",
+    "pendulum>=2.1.2",
+    "pytz>=2022.6"
 ]
 
 [project.urls]
 homepage = "https://transpara.com"
 
 [options]
 package_dir = "src"
```

### Comparing `transpara_sdk-0.29.0/src/transpara/logging_config.py` & `transpara_sdk-0.30.0/src/transpara/logging_config.py`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.29.0/src/transpara/tlogging.py` & `transpara_sdk-0.30.0/src/transpara/tlogging.py`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.29.0/src/transpara/tracing.py` & `transpara_sdk-0.30.0/src/transpara/tracing.py`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.29.0/tests/tests.py` & `transpara_sdk-0.30.0/tests/tests.py`

 * *Files identical despite different names*

