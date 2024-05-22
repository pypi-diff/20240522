# Comparing `tmp/gen_wrappers-0.4.8.tar.gz` & `tmp/gen_wrappers-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.4.8.tar", last modified: Wed May 22 20:56:13 2024, max compression
+gzip compressed data, was "gen_wrappers-0.4.9.tar", last modified: Wed May 22 21:04:33 2024, max compression
```

## Comparing `gen_wrappers-0.4.8.tar` & `gen_wrappers-0.4.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 20:56:13.932519 gen_wrappers-0.4.8/
--rw-rw-rw-   0        0        0      847 2024-05-22 20:56:13.931518 gen_wrappers-0.4.8/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-05-20 15:06:29.000000 gen_wrappers-0.4.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 20:56:13.689211 gen_wrappers-0.4.8/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.4.8/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 20:56:13.718012 gen_wrappers-0.4.8/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.4.8/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     7124 2024-05-20 18:57:41.000000 gen_wrappers-0.4.8/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     4055 2024-05-14 16:10:12.000000 gen_wrappers-0.4.8/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.4.8/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-22 20:56:13.756276 gen_wrappers-0.4.8/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.4.8/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1641 2024-05-20 18:57:41.000000 gen_wrappers-0.4.8/creator/base/base_app.py
--rw-rw-rw-   0        0        0      673 2024-05-20 18:57:41.000000 gen_wrappers-0.4.8/creator/base/base_request.py
--rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.4.8/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.4.8/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-22 20:56:13.808941 gen_wrappers-0.4.8/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.4.8/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0    11700 2024-05-20 18:57:41.000000 gen_wrappers-0.4.8/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0    16233 2024-05-20 17:09:18.000000 gen_wrappers-0.4.8/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.4.8/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-22 20:56:13.853939 gen_wrappers-0.4.8/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.4.8/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6899 2024-05-20 19:10:38.000000 gen_wrappers-0.4.8/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     6112 2024-05-22 20:55:15.000000 gen_wrappers-0.4.8/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.4.8/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-22 20:56:13.884794 gen_wrappers-0.4.8/creator/util/
--rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.4.8/creator/util/__init__.py
--rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.4.8/creator/util/helper.py
-drwxrwxrwx   0        0        0        0 2024-05-22 20:56:13.929520 gen_wrappers-0.4.8/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      847 2024-05-22 20:56:13.000000 gen_wrappers-0.4.8/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      768 2024-05-22 20:56:13.000000 gen_wrappers-0.4.8/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 20:56:13.000000 gen_wrappers-0.4.8/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-22 20:56:13.000000 gen_wrappers-0.4.8/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-22 20:56:13.000000 gen_wrappers-0.4.8/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 20:56:13.932519 gen_wrappers-0.4.8/setup.cfg
--rw-rw-rw-   0        0        0     1035 2024-05-22 20:56:07.000000 gen_wrappers-0.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:04:33.147000 gen_wrappers-0.4.9/
+-rw-rw-rw-   0        0        0      847 2024-05-22 21:04:33.145996 gen_wrappers-0.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2024-05-20 15:06:29.000000 gen_wrappers-0.4.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 21:04:33.092680 gen_wrappers-0.4.9/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.4.9/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:04:33.101620 gen_wrappers-0.4.9/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.4.9/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     7124 2024-05-20 18:57:41.000000 gen_wrappers-0.4.9/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     4055 2024-05-14 16:10:12.000000 gen_wrappers-0.4.9/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.4.9/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:04:33.110638 gen_wrappers-0.4.9/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.4.9/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1641 2024-05-20 18:57:41.000000 gen_wrappers-0.4.9/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      673 2024-05-20 18:57:41.000000 gen_wrappers-0.4.9/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.4.9/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.4.9/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:04:33.117409 gen_wrappers-0.4.9/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.4.9/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0    11700 2024-05-20 18:57:41.000000 gen_wrappers-0.4.9/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0    16233 2024-05-20 17:09:18.000000 gen_wrappers-0.4.9/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.4.9/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:04:33.121982 gen_wrappers-0.4.9/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.4.9/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     7207 2024-05-22 21:04:16.000000 gen_wrappers-0.4.9/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     6112 2024-05-22 20:55:15.000000 gen_wrappers-0.4.9/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.4.9/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:04:33.124949 gen_wrappers-0.4.9/creator/util/
+-rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.4.9/creator/util/__init__.py
+-rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.4.9/creator/util/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:04:33.144996 gen_wrappers-0.4.9/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-05-22 21:04:32.000000 gen_wrappers-0.4.9/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      768 2024-05-22 21:04:32.000000 gen_wrappers-0.4.9/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 21:04:32.000000 gen_wrappers-0.4.9/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-22 21:04:32.000000 gen_wrappers-0.4.9/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-22 21:04:32.000000 gen_wrappers-0.4.9/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 21:04:33.147999 gen_wrappers-0.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2024-05-22 21:04:24.000000 gen_wrappers-0.4.9/setup.py
```

### Comparing `gen_wrappers-0.4.8/PKG-INFO` & `gen_wrappers-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.4.8
+Version: 0.4.9
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.4.8/creator/auto/creator_auto.py` & `gen_wrappers-0.4.9/creator/auto/creator_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.8/creator/auto/request_auto.py` & `gen_wrappers-0.4.9/creator/auto/request_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.8/creator/auto/response_auto.py` & `gen_wrappers-0.4.9/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.8/creator/base/base_app.py` & `gen_wrappers-0.4.9/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.8/creator/base/base_request.py` & `gen_wrappers-0.4.9/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.8/creator/base/base_response.py` & `gen_wrappers-0.4.9/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.8/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.4.9/creator/cmfy/creator_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.8/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.4.9/creator/cmfy/request_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.8/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.4.9/creator/fcus_api/creator_fcus_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,38 +7,40 @@
 import httpx
 import requests
 
 from creator.base.base_app import BaseApp
 from creator.base.base_request import BaseRequest, CacheModelRequest, UploadImageRequest
 from creator.base.base_response import BaseResponse, ResponseDataType, ResponseData
 from creator.base.job_status import JobStatus
