# Comparing `tmp/uploadthing_py-0.2.2.tar.gz` & `tmp/uploadthing_py-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uploadthing_py-0.2.2.tar", max compression
+gzip compressed data, was "uploadthing_py-0.2.3.tar", max compression
```

## Comparing `uploadthing_py-0.2.2.tar` & `uploadthing_py-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2538 2024-05-20 13:13:12.737624 uploadthing_py-0.2.2/README.md
--rw-r--r--   0        0        0      618 2024-05-20 13:14:26.313092 uploadthing_py-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      663 2024-05-20 12:38:08.833457 uploadthing_py-0.2.2/uploadthing_py/__init__.py
--rw-r--r--   0        0        0     1323 2024-05-20 13:14:21.791225 uploadthing_py-0.2.2/uploadthing_py/builder.py
--rw-r--r--   0        0        0        0 2024-05-19 21:14:05.647788 uploadthing_py-0.2.2/uploadthing_py/py.typed
--rw-r--r--   0        0        0    11427 2024-05-20 12:57:24.105021 uploadthing_py-0.2.2/uploadthing_py/request_handler.py
--rw-r--r--   0        0        0     3367 2024-05-20 12:42:07.140803 uploadthing_py-0.2.2/uploadthing_py/types.py
--rw-r--r--   0        0        0     5539 2024-05-20 12:37:33.373772 uploadthing_py-0.2.2/uploadthing_py/utapi.py
--rw-r--r--   0        0        0      717 2024-05-19 21:11:35.769126 uploadthing_py-0.2.2/uploadthing_py/utils.py
--rw-r--r--   0        0        0     2893 1970-01-01 00:00:00.000000 uploadthing_py-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2538 2024-05-20 13:13:12.737624 uploadthing_py-0.2.3/README.md
+-rw-r--r--   0        0        0      618 2024-05-21 22:03:56.691424 uploadthing_py-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      663 2024-05-20 12:38:08.833457 uploadthing_py-0.2.3/uploadthing_py/__init__.py
+-rw-r--r--   0        0        0     1323 2024-05-20 13:14:21.791225 uploadthing_py-0.2.3/uploadthing_py/builder.py
+-rw-r--r--   0        0        0        0 2024-05-19 21:14:05.647788 uploadthing_py-0.2.3/uploadthing_py/py.typed
+-rw-r--r--   0        0        0    11391 2024-05-21 22:03:14.292986 uploadthing_py-0.2.3/uploadthing_py/request_handler.py
+-rw-r--r--   0        0        0     3719 2024-05-21 22:02:20.251415 uploadthing_py-0.2.3/uploadthing_py/types.py
+-rw-r--r--   0        0        0     5555 2024-05-21 21:50:15.091165 uploadthing_py-0.2.3/uploadthing_py/utapi.py
+-rw-r--r--   0        0        0      717 2024-05-21 21:48:45.411030 uploadthing_py-0.2.3/uploadthing_py/utils.py
+-rw-r--r--   0        0        0     2893 1970-01-01 00:00:00.000000 uploadthing_py-0.2.3/PKG-INFO
```

### Comparing `uploadthing_py-0.2.2/README.md` & `uploadthing_py-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `uploadthing_py-0.2.2/pyproject.toml` & `uploadthing_py-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uploadthing.py"
-version = "0.2.2"
+version = "0.2.3"
 description = "Python SDK for UploadThing"
 authors = ["juliusmarminge <julius0216@outlook.com>"]
 readme = "README.md"
 packages = [{ include = "uploadthing_py" }]
 license = "MIT"
```

### Comparing `uploadthing_py-0.2.2/uploadthing_py/__init__.py` & `uploadthing_py-0.2.3/uploadthing_py/__init__.py`

 * *Files identical despite different names*

### Comparing `uploadthing_py-0.2.2/uploadthing_py/builder.py` & `uploadthing_py-0.2.3/uploadthing_py/builder.py`

 * *Files identical despite different names*

### Comparing `uploadthing_py-0.2.2/uploadthing_py/request_handler.py` & `uploadthing_py-0.2.3/uploadthing_py/request_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from fastapi import Request, Response
 from httpx import AsyncClient
 from uploadthing_py.utils import json_stringify
 from uploadthing_py.builder import UploadThingBuilder
 import asyncio
-import json
 from uploadthing_py.types import (
     UploadRequest,
     CallbackRequest,
     CompleteMPURequest,
     FailureRequest,
 )
 from typing import Union
@@ -41,45 +40,46 @@
                 else 1
             )
 
         routes.append(route_config)
     return routes
 
 
-async def dev_hook(key: str, api_key: str):
+async def dev_hook(presigned: dict, api_key: str):
     retry_delay = 40e-3
     async with AsyncClient() as client:
         while True:
             response = await client.get(
-                f"https://api.uploadthing.com/v6/pollUpload/{key}",
+                presigned["pollingUrl"],
                 headers={
+                    "Authorization": presigned["pollingJwt"],
                     "x-uploadthing-api-key": api_key,
                     "x-uploadthing-version": "6.10.0",
                 },
             )
             polling_data = response.json()
             if polling_data["status"] == "done":
                 print("[DEV_HOOK] Polling done")
                 break
             await asyncio.sleep(retry_delay)
             retry_delay *= 2
 
