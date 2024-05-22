# Comparing `tmp/llm_ollama-0.3.0.tar.gz` & `tmp/llm_ollama-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_ollama-0.3.0.tar", last modified: Tue May  7 08:20:54 2024, max compression
+gzip compressed data, was "llm_ollama-0.4.0.tar", last modified: Wed May 22 07:11:44 2024, max compression
```

## Comparing `llm_ollama-0.3.0.tar` & `llm_ollama-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:20:54.749034 llm_ollama-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 08:20:49.000000 llm_ollama-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-07 08:20:54.749034 llm_ollama-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-07 08:20:49.000000 llm_ollama-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:20:54.749034 llm_ollama-0.3.0/llm_ollama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-07 08:20:54.000000 llm_ollama-0.3.0/llm_ollama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-07 08:20:54.000000 llm_ollama-0.3.0/llm_ollama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 08:20:54.000000 llm_ollama-0.3.0/llm_ollama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 08:20:54.000000 llm_ollama-0.3.0/llm_ollama.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 08:20:54.000000 llm_ollama-0.3.0/llm_ollama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 08:20:54.000000 llm_ollama-0.3.0/llm_ollama.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-07 08:20:49.000000 llm_ollama-0.3.0/llm_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-07 08:20:49.000000 llm_ollama-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 08:20:54.749034 llm_ollama-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:20:54.749034 llm_ollama-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-07 08:20:49.000000 llm_ollama-0.3.0/tests/test_ollama.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:11:44.575372 llm_ollama-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 07:11:38.000000 llm_ollama-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-22 07:11:44.575372 llm_ollama-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-22 07:11:38.000000 llm_ollama-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:11:44.571372 llm_ollama-0.4.0/llm_ollama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-22 07:11:44.000000 llm_ollama-0.4.0/llm_ollama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-22 07:11:44.000000 llm_ollama-0.4.0/llm_ollama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 07:11:44.000000 llm_ollama-0.4.0/llm_ollama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 07:11:44.000000 llm_ollama-0.4.0/llm_ollama.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 07:11:44.000000 llm_ollama-0.4.0/llm_ollama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 07:11:44.000000 llm_ollama-0.4.0/llm_ollama.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-22 07:11:38.000000 llm_ollama-0.4.0/llm_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-22 07:11:38.000000 llm_ollama-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 07:11:44.575372 llm_ollama-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:11:44.571372 llm_ollama-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-22 07:11:38.000000 llm_ollama-0.4.0/tests/test_ollama.py
```

### Comparing `llm_ollama-0.3.0/LICENSE` & `llm_ollama-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_ollama-0.3.0/PKG-INFO` & `llm_ollama-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: llm-ollama
-Version: 0.3.0
+Version: 0.4.0
 Summary: LLM plugin providing access to local Ollama models
 Author: Sergey Alexandrov
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/taketwo/llm-ollama
 Project-URL: Changelog, https://github.com/taketwo/llm-ollama/releases
 Project-URL: Issues, https://github.com/taketwo/llm-ollama/issues
 Project-URL: CI, https://github.com/taketwo/llm-ollama/actions
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: llm
 Requires-Dist: ollama
+Requires-Dist: pydantic>=2
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # llm-ollama
 
 [![PyPI](https://img.shields.io/pypi/v/llm-ollama.svg)](https://pypi.org/project/llm-ollama/)
 [![Changelog](https://img.shields.io/github/v/release/taketwo/llm-ollama?include_prereleases&label=changelog)](https://github.com/taketwo/llm-ollama/releases)
```

### Comparing `llm_ollama-0.3.0/README.md` & `llm_ollama-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `llm_ollama-0.3.0/llm_ollama.egg-info/PKG-INFO` & `llm_ollama-0.4.0/llm_ollama.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: llm-ollama
-Version: 0.3.0
+Version: 0.4.0
 Summary: LLM plugin providing access to local Ollama models
 Author: Sergey Alexandrov
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/taketwo/llm-ollama
 Project-URL: Changelog, https://github.com/taketwo/llm-ollama/releases
 Project-URL: Issues, https://github.com/taketwo/llm-ollama/issues
 Project-URL: CI, https://github.com/taketwo/llm-ollama/actions
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: llm
 Requires-Dist: ollama
+Requires-Dist: pydantic>=2
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # llm-ollama
 
 [![PyPI](https://img.shields.io/pypi/v/llm-ollama.svg)](https://pypi.org/project/llm-ollama/)
 [![Changelog](https://img.shields.io/github/v/release/taketwo/llm-ollama?include_prereleases&label=changelog)](https://github.com/taketwo/llm-ollama/releases)
```

### Comparing `llm_ollama-0.3.0/llm_ollama.py` & `llm_ollama-0.4.0/llm_ollama.py`

 * *Files identical despite different names*

### Comparing `llm_ollama-0.3.0/pyproject.toml` & `llm_ollama-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "llm-ollama"
-version = "0.3.0"
+version = "0.4.0"
 description = "LLM plugin providing access to local Ollama models"
 readme = "README.md"
 authors = [{ name = "Sergey Alexandrov" }]
 license = { text = "Apache-2.0" }
 classifiers = ["License :: OSI Approved :: Apache Software License"]
-dependencies = ["llm", "ollama"]
+dependencies = ["llm", "ollama", "pydantic>=2"]
 requires-python = ">=3.8"
 
 [project.urls]
 Homepage = "https://github.com/taketwo/llm-ollama"
 Changelog = "https://github.com/taketwo/llm-ollama/releases"
 Issues = "https://github.com/taketwo/llm-ollama/issues"
 CI = "https://github.com/taketwo/llm-ollama/actions"
```

### Comparing `llm_ollama-0.3.0/tests/test_ollama.py` & `llm_ollama-0.4.0/tests/test_ollama.py`

 * *Files identical despite different names*

