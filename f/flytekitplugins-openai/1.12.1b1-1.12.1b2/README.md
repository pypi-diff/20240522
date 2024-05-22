# Comparing `tmp/flytekitplugins_openai-1.12.1b1.tar.gz` & `tmp/flytekitplugins_openai-1.12.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins_openai-1.12.1b1.tar", last modified: Thu May 16 22:53:17 2024, max compression
+gzip compressed data, was "flytekitplugins_openai-1.12.1b2.tar", last modified: Wed May 22 13:27:15 2024, max compression
```

## Comparing `flytekitplugins_openai-1.12.1b1.tar` & `flytekitplugins_openai-1.12.1b2.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:17.475249 flytekitplugins_openai-1.12.1b1/
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-16 22:53:17.471249 flytekitplugins_openai-1.12.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-16 22:52:45.000000 flytekitplugins_openai-1.12.1b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:17.471249 flytekitplugins_openai-1.12.1b1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:17.471249 flytekitplugins_openai-1.12.1b1/flytekitplugins/openai/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-16 22:52:45.000000 flytekitplugins_openai-1.12.1b1/flytekitplugins/openai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:17.471249 flytekitplugins_openai-1.12.1b1/flytekitplugins/openai/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:52:45.000000 flytekitplugins_openai-1.12.1b1/flytekitplugins/openai/chatgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-16 22:52:45.000000 flytekitplugins_openai-1.12.1b1/flytekitplugins/openai/chatgpt/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-16 22:52:45.000000 flytekitplugins_openai-1.12.1b1/flytekitplugins/openai/chatgpt/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:17.471249 flytekitplugins_openai-1.12.1b1/flytekitplugins_openai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-16 22:53:17.000000 flytekitplugins_openai-1.12.1b1/flytekitplugins_openai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-16 22:53:17.000000 flytekitplugins_openai-1.12.1b1/flytekitplugins_openai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 22:53:17.000000 flytekitplugins_openai-1.12.1b1/flytekitplugins_openai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-16 22:53:17.000000 flytekitplugins_openai-1.12.1b1/flytekitplugins_openai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 22:53:17.000000 flytekitplugins_openai-1.12.1b1/flytekitplugins_openai.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-16 22:53:17.000000 flytekitplugins_openai-1.12.1b1/flytekitplugins_openai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 22:53:17.000000 flytekitplugins_openai-1.12.1b1/flytekitplugins_openai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 22:53:17.475249 flytekitplugins_openai-1.12.1b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-16 22:53:09.000000 flytekitplugins_openai-1.12.1b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:17.471249 flytekitplugins_openai-1.12.1b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-16 22:52:45.000000 flytekitplugins_openai-1.12.1b1/tests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-16 22:52:45.000000 flytekitplugins_openai-1.12.1b1/tests/test_chatgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:15.518363 flytekitplugins_openai-1.12.1b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-22 13:27:15.514363 flytekitplugins_openai-1.12.1b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-22 13:26:34.000000 flytekitplugins_openai-1.12.1b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:15.514363 flytekitplugins_openai-1.12.1b2/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:15.514363 flytekitplugins_openai-1.12.1b2/flytekitplugins/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-22 13:26:34.000000 flytekitplugins_openai-1.12.1b2/flytekitplugins/openai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:15.514363 flytekitplugins_openai-1.12.1b2/flytekitplugins/openai/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:26:34.000000 flytekitplugins_openai-1.12.1b2/flytekitplugins/openai/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-22 13:26:34.000000 flytekitplugins_openai-1.12.1b2/flytekitplugins/openai/batch/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-05-22 13:26:34.000000 flytekitplugins_openai-1.12.1b2/flytekitplugins/openai/batch/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-22 13:26:34.000000 flytekitplugins_openai-1.12.1b2/flytekitplugins/openai/batch/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:15.514363 flytekitplugins_openai-1.12.1b2/flytekitplugins/openai/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:26:34.000000 flytekitplugins_openai-1.12.1b2/flytekitplugins/openai/chatgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-22 13:26:34.000000 flytekitplugins_openai-1.12.1b2/flytekitplugins/openai/chatgpt/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-22 13:26:34.000000 flytekitplugins_openai-1.12.1b2/flytekitplugins/openai/chatgpt/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:15.514363 flytekitplugins_openai-1.12.1b2/flytekitplugins_openai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-22 13:27:15.000000 flytekitplugins_openai-1.12.1b2/flytekitplugins_openai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-22 13:27:15.000000 flytekitplugins_openai-1.12.1b2/flytekitplugins_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:27:15.000000 flytekitplugins_openai-1.12.1b2/flytekitplugins_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-22 13:27:15.000000 flytekitplugins_openai-1.12.1b2/flytekitplugins_openai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 13:27:15.000000 flytekitplugins_openai-1.12.1b2/flytekitplugins_openai.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-22 13:27:15.000000 flytekitplugins_openai-1.12.1b2/flytekitplugins_openai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 13:27:15.000000 flytekitplugins_openai-1.12.1b2/flytekitplugins_openai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:27:15.518363 flytekitplugins_openai-1.12.1b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-22 13:27:07.000000 flytekitplugins_openai-1.12.1b2/setup.py
```

### Comparing `flytekitplugins_openai-1.12.1b1/PKG-INFO` & `flytekitplugins_openai-1.12.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-openai
-Version: 1.12.1b1
+Version: 1.12.1b2
 Summary: This package holds the openai plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins_openai-1.12.1b1/flytekitplugins/openai/chatgpt/agent.py` & `flytekitplugins_openai-1.12.1b2/flytekitplugins/openai/chatgpt/agent.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_openai-1.12.1b1/flytekitplugins/openai/chatgpt/task.py` & `flytekitplugins_openai-1.12.1b2/flytekitplugins/openai/chatgpt/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_openai-1.12.1b1/flytekitplugins_openai.egg-info/PKG-INFO` & `flytekitplugins_openai-1.12.1b2/flytekitplugins_openai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-openai
