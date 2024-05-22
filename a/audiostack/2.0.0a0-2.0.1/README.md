# Comparing `tmp/audiostack-2.0.0a0.tar.gz` & `tmp/audiostack-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiostack-2.0.0a0.tar", max compression
+gzip compressed data, was "audiostack-2.0.1.tar", max compression
```

## Comparing `audiostack-2.0.0a0.tar` & `audiostack-2.0.1.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0     1061 2024-05-16 19:16:57.894489 audiostack-2.0.0a0/LICENSE
--rw-r--r--   0        0        0     4967 2024-05-21 09:54:00.601575 audiostack-2.0.0a0/README.md
--rw-r--r--   0        0        0      520 2024-05-21 09:54:00.601895 audiostack-2.0.0a0/audiostack/__init__.py
--rw-r--r--   0        0        0      819 2024-05-21 09:54:00.602382 audiostack-2.0.0a0/audiostack/content/__init__.py
--rw-r--r--   0        0        0     6199 2024-05-21 09:54:00.602974 audiostack-2.0.0a0/audiostack/content/file.py
--rw-r--r--   0        0        0     2321 2024-05-21 09:54:00.603553 audiostack-2.0.0a0/audiostack/content/media.py
--rw-r--r--   0        0        0     2178 2024-05-21 09:54:00.604277 audiostack-2.0.0a0/audiostack/content/recommend.py
--rw-r--r--   0        0        0     1029 2024-05-21 09:54:00.604729 audiostack-2.0.0a0/audiostack/content/root_functions.py
--rw-r--r--   0        0        0     4360 2024-05-21 09:54:00.605290 audiostack-2.0.0a0/audiostack/content/script.py
--rw-r--r--   0        0        0      120 2024-05-21 09:54:00.605797 audiostack-2.0.0a0/audiostack/delivery/__init__.py
--rw-r--r--   0        0        0     3564 2024-05-21 09:54:00.606302 audiostack-2.0.0a0/audiostack/delivery/encoder.py
--rw-r--r--   0        0        0     2116 2024-05-21 09:54:00.606819 audiostack-2.0.0a0/audiostack/delivery/video.py
--rw-r--r--   0        0        0       61 2024-05-21 09:54:00.607276 audiostack-2.0.0a0/audiostack/docs/__init__.py
--rw-r--r--   0        0        0      602 2024-05-21 09:54:00.607654 audiostack-2.0.0a0/audiostack/docs/docs.py
--rw-r--r--   0        0        0        0 2024-05-16 19:16:57.895701 audiostack-2.0.0a0/audiostack/helpers/__init__.py
--rw-r--r--   0        0        0      764 2024-05-21 09:54:00.607893 audiostack-2.0.0a0/audiostack/helpers/api_item.py
--rw-r--r--   0        0        0     1102 2024-05-21 09:54:00.608269 audiostack-2.0.0a0/audiostack/helpers/api_list.py
--rw-r--r--   0        0        0     4916 2024-05-21 09:54:00.608702 audiostack-2.0.0a0/audiostack/helpers/request_interface.py
--rw-r--r--   0        0        0      163 2024-05-16 19:16:57.895951 audiostack-2.0.0a0/audiostack/helpers/request_types.py
--rw-r--r--   0        0        0      388 2024-05-21 09:54:00.608998 audiostack-2.0.0a0/audiostack/helpers/response.py
--rw-r--r--   0        0        0      227 2024-05-16 19:16:57.896061 audiostack-2.0.0a0/audiostack/helpers/util.py
--rw-r--r--   0        0        0       58 2024-05-16 19:16:57.896140 audiostack-2.0.0a0/audiostack/orchestrator/__init__.py
--rw-r--r--   0        0        0      176 2024-05-21 09:54:00.609336 audiostack-2.0.0a0/audiostack/production/__init__.py
--rw-r--r--   0        0        0     5096 2024-05-21 09:54:00.609619 audiostack-2.0.0a0/audiostack/production/mix.py
--rw-r--r--   0        0        0     4542 2024-05-21 09:54:00.609917 audiostack-2.0.0a0/audiostack/production/sound.py
--rw-r--r--   0        0        0     4630 2024-05-21 09:54:00.610401 audiostack-2.0.0a0/audiostack/production/suite.py
--rw-r--r--   0        0        0      228 2024-05-21 09:54:00.611925 audiostack-2.0.0a0/audiostack/speech/__init__.py
--rw-r--r--   0        0        0     3179 2024-05-21 09:54:00.612294 audiostack-2.0.0a0/audiostack/speech/diction.py
--rw-r--r--   0        0        0     1294 2024-05-21 09:54:00.612830 audiostack-2.0.0a0/audiostack/speech/predict.py
--rw-r--r--   0        0        0     7903 2024-05-21 09:54:00.613361 audiostack-2.0.0a0/audiostack/speech/tts.py
--rw-r--r--   0        0        0     2325 2024-05-21 09:54:00.613771 audiostack-2.0.0a0/audiostack/speech/voice.py
--rw-r--r--   0        0        0     1200 2024-05-21 09:54:00.614173 audiostack-2.0.0a0/audiostack/tests/content/test_file.py
--rw-r--r--   0        0        0      673 2024-05-21 09:54:00.614999 audiostack-2.0.0a0/audiostack/tests/content/test_folder.py
--rw-r--r--   0        0        0     3832 2024-05-21 09:54:00.615377 audiostack-2.0.0a0/audiostack/tests/content/test_recommend.py
--rw-r--r--   0        0        0      906 2024-05-21 09:54:00.615688 audiostack-2.0.0a0/audiostack/tests/content/test_transfer.py
--rw-r--r--   0        0        0      495 2024-05-21 09:54:00.616144 audiostack-2.0.0a0/audiostack/tests/production/test_aes.py
--rw-r--r--   0        0        0      364 2024-05-21 09:54:00.616490 audiostack-2.0.0a0/audiostack/tests/production/test_sound.py
--rw-r--r--   0        0        0      978 2024-05-21 09:54:00.616717 audiostack-2.0.0a0/audiostack/tests/production/test_suite.py
--rw-r--r--   0        0        0      591 2024-05-21 09:54:00.616966 audiostack-2.0.0a0/audiostack/tests/production/test_video.py
--rw-r--r--   0        0        0     1292 2024-05-21 09:54:00.617179 audiostack-2.0.0a0/audiostack/tests/test_script.py
--rw-r--r--   0        0        0     1071 2024-05-21 09:54:00.617459 audiostack-2.0.0a0/audiostack/tests/tts/test_lexi.py
--rw-r--r--   0        0        0     1427 2024-05-21 09:54:00.617709 audiostack-2.0.0a0/audiostack/tests/tts/test_predict.py
--rw-r--r--   0        0        0      488 2024-05-21 09:54:00.617968 audiostack-2.0.0a0/audiostack/tests/tts/test_voice.py
--rw-r--r--   0        0        0     1825 2024-05-21 09:54:00.619085 audiostack-2.0.0a0/pyproject.toml
--rw-r--r--   0        0        0     5717 1970-01-01 00:00:00.000000 audiostack-2.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-22 09:05:46.228890 audiostack-2.0.1/LICENSE
+-rw-r--r--   0        0        0     4967 2024-05-22 09:05:46.228890 audiostack-2.0.1/README.md
+-rw-r--r--   0        0        0      520 2024-05-22 09:05:49.336877 audiostack-2.0.1/audiostack/__init__.py
+-rw-r--r--   0        0        0      819 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/content/__init__.py
+-rw-r--r--   0        0        0     6430 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/content/file.py
+-rw-r--r--   0        0        0     2321 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/content/media.py
+-rw-r--r--   0        0        0     2178 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/content/recommend.py
+-rw-r--r--   0        0        0     1029 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/content/root_functions.py
+-rw-r--r--   0        0        0     4360 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/content/script.py
+-rw-r--r--   0        0        0      120 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/delivery/__init__.py
+-rw-r--r--   0        0        0     3620 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/delivery/encoder.py
+-rw-r--r--   0        0        0     6216 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/delivery/video.py
+-rw-r--r--   0        0        0       61 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/docs/__init__.py
+-rw-r--r--   0        0        0      602 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/docs/docs.py
+-rw-r--r--   0        0        0        0 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/helpers/__init__.py
+-rw-r--r--   0        0        0      764 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/helpers/api_item.py
+-rw-r--r--   0        0        0     1102 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/helpers/api_list.py
+-rw-r--r--   0        0        0     4640 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/helpers/request_interface.py
+-rw-r--r--   0        0        0      163 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/helpers/request_types.py
+-rw-r--r--   0        0        0      388 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/helpers/response.py
+-rw-r--r--   0        0        0      227 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/helpers/util.py
+-rw-r--r--   0        0        0       58 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/orchestrator/__init__.py
+-rw-r--r--   0        0        0      176 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/production/__init__.py
+-rw-r--r--   0        0        0     5096 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/production/mix.py
+-rw-r--r--   0        0        0     4542 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/production/sound.py
+-rw-r--r--   0        0        0     4685 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/production/suite.py
+-rw-r--r--   0        0        0      228 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/speech/__init__.py
+-rw-r--r--   0        0        0     3179 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/speech/diction.py
+-rw-r--r--   0        0        0     1294 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/speech/predict.py
+-rw-r--r--   0        0        0     7902 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/speech/tts.py
+-rw-r--r--   0        0        0     2325 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/speech/voice.py
+-rw-r--r--   0        0        0     1200 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/content/test_file.py
+-rw-r--r--   0        0        0      672 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/content/test_folder.py
+-rw-r--r--   0        0        0     3832 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/content/test_recommend.py
+-rw-r--r--   0        0        0      906 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/content/test_transfer.py
+-rw-r--r--   0        0        0     2170 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/helpers/test_request_interface.py
+-rw-r--r--   0        0        0      495 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/production/test_aes.py
+-rw-r--r--   0        0        0      364 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/production/test_sound.py
+-rw-r--r--   0        0        0      978 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/production/test_suite.py
+-rw-r--r--   0        0        0     2385 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/production/test_video.py
+-rw-r--r--   0        0        0     1292 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/test_script.py
+-rw-r--r--   0        0        0     1071 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/tts/test_lexi.py
+-rw-r--r--   0        0        0     1427 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/tts/test_predict.py
+-rw-r--r--   0        0        0      488 2024-05-22 09:05:46.228890 audiostack-2.0.1/audiostack/tests/tts/test_voice.py
+-rw-r--r--   0        0        0     1819 2024-05-22 09:05:46.232890 audiostack-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5715 1970-01-01 00:00:00.000000 audiostack-2.0.1/PKG-INFO
```

### Comparing `audiostack-2.0.0a0/LICENSE` & `audiostack-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.0a0/README.md` & `audiostack-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.0a0/audiostack/__init__.py` & `audiostack-2.0.1/audiostack/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-sdk_version = "1.3.1"
+sdk_version = "2.0.1"
 api_base = "https://v2.api.audio"
 api_key = None
 assume_org_id = None
 app_info = None
 
 
 from audiostack import content as Content  # noqa: F401
