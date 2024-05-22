# Comparing `tmp/gen_wrappers-0.4.9.tar.gz` & `tmp/gen_wrappers-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.4.9.tar", last modified: Wed May 22 21:04:33 2024, max compression
+gzip compressed data, was "gen_wrappers-0.5.0.tar", last modified: Wed May 22 21:08:52 2024, max compression
```

## Comparing `gen_wrappers-0.4.9.tar` & `gen_wrappers-0.5.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 21:04:33.147000 gen_wrappers-0.4.9/
--rw-rw-rw-   0        0        0      847 2024-05-22 21:04:33.145996 gen_wrappers-0.4.9/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-05-20 15:06:29.000000 gen_wrappers-0.4.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 21:04:33.092680 gen_wrappers-0.4.9/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.4.9/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 21:04:33.101620 gen_wrappers-0.4.9/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.4.9/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     7124 2024-05-20 18:57:41.000000 gen_wrappers-0.4.9/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     4055 2024-05-14 16:10:12.000000 gen_wrappers-0.4.9/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.4.9/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-22 21:04:33.110638 gen_wrappers-0.4.9/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.4.9/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1641 2024-05-20 18:57:41.000000 gen_wrappers-0.4.9/creator/base/base_app.py
--rw-rw-rw-   0        0        0      673 2024-05-20 18:57:41.000000 gen_wrappers-0.4.9/creator/base/base_request.py
--rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.4.9/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.4.9/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-22 21:04:33.117409 gen_wrappers-0.4.9/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.4.9/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0    11700 2024-05-20 18:57:41.000000 gen_wrappers-0.4.9/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0    16233 2024-05-20 17:09:18.000000 gen_wrappers-0.4.9/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.4.9/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-22 21:04:33.121982 gen_wrappers-0.4.9/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.4.9/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     7207 2024-05-22 21:04:16.000000 gen_wrappers-0.4.9/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     6112 2024-05-22 20:55:15.000000 gen_wrappers-0.4.9/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.4.9/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-22 21:04:33.124949 gen_wrappers-0.4.9/creator/util/
--rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.4.9/creator/util/__init__.py
--rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.4.9/creator/util/helper.py
-drwxrwxrwx   0        0        0        0 2024-05-22 21:04:33.144996 gen_wrappers-0.4.9/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      847 2024-05-22 21:04:32.000000 gen_wrappers-0.4.9/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      768 2024-05-22 21:04:32.000000 gen_wrappers-0.4.9/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 21:04:32.000000 gen_wrappers-0.4.9/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-22 21:04:32.000000 gen_wrappers-0.4.9/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-22 21:04:32.000000 gen_wrappers-0.4.9/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 21:04:33.147999 gen_wrappers-0.4.9/setup.cfg
--rw-rw-rw-   0        0        0     1035 2024-05-22 21:04:24.000000 gen_wrappers-0.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:08:52.950013 gen_wrappers-0.5.0/
+-rw-rw-rw-   0        0        0      847 2024-05-22 21:08:52.949014 gen_wrappers-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2024-05-20 15:06:29.000000 gen_wrappers-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 21:08:52.906871 gen_wrappers-0.5.0/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.5.0/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:08:52.912870 gen_wrappers-0.5.0/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.5.0/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     7124 2024-05-20 18:57:41.000000 gen_wrappers-0.5.0/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     4055 2024-05-14 16:10:12.000000 gen_wrappers-0.5.0/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.5.0/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:08:52.920047 gen_wrappers-0.5.0/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.5.0/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1641 2024-05-20 18:57:41.000000 gen_wrappers-0.5.0/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      673 2024-05-20 18:57:41.000000 gen_wrappers-0.5.0/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.5.0/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.5.0/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:08:52.924547 gen_wrappers-0.5.0/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.5.0/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0    11700 2024-05-20 18:57:41.000000 gen_wrappers-0.5.0/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0    16233 2024-05-20 17:09:18.000000 gen_wrappers-0.5.0/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.5.0/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:08:52.929361 gen_wrappers-0.5.0/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.5.0/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     7207 2024-05-22 21:04:16.000000 gen_wrappers-0.5.0/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     6138 2024-05-22 21:07:49.000000 gen_wrappers-0.5.0/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.5.0/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:08:52.931591 gen_wrappers-0.5.0/creator/util/
+-rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.5.0/creator/util/__init__.py
+-rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.5.0/creator/util/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:08:52.947007 gen_wrappers-0.5.0/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-05-22 21:08:52.000000 gen_wrappers-0.5.0/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      768 2024-05-22 21:08:52.000000 gen_wrappers-0.5.0/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 21:08:52.000000 gen_wrappers-0.5.0/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-22 21:08:52.000000 gen_wrappers-0.5.0/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-22 21:08:52.000000 gen_wrappers-0.5.0/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 21:08:52.951013 gen_wrappers-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2024-05-22 21:08:36.000000 gen_wrappers-0.5.0/setup.py
```

### Comparing `gen_wrappers-0.4.9/PKG-INFO` & `gen_wrappers-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.4.9
+Version: 0.5.0
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.4.9/creator/auto/creator_auto.py` & `gen_wrappers-0.5.0/creator/auto/creator_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.9/creator/auto/request_auto.py` & `gen_wrappers-0.5.0/creator/auto/request_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.9/creator/auto/response_auto.py` & `gen_wrappers-0.5.0/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.9/creator/base/base_app.py` & `gen_wrappers-0.5.0/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.9/creator/base/base_request.py` & `gen_wrappers-0.5.0/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.9/creator/base/base_response.py` & `gen_wrappers-0.5.0/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.9/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.5.0/creator/cmfy/creator_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.9/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.5.0/creator/cmfy/request_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.9/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.5.0/creator/fcus_api/creator_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.9/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.5.0/creator/fcus_api/request_fcus_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -105,39 +105,39 @@
     loras: List[Lora] = Field(default_factory=list, examples=[[Lora()]])
     advanced_params: Optional[FcusAdvancedParams] = Field(default=None, examples=[FcusAdvancedParams()])
     require_base64: bool = False
     async_process: bool = True
 
 
 class FcusImagePrompt(BaseRequest):