-Version: 1.12.1b1
+Version: 1.12.1b2
 Summary: This package holds the openai plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins_openai-1.12.1b1/flytekitplugins_openai.egg-info/SOURCES.txt` & `flytekitplugins_openai-1.12.1b2/flytekitplugins_openai.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 README.md
 setup.py
 flytekitplugins/openai/__init__.py
+flytekitplugins/openai/batch/__init__.py
+flytekitplugins/openai/batch/agent.py
+flytekitplugins/openai/batch/task.py
+flytekitplugins/openai/batch/workflow.py
 flytekitplugins/openai/chatgpt/__init__.py
 flytekitplugins/openai/chatgpt/agent.py
 flytekitplugins/openai/chatgpt/task.py
 flytekitplugins_openai.egg-info/PKG-INFO
 flytekitplugins_openai.egg-info/SOURCES.txt
 flytekitplugins_openai.egg-info/dependency_links.txt
 flytekitplugins_openai.egg-info/entry_points.txt
 flytekitplugins_openai.egg-info/namespace_packages.txt
 flytekitplugins_openai.egg-info/requires.txt
-flytekitplugins_openai.egg-info/top_level.txt
-tests/test_agent.py
-tests/test_chatgpt.py
+flytekitplugins_openai.egg-info/top_level.txt
```

### Comparing `flytekitplugins_openai-1.12.1b1/setup.py` & `flytekitplugins_openai-1.12.1b2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,28 @@
 
 PLUGIN_NAME = "openai"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>1.10.7", "openai>=1.12.0", "flyteidl>=1.11.0"]
 
-__version__ = "1.12.1b1"
+__version__ = "1.12.1b2"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the openai plugins for flytekit",
     namespace_packages=["flytekitplugins"],
-    packages=[f"flytekitplugins.{PLUGIN_NAME}", f"flytekitplugins.{PLUGIN_NAME}.chatgpt"],
+    packages=[
+        f"flytekitplugins.{PLUGIN_NAME}",
+        f"flytekitplugins.{PLUGIN_NAME}.chatgpt",
+        f"flytekitplugins.{PLUGIN_NAME}.batch",
+    ],
     install_requires=plugin_requires,
     license="apache2",
     python_requires=">=3.8",
     classifiers=[
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
```

