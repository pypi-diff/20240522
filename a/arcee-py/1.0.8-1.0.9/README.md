# Comparing `tmp/arcee_py-1.0.8.tar.gz` & `tmp/arcee_py-1.0.9.tar.gz`

## Comparing `arcee_py-1.0.8.tar` & `arcee_py-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 arcee_py-1.0.8/.python-version
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 arcee_py-1.0.8/tasks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 arcee_py-1.0.8/.github/CODEOWNERS
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 arcee_py-1.0.8/.github/iced/test.yml
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 arcee_py-1.0.8/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 arcee_py-1.0.8/arcee/__init__.py
--rw-r--r--   0        0        0     7149 2020-02-02 00:00:00.000000 arcee_py-1.0.8/arcee/api.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 arcee_py-1.0.8/arcee/api_handler.py
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 arcee_py-1.0.8/arcee/cli.py
--rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 arcee_py-1.0.8/arcee/cli_handler.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 arcee_py-1.0.8/arcee/config.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 arcee_py-1.0.8/arcee/dalm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.8/arcee/schemas/__init__.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 arcee_py-1.0.8/arcee/schemas/doc.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 arcee_py-1.0.8/arcee/schemas/routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.8/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.8/tests/conftest.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 arcee_py-1.0.8/tests/test_api_handler.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 arcee_py-1.0.8/.gitignore
--rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 arcee_py-1.0.8/README.md
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 arcee_py-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 arcee_py-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 arcee_py-1.0.9/.python-version
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 arcee_py-1.0.9/tasks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 arcee_py-1.0.9/.github/CODEOWNERS
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 arcee_py-1.0.9/.github/iced/test.yml
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 arcee_py-1.0.9/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 arcee_py-1.0.9/arcee/__init__.py
+-rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 arcee_py-1.0.9/arcee/api.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 arcee_py-1.0.9/arcee/api_handler.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 arcee_py-1.0.9/arcee/cli.py
+-rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 arcee_py-1.0.9/arcee/cli_handler.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 arcee_py-1.0.9/arcee/config.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 arcee_py-1.0.9/arcee/dalm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.9/arcee/schemas/__init__.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 arcee_py-1.0.9/arcee/schemas/doc.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 arcee_py-1.0.9/arcee/schemas/routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.9/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.9/tests/conftest.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 arcee_py-1.0.9/tests/test_api_handler.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 arcee_py-1.0.9/.gitignore
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 arcee_py-1.0.9/README.md
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 arcee_py-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 arcee_py-1.0.9/PKG-INFO
```

### Comparing `arcee_py-1.0.8/tasks.py` & `arcee_py-1.0.9/tasks.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.8/.github/iced/test.yml` & `arcee_py-1.0.9/.github/iced/test.yml`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.8/.github/workflows/publish.yml` & `arcee_py-1.0.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.8/arcee/api_handler.py` & `arcee_py-1.0.9/arcee/api_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             raise Exception(exception)
 
         return decorator
 
     return retry_wrapper
 
 
-#@retry_call()
+# @retry_call()
 def make_request(
     request: Literal["post", "get"],
     route: Union[str, Route],
     body: Optional[Dict[str, Any]] = None,
     params: Optional[Dict[str, Any]] = None,
     headers: Optional[Dict[str, Any]] = None,
 ) -> Dict[str, str]:
```

### Comparing `arcee_py-1.0.8/arcee/cli.py` & `arcee_py-1.0.9/arcee/cli.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.8/arcee/cli_handler.py` & `arcee_py-1.0.9/arcee/cli_handler.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.8/arcee/config.py` & `arcee_py-1.0.9/arcee/config.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.8/arcee/dalm.py` & `arcee_py-1.0.9/arcee/dalm.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.8/tests/test_api_handler.py` & `arcee_py-1.0.9/tests/test_api_handler.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.8/.gitignore` & `arcee_py-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.8/README.md` & `arcee_py-1.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,20 @@
 In notebook:
 
 ```
 import os
 os.environ["ARCEE_API_KEY"] = "********"
 ```
 
+To customize the URL of the arcee platform:
+
+```
+export ARCEE_API_URL="https://your-url.arcee.ai"
+```
+
 ## Upload Context
 
 Upload context for your domain adapted langauge model to draw from.
 
 ```
 import arcee
 arcee.upload_doc("pubmed", doc_name="doc1", doc_text="whoa")
```

### Comparing `arcee_py-1.0.8/pyproject.toml` & `arcee_py-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.8/PKG-INFO` & `arcee_py-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcee-py
-Version: 1.0.8
+Version: 1.0.9
 Project-URL: Home, https://arcee.ai
 Author-email: Jacob Solowetz <jacob@arcee.ai>, Ben Epstein <ben@arcee.ai>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: pydantic<3.0,>=2.4.2
 Requires-Dist: requests
 Requires-Dist: rich
@@ -48,14 +48,20 @@
 In notebook:
 
 ```
 import os
 os.environ["ARCEE_API_KEY"] = "********"
 ```
 
+To customize the URL of the arcee platform:
+
+```
+export ARCEE_API_URL="https://your-url.arcee.ai"
+```
+
 ## Upload Context
 
 Upload context for your domain adapted langauge model to draw from.
 
 ```
 import arcee
 arcee.upload_doc("pubmed", doc_name="doc1", doc_text="whoa")
```