```

### Comparing `audiostack-2.0.0a0/audiostack/content/__init__.py` & `audiostack-2.0.1/audiostack/content/__init__.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.0a0/audiostack/content/file.py` & `audiostack-2.0.1/audiostack/content/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,14 @@
     def transfer(
         url: str,
         uploadPath: str,
         category: str = "",
         tags: list = [],
         metadata: dict = {},
     ) -> Item:
-
         data = {
             "filePath": uploadPath,
             "url": url,
             "category": category,
             "tags": tags,
             "metadata": metadata,
         }
@@ -103,15 +102,14 @@
     def modify(
         fileId: str,
         filePath: str = "",
         category: str = "",
         tags: list = [],
         metadata: dict = {},
     ) -> Item:
-
         data = {
             "filePath": filePath,
             "category": category,
             "tags": tags,
             "metadata": metadata,
         }
 
@@ -123,14 +121,19 @@
         return File.get(fileId)
 
     @staticmethod
     def get(fileId: str) -> Item:
         r = File.interface.send_request(
             rtype=RequestTypes.GET, route="file/id", path_parameters=fileId
         )
+        while r["statusCode"] == 202:
+            print("Response in progress please wait...")
+            r = File.interface.send_request(
+                rtype=RequestTypes.GET, route="file/id", path_parameters=fileId
+            )
         return File.Item(r)
 
     @staticmethod
     def delete(fileId: str) -> APIResponseItem:
         r = File.interface.send_request(
             rtype=RequestTypes.DELETE, route="file/id", path_parameters=fileId
         )
