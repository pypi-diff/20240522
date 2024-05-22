# Comparing `tmp/openllm_client-0.5.0a8.tar.gz` & `tmp/openllm_client-0.5.0a9.tar.gz`

## Comparing `openllm_client-0.5.0a8.tar` & `openllm_client-0.5.0a9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 openllm_client-0.5.0a8/README.md
--rw-r--r--   0        0        0     9489 2020-02-02 00:00:00.000000 openllm_client-0.5.0a8/protos/service.proto
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 openllm_client-0.5.0a8/src/openllm_client/__init__.py
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 openllm_client-0.5.0a8/src/openllm_client/__init__.pyi
--rw-r--r--   0        0        0     8016 2020-02-02 00:00:00.000000 openllm_client-0.5.0a8/src/openllm_client/_http.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 openllm_client-0.5.0a8/src/openllm_client/_schemas.py
--rw-r--r--   0        0        0    19482 2020-02-02 00:00:00.000000 openllm_client-0.5.0a8/src/openllm_client/_shim.py
--rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 openllm_client-0.5.0a8/src/openllm_client/_stream.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 openllm_client-0.5.0a8/src/openllm_client/_typing_compat.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 openllm_client-0.5.0a8/src/openllm_client/_utils.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 openllm_client-0.5.0a8/src/openllm_client/_utils.pyi
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 openllm_client-0.5.0a8/src/openllm_client/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm_client-0.5.0a8/src/openllm_client/py.typed
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm_client-0.5.0a8/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm_client-0.5.0a8/LICENSE.md
--rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 openllm_client-0.5.0a8/pyproject.toml
--rw-r--r--   0        0        0     7091 2020-02-02 00:00:00.000000 openllm_client-0.5.0a8/PKG-INFO
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/README.md
+-rw-r--r--   0        0        0     9489 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/protos/service.proto
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/src/openllm_client/__init__.py
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/src/openllm_client/__init__.pyi
+-rw-r--r--   0        0        0     8016 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/src/openllm_client/_http.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/src/openllm_client/_schemas.py
+-rw-r--r--   0        0        0    19482 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/src/openllm_client/_shim.py
+-rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/src/openllm_client/_stream.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/src/openllm_client/_typing_compat.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/src/openllm_client/_utils.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/src/openllm_client/_utils.pyi
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/src/openllm_client/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/src/openllm_client/py.typed
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/LICENSE.md
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/pyproject.toml
+-rw-r--r--   0        0        0     7091 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/PKG-INFO
```

### Comparing `openllm_client-0.5.0a8/README.md` & `openllm_client-0.5.0a9/README.md`

 * *Files identical despite different names*

### Comparing `openllm_client-0.5.0a8/protos/service.proto` & `openllm_client-0.5.0a9/protos/service.proto`

 * *Files identical despite different names*

### Comparing `openllm_client-0.5.0a8/src/openllm_client/__init__.pyi` & `openllm_client-0.5.0a9/src/openllm_client/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm_client-0.5.0a8/src/openllm_client/_http.py` & `openllm_client-0.5.0a9/src/openllm_client/_http.py`

 * *Files identical despite different names*

### Comparing `openllm_client-0.5.0a8/src/openllm_client/_schemas.py` & `openllm_client-0.5.0a9/src/openllm_client/_schemas.py`

 * *Files identical despite different names*

### Comparing `openllm_client-0.5.0a8/src/openllm_client/_shim.py` & `openllm_client-0.5.0a9/src/openllm_client/_shim.py`

 * *Files identical despite different names*

### Comparing `openllm_client-0.5.0a8/src/openllm_client/_stream.py` & `openllm_client-0.5.0a9/src/openllm_client/_stream.py`

 * *Files identical despite different names*

### Comparing `openllm_client-0.5.0a8/src/openllm_client/_typing_compat.py` & `openllm_client-0.5.0a9/src/openllm_client/_typing_compat.py`

 * *Files identical despite different names*

### Comparing `openllm_client-0.5.0a8/src/openllm_client/_utils.pyi` & `openllm_client-0.5.0a9/src/openllm_client/_utils.pyi`

 * *Files identical despite different names*

### Comparing `openllm_client-0.5.0a8/.gitignore` & `openllm_client-0.5.0a9/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm_client-0.5.0a8/LICENSE.md` & `openllm_client-0.5.0a9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm_client-0.5.0a8/pyproject.toml` & `openllm_client-0.5.0a9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openllm_client-0.5.0a8/PKG-INFO` & `openllm_client-0.5.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openllm-client
-Version: 0.5.0a8
+Version: 0.5.0a9
 Summary: OpenLLM Client: Interacting with OpenLLM HTTP/gRPC server, or any BentoML server.
 Project-URL: Blog, https://modelserving.com
 Project-URL: Chat, https://l.bentoml.com/join-openllm-discord
 Project-URL: Documentation, https://github.com/bentoml/OpenLLM/blob/main/openllm-client/README.md
 Project-URL: GitHub, https://github.com/bentoml/OpenLLM/blob/main/openllm-client
 Project-URL: History, https://github.com/bentoml/OpenLLM/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://bentoml.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openllm-client Version: 0.5.0a8 Summary: OpenLLM
+Metadata-Version: 2.1 Name: openllm-client Version: 0.5.0a9 Summary: OpenLLM
 Client: Interacting with OpenLLM HTTP/gRPC server, or any BentoML server.
 Project-URL: Blog, https://modelserving.com Project-URL: Chat, https://
 l.bentoml.com/join-openllm-discord Project-URL: Documentation, https://
 github.com/bentoml/OpenLLM/blob/main/openllm-client/README.md Project-URL:
 GitHub, https://github.com/bentoml/OpenLLM/blob/main/openllm-client Project-
 URL: History, https://github.com/bentoml/OpenLLM/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://bentoml.com Project-URL: Tracker, https://
```

