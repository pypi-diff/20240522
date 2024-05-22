# Comparing `tmp/arena_client-0.2.1.tar.gz` & `tmp/arena_client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arena_client-0.2.1.tar", max compression
+gzip compressed data, was "arena_client-0.2.2.tar", max compression
```

## Comparing `arena_client-0.2.1.tar` & `arena_client-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      570 2024-05-20 10:18:49.495750 arena_client-0.2.1/README.md
--rw-r--r--   0        0        0     1348 2024-05-20 10:18:49.495750 arena_client-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      154 2024-05-20 10:18:49.495750 arena_client-0.2.1/src/arena/__init__.py
--rw-r--r--   0        0        0    12669 2024-05-20 10:18:49.495750 arena_client-0.2.1/src/arena/client.py
--rw-r--r--   0        0        0     1018 2024-05-20 10:18:49.495750 arena_client-0.2.1/src/arena/models/__init__.py
--rw-r--r--   0        0        0     4009 2024-05-20 10:18:49.495750 arena_client-0.2.1/src/arena/models/anthropic.py
--rw-r--r--   0        0        0     4364 2024-05-20 10:18:49.495750 arena_client-0.2.1/src/arena/models/chat_completion.py
--rw-r--r--   0        0        0      281 2024-05-20 10:18:49.495750 arena_client-0.2.1/src/arena/models/evaluation.py
--rw-r--r--   0        0        0     2287 2024-05-20 10:18:49.495750 arena_client-0.2.1/src/arena/models/mistral.py
--rw-r--r--   0        0        0     1444 2024-05-20 10:18:49.495750 arena_client-0.2.1/src/arena/models/openai.py
--rw-r--r--   0        0        0      204 2024-05-20 10:18:49.495750 arena_client-0.2.1/src/arena/models/settings.py
--rw-r--r--   0        0        0     1195 1970-01-01 00:00:00.000000 arena_client-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      570 2024-05-22 09:26:09.375372 arena_client-0.2.2/README.md
+-rw-r--r--   0        0        0     1348 2024-05-22 09:26:09.375372 arena_client-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      154 2024-05-22 09:26:09.375372 arena_client-0.2.2/src/arena/__init__.py
+-rw-r--r--   0        0        0    12669 2024-05-22 09:26:09.375372 arena_client-0.2.2/src/arena/client.py
+-rw-r--r--   0        0        0     1018 2024-05-22 09:26:09.375372 arena_client-0.2.2/src/arena/models/__init__.py
+-rw-r--r--   0        0        0     4009 2024-05-22 09:26:09.375372 arena_client-0.2.2/src/arena/models/anthropic.py
+-rw-r--r--   0        0        0     4364 2024-05-22 09:26:09.375372 arena_client-0.2.2/src/arena/models/chat_completion.py
+-rw-r--r--   0        0        0      281 2024-05-22 09:26:09.375372 arena_client-0.2.2/src/arena/models/evaluation.py
+-rw-r--r--   0        0        0     2287 2024-05-22 09:26:09.375372 arena_client-0.2.2/src/arena/models/mistral.py
+-rw-r--r--   0        0        0     1444 2024-05-22 09:26:09.375372 arena_client-0.2.2/src/arena/models/openai.py
+-rw-r--r--   0        0        0      237 2024-05-22 09:26:09.375372 arena_client-0.2.2/src/arena/models/settings.py
+-rw-r--r--   0        0        0     1195 1970-01-01 00:00:00.000000 arena_client-0.2.2/PKG-INFO
```

### Comparing `arena_client-0.2.1/README.md` & `arena_client-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `arena_client-0.2.1/pyproject.toml` & `arena_client-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arena-client"
-version = "0.2.1"
+version = "0.2.2"
 description = "A client to use arena AI"
 authors = ["Nicolas Grislain <ng@sarus.tech>"]
 license = "Apache-2"
 readme = "README.md"
 packages = [{from = "src", include = "arena"}]
 
 [tool.poetry.dependencies]
```

### Comparing `arena_client-0.2.1/src/arena/client.py` & `arena_client-0.2.2/src/arena/client.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.2.1/src/arena/models/__init__.py` & `arena_client-0.2.2/src/arena/models/__init__.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.2.1/src/arena/models/anthropic.py` & `arena_client-0.2.2/src/arena/models/anthropic.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.2.1/src/arena/models/chat_completion.py` & `arena_client-0.2.2/src/arena/models/chat_completion.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.2.1/src/arena/models/mistral.py` & `arena_client-0.2.2/src/arena/models/mistral.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.2.1/src/arena/models/openai.py` & `arena_client-0.2.2/src/arena/models/openai.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.2.1/PKG-INFO` & `arena_client-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arena-client
-Version: 0.2.1
+Version: 0.2.2
 Summary: A client to use arena AI
 License: Apache-2
 Author: Nicolas Grislain
 Author-email: ng@sarus.tech
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