-    input_image: bytes = Field(..., description="binary image, used for inpaint")
-    input_mask: bytes = Field(..., description="binary image mask, used for inpaint")
+    input_image: bytes = Field(None, description="binary image, used for inpaint")
+    input_mask: bytes = Field(None, description="binary image mask, used for inpaint")
     inpaint_additional_prompt: str = ""
     outpaint_selections: str = Field(default="",
                                      description="Image extension direction, 'Left', 'Right', 'Top', 'Bottom' separated by commas")
     outpaint_distance_left: int = 0
     outpaint_distance_right: int = 0
     outpaint_distance_top: int = 0
     outpaint_distance_bottom: int = 0
-    cn_img1: bytes = Field(..., description="binary image")
+    cn_img1: bytes = Field(None, description="binary image")
     cn_stop1: float = 0.6
     cn_weight1: float = 0.6
-    cn_type1: str
-    cn_img2: bytes = Field(..., description="binary image")
+    cn_type1: str = ""
+    cn_img2: bytes = Field(None, description="binary image")
     cn_stop2: float = 0.6
     cn_weight2: float = 0.6
-    cn_type2: str
-    cn_img3: bytes = Field(..., description="binary image")
+    cn_type2: str = ""
+    cn_img3: bytes = Field(None, description="binary image")
     cn_stop3: float = 0.6
     cn_weight3: float = 0.6
-    cn_type3: str
-    cn_img4: bytes = Field(..., description="binary image")
+    cn_type3: str = ""
+    cn_img4: bytes = Field(None, description="binary image")
     cn_stop4: float = 0.6
     cn_weight4: float = 0.6
-    cn_type4: str
+    cn_type4: str = ""
     style_selections: List[str] = Field(default_factory=list, description="List of Fooocus style segments with commas")
     loras: List[Lora] = Field(default_factory=list)
     advanced_params: Optional[FcusAdvancedParams] = Field(default=None)
 
     class Config:
         schema_extra = {
             "example": {
```

### Comparing `gen_wrappers-0.4.9/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.5.0/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.9/creator/util/helper.py` & `gen_wrappers-0.5.0/creator/util/helper.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.9/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.5.0/gen_wrappers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.4.9
+Version: 0.5.0
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.4.9/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.5.0/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.9/setup.py` & `gen_wrappers-0.5.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.4.9',
+    version='0.5.0',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```

