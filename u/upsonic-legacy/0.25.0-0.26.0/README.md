# Comparing `tmp/upsonic_legacy-0.25.0.tar.gz` & `tmp/upsonic_legacy-0.26.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upsonic_legacy-0.25.0.tar", last modified: Mon May 13 12:25:48 2024, max compression
+gzip compressed data, was "upsonic_legacy-0.26.0.tar", last modified: Wed May 22 15:39:02 2024, max compression
```

## Comparing `upsonic_legacy-0.25.0.tar` & `upsonic_legacy-0.26.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:25:48.939026 upsonic_legacy-0.25.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-13 12:25:39.000000 upsonic_legacy-0.25.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-13 12:25:39.000000 upsonic_legacy-0.25.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-05-13 12:25:48.939026 upsonic_legacy-0.25.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-13 12:25:39.000000 upsonic_legacy-0.25.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 12:25:39.000000 upsonic_legacy-0.25.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:25:48.939026 upsonic_legacy-0.25.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-13 12:25:39.000000 upsonic_legacy-0.25.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:25:48.939026 upsonic_legacy-0.25.0/upsonic/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-13 12:25:39.000000 upsonic_legacy-0.25.0/upsonic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:25:48.939026 upsonic_legacy-0.25.0/upsonic/remote/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-13 12:25:39.000000 upsonic_legacy-0.25.0/upsonic/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25476 2024-05-13 12:25:39.000000 upsonic_legacy-0.25.0/upsonic/remote/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-13 12:25:39.000000 upsonic_legacy-0.25.0/upsonic/remote/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    15387 2024-05-13 12:25:39.000000 upsonic_legacy-0.25.0/upsonic/remote/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:25:48.939026 upsonic_legacy-0.25.0/upsonic/remote/localimport/
--rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-05-13 12:25:39.000000 upsonic_legacy-0.25.0/upsonic/remote/localimport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52330 2024-05-13 12:25:39.000000 upsonic_legacy-0.25.0/upsonic/remote/on_prem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:25:48.939026 upsonic_legacy-0.25.0/upsonic_legacy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-05-13 12:25:48.000000 upsonic_legacy-0.25.0/upsonic_legacy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-13 12:25:48.000000 upsonic_legacy-0.25.0/upsonic_legacy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:25:48.000000 upsonic_legacy-0.25.0/upsonic_legacy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 12:25:48.000000 upsonic_legacy-0.25.0/upsonic_legacy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:25:48.000000 upsonic_legacy-0.25.0/upsonic_legacy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 12:25:48.000000 upsonic_legacy-0.25.0/upsonic_legacy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 12:25:48.000000 upsonic_legacy-0.25.0/upsonic_legacy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:39:02.389407 upsonic_legacy-0.26.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-05-22 15:39:02.389407 upsonic_legacy-0.26.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:39:02.389407 upsonic_legacy-0.26.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:39:02.389407 upsonic_legacy-0.26.0/upsonic/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/upsonic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:39:02.389407 upsonic_legacy-0.26.0/upsonic/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/upsonic/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25476 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/upsonic/remote/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/upsonic/remote/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15387 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/upsonic/remote/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:39:02.389407 upsonic_legacy-0.26.0/upsonic/remote/localimport/
+-rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/upsonic/remote/localimport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17647 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/upsonic/remote/ollama_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52869 2024-05-22 15:38:52.000000 upsonic_legacy-0.26.0/upsonic/remote/on_prem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:39:02.389407 upsonic_legacy-0.26.0/upsonic_legacy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-05-22 15:39:02.000000 upsonic_legacy-0.26.0/upsonic_legacy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-22 15:39:02.000000 upsonic_legacy-0.26.0/upsonic_legacy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:39:02.000000 upsonic_legacy-0.26.0/upsonic_legacy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-22 15:39:02.000000 upsonic_legacy-0.26.0/upsonic_legacy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:39:02.000000 upsonic_legacy-0.26.0/upsonic_legacy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-22 15:39:02.000000 upsonic_legacy-0.26.0/upsonic_legacy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 15:39:02.000000 upsonic_legacy-0.26.0/upsonic_legacy.egg-info/top_level.txt
```

### Comparing `upsonic_legacy-0.25.0/LICENSE` & `upsonic_legacy-0.26.0/LICENSE`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.25.0/PKG-INFO` & `upsonic_legacy-0.26.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upsonic_legacy
-Version: 0.25.0
+Version: 0.26.0
 Summary: Magic Cloud Layer
 Home-page: https://github.com/Upsonic/Upsonic
 Author: Upsonic
 Author-email: onur.atakan.ulusoy@upsonic.co
 License: MIT
 Description: # Upsonic | Self-Driven Autonomous Python Libraries
```