@@ -179,15 +182,14 @@
             if list_type == "folders":
                 return {"data": item}
             else:
                 raise Exception()
 
     @staticmethod
     def create(name: Any) -> APIResponseItem:
-
         r = File.interface.send_request(
             rtype=RequestTypes.POST,
             route="folder",
             json={"folder": name},
         )
         return APIResponseItem(r)
```

### Comparing `audiostack-2.0.0a0/audiostack/content/media.py` & `audiostack-2.0.1/audiostack/content/media.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.0a0/audiostack/content/recommend.py` & `audiostack-2.0.1/audiostack/content/recommend.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.0a0/audiostack/content/root_functions.py` & `audiostack-2.0.1/audiostack/content/root_functions.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.0a0/audiostack/content/script.py` & `audiostack-2.0.1/audiostack/content/script.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.0a0/audiostack/delivery/encoder.py` & `audiostack-2.0.1/audiostack/delivery/encoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,14 @@
         bitRateType: str = "",
         bitRate: Optional[int] = None,
         sampleRate: Optional[int] = None,
         format: str = "",
         bitDepth: Optional[int] = None,
         channels: Optional[int] = None,
     ) -> Item:
-
         if productionId and productionItem:
             raise Exception(
                 "productionId or productionItem should be supplied not both"
             )
         if not (productionId or productionItem):
             raise Exception("productionId or productionItem should be supplied")
 
