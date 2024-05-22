# Comparing `tmp/brainchain-0.6.9.tar.gz` & `tmp/brainchain-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainchain-0.6.9.tar", max compression
+gzip compressed data, was "brainchain-0.7.0.tar", max compression
```

## Comparing `brainchain-0.6.9.tar` & `brainchain-0.7.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.6.9/brainchain/README.md
--rw-r--r--   0        0        0     2982 2024-05-10 17:23:42.151722 brainchain-0.6.9/brainchain/__init__.py
--rw-r--r--   0        0        0    13624 2024-05-21 22:55:20.072457 brainchain-0.6.9/brainchain/assistants.py
--rw-r--r--   0        0        0    11920 2024-05-22 17:01:54.871959 brainchain-0.6.9/brainchain/brainchain.py
--rw-r--r--   0        0        0     5663 2024-05-09 05:35:25.596909 brainchain-0.6.9/brainchain/carnivore.py
--rw-r--r--   0        0        0     2243 2024-02-14 04:10:52.129450 brainchain-0.6.9/brainchain/coredata.py
--rw-r--r--   0        0        0     2155 2023-09-12 01:13:30.915323 brainchain-0.6.9/brainchain/embeddings.py
--rw-r--r--   0        0        0    17861 2024-05-11 18:01:39.002320 brainchain-0.6.9/brainchain/graph/base.py
--rw-r--r--   0        0        0     7386 2024-05-10 17:23:37.046295 brainchain-0.6.9/brainchain/graph/schema.py
--rw-r--r--   0        0        0     3949 2024-05-21 23:34:38.931062 brainchain-0.6.9/brainchain/logger.py
--rw-r--r--   0        0        0    11959 2024-05-07 16:51:46.072448 brainchain-0.6.9/brainchain/products.py
--rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.6.9/brainchain/requirements.txt
--rw-r--r--   0        0        0     6024 2024-05-07 16:20:56.058058 brainchain-0.6.9/brainchain/sales_intel.py
--rw-r--r--   0        0        0     1977 2024-02-29 23:10:12.854747 brainchain-0.6.9/brainchain/search_v2.py
--rw-r--r--   0        0        0      595 2024-04-12 19:05:17.907126 brainchain-0.6.9/brainchain/tools/__init__.py
--rw-r--r--   0        0        0     2118 2024-05-09 17:28:37.403805 brainchain-0.6.9/brainchain/tools/coding.py
--rw-r--r--   0        0        0     3948 2024-05-07 16:51:46.073351 brainchain-0.6.9/brainchain/tools/diffbot.py
--rw-r--r--   0        0        0      632 2024-02-29 23:10:12.855578 brainchain-0.6.9/brainchain/tools/factual.py
--rw-r--r--   0        0        0     5800 2024-04-10 01:04:48.531327 brainchain-0.6.9/brainchain/tools/fts.py
--rw-r--r--   0        0        0     1450 2024-02-29 23:10:12.856798 brainchain-0.6.9/brainchain/tools/graph.py
--rw-r--r--   0        0        0     1029 2024-02-29 23:10:12.857047 brainchain-0.6.9/brainchain/tools/memory.py
--rw-r--r--   0        0        0     2154 2024-02-29 23:10:12.857190 brainchain-0.6.9/brainchain/tools/plan.py
--rw-r--r--   0        0        0     1660 2024-04-15 19:40:33.833814 brainchain-0.6.9/brainchain/tools/tokens.py
--rw-r--r--   0        0        0    21273 2024-05-21 21:16:24.442049 brainchain-0.6.9/brainchain/tools/tools.py
--rw-r--r--   0        0        0    12159 2024-05-07 16:51:46.074887 brainchain-0.6.9/brainchain/tools/web.py
--rw-r--r--   0        0        0      734 2024-05-21 22:23:01.506213 brainchain-0.6.9/brainchain/tools.py
--rw-r--r--   0        0        0      791 2024-05-07 16:51:51.752365 brainchain-0.6.9/brainchain/webapp/__init__.py
--rw-r--r--   0        0        0       82 2024-05-07 16:51:51.752653 brainchain-0.6.9/brainchain/webapp/agents.py
--rw-r--r--   0        0        0      173 2024-05-07 16:51:51.752960 brainchain-0.6.9/brainchain/webapp/base.py
--rw-r--r--   0        0        0      977 2024-05-07 16:51:51.753234 brainchain-0.6.9/brainchain/webapp/business_ideas.py
--rw-r--r--   0        0        0     1282 2024-05-07 16:51:51.753423 brainchain-0.6.9/brainchain/webapp/contents.py
--rw-r--r--   0        0        0      895 2024-05-07 16:51:51.753590 brainchain-0.6.9/brainchain/webapp/conversations.py
--rw-r--r--   0        0        0       91 2024-05-07 16:51:51.753815 brainchain-0.6.9/brainchain/webapp/embedding_models.py
--rw-r--r--   0        0        0     2709 2024-05-07 16:51:51.753990 brainchain-0.6.9/brainchain/webapp/embeddings.py
--rw-r--r--   0        0        0     1138 2024-05-07 16:51:51.754142 brainchain-0.6.9/brainchain/webapp/files.py
--rw-r--r--   0        0        0      218 2024-05-07 16:51:51.754320 brainchain-0.6.9/brainchain/webapp/health.py
--rw-r--r--   0        0        0       90 2024-05-07 16:51:51.754539 brainchain-0.6.9/brainchain/webapp/language_models.py
--rw-r--r--   0        0        0      622 2024-05-07 16:51:51.754700 brainchain-0.6.9/brainchain/webapp/laws.py
--rw-r--r--   0        0        0     1110 2024-05-07 16:51:51.754849 brainchain-0.6.9/brainchain/webapp/messages.py
--rw-r--r--   0        0        0     2220 2024-05-07 16:51:51.755068 brainchain-0.6.9/brainchain/webapp/namespaces.py
--rw-r--r--   0        0        0     1029 2024-05-07 16:51:51.755220 brainchain-0.6.9/brainchain/webapp/programs.py
--rw-r--r--   0        0        0      626 2024-05-07 16:51:51.755369 brainchain-0.6.9/brainchain/webapp/tasks.py
--rw-r--r--   0        0        0      853 2024-05-07 16:51:51.755565 brainchain-0.6.9/brainchain/webapp/tools.py
--rw-r--r--   0        0        0      677 2024-05-07 16:51:51.755730 brainchain-0.6.9/brainchain/webapp/users.py
--rw-r--r--   0        0        0      538 2024-05-22 17:00:49.902284 brainchain-0.6.9/pyproject.toml
--rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 brainchain-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.7.0/brainchain/README.md
+-rw-r--r--   0        0        0     2982 2024-05-10 17:23:42.151722 brainchain-0.7.0/brainchain/__init__.py
+-rw-r--r--   0        0        0    13624 2024-05-21 22:55:20.072457 brainchain-0.7.0/brainchain/assistants.py
+-rw-r--r--   0        0        0    11704 2024-05-22 17:23:08.619843 brainchain-0.7.0/brainchain/brainchain.py
+-rw-r--r--   0        0        0     5663 2024-05-09 05:35:25.596909 brainchain-0.7.0/brainchain/carnivore.py
+-rw-r--r--   0        0        0     2243 2024-02-14 04:10:52.129450 brainchain-0.7.0/brainchain/coredata.py
+-rw-r--r--   0        0        0     2155 2023-09-12 01:13:30.915323 brainchain-0.7.0/brainchain/embeddings.py
+-rw-r--r--   0        0        0    17861 2024-05-11 18:01:39.002320 brainchain-0.7.0/brainchain/graph/base.py
+-rw-r--r--   0        0        0     7386 2024-05-10 17:23:37.046295 brainchain-0.7.0/brainchain/graph/schema.py
+-rw-r--r--   0        0        0     3949 2024-05-21 23:34:38.931062 brainchain-0.7.0/brainchain/logger.py
+-rw-r--r--   0        0        0    11959 2024-05-07 16:51:46.072448 brainchain-0.7.0/brainchain/products.py
+-rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.7.0/brainchain/requirements.txt
+-rw-r--r--   0        0        0     6024 2024-05-07 16:20:56.058058 brainchain-0.7.0/brainchain/sales_intel.py
+-rw-r--r--   0        0        0     1977 2024-02-29 23:10:12.854747 brainchain-0.7.0/brainchain/search_v2.py
+-rw-r--r--   0        0        0      595 2024-04-12 19:05:17.907126 brainchain-0.7.0/brainchain/tools/__init__.py
+-rw-r--r--   0        0        0     2118 2024-05-09 17:28:37.403805 brainchain-0.7.0/brainchain/tools/coding.py
+-rw-r--r--   0        0        0     3948 2024-05-07 16:51:46.073351 brainchain-0.7.0/brainchain/tools/diffbot.py
+-rw-r--r--   0        0        0      632 2024-02-29 23:10:12.855578 brainchain-0.7.0/brainchain/tools/factual.py
+-rw-r--r--   0        0        0     5800 2024-04-10 01:04:48.531327 brainchain-0.7.0/brainchain/tools/fts.py
+-rw-r--r--   0        0        0     1450 2024-02-29 23:10:12.856798 brainchain-0.7.0/brainchain/tools/graph.py
+-rw-r--r--   0        0        0     1029 2024-02-29 23:10:12.857047 brainchain-0.7.0/brainchain/tools/memory.py
+-rw-r--r--   0        0        0     2154 2024-02-29 23:10:12.857190 brainchain-0.7.0/brainchain/tools/plan.py
+-rw-r--r--   0        0        0     1660 2024-04-15 19:40:33.833814 brainchain-0.7.0/brainchain/tools/tokens.py
+-rw-r--r--   0        0        0    21273 2024-05-21 21:16:24.442049 brainchain-0.7.0/brainchain/tools/tools.py
+-rw-r--r--   0        0        0    12159 2024-05-07 16:51:46.074887 brainchain-0.7.0/brainchain/tools/web.py
+-rw-r--r--   0        0        0      734 2024-05-21 22:23:01.506213 brainchain-0.7.0/brainchain/tools.py
+-rw-r--r--   0        0        0      791 2024-05-07 16:51:51.752365 brainchain-0.7.0/brainchain/webapp/__init__.py
+-rw-r--r--   0        0        0       82 2024-05-07 16:51:51.752653 brainchain-0.7.0/brainchain/webapp/agents.py
+-rw-r--r--   0        0        0      173 2024-05-07 16:51:51.752960 brainchain-0.7.0/brainchain/webapp/base.py
+-rw-r--r--   0        0        0      977 2024-05-07 16:51:51.753234 brainchain-0.7.0/brainchain/webapp/business_ideas.py
+-rw-r--r--   0        0        0     1282 2024-05-07 16:51:51.753423 brainchain-0.7.0/brainchain/webapp/contents.py
+-rw-r--r--   0        0        0      895 2024-05-07 16:51:51.753590 brainchain-0.7.0/brainchain/webapp/conversations.py
+-rw-r--r--   0        0        0       91 2024-05-07 16:51:51.753815 brainchain-0.7.0/brainchain/webapp/embedding_models.py
+-rw-r--r--   0        0        0     2709 2024-05-07 16:51:51.753990 brainchain-0.7.0/brainchain/webapp/embeddings.py
+-rw-r--r--   0        0        0     1138 2024-05-07 16:51:51.754142 brainchain-0.7.0/brainchain/webapp/files.py
+-rw-r--r--   0        0        0      218 2024-05-07 16:51:51.754320 brainchain-0.7.0/brainchain/webapp/health.py
+-rw-r--r--   0        0        0       90 2024-05-07 16:51:51.754539 brainchain-0.7.0/brainchain/webapp/language_models.py
+-rw-r--r--   0        0        0      622 2024-05-07 16:51:51.754700 brainchain-0.7.0/brainchain/webapp/laws.py
+-rw-r--r--   0        0        0     1110 2024-05-07 16:51:51.754849 brainchain-0.7.0/brainchain/webapp/messages.py
+-rw-r--r--   0        0        0     2220 2024-05-07 16:51:51.755068 brainchain-0.7.0/brainchain/webapp/namespaces.py
+-rw-r--r--   0        0        0     1029 2024-05-07 16:51:51.755220 brainchain-0.7.0/brainchain/webapp/programs.py
+-rw-r--r--   0        0        0      626 2024-05-07 16:51:51.755369 brainchain-0.7.0/brainchain/webapp/tasks.py
+-rw-r--r--   0        0        0      853 2024-05-07 16:51:51.755565 brainchain-0.7.0/brainchain/webapp/tools.py
+-rw-r--r--   0        0        0      677 2024-05-07 16:51:51.755730 brainchain-0.7.0/brainchain/webapp/users.py
+-rw-r--r--   0        0        0      538 2024-05-22 17:23:28.243670 brainchain-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 brainchain-0.7.0/PKG-INFO
```

### Comparing `brainchain-0.6.9/brainchain/README.md` & `brainchain-0.7.0/brainchain/README.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/__init__.py` & `brainchain-0.7.0/brainchain/__init__.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/assistants.py` & `brainchain-0.7.0/brainchain/assistants.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/brainchain.py` & `brainchain-0.7.0/brainchain/brainchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,20 +162,14 @@
             Tasks,
             Tools,
             Users,
         ]
         for cls in webapp_classes:
             setattr(self, cls.__name__.lower(), self._init_component(cls))
 