### Comparing `upsonic_legacy-0.25.0/README.md` & `upsonic_legacy-0.26.0/README.md`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.25.0/setup.py` & `upsonic_legacy-0.26.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup
 
 with open('requirements.txt') as fp:
     install_requires = fp.read()
 setup(
     name="upsonic_legacy",
-    version="0.25.0",
+    version="0.26.0",
     description="""Magic Cloud Layer""",
     long_description="".join(open("README.md", encoding="utf-8").readlines()),
     long_description_content_type="text/markdown",
     url="https://github.com/Upsonic/Upsonic",
     author="Upsonic",
     author_email="onur.atakan.ulusoy@upsonic.co",
     license="MIT",
```

### Comparing `upsonic_legacy-0.25.0/upsonic/__init__.py` & `upsonic_legacy-0.26.0/upsonic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,12 +24,12 @@
 from .remote import decrypt
 from .remote import upsonic_serializer
 from .remote import interface
 
 
 open_databases = {}
 
-__version__ = '0.25.0'
+__version__ = '0.26.0'
```

### Comparing `upsonic_legacy-0.25.0/upsonic/remote/__init__.py` & `upsonic_legacy-0.26.0/upsonic/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.25.0/upsonic/remote/controller.py` & `upsonic_legacy-0.26.0/upsonic/remote/controller.py`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.25.0/upsonic/remote/helper.py` & `upsonic_legacy-0.26.0/upsonic/remote/helper.py`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.25.0/upsonic/remote/interface.py` & `upsonic_legacy-0.26.0/upsonic/remote/interface.py`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.25.0/upsonic/remote/localimport/__init__.py` & `upsonic_legacy-0.26.0/upsonic/remote/localimport/__init__.py`

 * *Files identical despite different names*

### Comparing `upsonic_legacy-0.25.0/upsonic/remote/on_prem.py` & `upsonic_legacy-0.26.0/upsonic/remote/on_prem.py`

 * *Files 0% similar despite different names*

```diff
@@ -1507,13 +1507,31 @@
 ```
     
 Do not import the anythink, They are already imported.
     """
 
 
 
+    def return_openai_llm(self, model=None):
+        from langchain_openai import ChatOpenAI
+        import httpx
+        httpx_client = httpx.Client(verify=False)
+
+        llm = ChatOpenAI(openai_api_key=self.password, http_client=httpx_client, openai_api_base=self.api_url+'/openai/', model_name=model)        
+        return llm
+
+
+
+    def return_ollama_llm(self, model=None):
+
+        from .ollama_langchain import Ollama
+
+        llm = Ollama(model=f"{model}**{self.password}", base_url = self.api_url+'/ollama')
+        return llm
+
+
 def Tiger():
     return Upsonic_On_Prem("https://api_tiger.upsonic.co", 'ACK_xmxIiqsgGySvBPPd55M0Ldm5AcR2kt6r3kmL52Ptqo', engine="upsonic_serializer", pass_python_version_check=True)
 
 
 def Tiger_Admin(api_url, access_key):
     return Upsonic_On_Prem(api_url, access_key, engine="upsonic_serializer", pass_python_version_check=True)
```

### Comparing `upsonic_legacy-0.25.0/upsonic_legacy.egg-info/PKG-INFO` & `upsonic_legacy-0.26.0/upsonic_legacy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upsonic-legacy
-Version: 0.25.0
+Version: 0.26.0
 Summary: Magic Cloud Layer
 Home-page: https://github.com/Upsonic/Upsonic
 Author: Upsonic
 Author-email: onur.atakan.ulusoy@upsonic.co
 License: MIT
 Description: # Upsonic | Self-Driven Autonomous Python Libraries
```

### Comparing `upsonic_legacy-0.25.0/upsonic_legacy.egg-info/SOURCES.txt` & `upsonic_legacy-0.26.0/upsonic_legacy.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 ./requirements.txt
 upsonic/__init__.py
 upsonic/remote/__init__.py
 upsonic/remote/controller.py
 upsonic/remote/helper.py
 upsonic/remote/interface.py
+upsonic/remote/ollama_langchain.py
 upsonic/remote/on_prem.py
 upsonic/remote/localimport/__init__.py
 upsonic_legacy.egg-info/PKG-INFO
 upsonic_legacy.egg-info/SOURCES.txt
 upsonic_legacy.egg-info/dependency_links.txt
 upsonic_legacy.egg-info/entry_points.txt
 upsonic_legacy.egg-info/not-zip-safe
```

