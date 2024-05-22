# Comparing `tmp/opentelemetry_instrumentation_milvus-0.18.2.tar.gz` & `tmp/opentelemetry_instrumentation_milvus-0.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_instrumentation_milvus-0.18.2.tar", max compression
+gzip compressed data, was "opentelemetry_instrumentation_milvus-0.19.0.tar", max compression
```

## Comparing `opentelemetry_instrumentation_milvus-0.18.2.tar` & `opentelemetry_instrumentation_milvus-0.19.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      561 2024-05-20 10:47:22.941740 opentelemetry_instrumentation_milvus-0.18.2/README.md
--rw-r--r--   0        0        0     2750 2024-05-20 10:44:16.559836 opentelemetry_instrumentation_milvus-0.18.2/opentelemetry/instrumentation/milvus/__init__.py
--rw-r--r--   0        0        0       42 2024-05-20 10:44:16.560078 opentelemetry_instrumentation_milvus-0.18.2/opentelemetry/instrumentation/milvus/config.py
--rw-r--r--   0        0        0      699 2024-05-20 10:44:16.560214 opentelemetry_instrumentation_milvus-0.18.2/opentelemetry/instrumentation/milvus/utils.py
--rw-r--r--   0        0        0       23 2024-05-20 10:45:29.672351 opentelemetry_instrumentation_milvus-0.18.2/opentelemetry/instrumentation/milvus/version.py
--rw-r--r--   0        0        0     6793 2024-05-20 10:44:16.560453 opentelemetry_instrumentation_milvus-0.18.2/opentelemetry/instrumentation/milvus/wrapper.py
--rw-r--r--   0        0        0     1389 2024-05-20 10:46:18.201897 opentelemetry_instrumentation_milvus-0.18.2/pyproject.toml
--rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_milvus-0.18.2/PKG-INFO
+-rw-r--r--   0        0        0      561 2024-05-22 14:59:30.703421 opentelemetry_instrumentation_milvus-0.19.0/README.md
+-rw-r--r--   0        0        0     2750 2024-05-22 14:59:30.703421 opentelemetry_instrumentation_milvus-0.19.0/opentelemetry/instrumentation/milvus/__init__.py
+-rw-r--r--   0        0        0       42 2024-05-22 14:59:30.703421 opentelemetry_instrumentation_milvus-0.19.0/opentelemetry/instrumentation/milvus/config.py
+-rw-r--r--   0        0        0      699 2024-05-22 14:59:30.703421 opentelemetry_instrumentation_milvus-0.19.0/opentelemetry/instrumentation/milvus/utils.py
+-rw-r--r--   0        0        0       23 2024-05-22 14:59:30.703421 opentelemetry_instrumentation_milvus-0.19.0/opentelemetry/instrumentation/milvus/version.py
+-rw-r--r--   0        0        0     6793 2024-05-22 14:59:30.703421 opentelemetry_instrumentation_milvus-0.19.0/opentelemetry/instrumentation/milvus/wrapper.py
+-rw-r--r--   0        0        0     1389 2024-05-22 14:59:56.195365 opentelemetry_instrumentation_milvus-0.19.0/pyproject.toml
+-rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_milvus-0.19.0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_milvus-0.18.2/README.md` & `opentelemetry_instrumentation_milvus-0.19.0/README.md`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_milvus-0.18.2/opentelemetry/instrumentation/milvus/__init__.py` & `opentelemetry_instrumentation_milvus-0.19.0/opentelemetry/instrumentation/milvus/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_milvus-0.18.2/opentelemetry/instrumentation/milvus/utils.py` & `opentelemetry_instrumentation_milvus-0.19.0/opentelemetry/instrumentation/milvus/utils.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_milvus-0.18.2/opentelemetry/instrumentation/milvus/wrapper.py` & `opentelemetry_instrumentation_milvus-0.19.0/opentelemetry/instrumentation/milvus/wrapper.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_milvus-0.18.2/pyproject.toml` & `opentelemetry_instrumentation_milvus-0.19.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = ['if TYPE_CHECKING:']
 show_missing = true
 
 [tool.poetry]
 name = "opentelemetry-instrumentation-milvus"
-version = "0.18.2"
+version = "0.19.0"
 description = "OpenTelemetry Milvus instrumentation"
 authors = [
   "Gal Kleinman <gal@traceloop.com>",
   "Nir Gazit <nir@traceloop.com>",
   "Tomer Friedman <tomer@traceloop.com>"
 ]
 repository = "https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-milvus"
```

### Comparing `opentelemetry_instrumentation_milvus-0.18.2/PKG-INFO` & `opentelemetry_instrumentation_milvus-0.19.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-milvus
-Version: 0.18.2
+Version: 0.19.0
 Summary: OpenTelemetry Milvus instrumentation
 Home-page: https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-milvus
 License: Apache-2.0
 Author: Gal Kleinman
 Author-email: gal@traceloop.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: opentelemetry-instrumentation-milvus Version:
-0.18.2 Summary: OpenTelemetry Milvus instrumentation Home-page: https://
+0.19.0 Summary: OpenTelemetry Milvus instrumentation Home-page: https://
 github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-
 instrumentation-milvus License: Apache-2.0 Author: Gal Kleinman Author-email:
 gal@traceloop.com Requires-Python: >=3.9,<4 Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Provides-Extra: instruments
```

