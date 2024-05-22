# Comparing `tmp/jupyter_server_terminals_proxy-0.1.4.tar.gz` & `tmp/jupyter_server_terminals_proxy-0.2.0.tar.gz`

## Comparing `jupyter_server_terminals_proxy-0.1.4.tar` & `jupyter_server_terminals_proxy-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,9 @@
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 jupyter_server_terminals_proxy-0.1.4/Untitled.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_server_terminals_proxy-0.1.4/fps.log
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_server_terminals_proxy-0.1.4/fps_cli_args.toml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 jupyter_server_terminals_proxy-0.1.4/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 jupyter_server_terminals_proxy-0.1.4/jupyter-config/jupyter_server_terminals_proxy.json
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 jupyter_server_terminals_proxy-0.1.4/jupyter_server_terminals_proxy/__init__.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 jupyter_server_terminals_proxy-0.1.4/jupyter_server_terminals_proxy/api_handlers.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 jupyter_server_terminals_proxy-0.1.4/jupyter_server_terminals_proxy/app.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 jupyter_server_terminals_proxy-0.1.4/jupyter_server_terminals_proxy/handlers.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 jupyter_server_terminals_proxy-0.1.4/jupyter_server_terminals_proxy/.ipynb_checkpoints/handlers-checkpoint.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 jupyter_server_terminals_proxy-0.1.4/LICENSE
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 jupyter_server_terminals_proxy-0.1.4/README.md
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 jupyter_server_terminals_proxy-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 jupyter_server_terminals_proxy-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 jupyter_server_terminals_proxy-0.2.0/jupyter-config/jupyter_server_terminals_proxy.json
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 jupyter_server_terminals_proxy-0.2.0/jupyter_server_terminals_proxy/__init__.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 jupyter_server_terminals_proxy-0.2.0/jupyter_server_terminals_proxy/api_handlers.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 jupyter_server_terminals_proxy-0.2.0/jupyter_server_terminals_proxy/app.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 jupyter_server_terminals_proxy-0.2.0/jupyter_server_terminals_proxy/handlers.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 jupyter_server_terminals_proxy-0.2.0/LICENSE
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 jupyter_server_terminals_proxy-0.2.0/README.md
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 jupyter_server_terminals_proxy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 jupyter_server_terminals_proxy-0.2.0/PKG-INFO
```

### Comparing `jupyter_server_terminals_proxy-0.1.4/jupyter_server_terminals_proxy/api_handlers.py` & `jupyter_server_terminals_proxy-0.2.0/jupyter_server_terminals_proxy/api_handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_terminals_proxy-0.1.4/jupyter_server_terminals_proxy/app.py` & `jupyter_server_terminals_proxy-0.2.0/jupyter_server_terminals_proxy/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,10 +22,7 @@
                 handlers.TermSocket,
             )
         )
         self.handlers.extend(api_handlers.default_handlers)
         self.serverapp.web_app.settings["terminals_available"] = self.settings[
             "terminals_available"
         ]
-        #print(f"{self.serverapp.terminals_enabled=}")
-        #self.serverapp.terminals_enabled = False
-
```

### Comparing `jupyter_server_terminals_proxy-0.1.4/LICENSE` & `jupyter_server_terminals_proxy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_server_terminals_proxy-0.1.4/pyproject.toml` & `jupyter_server_terminals_proxy-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["hatchling>=1.5"]
+requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyter_server_terminals_proxy"
 readme = "README.md"
 dynamic = ["version"]
 license = { file = "LICENSE" }
@@ -11,25 +11,26 @@
 keywords = ["ipython", "jupyter"]
 classifiers = [
   "Intended Audience :: Developers",
   "Intended Audience :: System Administrators",
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
-  "jupyter_server>=1.0.0",
-  "httpx>=0.23.1",
-  "websockets>=10.4",
+  "anyio >=4.3.0,<5.0.0",
+  "httpx >=0.27.0,<0.28",
+  "httpx-ws >=0.6.0,<0.7.0",
+  "jupyter_server >=1.0.0,<3.0.0",
 ]
 
 [[project.authors]]
 name = "David Brochart"
 email = "david.brochart@gmail.com"
 
 [project.urls]
```

### Comparing `jupyter_server_terminals_proxy-0.1.4/PKG-INFO` & `jupyter_server_terminals_proxy-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jupyter_server_terminals_proxy
-Version: 0.1.4
+Version: 0.2.0
 Summary: A Jupyter Server Extension Proxying Terminals.
 Project-URL: Homepage, https://github.com/davidbrochart/jupyter_server_terminals_proxy
 Author-email: David Brochart <david.brochart@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 David Brochart
         
@@ -28,42 +28,43 @@
 License-File: LICENSE
 Keywords: ipython,jupyter
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Requires-Dist: httpx>=0.23.1
-Requires-Dist: jupyter-server>=1.0.0
-Requires-Dist: websockets>=10.4
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Requires-Dist: anyio<5.0.0,>=4.3.0
+Requires-Dist: httpx-ws<0.7.0,>=0.6.0
+Requires-Dist: httpx<0.28,>=0.27.0
+Requires-Dist: jupyter-server<3.0.0,>=1.0.0
 Description-Content-Type: text/markdown
 
 # Jupyter Server Terminals Proxy
 
 In one terminal/environment:
 
 ```console
-pip install fps_uvicorn
-pip install fps_terminals
+pip install jupyverse-api
+pip install fps-terminals
 pip install fps-noauth
 
 # launch a terminal server at http://127.0.0.1:8000
-fps-uvicorn --port=8000 --no-open-browser
+jupyverse --port=8000
 ```
 
 In another terminal/environment:
 
 ```console
 pip install jupyter_server_terminals_proxy
 pip install jupyterlab
 
 # launch JupyterLab at http://127.0.0.1:8888 and proxy terminals at http://127.0.0.1:8000
-jupyter lab --port=8888 --ServerApp.terminals_enabled=False --TerminalsProxyExtensionApp.proxy_url='http://127.0.0.1:8000'
+jupyter lab --port=8888 --ServerApp.jpserver_extensions=jupyter_server_terminals=False --TerminalsProxyExtensionApp.proxy_url='http://127.0.0.1:8000'
 ```
 
 Terminals should now be served from http://127.0.0.1:8000.
```

