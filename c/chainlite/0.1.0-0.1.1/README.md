# Comparing `tmp/chainlite-0.1.0.tar.gz` & `tmp/chainlite-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlite-0.1.0.tar", last modified: Tue May 21 23:10:02 2024, max compression
+gzip compressed data, was "chainlite-0.1.1.tar", last modified: Tue May 21 23:42:11 2024, max compression
```

## Comparing `chainlite-0.1.0.tar` & `chainlite-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwx------   0 sina      (1013) users      (100)        0 2024-05-21 23:10:02.958841 chainlite-0.1.0/
--rw-------   0 sina      (1013) users      (100)    11357 2024-05-19 03:42:10.000000 chainlite-0.1.0/LICENSE
--rw-r--r--   0 sina      (1013) users      (100)     4310 2024-05-21 23:10:02.958841 chainlite-0.1.0/PKG-INFO
--rw-------   0 sina      (1013) users      (100)     3177 2024-05-21 23:03:24.000000 chainlite-0.1.0/README.md
-drwx------   0 sina      (1013) users      (100)        0 2024-05-21 23:10:02.958841 chainlite-0.1.0/chainlite/
--rw-------   0 sina      (1013) users      (100)      341 2024-05-21 22:27:15.000000 chainlite-0.1.0/chainlite/__init__.py
--rw-------   0 sina      (1013) users      (100)     5106 2024-05-21 20:48:09.000000 chainlite-0.1.0/chainlite/llm_config.py
--rw-------   0 sina      (1013) users      (100)     9241 2024-05-21 22:56:29.000000 chainlite-0.1.0/chainlite/llm_generate.py
--rw-------   0 sina      (1013) users      (100)     7938 2024-05-19 07:42:59.000000 chainlite-0.1.0/chainlite/load_prompt.py
--rw-------   0 sina      (1013) users      (100)      463 2024-05-19 04:16:39.000000 chainlite-0.1.0/chainlite/utils.py
-drwx------   0 sina      (1013) users      (100)        0 2024-05-21 23:10:02.958841 chainlite-0.1.0/chainlite.egg-info/
--rw-r--r--   0 sina      (1013) users      (100)     4310 2024-05-21 23:10:02.000000 chainlite-0.1.0/chainlite.egg-info/PKG-INFO
--rw-------   0 sina      (1013) users      (100)      380 2024-05-21 23:10:02.000000 chainlite-0.1.0/chainlite.egg-info/SOURCES.txt
--rw-------   0 sina      (1013) users      (100)        1 2024-05-21 23:10:02.000000 chainlite-0.1.0/chainlite.egg-info/dependency_links.txt
--rw-------   0 sina      (1013) users      (100)      247 2024-05-21 23:10:02.000000 chainlite-0.1.0/chainlite.egg-info/requires.txt
--rw-------   0 sina      (1013) users      (100)       16 2024-05-21 23:10:02.000000 chainlite-0.1.0/chainlite.egg-info/top_level.txt
--rw-------   0 sina      (1013) users      (100)       95 2024-05-21 23:08:53.000000 chainlite-0.1.0/pyproject.toml
--rw-------   0 sina      (1013) users      (100)       38 2024-05-21 23:10:02.958841 chainlite-0.1.0/setup.cfg
--rw-------   0 sina      (1013) users      (100)     1144 2024-05-21 23:05:41.000000 chainlite-0.1.0/setup.py
-drwx------   0 sina      (1013) users      (100)        0 2024-05-21 23:10:02.958841 chainlite-0.1.0/tasks/
--rw-------   0 sina      (1013) users      (100)       24 2024-05-19 04:16:50.000000 chainlite-0.1.0/tasks/__init__.py
--rw-------   0 sina      (1013) users      (100)     1654 2024-05-19 04:22:14.000000 chainlite-0.1.0/tasks/main.py
-drwx------   0 sina      (1013) users      (100)        0 2024-05-21 23:10:02.958841 chainlite-0.1.0/tests/
--rw-------   0 sina      (1013) users      (100)      666 2024-05-21 20:34:10.000000 chainlite-0.1.0/tests/test_llm_generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:42:11.215075 chainlite-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-21 23:42:06.000000 chainlite-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-05-21 23:42:11.215075 chainlite-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-21 23:42:06.000000 chainlite-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:42:11.215075 chainlite-0.1.1/chainlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-21 23:42:06.000000 chainlite-0.1.1/chainlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-05-21 23:42:06.000000 chainlite-0.1.1/chainlite/llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9241 2024-05-21 23:42:06.000000 chainlite-0.1.1/chainlite/llm_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7938 2024-05-21 23:42:06.000000 chainlite-0.1.1/chainlite/load_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-21 23:42:06.000000 chainlite-0.1.1/chainlite/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:42:11.215075 chainlite-0.1.1/chainlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-05-21 23:42:11.000000 chainlite-0.1.1/chainlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-21 23:42:11.000000 chainlite-0.1.1/chainlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 23:42:11.000000 chainlite-0.1.1/chainlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-21 23:42:11.000000 chainlite-0.1.1/chainlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 23:42:11.000000 chainlite-0.1.1/chainlite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-21 23:42:06.000000 chainlite-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 23:42:11.215075 chainlite-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-21 23:42:06.000000 chainlite-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:42:11.215075 chainlite-0.1.1/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 23:42:06.000000 chainlite-0.1.1/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-21 23:42:06.000000 chainlite-0.1.1/tasks/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:42:11.215075 chainlite-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-21 23:42:06.000000 chainlite-0.1.1/tests/test_llm_generate.py
```

### Comparing `chainlite-0.1.0/LICENSE` & `chainlite-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.0/PKG-INFO` & `chainlite-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlite
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package that uses LangChain and LiteLLM to call large language model APIs easily
 Home-page: https://github.com/stanford-oval/chainlite
 Author: Sina Semnani
 Author-email: sinaj@cs.stanford.edu
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `chainlite-0.1.0/README.md` & `chainlite-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.0/chainlite/llm_config.py` & `chainlite-0.1.1/chainlite/llm_config.py`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.0/chainlite/llm_generate.py` & `chainlite-0.1.1/chainlite/llm_generate.py`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.0/chainlite/load_prompt.py` & `chainlite-0.1.1/chainlite/load_prompt.py`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.0/chainlite.egg-info/PKG-INFO` & `chainlite-0.1.1/chainlite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlite
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package that uses LangChain and LiteLLM to call large language model APIs easily
 Home-page: https://github.com/stanford-oval/chainlite
 Author: Sina Semnani
 Author-email: sinaj@cs.stanford.edu
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `chainlite-0.1.0/setup.py` & `chainlite-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chainlite",
-    version="0.1.0",
+    version="0.1.1",
     author="Sina Semnani",
     author_email="sinaj@cs.stanford.edu",
     description="A Python package that uses LangChain and LiteLLM to call large language model APIs easily",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/stanford-oval/chainlite",
     packages=find_packages(),
```

### Comparing `chainlite-0.1.0/tasks/main.py` & `chainlite-0.1.1/tasks/main.py`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.0/tests/test_llm_generate.py` & `chainlite-0.1.1/tests/test_llm_generate.py`

 * *Files identical despite different names*

