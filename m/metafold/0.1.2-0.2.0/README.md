# Comparing `tmp/metafold-0.1.2.tar.gz` & `tmp/metafold-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metafold-0.1.2.tar", last modified: Thu May  9 13:26:46 2024, max compression
+gzip compressed data, was "metafold-0.2.0.tar", last modified: Wed May 22 15:45:22 2024, max compression
```

## Comparing `metafold-0.1.2.tar` & `metafold-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:26:46.770036 metafold-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-09 13:26:43.000000 metafold-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-09 13:26:46.770036 metafold-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-09 13:26:43.000000 metafold-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:26:46.766036 metafold-0.1.2/metafold/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-09 13:26:43.000000 metafold-0.1.2/metafold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-09 13:26:43.000000 metafold-0.1.2/metafold/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-09 13:26:43.000000 metafold-0.1.2/metafold/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-09 13:26:43.000000 metafold-0.1.2/metafold/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-09 13:26:43.000000 metafold-0.1.2/metafold/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-09 13:26:43.000000 metafold-0.1.2/metafold/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:26:46.766036 metafold-0.1.2/metafold.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-09 13:26:46.000000 metafold-0.1.2/metafold.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-09 13:26:46.000000 metafold-0.1.2/metafold.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:26:46.000000 metafold-0.1.2/metafold.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-09 13:26:46.000000 metafold-0.1.2/metafold.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 13:26:46.000000 metafold-0.1.2/metafold.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-09 13:26:43.000000 metafold-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:26:46.770036 metafold-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:26:46.766036 metafold-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-05-09 13:26:43.000000 metafold-0.1.2/tests/test_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-09 13:26:43.000000 metafold-0.1.2/tests/test_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:45:22.048795 metafold-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-22 15:45:18.000000 metafold-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-22 15:45:22.048795 metafold-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-22 15:45:18.000000 metafold-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:45:22.048795 metafold-0.2.0/metafold/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-22 15:45:18.000000 metafold-0.2.0/metafold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-22 15:45:18.000000 metafold-0.2.0/metafold/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-22 15:45:18.000000 metafold-0.2.0/metafold/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-22 15:45:18.000000 metafold-0.2.0/metafold/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-22 15:45:18.000000 metafold-0.2.0/metafold/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23898 2024-05-22 15:45:18.000000 metafold-0.2.0/metafold/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-22 15:45:18.000000 metafold-0.2.0/metafold/func_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-22 15:45:18.000000 metafold-0.2.0/metafold/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-22 15:45:18.000000 metafold-0.2.0/metafold/nx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:45:22.048795 metafold-0.2.0/metafold.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-22 15:45:22.000000 metafold-0.2.0/metafold.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-22 15:45:22.000000 metafold-0.2.0/metafold.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:45:22.000000 metafold-0.2.0/metafold.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-22 15:45:22.000000 metafold-0.2.0/metafold.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 15:45:22.000000 metafold-0.2.0/metafold.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-22 15:45:18.000000 metafold-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:45:22.048795 metafold-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:45:22.048795 metafold-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-05-22 15:45:18.000000 metafold-0.2.0/tests/test_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-05-22 15:45:18.000000 metafold-0.2.0/tests/test_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-22 15:45:18.000000 metafold-0.2.0/tests/test_jobs.py
```

### Comparing `metafold-0.1.2/LICENSE` & `metafold-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metafold-0.1.2/PKG-INFO` & `metafold-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metafold
-Version: 0.1.2
+Version: 0.2.0
 Summary: Metafold SDK for Python
 Author-email: Metafold 3D <info@metafold3d.com>
 License: Copyright 2024 Metafold 3D
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -30,17 +30,24 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs>=23.2
 Requires-Dist: requests>=2.31
 Provides-Extra: docs
 Requires-Dist: sphinx>=7.2; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=2.0; extra == "docs"
+Provides-Extra: lint
+Requires-Dist: mypy>=1.10; extra == "lint"
+Requires-Dist: types-requests>=2.31; extra == "lint"
 Provides-Extra: test
+Requires-Dist: numpy>=1.26; extra == "test"
 Requires-Dist: pytest>=7.3; extra == "test"
 Requires-Dist: requests-toolbelt>=1.0; extra == "test"