-    def __getattr__(self, name):
-        if name in self.tool_functions:
-            return self.tool_functions[name]
-        else:
-            raise AttributeError(f"Brainchain object has no attribute {name}")
-    
     def set_auth_header(self):
         if self.access_token:
             self.session.headers.update({"Authorization": f"Bearer {self.access_token}"})
         else:
             self.session.headers.pop("Authorization", None)
 
     # Authentication
```

### Comparing `brainchain-0.6.9/brainchain/carnivore.py` & `brainchain-0.7.0/brainchain/carnivore.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/coredata.py` & `brainchain-0.7.0/brainchain/coredata.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/embeddings.py` & `brainchain-0.7.0/brainchain/embeddings.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/graph/base.py` & `brainchain-0.7.0/brainchain/graph/base.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/graph/schema.py` & `brainchain-0.7.0/brainchain/graph/schema.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/logger.py` & `brainchain-0.7.0/brainchain/logger.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/products.py` & `brainchain-0.7.0/brainchain/products.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/requirements.txt` & `brainchain-0.7.0/brainchain/requirements.txt`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/sales_intel.py` & `brainchain-0.7.0/brainchain/sales_intel.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/search_v2.py` & `brainchain-0.7.0/brainchain/search_v2.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/tools/__init__.py` & `brainchain-0.7.0/brainchain/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/tools/coding.py` & `brainchain-0.7.0/brainchain/tools/coding.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/tools/diffbot.py` & `brainchain-0.7.0/brainchain/tools/diffbot.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/tools/factual.py` & `brainchain-0.7.0/brainchain/tools/factual.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/tools/fts.py` & `brainchain-0.7.0/brainchain/tools/fts.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/tools/graph.py` & `brainchain-0.7.0/brainchain/tools/graph.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/tools/memory.py` & `brainchain-0.7.0/brainchain/tools/memory.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/tools/plan.py` & `brainchain-0.7.0/brainchain/tools/plan.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/tools/tokens.py` & `brainchain-0.7.0/brainchain/tools/tokens.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/tools/tools.py` & `brainchain-0.7.0/brainchain/tools/tools.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/tools/web.py` & `brainchain-0.7.0/brainchain/tools/web.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/tools.py` & `brainchain-0.7.0/brainchain/tools.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/webapp/__init__.py` & `brainchain-0.7.0/brainchain/webapp/__init__.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/webapp/business_ideas.py` & `brainchain-0.7.0/brainchain/webapp/business_ideas.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/webapp/contents.py` & `brainchain-0.7.0/brainchain/webapp/contents.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/webapp/conversations.py` & `brainchain-0.7.0/brainchain/webapp/conversations.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/webapp/embeddings.py` & `brainchain-0.7.0/brainchain/webapp/embeddings.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/webapp/files.py` & `brainchain-0.7.0/brainchain/webapp/files.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/webapp/laws.py` & `brainchain-0.7.0/brainchain/webapp/laws.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/webapp/messages.py` & `brainchain-0.7.0/brainchain/webapp/messages.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/webapp/namespaces.py` & `brainchain-0.7.0/brainchain/webapp/namespaces.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/webapp/programs.py` & `brainchain-0.7.0/brainchain/webapp/programs.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/webapp/tasks.py` & `brainchain-0.7.0/brainchain/webapp/tasks.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/webapp/tools.py` & `brainchain-0.7.0/brainchain/webapp/tools.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/brainchain/webapp/users.py` & `brainchain-0.7.0/brainchain/webapp/users.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.9/pyproject.toml` & `brainchain-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brainchain"
-version = "0.6.9"
+version = "0.7.0"
 description = "Brainchain API client"
 authors = ["Arthur M. Collé <arthur@brainchain.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 urllib3 = "2.0.6"
 requests = "2.31.0"
```

### Comparing `brainchain-0.6.9/PKG-INFO` & `brainchain-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainchain
-Version: 0.6.9
+Version: 0.7.0
 Summary: Brainchain API client
 Author: Arthur M. Collé
 Author-email: arthur@brainchain.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

