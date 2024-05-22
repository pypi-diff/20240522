# Comparing `tmp/gen_wrappers-0.4.7.tar.gz` & `tmp/gen_wrappers-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.4.7.tar", last modified: Mon May 20 19:01:52 2024, max compression
+gzip compressed data, was "gen_wrappers-0.4.8.tar", last modified: Wed May 22 20:56:13 2024, max compression
```

## Comparing `gen_wrappers-0.4.7.tar` & `gen_wrappers-0.4.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 19:01:52.739798 gen_wrappers-0.4.7/
--rw-rw-rw-   0        0        0      847 2024-05-20 19:01:52.737777 gen_wrappers-0.4.7/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-05-20 15:06:29.000000 gen_wrappers-0.4.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 19:01:52.630189 gen_wrappers-0.4.7/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.4.7/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:01:52.650124 gen_wrappers-0.4.7/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.4.7/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     7124 2024-05-20 18:57:41.000000 gen_wrappers-0.4.7/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     4055 2024-05-14 16:10:12.000000 gen_wrappers-0.4.7/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.4.7/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:01:52.675563 gen_wrappers-0.4.7/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.4.7/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1641 2024-05-20 18:57:41.000000 gen_wrappers-0.4.7/creator/base/base_app.py
--rw-rw-rw-   0        0        0      673 2024-05-20 18:57:41.000000 gen_wrappers-0.4.7/creator/base/base_request.py
--rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.4.7/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.4.7/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:01:52.687877 gen_wrappers-0.4.7/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.4.7/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0    11700 2024-05-20 18:57:41.000000 gen_wrappers-0.4.7/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0    16233 2024-05-20 17:09:18.000000 gen_wrappers-0.4.7/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.4.7/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:01:52.697113 gen_wrappers-0.4.7/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.4.7/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6909 2024-05-20 18:57:41.000000 gen_wrappers-0.4.7/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3934 2024-05-20 16:34:32.000000 gen_wrappers-0.4.7/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.4.7/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:01:52.700636 gen_wrappers-0.4.7/creator/util/
--rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.4.7/creator/util/__init__.py
--rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.4.7/creator/util/helper.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:01:52.734796 gen_wrappers-0.4.7/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      847 2024-05-20 19:01:52.000000 gen_wrappers-0.4.7/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      768 2024-05-20 19:01:52.000000 gen_wrappers-0.4.7/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 19:01:52.000000 gen_wrappers-0.4.7/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-20 19:01:52.000000 gen_wrappers-0.4.7/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-20 19:01:52.000000 gen_wrappers-0.4.7/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 19:01:52.740778 gen_wrappers-0.4.7/setup.cfg
--rw-rw-rw-   0        0        0     1035 2024-05-20 18:57:59.000000 gen_wrappers-0.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:56:13.932519 gen_wrappers-0.4.8/
+-rw-rw-rw-   0        0        0      847 2024-05-22 20:56:13.931518 gen_wrappers-0.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2024-05-20 15:06:29.000000 gen_wrappers-0.4.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 20:56:13.689211 gen_wrappers-0.4.8/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.4.8/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:56:13.718012 gen_wrappers-0.4.8/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.4.8/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     7124 2024-05-20 18:57:41.000000 gen_wrappers-0.4.8/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     4055 2024-05-14 16:10:12.000000 gen_wrappers-0.4.8/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.4.8/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:56:13.756276 gen_wrappers-0.4.8/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.4.8/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1641 2024-05-20 18:57:41.000000 gen_wrappers-0.4.8/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      673 2024-05-20 18:57:41.000000 gen_wrappers-0.4.8/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.4.8/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.4.8/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:56:13.808941 gen_wrappers-0.4.8/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.4.8/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0    11700 2024-05-20 18:57:41.000000 gen_wrappers-0.4.8/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0    16233 2024-05-20 17:09:18.000000 gen_wrappers-0.4.8/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.4.8/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:56:13.853939 gen_wrappers-0.4.8/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.4.8/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6899 2024-05-20 19:10:38.000000 gen_wrappers-0.4.8/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     6112 2024-05-22 20:55:15.000000 gen_wrappers-0.4.8/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.4.8/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:56:13.884794 gen_wrappers-0.4.8/creator/util/
+-rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.4.8/creator/util/__init__.py
+-rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.4.8/creator/util/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:56:13.929520 gen_wrappers-0.4.8/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-05-22 20:56:13.000000 gen_wrappers-0.4.8/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      768 2024-05-22 20:56:13.000000 gen_wrappers-0.4.8/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 20:56:13.000000 gen_wrappers-0.4.8/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-22 20:56:13.000000 gen_wrappers-0.4.8/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-22 20:56:13.000000 gen_wrappers-0.4.8/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 20:56:13.932519 gen_wrappers-0.4.8/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2024-05-22 20:56:07.000000 gen_wrappers-0.4.8/setup.py
```

### Comparing `gen_wrappers-0.4.7/PKG-INFO` & `gen_wrappers-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.4.7
+Version: 0.4.8
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.4.7/creator/auto/creator_auto.py` & `gen_wrappers-0.4.8/creator/auto/creator_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.7/creator/auto/request_auto.py` & `gen_wrappers-0.4.8/creator/auto/request_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.7/creator/auto/response_auto.py` & `gen_wrappers-0.4.8/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.7/creator/base/base_app.py` & `gen_wrappers-0.4.8/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.7/creator/base/base_request.py` & `gen_wrappers-0.4.8/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.7/creator/base/base_response.py` & `gen_wrappers-0.4.8/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.7/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.4.8/creator/cmfy/creator_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.7/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.4.8/creator/cmfy/request_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.7/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.4.8/creator/fcus_api/creator_fcus_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
                 return []
             outputs = [result.get('base64') for result in response_json.get('job_result', []) if result.get('finish_reason', "UNKNOWN") == "SUCCESS"]
             return outputs
 
     async def cache_model(self, req: CacheModelRequest) -> bool:
         # FCUS_API doesn't have a specific endpoint for caching models, so we just
         # Run a txt2img job with a very low resolution to load the model