-        file_data = polling_data["fileData"]
-        callback_url = f"{file_data['callbackUrl']}?slug={file_data['callbackSlug']}"
+        file = polling_data["file"]
+        callback_url = f"{file['callbackUrl']}?slug={file['callbackSlug']}"
         payload = json_stringify(
             {
                 "status": "uploaded",
-                "metadata": json.loads(file_data["metadata"]),
+                "metadata": polling_data["metadata"],
                 "file": {
-                    "url": f"https://utfs.io/f/{key}",
-                    "key": key,
-                    "name": file_data["fileName"],
-                    "size": file_data["fileSize"],
-                    "custom_id": file_data["customId"],
-                    "type": file_data["fileType"],
+                    "url": file["fileUrl"],
+                    "key": file["fileKey"],
+                    "name": file["fileName"],
+                    "size": file["fileSize"],
+                    "custom_id": file["customId"],
+                    "type": file["fileType"],
                 },
             }
         )
 
         # (TODO) Sign payload
         signature = "TODO"
 
@@ -152,15 +152,15 @@
         if response.status_code != 200:
             return {"error": "Failed to get presigned URLs"}
 
         presigned_urls = response.json()["data"]
 
         if is_dev:
             asyncio.gather(
-                *[dev_hook(presigned["key"], api_key) for presigned in presigned_urls]
+                *[dev_hook(presigned, api_key) for presigned in presigned_urls]
             )
 
         return presigned_urls
 
 
 async def handle_callback_request(
     uploader: UploadThingBuilder, body: CallbackRequest, api_key: str
@@ -281,35 +281,35 @@
         is_dev=os.getenv("ENVIRONMENT", "development") == "development",
     )
 
 
     @app.get("/api")
     async def greeting():
         return "Hello from FastAPI"
-    
-    
+
+        
     @app.get("/api/uploadthing")
     async def ut_get():
         return handlers["GET"]()
-    
-    
+
+
     @app.post("/api/uploadthing")
     async def ut_post(
         request: Request,
         response: Response,
         body: UploadThingRequestBody,
     ):
         return await handlers["POST"](
             request=request,
             response=response,
             body=body,
         )
     ```
     """
-    
+
     def ut_get():
         return extract_router_config(router)
 
     async def ut_post(
         request: Request,
         response: Response,
         body: Union[UploadRequest, CallbackRequest, CompleteMPURequest],
```

### Comparing `uploadthing_py-0.2.2/uploadthing_py/types.py` & `uploadthing_py-0.2.3/uploadthing_py/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,16 +38,26 @@
 class DeleteFiles:
     @dataclass
     class DeleteFileOptions(KeyTypeOptions):
         pass
 
     @dataclass
     class DeleteFileResponse:
+        deleted_count: int
         success: bool
 
+        @classmethod
+        def from_api_response(
+            cls, api_response: dict
+        ) -> "DeleteFiles.DeleteFileResponse":
+            return DeleteFiles.DeleteFileResponse(
+                deleted_count=api_response["deletedCount"],
+                success=api_response["success"],
+            )
+
 
 class ListFiles:
     @dataclass
     class ListFilesOptions:
         limit: int | None = None
         offset: int | None = None
 
@@ -104,14 +114,15 @@
             )
 
 
 class GetSignedUrl:
     class GetSignedUrlOptions(KeyTypeOptions):
         expires_in: int | None = None
 
+    @dataclass
     class GetSignedUrlResponse:
         url: str
 
 
 class UpdateACL:
     class UpdateACLOptions(KeyTypeOptions):
         acl: ACL
```

### Comparing `uploadthing_py-0.2.2/uploadthing_py/utapi.py` & `uploadthing_py-0.2.3/uploadthing_py/utapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         if not isinstance(keys, t.List):
             keys = [keys]
 
         key_type = options["key_type"] if options else self._default_key_type
         payload = {"fileKeys": keys} if key_type == "file_key" else {"customIds": keys}
 
         api_response = await self._request_ut_api("/v6/deleteFiles", payload)
-        response = DeleteFiles.DeleteFileResponse(**api_response)
+        response = DeleteFiles.DeleteFileResponse.from_api_response(api_response)
 
         return response
 
     async def list_files(self, options: t.Optional[ListFiles.ListFilesOptions] = None):
         api_response = await self._request_ut_api("/v6/listFiles", options)
         response = ListFiles.ListFilesResponse(**api_response)
```

### Comparing `uploadthing_py-0.2.2/uploadthing_py/utils.py` & `uploadthing_py-0.2.3/uploadthing_py/utils.py`

 * *Files identical despite different names*

### Comparing `uploadthing_py-0.2.2/PKG-INFO` & `uploadthing_py-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uploadthing.py
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python SDK for UploadThing
 License: MIT
 Author: juliusmarminge
 Author-email: julius0216@outlook.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