@@ -80,14 +79,15 @@
             "loudnessPreset": loudnessPreset,
         }
         r = Encoder.interface.send_request(
             rtype=RequestTypes.POST, route="encoder", json=body
         )
 
         while r["statusCode"] == 202:
+            print("Response in progress please wait...")
             encoderId = r["data"]["encoderId"]
             r = Encoder.interface.send_request(
                 rtype=RequestTypes.GET, route="encoder", path_parameters=encoderId
             )
         return Encoder.Item(r)
 
     @staticmethod
```

### Comparing `audiostack-2.0.0a0/audiostack/docs/docs.py` & `audiostack-2.0.1/audiostack/docs/docs.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.0a0/audiostack/helpers/api_item.py` & `audiostack-2.0.1/audiostack/helpers/api_item.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.0a0/audiostack/helpers/api_list.py` & `audiostack-2.0.1/audiostack/helpers/api_list.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.0a0/audiostack/helpers/request_interface.py` & `audiostack-2.0.1/audiostack/helpers/request_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 class RequestInterface:
     # disable debug print
     DEBUG_PRINT = False
 
     def __init__(self, family: str) -> None:
         self.family = family
 
-    def make_header(self) -> dict:
+    @staticmethod
+    def make_header() -> dict:
         header = {
             "x-api-key": audiostack.api_key,
             "x-python-sdk-version": audiostack.sdk_version,
         }
         if audiostack.assume_org_id:
             header["x-assume-org"] = audiostack.assume_org_id
         return header
@@ -54,23 +55,14 @@
             msg = (
                 r.json()["message"]
                 + ". Errors listed as follows: \n\t"
                 + "\t".join(r.json()["errors"])
             )
             raise Exception(msg)
 
-        # if isinstance(r.content, bytes):
-        #     if self.DEBUG_PRINT:
-        #         print("Is bytes")
-        #     return {
-        #         "bytes" : r.content,
-        #         "statusCode" : r.status_code
-        #     }
-
-        # else:
         if "meta" in r.json():
             if "creditsUsed" in r.json()["meta"]:
                 audiostack.billing_session += r.json()["meta"]["creditsUsed"]
 
         return {**r.json(), **{"statusCode": r.status_code}}
 
     def send_upload_request(self, local_path: str, upload_url: str) -> int:
@@ -136,19 +128,17 @@
 
             return self.resolve_response(
                 requests.delete(
                     url=url, params=query_parameters, headers=self.make_header()
                 )
             )
 
-    @staticmethod
-    def download_url(url: str, name: str, destination: str) -> None:
-        r = requests.get(
-            url=url, stream=True, headers={"x-api-key": audiostack.api_key}
-        )
+    @classmethod
+    def download_url(cls, url: str, name: str, destination: str) -> None:
+        r = requests.get(url=url, stream=True, headers=cls.make_header())
 
         if r.status_code >= 400:
             raise Exception("Failed to download file")
 
         local_filename = f"{destination}/{name}"
         with open(local_filename, "wb") as f:
             shutil.copyfileobj(r.raw, f)
```

### Comparing `audiostack-2.0.0a0/audiostack/production/mix.py` & `audiostack-2.0.1/audiostack/production/mix.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.0a0/audiostack/production/sound.py` & `audiostack-2.0.1/audiostack/production/sound.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.0a0/audiostack/production/suite.py` & `audiostack-2.0.1/audiostack/production/suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,39 +80,38 @@
 
         return Suite.EvaluationItem(r)
 
     @staticmethod
     def separate(
         fileId: str, wait: bool = True
     ) -> Union["Suite.PipelineInProgressItem", "Suite.PipelineFinishedItem"]:
