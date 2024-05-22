# Comparing `tmp/railtownai-1.0.2.tar.gz` & `tmp/railtownai-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "railtownai-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "railtownai-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `railtownai-1.0.2.tar` & `railtownai-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      627 2024-01-08 20:13:24.125799 railtownai-1.0.2/.gitattributes
--rw-r--r--   0        0        0       96 2024-01-08 20:13:24.131979 railtownai-1.0.2/.gitignore
--rw-r--r--   0        0        0      705 2024-02-01 10:59:18.616687 railtownai-1.0.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1099 2024-03-11 22:13:03.599913 railtownai-1.0.2/LICENSE
--rw-r--r--   0        0        0      951 2024-03-11 22:13:03.599913 railtownai-1.0.2/README.md
--rw-r--r--   0        0        0      921 2024-01-08 20:23:58.473895 railtownai-1.0.2/azure-pipelines.yml
--rw-r--r--   0        0        0     1005 2024-01-08 20:13:24.135980 railtownai-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     5069 2024-03-11 22:43:58.682227 railtownai-1.0.2/src/railtownai/__init__.py
--rw-r--r--   0        0        0      802 2024-01-08 20:13:24.137974 railtownai-1.0.2/tests/test_integration_log.py
--rw-r--r--   0        0        0      713 2024-01-08 20:13:24.139981 railtownai-1.0.2/tests/test_methods.py
--rw-r--r--   0        0        0     1494 1970-01-01 00:00:00.000000 railtownai-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      627 2024-05-03 19:57:19.600427 railtownai-1.0.3/.gitattributes
+-rw-r--r--   0        0        0       96 2024-05-03 19:57:19.600427 railtownai-1.0.3/.gitignore
+-rw-r--r--   0        0        0      824 2024-05-22 16:18:48.207952 railtownai-1.0.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1099 2024-05-03 19:57:19.600427 railtownai-1.0.3/LICENSE
+-rw-r--r--   0        0        0      951 2024-05-03 19:57:19.600427 railtownai-1.0.3/README.md
+-rw-r--r--   0        0        0      921 2024-05-03 19:57:19.600427 railtownai-1.0.3/azure-pipelines.yml
+-rw-r--r--   0        0        0      981 2024-05-22 16:18:48.208953 railtownai-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5069 2024-05-22 16:18:48.209955 railtownai-1.0.3/src/railtownai/__init__.py
+-rw-r--r--   0        0        0      802 2024-05-03 19:57:19.600427 railtownai-1.0.3/tests/test_integration_log.py
+-rw-r--r--   0        0        0      765 2024-05-22 16:18:48.209955 railtownai-1.0.3/tests/test_methods.py
+-rw-r--r--   0        0        0     1497 1970-01-01 00:00:00.000000 railtownai-1.0.3/PKG-INFO
```

### Comparing `railtownai-1.0.2/.gitattributes` & `railtownai-1.0.3/.gitattributes`

 * *Files identical despite different names*

### Comparing `railtownai-1.0.2/CONTRIBUTING.md` & `railtownai-1.0.3/CONTRIBUTING.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Setup for development
 
 ## Setup steps
 
+1. Setup your python venv in this repository: `python -m venv .venv`
+1. Activate your venv: `.venv\Scripts\activate`
 1. Ensure you have [flit installed](https://flit.pypa.io/en/stable/)
 1. `flit install --python .venv/Scripts/python.exe`
 1. `flit build`
 
 ## Running Tests
 
 `pytest`
```

### Comparing `railtownai-1.0.2/LICENSE` & `railtownai-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `railtownai-1.0.2/README.md` & `railtownai-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `railtownai-1.0.2/azure-pipelines.yml` & `railtownai-1.0.3/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `railtownai-1.0.2/pyproject.toml` & `railtownai-1.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,47 @@
 [build-system]
-requires = [
-  "flit_core >=3.2,<4"
-]
+requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 
-
 [project]
 name = "railtownai"
 authors = [
-  {name = "Guan Zheng Huang", email = "guan@railtown.ai"}, 
-  {name = "Jaime Bueza", email = "jaime@railtown.ai"}
+  { name = "Guan Zheng Huang", email = "guan@railtown.ai" },
+  { name = "Jaime Bueza", email = "jaime@railtown.ai" },
 ]
 readme = "README.md"
-license = {file = "LICENSE"}
+license = { file = "LICENSE" }
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
-dependencies = [ 
-  "requests == 2.31.0",
-  "pydantic == 2.5.3",
-  "requests-mock == 1.11.0",
+dependencies = [
+  "requests >=2.31,<3",
+  "pydantic >= 2.5.3,<3",
+  "requests-mock >= 1.12.1",
   "python-dotenv == 1.0.0",
 ]
 
 [project.urls]
 Home = "https://railtown.ai"
- 
+
 
 [tool.flit.module]
 name = "railtownai"
 
 [tool.black]
 line-length = 120
-fast = true 
- 
+fast = true
+
 reportMissingImports = true
 reportMissingTypeStubs = false
 
 pythonVersion = "3.10"
 pythonPlatform = "Linux"
 
-executionEnvironments = [
-  { root = "src" }
-]
+executionEnvironments = [{ root = "src" }]
 
 [project.optional-dependencies]
-test = [
-    "pytest >=7.1.2",
-]
+test = ["pytest >=7.1.2"]
 
 [tool.pytest.ini_options]
-pythonpath = [
-  "src"
-]
+pythonpath = ["src"]
 testpaths = ["tests"]
```

### Comparing `railtownai-1.0.2/src/railtownai/__init__.py` & `railtownai-1.0.3/src/railtownai/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import os
 
 load_dotenv()
 
 railtown_api_key: str = os.environ.get("RAILTOWN_API_KEY", None)
 
 # TODO: Bump this
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 
 
 class RailtownPayload(BaseModel):
     Message: str
     Level: str
     OrganizationId: str
     ProjectId: str
```

### Comparing `railtownai-1.0.2/tests/test_integration_log.py` & `railtownai-1.0.3/tests/test_integration_log.py`

 * *Files identical despite different names*

### Comparing `railtownai-1.0.2/PKG-INFO` & `railtownai-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: railtownai
-Version: 1.0.2
+Version: 1.0.3
 Summary: Railtown AI Python SDK for tracking errors and exceptions in your Python applications
 Author-email: Guan Zheng Huang <guan@railtown.ai>, Jaime Bueza <jaime@railtown.ai>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: requests == 2.31.0
-Requires-Dist: pydantic == 2.5.3
-Requires-Dist: requests-mock == 1.11.0
+Requires-Dist: requests >=2.31,<3
+Requires-Dist: pydantic >= 2.5.3,<3
+Requires-Dist: requests-mock >= 1.12.1
 Requires-Dist: python-dotenv == 1.0.0
 Requires-Dist: pytest >=7.1.2 ; extra == "test"
 Project-URL: Home, https://railtown.ai
 Provides-Extra: test
 
 # Railtown AI Logging Python Package
```