-        request = FcusTxt2Img().example()
+        request = FcusTxt2Img()
         request.prompt = "foo"
         request.base_model_name = req.model
         request.aspect_ratios_selection = "64*64"
         response = await self.create(request)
         if response.status == JobStatus.FINISHED:
             return True
         return False
```

### Comparing `gen_wrappers-0.4.7/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.4.8/creator/fcus_api/request_fcus_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from dataclasses import dataclass, field
-from typing import List, Dict, Optional
+from dataclasses import dataclass
+from typing import List, Optional
 
-from pydantic import BaseModel, Field
+from pydantic import Field
 
 from creator.base.base_request import BaseRequest
 
 
 @dataclass
 class FcusAdvancedParams:
     adm_scaler_positive: float = 1.5
@@ -41,15 +41,16 @@
     model_name: str = ""
     weight: float = 1.0
 
 
 class FcusTxt2Img(BaseRequest):
     prompt: str = ""
     negative_prompt: str = ""
-    style_selections: List[str] = Field(default_factory=list, examples=[["Fooocus V2", "Fooocus Enhance", "Fooocus Sharp"]])
+    style_selections: List[str] = Field(default_factory=list,
+                                        examples=[["Fooocus V2", "Fooocus Enhance", "Fooocus Sharp"]])
     performance_selection: str = "Speed"
     aspect_ratios_selection: str = "1152*896"
     image_number: int = 2
     image_seed: int = -1
     sharpness: float = 0.0
     guidance_scale: float = 7.5
     base_model_name: str = "Juggernaut-XI-Prototype.safetensors"
@@ -101,7 +102,56 @@
     base_model_name: str = "RunDiffusion-XL-Photo.safetensors"
     refiner_model_name: str = "None"
     refiner_switch: float = 0.1
     loras: List[Lora] = Field(default_factory=list, examples=[[Lora()]])
     advanced_params: Optional[FcusAdvancedParams] = Field(default=None, examples=[FcusAdvancedParams()])
     require_base64: bool = False
     async_process: bool = True
+
+
+class FcusImagePrompt(BaseRequest):
+    input_image: bytes = Field(..., description="binary image, used for inpaint")
+    input_mask: bytes = Field(..., description="binary image mask, used for inpaint")
+    inpaint_additional_prompt: str = ""
+    outpaint_selections: str = Field(default="",
+                                     description="Image extension direction, 'Left', 'Right', 'Top', 'Bottom' separated by commas")
+    outpaint_distance_left: int = 0
+    outpaint_distance_right: int = 0
+    outpaint_distance_top: int = 0
+    outpaint_distance_bottom: int = 0
+    cn_img1: bytes = Field(..., description="binary image")
+    cn_stop1: float = 0.6
+    cn_weight1: float = 0.6
+    cn_type1: str
+    cn_img2: bytes = Field(..., description="binary image")
+    cn_stop2: float = 0.6
+    cn_weight2: float = 0.6
+    cn_type2: str
+    cn_img3: bytes = Field(..., description="binary image")
+    cn_stop3: float = 0.6
+    cn_weight3: float = 0.6
+    cn_type3: str
+    cn_img4: bytes = Field(..., description="binary image")
+    cn_stop4: float = 0.6
+    cn_weight4: float = 0.6
+    cn_type4: str
+    style_selections: List[str] = Field(default_factory=list, description="List of Fooocus style segments with commas")
+    loras: List[Lora] = Field(default_factory=list)
+    advanced_params: Optional[FcusAdvancedParams] = Field(default=None)
+
+    class Config:
+        schema_extra = {
+            "example": {
+                "input_image": "base64_encoded_image",
+                "input_mask": "base64_encoded_mask",
+                "inpaint_additional_prompt": "Additional details for inpainting",
+                "outpaint_selections": "Left,Right",
+                "outpaint_distance_left": 100,
+                "outpaint_distance_right": 100,
+                "cn_img1": "base64_encoded_image",
+                "cn_stop1": 0.6,
+                "cn_weight1": 0.6,
+                "cn_type1": "ImagePrompt",
+                "style_selections": ["Fooocus V2", "Fooocus Enhance"],
+                "loras": [{"model_name": "sd_xl_offset_example-lora_1.0.safetensors", "weight": 0.5}],
+            }
+        }
```

### Comparing `gen_wrappers-0.4.7/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.4.8/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.7/creator/util/helper.py` & `gen_wrappers-0.4.8/creator/util/helper.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.7/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.4.8/gen_wrappers.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.4.7
+Version: 0.4.8
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.4.7/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.4.8/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.7/setup.py` & `gen_wrappers-0.4.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.4.7',
+    version='0.4.8',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```