+Provides-Extra: networkx
+Requires-Dist: networkx>=3.2; extra == "networkx"
+Requires-Dist: types-networkx>=3.2; extra == "networkx"
 
 # Metafold SDK for Python
 
 [![PyPi](https://img.shields.io/pypi/v/metafold.svg)](https://pypi.python.org/pypi/metafold)
 
 ## Installation
```

### Comparing `metafold-0.1.2/README.md` & `metafold-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `metafold-0.1.2/metafold/__init__.py` & `metafold-0.2.0/metafold/__init__.py`

 * *Files identical despite different names*

### Comparing `metafold-0.1.2/metafold/api.py` & `metafold-0.2.0/metafold/api.py`

 * *Files identical despite different names*

### Comparing `metafold-0.1.2/metafold/assets.py` & `metafold-0.2.0/metafold/assets.py`

 * *Files identical despite different names*

### Comparing `metafold-0.1.2/metafold/client.py` & `metafold-0.2.0/metafold/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,18 +25,18 @@
     def _request(
         self, request: Callable[..., Response], url: str,
         *args: Any, **kwargs: Any,
     ) -> Response:
         url = urljoin(self._base_url, url)
         r: Response = request(url, *args, **kwargs)
         if not r.ok:
-            r: dict[str, Any] = r.json()
+            body: dict[str, Any] = r.json()
             # Error responses aren't entirely consistent in the Metafold API,
             # for now we check for a handful of possible fields.
-            reason = r.get("errors") or r.get("msg") or r.get("description")
+            reason = body.get("errors") or body.get("msg") or body.get("description")
             raise HTTPError(f"HTTP error occurred: {reason or r.reason}")
         return r
 
     def get(self, url: str, *args: Any, **kwargs: Any) ->  Response:
         return self._request(self._session.get, url, *args, **kwargs)
 
     def post(self, url: str, *args: Any, **kwargs: Any) ->  Response:
```

### Comparing `metafold-0.1.2/metafold/jobs.py` & `metafold-0.2.0/metafold/jobs.py`

 * *Files identical despite different names*

### Comparing `metafold-0.1.2/metafold.egg-info/PKG-INFO` & `metafold-0.2.0/metafold.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metafold
-Version: 0.1.2
+Version: 0.2.0
 Summary: Metafold SDK for Python
 Author-email: Metafold 3D <info@metafold3d.com>
 License: Copyright 2024 Metafold 3D
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -30,17 +30,24 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs>=23.2
 Requires-Dist: requests>=2.31
 Provides-Extra: docs
 Requires-Dist: sphinx>=7.2; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=2.0; extra == "docs"
+Provides-Extra: lint
+Requires-Dist: mypy>=1.10; extra == "lint"
+Requires-Dist: types-requests>=2.31; extra == "lint"
 Provides-Extra: test
+Requires-Dist: numpy>=1.26; extra == "test"
 Requires-Dist: pytest>=7.3; extra == "test"
 Requires-Dist: requests-toolbelt>=1.0; extra == "test"
+Provides-Extra: networkx
+Requires-Dist: networkx>=3.2; extra == "networkx"
+Requires-Dist: types-networkx>=3.2; extra == "networkx"
 
 # Metafold SDK for Python
 
 [![PyPi](https://img.shields.io/pypi/v/metafold.svg)](https://pypi.python.org/pypi/metafold)
 
 ## Installation
```

### Comparing `metafold-0.1.2/pyproject.toml` & `metafold-0.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metafold"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
     {name = "Metafold 3D", email = "info@metafold3d.com"},
 ]
 dependencies = [
     "attrs>=23.2",
     "requests>=2.31",
 ]
@@ -37,11 +37,23 @@
 Issues = "https://github.com/Metafold3d/metafold-python/issues"
 
 [project.optional-dependencies]
 docs = [
     "sphinx>=7.2",
     "sphinx_rtd_theme>=2.0",
 ]
+lint = [
+    "mypy>=1.10",
+    "types-requests>=2.31",
+]
 test = [
+    "numpy>=1.26",
     "pytest>=7.3",
     "requests-toolbelt>=1.0",
 ]
+networkx = [
+    "networkx>=3.2",
+    "types-networkx>=3.2",
+]
+
+[tool.setuptools]
+packages = ["metafold"]
```

### Comparing `metafold-0.1.2/tests/test_assets.py` & `metafold-0.2.0/tests/test_assets.py`

 * *Files identical despite different names*

### Comparing `metafold-0.1.2/tests/test_jobs.py` & `metafold-0.2.0/tests/test_jobs.py`

 * *Files identical despite different names*