-from creator.fcus_api.request_fcus_api import FcusTxt2Img, FcusUpscaleOrVary, FcusInpaintOrOutpaint
+from creator.fcus_api.request_fcus_api import FcusTxt2Img, FcusUpscaleOrVary, FcusInpaintOrOutpaint, FcusImagePrompt
 from creator.fcus_api.response_fcus_api import ResponseFcusApi
 
 logger = logging.getLogger(__name__)
 
 
 class AppFcusApi(BaseApp):
-    param_classes = [FcusTxt2Img, FcusUpscaleOrVary, FcusInpaintOrOutpaint]
+    param_classes = [FcusTxt2Img, FcusUpscaleOrVary, FcusInpaintOrOutpaint, FcusImagePrompt]
     output = {}
 
     def __init__(self):
         super().__init__()
         focus_port = os.environ.get("PORT_FCUS_API", 8888)
         if isinstance(focus_port, str):
             focus_port = int(focus_port)
         self.api_base_url = f"http://0.0.0.0:{focus_port}"
 
-    async def create(self, params: Union[FcusTxt2Img, FcusUpscaleOrVary, FcusInpaintOrOutpaint]) -> BaseResponse:
+    async def create(self, params: Union[FcusTxt2Img, FcusUpscaleOrVary, FcusInpaintOrOutpaint, FcusImagePrompt]) -> BaseResponse:
         if isinstance(params, FcusTxt2Img):
             url = f"{self.api_base_url}/v1/generation/text-to-image"
         elif isinstance(params, FcusUpscaleOrVary):
             url = f"{self.api_base_url}/v1/generation/image-upscale-vary"
         elif isinstance(params, FcusInpaintOrOutpaint):
             url = f"{self.api_base_url}/v1/generation/image-inpaint-outpaint"
+        elif isinstance(params, FcusImagePrompt):
+            url = f"{self.api_base_url}/v1/generation/image-prompt"
         else:
             raise ValueError("Invalid parameters for creation")
 
         data = json.dumps(params.__dict__)
         headers = {'Content-Type': 'application/json'}
         response = requests.post(url, data=data, headers=headers)
         # If we have a 422 here, print what the unprocessable entity is
@@ -57,24 +59,26 @@
                 output = await self._get_output(job_id)
                 job_count += 1
                 if output is None:
                     await asyncio.sleep(1)
             response_data = ResponseData(data=output, data_type=ResponseDataType.IMAGE, total_count=len(output))
             return ResponseFcusApi(status="Job Finished", output=response_data, job_id=job_id)
 
-    async def create_async(self, params: Union[FcusTxt2Img, FcusUpscaleOrVary, FcusInpaintOrOutpaint]) -> BaseResponse:
+    async def create_async(self, params: Union[FcusTxt2Img, FcusUpscaleOrVary, FcusInpaintOrOutpaint, FcusImagePrompt]) -> BaseResponse:
         if isinstance(params, FcusTxt2Img):
             model = params.base_model_name
             url = f"{self.api_base_url}/v1/generation/text-to-image"
         elif isinstance(params, FcusUpscaleOrVary):
             model = params.base_model_name
             url = f"{self.api_base_url}/v1/generation/image-upscale-vary"
         elif isinstance(params, FcusInpaintOrOutpaint):
             model = params.base_model_name
             url = f"{self.api_base_url}/v1/generation/image-inpaint-outpaint"
+        elif isinstance(params, FcusImagePrompt):
+            url = f"{self.api_base_url}/v1/generation/image-prompt"
         else:
             raise ValueError("Invalid parameters for creation")
         if model is not None and model not in self.loaded_models:
             self.loaded_models.append(model)
         max_cached_models = os.environ.get("MAX_CACHED_MODELS", 3)
         if len(self.loaded_models) > max_cached_models:
             self.loaded_models = self.loaded_models[-max_cached_models:]
```

### Comparing `gen_wrappers-0.4.8/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.4.9/creator/fcus_api/request_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.8/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.4.9/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.8/creator/util/helper.py` & `gen_wrappers-0.4.9/creator/util/helper.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.8/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.4.9/gen_wrappers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.4.8
+Version: 0.4.9
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.4.8/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.4.9/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

