# Comparing `tmp/supabase-2.4.5.tar.gz` & `tmp/supabase-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supabase-2.4.5.tar", max compression
+gzip compressed data, was "supabase-2.4.6.tar", max compression
```

## Comparing `supabase-2.4.5.tar` & `supabase-2.4.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1067 2024-05-01 19:00:59.739845 supabase-2.4.5/LICENSE
--rw-r--r--   0        0        0     8244 2024-05-01 19:00:59.739845 supabase-2.4.5/README.md
--rw-r--r--   0        0        0     1892 2024-05-01 19:01:05.903834 supabase-2.4.5/pyproject.toml
--rw-r--r--   0        0        0     1224 2024-05-01 19:00:59.739845 supabase-2.4.5/supabase/__init__.py
--rw-r--r--   0        0        0       22 2024-05-01 19:01:05.903834 supabase-2.4.5/supabase/__version__.py
--rw-r--r--   0        0        0       35 2024-05-01 19:00:59.739845 supabase-2.4.5/supabase/_async/__init__.py
--rw-r--r--   0        0        0     1130 2024-05-01 19:00:59.739845 supabase-2.4.5/supabase/_async/auth_client.py
--rw-r--r--   0        0        0    10127 2024-05-01 19:00:59.739845 supabase-2.4.5/supabase/_async/client.py
--rw-r--r--   0        0        0       35 2024-05-01 19:00:59.739845 supabase-2.4.5/supabase/_sync/__init__.py
--rw-r--r--   0        0        0     1120 2024-05-01 19:00:59.739845 supabase-2.4.5/supabase/_sync/auth_client.py
--rw-r--r--   0        0        0    10088 2024-05-01 19:00:59.739845 supabase-2.4.5/supabase/_sync/client.py
--rw-r--r--   0        0        0     1172 2024-05-01 19:00:59.739845 supabase-2.4.5/supabase/client.py
--rw-r--r--   0        0        0      127 2024-05-01 19:00:59.739845 supabase-2.4.5/supabase/lib/__init__.py
--rw-r--r--   0        0        0     3135 2024-05-01 19:00:59.739845 supabase-2.4.5/supabase/lib/client_options.py
--rw-r--r--   0        0        0     1892 2024-05-01 19:00:59.739845 supabase-2.4.5/supabase/lib/realtime_client.py
--rw-r--r--   0        0        0        0 2024-05-01 19:00:59.739845 supabase-2.4.5/supabase/py.typed
--rw-r--r--   0        0        0     9313 1970-01-01 00:00:00.000000 supabase-2.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-22 20:10:06.418868 supabase-2.4.6/LICENSE
+-rw-r--r--   0        0        0     8244 2024-05-22 20:10:06.418868 supabase-2.4.6/README.md
+-rw-r--r--   0        0        0     1892 2024-05-22 20:10:14.842875 supabase-2.4.6/pyproject.toml
+-rw-r--r--   0        0        0     1224 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-22 20:10:14.842875 supabase-2.4.6/supabase/__version__.py
+-rw-r--r--   0        0        0       35 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/_async/__init__.py
+-rw-r--r--   0        0        0     1130 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/_async/auth_client.py
+-rw-r--r--   0        0        0    10114 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/_async/client.py
+-rw-r--r--   0        0        0       35 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/_sync/__init__.py
+-rw-r--r--   0        0        0     1120 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/_sync/auth_client.py
+-rw-r--r--   0        0        0    10081 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/_sync/client.py
+-rw-r--r--   0        0        0     1172 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/client.py
+-rw-r--r--   0        0        0      127 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/lib/__init__.py
+-rw-r--r--   0        0        0     3135 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/lib/client_options.py
+-rw-r--r--   0        0        0     1892 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/lib/realtime_client.py
+-rw-r--r--   0        0        0        0 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/py.typed
+-rw-r--r--   0        0        0     9313 1970-01-01 00:00:00.000000 supabase-2.4.6/PKG-INFO
```

### Comparing `supabase-2.4.5/LICENSE` & `supabase-2.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `supabase-2.4.5/README.md` & `supabase-2.4.6/README.md`

 * *Files identical despite different names*

### Comparing `supabase-2.4.5/pyproject.toml` & `supabase-2.4.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "supabase"
-version = "2.4.5"
+version = "2.4.6"
 description = "Supabase client for Python."
 authors = ["Joel Lee <joel@joellee.org>", "Leon Fedden <leonfedden@gmail.com>", "Daniel Reinón García <danielreinon@outlook.com>", "Leynier Gutiérrez González <leynier41@gmail.com>", "Anand", "Andrew Smith <a.smith@silentworks.co.uk>"]
 homepage = "https://github.com/supabase-community/supabase-py"
 repository = "https://github.com/supabase-community/supabase-py"
 documentation = "https://github.com/supabase-community/supabase-py"
 readme = "README.md"
 license = "MIT"
@@ -22,20 +22,20 @@
 httpx = ">=0.24,<0.28"
 storage3 = ">=0.5.3,<0.8.0"
 supafunc = ">=0.3.1,<0.5.0"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^3.5.0"
 black = "^24.4"
-pytest = "^8.2.0"
+pytest = "^8.2.1"
 flake8 = "^5.0.4"
 isort = "^5.10.1"
 pytest-cov = "^5.0.0"
-commitizen = "^3.25.0"
-python-semantic-release = "^9.6.0"
+commitizen = "^3.26.0"
+python-semantic-release = "^9.7.3"
 python-dotenv = "^1.0.1"
 
 [tool.poetry.scripts]
 tests = 'poetry_scripts:run_tests'
 
 [tool.poetry.group.dev.dependencies]
 unasync-cli = "^0.0.9"
```

### Comparing `supabase-2.4.5/supabase/__init__.py` & `supabase-2.4.6/supabase/__init__.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.5/supabase/_async/auth_client.py` & `supabase-2.4.6/supabase/_async/auth_client.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.5/supabase/_async/client.py` & `supabase-2.4.6/supabase/_async/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,10 +292,10 @@
     >>> key: str = os.environ.get("SUPABASE_TEST_KEY")
     >>> supabase: Client = create_client(url, key)
 
     Returns
     -------
     Client
     """
-    return await AsyncClient.create(
+    return AsyncClient(
         supabase_url=supabase_url, supabase_key=supabase_key, options=options
     )
```

### Comparing `supabase-2.4.5/supabase/_sync/auth_client.py` & `supabase-2.4.6/supabase/_sync/auth_client.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.5/supabase/_sync/client.py` & `supabase-2.4.6/supabase/_sync/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,10 +292,10 @@
     >>> key: str = os.environ.get("SUPABASE_TEST_KEY")
     >>> supabase: Client = create_client(url, key)
 
     Returns
     -------
     Client
     """
-    return SyncClient.create(
+    return SyncClient(
         supabase_url=supabase_url, supabase_key=supabase_key, options=options
     )
```

### Comparing `supabase-2.4.5/supabase/client.py` & `supabase-2.4.6/supabase/client.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.5/supabase/lib/client_options.py` & `supabase-2.4.6/supabase/lib/client_options.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.5/supabase/lib/realtime_client.py` & `supabase-2.4.6/supabase/lib/realtime_client.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.5/PKG-INFO` & `supabase-2.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supabase
-Version: 2.4.5
+Version: 2.4.6
 Summary: Supabase client for Python.
 Home-page: https://github.com/supabase-community/supabase-py
 License: MIT
 Author: Joel Lee
 Author-email: joel@joellee.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