-
         body = {
             "fileId": fileId,
         }
         r = Suite.interface.send_request(
             rtype=RequestTypes.POST, route="suite/separate", json=body
         )
         item = Suite.PipelineInProgressItem(r)
         return Suite._poll(r, item.pipelineId) if wait else item
 
     @staticmethod
     def denoise(
         fileId: str, level: Optional[int] = None, wait: bool = True
     ) -> Union["Suite.PipelineInProgressItem", "Suite.PipelineFinishedItem"]:
-
         body = {"fileId": fileId, "level": level}
         r = Suite.interface.send_request(
             rtype=RequestTypes.POST, route=Suite.DENOISE_ENDPOINT, json=body
         )
         item = Suite.PipelineInProgressItem(r)
         return Suite._poll(r, item.pipelineId) if wait else item
 
     @staticmethod
     def _poll(r: Any, pipelineId: str) -> "Suite.PipelineFinishedItem":
         while r["statusCode"] == 202:
+            print("Response in progress please wait...")
             r = Suite.interface.send_request(
                 rtype=RequestTypes.GET,
                 route="suite/pipeline",
                 path_parameters=pipelineId,
             )
 
         status = r.get("data", {}).get("status", 200)
```

### Comparing `audiostack-2.0.0a0/audiostack/speech/diction.py` & `audiostack-2.0.1/audiostack/speech/diction.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.0a0/audiostack/speech/predict.py` & `audiostack-2.0.1/audiostack/speech/predict.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.0a0/audiostack/speech/tts.py` & `audiostack-2.0.1/audiostack/speech/tts.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,14 @@
     @staticmethod
     def annotate(
         speechId: str,
         scriptReference: str = "",
         languageCode: str = "",
         continuousRecognition: bool = False,
     ) -> dict:
-
         body = {
             "speechId": speechId,
             "scriptReference": scriptReference,
             "language_code": languageCode,
             "continuous_recognition": continuousRecognition,
         }
         r = TTS.interface.send_request(
```

### Comparing `audiostack-2.0.0a0/audiostack/speech/voice.py` & `audiostack-2.0.1/audiostack/speech/voice.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.0a0/audiostack/tests/content/test_file.py` & `audiostack-2.0.1/audiostack/tests/content/test_file.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.0a0/audiostack/tests/content/test_folder.py` & `audiostack-2.0.1/audiostack/tests/content/test_folder.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     for fol in r.folders:
         print(fol)
     for fi in r.files:
         print(fi)
 
 
 def test_create() -> None:
-
     r = Folder.delete(folder="__PYTHON_TEST", delete_files=True)
     r = Folder.create(name="__PYTHON_TEST")  # type: ignore
     print(r)
 
 
 def test_delete() -> None:
     Folder.delete(folder="__PYTHON_TEST", delete_files=True)
```

### Comparing `audiostack-2.0.0a0/audiostack/tests/content/test_recommend.py` & `audiostack-2.0.1/audiostack/tests/content/test_recommend.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.0a0/audiostack/tests/content/test_transfer.py` & `audiostack-2.0.1/audiostack/tests/content/test_transfer.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.0a0/audiostack/tests/production/test_suite.py` & `audiostack-2.0.1/audiostack/tests/production/test_suite.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.0a0/audiostack/tests/test_script.py` & `audiostack-2.0.1/audiostack/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.0a0/audiostack/tests/tts/test_lexi.py` & `audiostack-2.0.1/audiostack/tests/tts/test_lexi.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.0a0/audiostack/tests/tts/test_predict.py` & `audiostack-2.0.1/audiostack/tests/tts/test_predict.py`

 * *Files identical despite different names*

### Comparing `audiostack-2.0.0a0/pyproject.toml` & `audiostack-2.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "audiostack"
-version = "2.0.0.alpha"
+version = "2.0.1"
 description = "Python SDK for Audiostack API"
 authors = ["Aflorithmic <support@audiostack.ai>"]
 repository = "https://github.com/aflorithmic/audiostack-python"
 readme = "README.md"
 classifiers = [
    "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `audiostack-2.0.0a0/PKG-INFO` & `audiostack-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostack
-Version: 2.0.0a0
+Version: 2.0.1
 Summary: Python SDK for Audiostack API
 Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic
 Author-email: support@audiostack.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: audiostack Version: 2.0.0a0 Summary: Python SDK for
+Metadata-Version: 2.1 Name: audiostack Version: 2.0.1 Summary: Python SDK for
 Audiostack API Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic Author-email: support@audiostack.ai Requires-Python:
 >=3.8.1,<4.0.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: requests
```

