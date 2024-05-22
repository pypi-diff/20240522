# Comparing `tmp/composio_julep-0.2.61.tar.gz` & `tmp/composio_julep-0.2.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_julep-0.2.61.tar", last modified: Tue May 21 20:13:22 2024, max compression
+gzip compressed data, was "composio_julep-0.2.62.tar", last modified: Wed May 22 10:40:36 2024, max compression
```

## Comparing `composio_julep-0.2.61.tar` & `composio_julep-0.2.62.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-21 20:13:22.055943 composio_julep-0.2.61/
--rw-r--r--   0 sawradip   (501) staff       (20)     4458 2024-05-21 20:13:22.055748 composio_julep-0.2.61/PKG-INFO
--rw-r--r--   0 sawradip   (501) staff       (20)     3928 2024-05-21 04:53:37.000000 composio_julep-0.2.61/README.md
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-21 20:13:22.054668 composio_julep-0.2.61/composio_julep/
--rw-r--r--   0 sawradip   (501) staff       (20)      158 2024-05-20 14:09:13.000000 composio_julep-0.2.61/composio_julep/__init__.py
--rw-r--r--   0 sawradip   (501) staff       (20)     1397 2024-05-20 14:09:13.000000 composio_julep-0.2.61/composio_julep/julep_toolspec.py
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-21 20:13:22.055463 composio_julep-0.2.61/composio_julep.egg-info/
--rw-r--r--   0 sawradip   (501) staff       (20)     4458 2024-05-21 20:13:22.000000 composio_julep-0.2.61/composio_julep.egg-info/PKG-INFO
--rw-r--r--   0 sawradip   (501) staff       (20)      267 2024-05-21 20:13:22.000000 composio_julep-0.2.61/composio_julep.egg-info/SOURCES.txt
--rw-r--r--   0 sawradip   (501) staff       (20)        1 2024-05-21 20:13:22.000000 composio_julep-0.2.61/composio_julep.egg-info/dependency_links.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-21 20:13:22.000000 composio_julep-0.2.61/composio_julep.egg-info/requires.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       15 2024-05-21 20:13:22.000000 composio_julep-0.2.61/composio_julep.egg-info/top_level.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-21 20:13:22.055982 composio_julep-0.2.61/setup.cfg
--rw-r--r--   0 sawradip   (501) staff       (20)      820 2024-05-21 20:12:30.000000 composio_julep-0.2.61/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-22 10:40:36.105144 composio_julep-0.2.62/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     4458 2024-05-22 10:40:36.104952 composio_julep-0.2.62/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3928 2024-05-22 10:40:02.000000 composio_julep-0.2.62/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-22 10:40:36.103804 composio_julep-0.2.62/composio_julep/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      158 2024-05-20 14:51:26.000000 composio_julep-0.2.62/composio_julep/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1397 2024-05-20 14:51:26.000000 composio_julep-0.2.62/composio_julep/julep_toolspec.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-22 10:40:36.104707 composio_julep-0.2.62/composio_julep.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     4458 2024-05-22 10:40:36.000000 composio_julep-0.2.62/composio_julep.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      267 2024-05-22 10:40:36.000000 composio_julep-0.2.62/composio_julep.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-05-22 10:40:36.000000 composio_julep-0.2.62/composio_julep.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-05-22 10:40:36.000000 composio_julep-0.2.62/composio_julep.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       15 2024-05-22 10:40:36.000000 composio_julep-0.2.62/composio_julep.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-05-22 10:40:36.105182 composio_julep-0.2.62/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      820 2024-05-22 10:40:15.000000 composio_julep-0.2.62/setup.py
```

### Comparing `composio_julep-0.2.61/PKG-INFO` & `composio_julep-0.2.62/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_julep
-Version: 0.2.61
+Version: 0.2.62
 Summary: Use Composio to get an array of tools with your Julep wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.2.61
+Requires-Dist: composio_openai===0.2.62
 Requires-Dist: julep>=0.3.2
 
 ## 🚀🔗 Integrating Composio with Julep
 
 Streamline the integration of Composio within the Julep agentic framework to enhance the interaction capabilities of Julep agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_julep-0.2.61/README.md` & `composio_julep-0.2.62/README.md`

 * *Files identical despite different names*

### Comparing `composio_julep-0.2.61/composio_julep/julep_toolspec.py` & `composio_julep-0.2.62/composio_julep/julep_toolspec.py`

 * *Files identical despite different names*

### Comparing `composio_julep-0.2.61/composio_julep.egg-info/PKG-INFO` & `composio_julep-0.2.62/composio_julep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_julep
-Version: 0.2.61
+Version: 0.2.62
 Summary: Use Composio to get an array of tools with your Julep wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.2.61
+Requires-Dist: composio_openai===0.2.62
 Requires-Dist: julep>=0.3.2
 
 ## 🚀🔗 Integrating Composio with Julep
 
 Streamline the integration of Composio within the Julep agentic framework to enhance the interaction capabilities of Julep agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_julep-0.2.61/setup.py` & `composio_julep-0.2.62/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_julep",
-    version="0.2.61",
+    version="0.2.62",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Julep wokflow.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9,<4",
-    install_requires=["composio_openai===0.2.61", "julep>=0.3.2"],
+    install_requires=["composio_openai===0.2.62", "julep>=0.3.2"],
     include_package_data=True,
 )
```

