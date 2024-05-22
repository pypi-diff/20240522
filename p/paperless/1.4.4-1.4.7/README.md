# Comparing `tmp/paperless-1.4.4.tar.gz` & `tmp/paperless-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paperless-1.4.4.tar", last modified: Mon Feb  5 11:27:31 2024, max compression
+gzip compressed data, was "paperless-1.4.7.tar", last modified: Wed May 22 13:24:17 2024, max compression
```

## Comparing `paperless-1.4.4.tar` & `paperless-1.4.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 11:27:31.646458 paperless-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-05 11:27:19.000000 paperless-1.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-05 11:27:19.000000 paperless-1.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-02-05 11:27:31.646458 paperless-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-02-05 11:27:19.000000 paperless-1.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 11:27:31.646458 paperless-1.4.4/paperless/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 11:27:19.000000 paperless-1.4.4/paperless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-02-05 11:27:19.000000 paperless-1.4.4/paperless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-05 11:27:19.000000 paperless-1.4.4/paperless/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 11:27:31.646458 paperless-1.4.4/paperless/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 11:27:19.000000 paperless-1.4.4/paperless/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-02-05 11:27:19.000000 paperless-1.4.4/paperless/kernels/kernel_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-02-05 11:27:19.000000 paperless-1.4.4/paperless/kernels/kernel_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 11:27:31.646458 paperless-1.4.4/paperless/notebook/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 11:27:19.000000 paperless-1.4.4/paperless/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-02-05 11:27:19.000000 paperless-1.4.4/paperless/notebook/notebook_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-02-05 11:27:19.000000 paperless-1.4.4/paperless/paperless.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 11:27:31.646458 paperless-1.4.4/paperless/serverless/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 11:27:19.000000 paperless-1.4.4/paperless/serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-02-05 11:27:19.000000 paperless-1.4.4/paperless/serverless/serverless_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-05 11:27:19.000000 paperless-1.4.4/paperless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 11:27:31.646458 paperless-1.4.4/paperless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-02-05 11:27:31.000000 paperless-1.4.4/paperless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-02-05 11:27:31.000000 paperless-1.4.4/paperless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 11:27:31.000000 paperless-1.4.4/paperless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-05 11:27:31.000000 paperless-1.4.4/paperless.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-05 11:27:31.000000 paperless-1.4.4/paperless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-05 11:27:31.000000 paperless-1.4.4/paperless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-05 11:27:19.000000 paperless-1.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 11:27:31.646458 paperless-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-02-05 11:27:19.000000 paperless-1.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 11:27:31.646458 paperless-1.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-02-05 11:27:19.000000 paperless-1.4.4/tests/test_e2e_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:17.164464 paperless-1.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-22 13:24:13.000000 paperless-1.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-22 13:24:13.000000 paperless-1.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-22 13:24:17.164464 paperless-1.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-22 13:24:13.000000 paperless-1.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:17.160464 paperless-1.4.7/paperless/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:17.164464 paperless-1.4.7/paperless/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/kernels/kernel_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/kernels/kernel_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:17.164464 paperless-1.4.7/paperless/notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/notebook/notebook_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/paperless.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:17.164464 paperless-1.4.7/paperless/serverless/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/serverless/serverless_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 13:24:13.000000 paperless-1.4.7/paperless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:17.164464 paperless-1.4.7/paperless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-22 13:24:17.000000 paperless-1.4.7/paperless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-22 13:24:17.000000 paperless-1.4.7/paperless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:24:17.000000 paperless-1.4.7/paperless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 13:24:17.000000 paperless-1.4.7/paperless.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-22 13:24:17.000000 paperless-1.4.7/paperless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 13:24:17.000000 paperless-1.4.7/paperless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-22 13:24:13.000000 paperless-1.4.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:24:17.164464 paperless-1.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-22 13:24:13.000000 paperless-1.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:17.164464 paperless-1.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-22 13:24:13.000000 paperless-1.4.7/tests/test_e2e_test.py
```

### Comparing `paperless-1.4.4/LICENSE` & `paperless-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `paperless-1.4.4/PKG-INFO` & `paperless-1.4.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: paperless
-Version: 1.4.4
+Version: 1.4.7
 Summary: A papermill implementation to run notebooks inside dataproc serverless
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: papermill
 Requires-Dist: dataproc_jupyter_plugin
 Requires-Dist: pytest
 Requires-Dist: loguru
 Requires-Dist: gcsfs
 Requires-Dist: click
+Requires-Dist: jupyter_client
 
 # Paperless
 Made With Love ❤️ from  :israel: :israel:      
 
 [Paperless](https://github.com/Plarium-Repo/paperless.git) is a tool that extends the capabilities of [Papermill](https://papermill.readthedocs.io/) by providing the ability to run Papermill via [Google Cloud Dataproc Serverless](https://cloud.google.com/dataproc-serverless/docs).   
 
 [![ICON](https://skillicons.dev/icons?i=gcp,py&perline=3)](https://skillicons.dev) 
@@ -87,19 +88,20 @@
 
 Paperless excepts && supports all list or arguments exists in original [Papermill](https://papermill.readthedocs.io/) package -
 the minimum needed for testing:
 
 ```bash
  paperless <input_path> <output_path> ...
 ``` 
-An extra parameter that is special for Paperless: --template_name
+An extra environment variable  that is special for Paperless:  TEMPLATE_NAME=paperless-interactive
 Example:
 
 ```bash
