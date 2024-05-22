# Comparing `tmp/kilmlogger-0.0.9.tar.gz` & `tmp/kilmlogger-0.1.0.tar.gz`

## Comparing `kilmlogger-0.0.9.tar` & `kilmlogger-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/.vscode/settings.json
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/__init__.py
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/config.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/constants.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/correlation.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/envs.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/handler.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/processor.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/styles.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/utils.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/services/scribe/client.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/services/scribe/grpc/scribelog.proto
--rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/services/scribe/grpc/scribelog_pb2.py
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/services/scribe/grpc/scribelog_pb2.pyi
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/services/scribe/grpc/scribelog_pb2_grpc.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/README.md
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 kilmlogger-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 kilmlogger-0.1.0/requirements.txt
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 kilmlogger-0.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 kilmlogger-0.1.0/kilmlogger/__init__.py
+-rw-r--r--   0        0        0     7589 2020-02-02 00:00:00.000000 kilmlogger-0.1.0/kilmlogger/config.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 kilmlogger-0.1.0/kilmlogger/constants.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 kilmlogger-0.1.0/kilmlogger/correlation.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 kilmlogger-0.1.0/kilmlogger/envs.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 kilmlogger-0.1.0/kilmlogger/handler.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 kilmlogger-0.1.0/kilmlogger/processor.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 kilmlogger-0.1.0/kilmlogger/styles.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 kilmlogger-0.1.0/kilmlogger/utils.py
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 kilmlogger-0.1.0/kilmlogger/services/scribe/client.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 kilmlogger-0.1.0/kilmlogger/services/scribe/grpc/scribelog.proto
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 kilmlogger-0.1.0/kilmlogger/services/scribe/grpc/scribelog_pb2.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 kilmlogger-0.1.0/kilmlogger/services/scribe/grpc/scribelog_pb2.pyi
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 kilmlogger-0.1.0/kilmlogger/services/scribe/grpc/scribelog_pb2_grpc.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 kilmlogger-0.1.0/.gitignore
+-rw-r--r--   0        0        0     7541 2020-02-02 00:00:00.000000 kilmlogger-0.1.0/README.md
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 kilmlogger-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8630 2020-02-02 00:00:00.000000 kilmlogger-0.1.0/PKG-INFO
```

### Comparing `kilmlogger-0.0.9/kilmlogger/correlation.py` & `kilmlogger-0.1.0/kilmlogger/correlation.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     def __init__(self, app, **kwargs):
         if "header_name" in kwargs:
             self.header_name = kwargs.pop("header_name")
         if "is_required_header" in kwargs:
             self.is_required_header = kwargs.pop("is_required_header")
 
-        super().__init__(app, header_name=self.header_name)
+        super().__init__(app, header_name=self.header_name, **kwargs)
 
     async def __call__(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
         """
         Check header
         """
         # Try to load correlation ID from the request headers
         headers = MutableHeaders(scope=scope)
```

### Comparing `kilmlogger-0.0.9/kilmlogger/processor.py` & `kilmlogger-0.1.0/kilmlogger/processor.py`

 * *Files identical despite different names*

### Comparing `kilmlogger-0.0.9/kilmlogger/styles.py` & `kilmlogger-0.1.0/kilmlogger/styles.py`

 * *Files identical despite different names*

### Comparing `kilmlogger-0.0.9/kilmlogger/services/scribe/grpc/scribelog.proto` & `kilmlogger-0.1.0/kilmlogger/services/scribe/grpc/scribelog.proto`

 * *Files identical despite different names*

### Comparing `kilmlogger-0.0.9/kilmlogger/services/scribe/grpc/scribelog_pb2.py` & `kilmlogger-0.1.0/kilmlogger/services/scribe/grpc/scribelog_pb2.py`

 * *Files identical despite different names*

### Comparing `kilmlogger-0.0.9/kilmlogger/services/scribe/grpc/scribelog_pb2.pyi` & `kilmlogger-0.1.0/kilmlogger/services/scribe/grpc/scribelog_pb2.pyi`

 * *Files identical despite different names*

### Comparing `kilmlogger-0.0.9/kilmlogger/services/scribe/grpc/scribelog_pb2_grpc.py` & `kilmlogger-0.1.0/kilmlogger/services/scribe/grpc/scribelog_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kilmlogger-0.0.9/pyproject.toml` & `kilmlogger-0.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kilmlogger"
 dynamic = ["version"]
-description = "The Python Logger for all ZLB's Project"
+description = "The Python Logger for all KiLM's Project"
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = []
 authors = [
   { name = "vietnh8", email = "vietnh8@vng.com.vn" },
 ]
@@ -18,20 +18,22 @@
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "asgi-correlation-id==4.2.0",
-  "structlog==23.3.0",
-  "starlette==0.32.0",
-  "protobuf==4.25.1",
-  "pydantic-settings==2.1.0",
-  "grpcio==1.60.0",
+  "asgi-correlation-id >=4.2.0, <5.0.0",
+  "structlog >=23.3.0, <24.0.0",
+  "starlette >=0.36.3, <0.37.0",
+  "protobuf >=4.25.1, <5.0.0",
+  "pydantic-settings >=2.1.0, <3.0.0",
+  "grpcio >=1.60.0, <2.0.0",
+  "ujson >=5.9.0, <6.0.0",
+  "pydantic >=2.5.3, <3.0.0",
 ]
 
 [tool.hatch.build.targets.sdist]
 ignore-vcs = true
 
 [project.urls]
 Documentation = "https://github.com/unknown/kilmlogger#readme"
@@ -96,8 +98,8 @@
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
 # Ignore `E402` (import violations) in all `__init__.py` files, and in `path/to/file.py`.
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["E402", "F401"]
 "constants.py" = ["E501"]
-"kilmlogger/services/scribe/grpc/*" = ["E501", "E722", "E712"]
+"kilmlogger/services/scribe/grpc/*" = ["E501", "E722", "E712"]
```