- paperless ./resources/spark.ipynb ./resources/spark-out.ipynb --template_name paperless-interactive
+ export TEMPLATE_NAME=paperless-interactive && \
+     paperless ./resources/spark.ipynb ./resources/spark-out.ipynb
 
 ```
 
 You're all set, enjoy :)
 
 ----
 
@@ -123,15 +125,15 @@
 # Install requirements
 pip install -r requirements.txt
 
 # Install the command line
 python setup.py install 
 
 # Execute example
-paperless ./resources/spark.ipynb ./resources/spark-out.ipynb
+export TEMPLATE_NAME=paperless-interactive && paperless ./resources/spark.ipynb ./resources/spark-out.ipynb
 
 ```
 
 ---
 [MIT License](LICENSE)
 
 [Contribution](CONTRIBUTION)
```

### Comparing `paperless-1.4.4/README.md` & `paperless-1.4.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -71,19 +71,20 @@
 
 Paperless excepts && supports all list or arguments exists in original [Papermill](https://papermill.readthedocs.io/) package -
 the minimum needed for testing:
 
 ```bash
  paperless <input_path> <output_path> ...
 ``` 
-An extra parameter that is special for Paperless: --template_name
+An extra environment variable  that is special for Paperless:  TEMPLATE_NAME=paperless-interactive
 Example:
 
 ```bash
- paperless ./resources/spark.ipynb ./resources/spark-out.ipynb --template_name paperless-interactive
+ export TEMPLATE_NAME=paperless-interactive && \
+     paperless ./resources/spark.ipynb ./resources/spark-out.ipynb
 
 ```
 
 You're all set, enjoy :)
 
 ----
 
@@ -107,15 +108,15 @@
 # Install requirements
 pip install -r requirements.txt
 
 # Install the command line
 python setup.py install 
 
 # Execute example
-paperless ./resources/spark.ipynb ./resources/spark-out.ipynb
+export TEMPLATE_NAME=paperless-interactive && paperless ./resources/spark.ipynb ./resources/spark-out.ipynb
 
 ```
 
 ---
 [MIT License](LICENSE)
 
 [Contribution](CONTRIBUTION)
```

### Comparing `paperless-1.4.4/paperless/__main__.py` & `paperless-1.4.7/paperless/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 from collections import OrderedDict
 import inspect
+import os
 import sys
 from pydoc import cli
 import papermill
 import click
 from loguru import logger
 from paperless.paperless import Paperless
 
@@ -23,22 +24,20 @@
     Args:
         *args: Positional arguments passed to the Paperless application.
         **kwargs: Keyword arguments passed to the Paperless application.
 
     Returns:
         The result of executing the Paperless application.
     """
-    template_name = None 
-    if 'template_name' in kwargs:
-        template_name = kwargs['template_name']
-    logger.info("paperless execution started!")
+    template_name = os.getenv("TEMPLATE_NAME", "")
+    logger.info("paperless execution started! with template_name: {template_name}", template_name=template_name)
     return Paperless(notebookPath=kwargs['input_path'], \
                      templateName=template_name).\
         configure().\
-        wait_for_session().\
+        build_session().\
         verify().\
         execute(args,kwargs).\
         shutdown()
     
 
 # replace the execute_notebook function with the PaperlessExecuter
 module = sys.modules["papermill.execute"]
```

### Comparing `paperless-1.4.4/paperless/kernels/kernel_client.py` & `paperless-1.4.7/paperless/kernels/kernel_client.py`

 * *Files identical despite different names*

### Comparing `paperless-1.4.4/paperless/kernels/kernel_manager.py` & `paperless-1.4.7/paperless/kernels/kernel_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from .kernel_client import ServerlessGatewayKernelClient
 
 
 class ServerlessMixingKernelManager(MixingKernelManager):
 
     def __init__(self, c_kernel, c_kernel_spec,  *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.kernel_id = c_kernel[0]['id']
+        self.kernel_id = c_kernel['id']
         self.kernel_name = c_kernel_spec['default']
         self.remote_manager =  ServerlessGatewayKernelClient(
             kernel_id=self.kernel_id ,
             parent=self,
             log=self.log,
             connection_file=self.connection_file,
             kernel_spec_manager=MixingKernelSpecManager(*args, **kwargs))
```

### Comparing `paperless-1.4.4/paperless/paperless.py` & `paperless-1.4.7/paperless/paperless.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import asyncio
 import uuid
 import papermill as pm
 from loguru import logger
 from .kernels.kernel_manager import ServerlessMixingKernelManager
 from jupyter_server.gateway.gateway_client import GatewayClient
 
-from tornado.escape import json_decode
+from tornado.escape import json_decode, json_encode
 from jupyter_server.gateway.gateway_client import gateway_request
 from jupyter_server.utils import url_path_join
 from dataproc_jupyter_plugin.handlers import get_cached_credentials
 from google.cloud.jupyter_config.config import gcp_kernel_gateway_url
 from papermill.iorw import papermill_io
 
 from paperless.constants import *
@@ -52,30 +52,27 @@
 
         metadata = self.notebook['metadata']
         
         # get session id from notebook metadata
         if METADATA_KEY in metadata and  serverless_manager.\
             is_session_active_and_ready(metadata[METADATA_KEY]["session_id"]):
             logger.debug("found metadata in notebook: ", metadata[METADATA_KEY])
-            self.sessionid = metadata[METADATA_KEY]["session_id"]
+            self.dataproc_sessionid = metadata[METADATA_KEY]["session_id"]
             self.kernel_name = metadata[METADATA_KEY]["kernel_name"]
             self.session_template = metadata[METADATA_KEY]["session_template"]
             self.session_exists = True
             self.session_ready = False
         else:
             logger.debug("no metadata found in notebook, generating new session")
-            self.sessionid = str(uuid.uuid4())
-            self.kernel_name =  f"paperless-{self.sessionid}"
 
             if templateName is not None:
                 self.session_template =  serverless_manager.build_session_template(templateName)
             else: 
-                serverless_manager.build_session_template()
-            self.notebook['metadata'][METADATA_KEY] = {"session_id": self.sessionid, "kernel_name": self.kernel_name, "session_template": self.session_template}
-            notebook_manager.save_notebook(self.notebook, self.notebook_path)
+                self.session_template = serverless_manager.build_session_template()
+
             logger.debug("saved new notebook with metadata")
             self.session_exists = False
             self.session_ready = False
 
         self.crad = get_cached_credentials(log=None)
         logger.debug("got credentials - ready", self.crad)
 
@@ -91,37 +88,36 @@
         GatewayClient.instance().kernel_ws_protocol=""
         GatewayClient.instance().auth_scheme = 'Bearer'
         GatewayClient.instance().auth_token = self.crad["access_token"]
         GatewayClient.instance().headers = '{"Cookie": "_xsrf=XSRF", "X-XSRFToken": "XSRF","authorization":"Bearer ' + self.crad["access_token"] + '"}'
         logger.debug("configured gateway client")
         return self
 
-    def wait_for_session(self):
+    def build_session(self):
         """
-        Waits for the session to be available and saves the notebook with session metadata.
+        Verifies the session by getting the kernel spec and preparing the kernel.
 
         Returns:
             self: The current instance of the InteractiveSession class.
         """
-        ## getting session
-        logger.debug("waiting for session")
-        if not self.session_exists:
-            serverless_manager.create_session(sessionid=self.sessionid, templateName=self.session_template)
-        logger.debug("session created")
+        asyncio.run(self.get_kernel_spec())
+        asyncio.run(self.prepare_the_kernel())
+        logger.debug("building session with kernel: ", self.kernel)
+        self.dataproc_sessionid = serverless_manager.recognize_dataproc_sessionid(self.kernel.get("metadata"))
+        logger.debug("dataproc session id: ", self.dataproc_sessionid)
+        self.notebook['metadata'][METADATA_KEY] = {"session_id": self.dataproc_sessionid, "kernel_name": self.kernel.get("name"), "session_template": self.session_template, "kernel_name_e": \
+                                                   self.kernel.get("kernel_name_e"), "kernel_id_e": self.kernel.get("id") }
+        
+        notebook_manager.save_notebook(self.notebook, self.notebook_path)
+        logger.debug("saved notebook with metadata")
         return self
 
     def verify(self):
-        """
-        Verifies the session by getting the kernel spec and preparing the kernel.
 
-        Returns:
-            self: The current instance of the InteractiveSession class.
-        """
-        asyncio.run(self.get_kernel_spec())
-        asyncio.run(self.prepare_the_kernel())
+        serverless_manager.wait_til_ready(self.dataproc_sessionid)
         return self
 
     def execute(self, *args, **kwargs):
         """
         Executes the notebook.
 
         Returns:
@@ -136,16 +132,15 @@
         pm.execute_notebook(**kwargs)
         return self
     
     def shutdown(self):
         """
         Shuts down the session.
         """
-        # serverless_manager.delete_session(sessionid=self.sessionid)
-        # sys.exit()
+        serverless_manager.delete_session(sessionid=self.dataproc_sessionid)
 
     async def get_kernel_spec(self):
         """
         Gets the kernel spec.
         """
         kernelspec_url = url_path_join(GatewayClient.instance().url, GatewayClient.instance().kernelspecs_endpoint)
         response = await gateway_request(
@@ -157,18 +152,49 @@
         logger.debug(self.kernel_spec)
         return self.kernel_spec
 
     async def prepare_the_kernel(self):
         """
         Prepares the kernel.
         """
+        notebook_metadata = self.notebook['metadata']
+        endpoint_kernels = await self.get_kernels()
+        if endpoint_kernels is not None and len(endpoint_kernels) > 0:
+            if METADATA_KEY in notebook_metadata:
+                kernel = next((x for x in endpoint_kernels if x["id"] == notebook_metadata[METADATA_KEY]["kernel_id_e"]), None)
+                if kernel is not None:
+                    self.kernel = kernel
+                    return self.kernel
+                else:
+                    return await self.build_kernel()
+            else:
+                self.kernel = endpoint_kernels[0]
+                return self.kernel  
+        else:   
+            return await self.build_kernel()
+        
+    async def build_kernel(self):
+        try:
+            kernels_url = url_path_join(GatewayClient.instance().url, GatewayClient.instance().kernels_endpoint)
+            start_responed = await gateway_request(
+                kernels_url,
+                method="POST",
+                body=json_encode({ "name": self.kernel_spec.get("default")}),
+                headers={"Content-Type": "application/json","Cookie": "_xsrf=XSRF", "X-XSRFToken": "XSRF","authorization":"Bearer " + self.crad["access_token"]},
+            )
+            self.kernel = json_decode(start_responed.body)
+            return self.kernel
+        except Exception as e:
+            logger.error(e)
+            raise e
+ 
+    async def get_kernels(self):
+        """
+        Gets the kernel.
+        """
         kernels_url = url_path_join(GatewayClient.instance().url, GatewayClient.instance().kernels_endpoint)
         response = await gateway_request(
             kernels_url,
             method="GET",
             headers={"Content-Type": "application/json"},
         )
-        self.kernel = json_decode(response.body)
-        logger.debug(self.kernel)
-        return self.kernel
-        
- 
+        return json_decode(response.body)
```

### Comparing `paperless-1.4.4/paperless/serverless/serverless_manager.py` & `paperless-1.4.7/paperless/serverless/serverless_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 
 
 
 import subprocess
+import time
 from loguru import logger
 from tornado.escape import json_decode
 import paperless.constants as constants
 from google.cloud.jupyter_config.config import gcp_project, gcp_region
 
 def build_session_template(templateName=constants.DEFAULT_SESSION_TEMPLATE_NAME):
     project_id = gcp_project()
     region = gcp_region()
     return f"projects/{project_id}/regions/{region}/sessionTemplates/{templateName}"
 
+def recognize_dataproc_sessionid(metadata):
+    endpointParentResource = metadata.get("endpointParentResource")
+    return endpointParentResource.split("/")[-1]
+
+def wait_til_ready(sessionid):
+    logger.debug("waiting for session to be ready")
+    while not is_session_active_and_ready(sessionid):
+        logger.debug("session is not ready, waiting for 5 seconds")
+        time.sleep(5)
+    logger.debug("session is ready")
+
 def is_session_active_and_ready(sessionid):
     logger.debug("checking if session is active and ready")
     session = get_session(sessionid)
     if session and session["state"] == "ACTIVE":
         logger.debug("session is active and ready")
         return True
     else:
```

### Comparing `paperless-1.4.4/paperless.egg-info/PKG-INFO` & `paperless-1.4.7/paperless.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: paperless
-Version: 1.4.4
+Version: 1.4.7
 Summary: A papermill implementation to run notebooks inside dataproc serverless
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: papermill
 Requires-Dist: dataproc_jupyter_plugin
 Requires-Dist: pytest
 Requires-Dist: loguru
 Requires-Dist: gcsfs
 Requires-Dist: click
+Requires-Dist: jupyter_client
 
 # Paperless
 Made With Love ❤️ from  :israel: :israel:      
 
 [Paperless](https://github.com/Plarium-Repo/paperless.git) is a tool that extends the capabilities of [Papermill](https://papermill.readthedocs.io/) by providing the ability to run Papermill via [Google Cloud Dataproc Serverless](https://cloud.google.com/dataproc-serverless/docs).   
 
 [![ICON](https://skillicons.dev/icons?i=gcp,py&perline=3)](https://skillicons.dev) 
@@ -87,19 +88,20 @@
 
 Paperless excepts && supports all list or arguments exists in original [Papermill](https://papermill.readthedocs.io/) package -
 the minimum needed for testing:
 
 ```bash
  paperless <input_path> <output_path> ...
 ``` 
-An extra parameter that is special for Paperless: --template_name
+An extra environment variable  that is special for Paperless:  TEMPLATE_NAME=paperless-interactive
 Example:
 
 ```bash
- paperless ./resources/spark.ipynb ./resources/spark-out.ipynb --template_name paperless-interactive
+ export TEMPLATE_NAME=paperless-interactive && \
+     paperless ./resources/spark.ipynb ./resources/spark-out.ipynb
 
 ```
 
 You're all set, enjoy :)
 
 ----
 
@@ -123,15 +125,15 @@
 # Install requirements
 pip install -r requirements.txt
 
 # Install the command line
 python setup.py install 
 
 # Execute example
-paperless ./resources/spark.ipynb ./resources/spark-out.ipynb
+export TEMPLATE_NAME=paperless-interactive && paperless ./resources/spark.ipynb ./resources/spark-out.ipynb
 
 ```
 
 ---
 [MIT License](LICENSE)
 
 [Contribution](CONTRIBUTION)
```

### Comparing `paperless-1.4.4/paperless.egg-info/SOURCES.txt` & `paperless-1.4.7/paperless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paperless-1.4.4/setup.py` & `paperless-1.4.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 setup(
     name="paperless",
-    version="1.4.4",
+    version="1.4.7",
     description="A papermill implementation to run notebooks inside dataproc serverless",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     py_modules = ['paperless', 'app'],
     python_requires=">=3.10",
     packages=find_packages(exclude=("tests",)),
```

