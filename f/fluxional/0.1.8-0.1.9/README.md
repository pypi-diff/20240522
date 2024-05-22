# Comparing `tmp/fluxional-0.1.8.tar.gz` & `tmp/fluxional-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluxional-0.1.8.tar", max compression
+gzip compressed data, was "fluxional-0.1.9.tar", max compression
```

## Comparing `fluxional-0.1.8.tar` & `fluxional-0.1.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1066 2024-04-28 17:10:39.085356 fluxional-0.1.8/LICENSE
--rw-r--r--   0        0        0     3908 2024-04-29 21:12:21.619975 fluxional-0.1.8/README.md
--rw-r--r--   0        0        0      421 2024-05-17 00:45:08.982031 fluxional-0.1.8/fluxional/__init__.py
--rw-r--r--   0        0        0       85 2024-04-28 18:14:21.913877 fluxional-0.1.8/fluxional/__main__.py
--rw-r--r--   0        0        0     1429 2024-04-28 18:14:21.923877 fluxional-0.1.8/fluxional/cli/__init__.py
--rw-r--r--   0        0        0      397 2024-04-28 18:14:21.923877 fluxional-0.1.8/fluxional/core/__init__.py
--rw-r--r--   0        0        0    21405 2024-05-09 01:45:17.632254 fluxional-0.1.8/fluxional/core/app.py
--rw-r--r--   0        0        0     6976 2024-04-28 18:14:21.933877 fluxional-0.1.8/fluxional/core/core.py
--rw-r--r--   0        0        0     2927 2024-04-28 18:14:21.933877 fluxional-0.1.8/fluxional/core/events.py
--rw-r--r--   0        0        0    11708 2024-04-28 18:14:21.943877 fluxional-0.1.8/fluxional/core/handlers.py
--rw-r--r--   0        0        0        1 2024-04-28 18:14:21.943877 fluxional-0.1.8/fluxional/core/infrastructure/__init__.py
--rw-r--r--   0        0        0    20142 2024-05-15 19:51:13.339223 fluxional-0.1.8/fluxional/core/infrastructure/base.py
--rw-r--r--   0        0        0     7699 2024-04-28 18:14:21.953877 fluxional-0.1.8/fluxional/core/infrastructure/cdk.py
--rw-r--r--   0        0        0     9554 2024-04-28 18:14:21.953877 fluxional-0.1.8/fluxional/core/infrastructure/resources.py
--rw-r--r--   0        0        0      816 2024-04-28 18:14:21.953877 fluxional-0.1.8/fluxional/core/infrastructure/types.py
--rw-r--r--   0        0        0     5818 2024-04-28 18:14:21.953877 fluxional-0.1.8/fluxional/core/logic.py
--rw-r--r--   0        0        0     8343 2024-04-28 18:14:21.953877 fluxional-0.1.8/fluxional/core/settings.py
--rw-r--r--   0        0        0     4045 2024-04-28 18:14:21.953877 fluxional-0.1.8/fluxional/core/tools.py
--rw-r--r--   0        0        0     5158 2024-04-28 18:14:21.953877 fluxional-0.1.8/fluxional/core/types.py
--rw-r--r--   0        0        0       74 2024-04-28 18:14:21.953877 fluxional-0.1.8/fluxional/deployment/__init__.py
--rw-r--r--   0        0        0     1164 2024-04-28 18:14:21.953877 fluxional-0.1.8/fluxional/deployment/constants.py
--rw-r--r--   0        0        0    15517 2024-04-30 22:02:31.375706 fluxional-0.1.8/fluxional/deployment/engine.py
--rw-r--r--   0        0        0      345 2024-04-28 18:14:21.953877 fluxional-0.1.8/fluxional/deployment/exceptions.py
--rw-r--r--   0        0        0        1 2024-04-30 22:01:04.012000 fluxional-0.1.8/fluxional/deployment/utils.py
--rw-r--r--   0        0        0     3652 2024-04-28 18:14:21.963877 fluxional-0.1.8/fluxional/dev/__init__.py
--rw-r--r--   0        0        0     3003 2024-04-28 18:14:21.963877 fluxional-0.1.8/fluxional/dev/client.py
--rw-r--r--   0        0        0     3350 2024-04-28 18:14:21.963877 fluxional-0.1.8/fluxional/dev/runner.py
--rw-r--r--   0        0        0      326 2024-04-28 18:14:21.963877 fluxional-0.1.8/fluxional/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-28 18:14:21.963877 fluxional-0.1.8/fluxional/py.typed
--rw-r--r--   0        0        0      461 2024-04-28 18:14:21.963877 fluxional-0.1.8/fluxional/types.py
--rw-r--r--   0        0        0      935 2024-04-28 18:14:21.963877 fluxional-0.1.8/fluxional/utils.py
--rw-r--r--   0        0        0     1152 2024-05-17 00:45:30.382028 fluxional-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4852 1970-01-01 00:00:00.000000 fluxional-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-28 17:10:39.085356 fluxional-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3908 2024-04-29 21:12:21.619975 fluxional-0.1.9/README.md
+-rw-r--r--   0        0        0      421 2024-05-22 17:54:55.031895 fluxional-0.1.9/fluxional/__init__.py
+-rw-r--r--   0        0        0       85 2024-04-28 18:14:21.913877 fluxional-0.1.9/fluxional/__main__.py
+-rw-r--r--   0        0        0     1429 2024-04-28 18:14:21.923877 fluxional-0.1.9/fluxional/cli/__init__.py
+-rw-r--r--   0        0        0      397 2024-04-28 18:14:21.923877 fluxional-0.1.9/fluxional/core/__init__.py
+-rw-r--r--   0        0        0    21993 2024-05-22 17:43:52.123693 fluxional-0.1.9/fluxional/core/app.py
+-rw-r--r--   0        0        0     6976 2024-04-28 18:14:21.933877 fluxional-0.1.9/fluxional/core/core.py
+-rw-r--r--   0        0        0     2927 2024-04-28 18:14:21.933877 fluxional-0.1.9/fluxional/core/events.py
+-rw-r--r--   0        0        0    11708 2024-04-28 18:14:21.943877 fluxional-0.1.9/fluxional/core/handlers.py
+-rw-r--r--   0        0        0        1 2024-04-28 18:14:21.943877 fluxional-0.1.9/fluxional/core/infrastructure/__init__.py
+-rw-r--r--   0        0        0    20792 2024-05-22 17:54:45.570205 fluxional-0.1.9/fluxional/core/infrastructure/base.py
+-rw-r--r--   0        0        0     7699 2024-04-28 18:14:21.953877 fluxional-0.1.9/fluxional/core/infrastructure/cdk.py
+-rw-r--r--   0        0        0     9773 2024-05-22 17:43:20.202417 fluxional-0.1.9/fluxional/core/infrastructure/resources.py
+-rw-r--r--   0        0        0      816 2024-04-28 18:14:21.953877 fluxional-0.1.9/fluxional/core/infrastructure/types.py
+-rw-r--r--   0        0        0     5818 2024-04-28 18:14:21.953877 fluxional-0.1.9/fluxional/core/logic.py
+-rw-r--r--   0        0        0     8565 2024-05-22 17:41:36.424841 fluxional-0.1.9/fluxional/core/settings.py
+-rw-r--r--   0        0        0     4045 2024-04-28 18:14:21.953877 fluxional-0.1.9/fluxional/core/tools.py
+-rw-r--r--   0        0        0     5158 2024-04-28 18:14:21.953877 fluxional-0.1.9/fluxional/core/types.py
+-rw-r--r--   0        0        0       74 2024-04-28 18:14:21.953877 fluxional-0.1.9/fluxional/deployment/__init__.py
+-rw-r--r--   0        0        0     1164 2024-04-28 18:14:21.953877 fluxional-0.1.9/fluxional/deployment/constants.py
+-rw-r--r--   0        0        0    15517 2024-04-30 22:02:31.375706 fluxional-0.1.9/fluxional/deployment/engine.py
+-rw-r--r--   0        0        0      345 2024-04-28 18:14:21.953877 fluxional-0.1.9/fluxional/deployment/exceptions.py
+-rw-r--r--   0        0        0        1 2024-04-30 22:01:04.012000 fluxional-0.1.9/fluxional/deployment/utils.py
+-rw-r--r--   0        0        0     3652 2024-04-28 18:14:21.963877 fluxional-0.1.9/fluxional/dev/__init__.py
+-rw-r--r--   0        0        0     3003 2024-04-28 18:14:21.963877 fluxional-0.1.9/fluxional/dev/client.py
+-rw-r--r--   0        0        0     3350 2024-04-28 18:14:21.963877 fluxional-0.1.9/fluxional/dev/runner.py
+-rw-r--r--   0        0        0      326 2024-04-28 18:14:21.963877 fluxional-0.1.9/fluxional/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-28 18:14:21.963877 fluxional-0.1.9/fluxional/py.typed
+-rw-r--r--   0        0        0      461 2024-04-28 18:14:21.963877 fluxional-0.1.9/fluxional/types.py
+-rw-r--r--   0        0        0      935 2024-04-28 18:14:21.963877 fluxional-0.1.9/fluxional/utils.py
+-rw-r--r--   0        0        0     1152 2024-05-22 17:55:00.731877 fluxional-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4852 1970-01-01 00:00:00.000000 fluxional-0.1.9/PKG-INFO
```

### Comparing `fluxional-0.1.8/LICENSE` & `fluxional-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.8/README.md` & `fluxional-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.8/fluxional/cli/__init__.py` & `fluxional-0.1.9/fluxional/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.8/fluxional/core/app.py` & `fluxional-0.1.9/fluxional/core/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,21 @@
 
         # @TODO: May need to refractor the whole storage workflow
         # Check
         if not self.settings.storage.enable and not self.storage.active:
             return
 
         # Resources
-        self.add_storage_bucket(remove_on_delete=self.settings.storage.remove_on_delete)
+        self.add_storage_bucket(
+            remove_on_delete=self.settings.storage.remove_on_delete,
+            allowed_origins=self.settings.storage.allowed_origins,
+            allowed_methods=self.settings.storage.allowed_methods,
+            allowed_headers=self.settings.storage.allowed_headers,
+            max_age=self.settings.storage.max_age,
+        )
 
         if isinstance(self.storage_bucket, S3Bucket):
             resources[self.storage_bucket.id] = self.storage_bucket
 
             storage_lambda = LambdaFunction(
                 id=self.settings.system.default_storage_lambda_id,
                 function_name=f"{stack_name}_{self.settings.system.default_storage_lambda_id}",
@@ -617,14 +623,18 @@
 
         self.database = dynamodb
 
     def add_storage_bucket(
         self,
         bucket_name: str | None = None,
         remove_on_delete: bool = True,
+        allowed_origins: list[str] = [],
+        allowed_methods: list[str] = [],
+        allowed_headers: list[str] = [],
+        max_age: int = 0,
     ) -> None:
         """
         Add an Storage bucket to the application
         """
 
         safe = lambda x: x.replace("_", "-").lower()  # noqa
 
@@ -633,13 +643,17 @@
             bucket_name=(
                 bucket_name
                 if bucket_name
                 else safe(self.settings.stack_name)
                 + safe(self.settings.system.default_storage_bucket_id)
             ),
             remove_on_delete=remove_on_delete,
+            allowed_origins=allowed_origins,
+            allowed_methods=allowed_methods,
+            allowed_headers=allowed_headers,
+            max_age=max_age,
         )
 
         self.storage_bucket = storage_bucket
 
     def set_api(self):
         self.api.active = True
```

### Comparing `fluxional-0.1.8/fluxional/core/core.py` & `fluxional-0.1.9/fluxional/core/core.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.8/fluxional/core/events.py` & `fluxional-0.1.9/fluxional/core/events.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.8/fluxional/core/handlers.py` & `fluxional-0.1.9/fluxional/core/handlers.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.8/fluxional/core/infrastructure/base.py` & `fluxional-0.1.9/fluxional/core/infrastructure/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     aws_events,
     aws_sqs,
     aws_s3,
     aws_lambda_event_sources,
 )
 from aws_cdk.aws_apigatewayv2_integrations_alpha import WebSocketLambdaIntegration
 from aws_cdk.aws_apigatewayv2 import WebSocketApi
+from aws_cdk.aws_s3 import HttpMethods
 from fluxional.exceptions import MissingStackResource
 from fluxional.utils import default_aws_account_id, default_aws_region
 from fluxional.core.tools import LookupKey
 
 
 class Stack(CDKStack):
     def __init__(
@@ -401,14 +402,32 @@
         bucket = add_s3_bucket_to_stack(
             stack=self,
             id=resource.id,
             bucket_name=resource.bucket_name,
             remove_on_delete=resource.remove_on_delete,
         )
 
+        # @TODO Move this to add s3 to stack and add tests
+        # To ensure cors is added correctly
+        http_methods_mapper = {
+            "get": HttpMethods.GET,
+            "put": HttpMethods.PUT,
+            "post": HttpMethods.POST,
+            "delete": HttpMethods.DELETE,
+        }
+
+        bucket.add_cors_rule(
+            allowed_headers=resource.allowed_headers,
+            allowed_methods=[
+                http_methods_mapper[k.lower()] for k in resource.allowed_methods
+            ],
+            allowed_origins=resource.allowed_origins,
+            max_age=resource.max_age,
+        )
+
         if resource.permissions:
             for k in resource.permissions:
                 if ResourceTypeGuard.is_lambda_permission(k) and k.allow_invoke:
                     func: aws_lambda.Function = getattr(self, k.resource_id)
 
                     bucket.add_object_created_notification(
                         aws_s3_notifications.LambdaDestination(func)
```

### Comparing `fluxional-0.1.8/fluxional/core/infrastructure/cdk.py` & `fluxional-0.1.9/fluxional/core/infrastructure/cdk.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.8/fluxional/core/infrastructure/resources.py` & `fluxional-0.1.9/fluxional/core/infrastructure/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,18 @@
     resource_type: Literal["sqs_queue"] = field(default="sqs_queue")
 
 
 @dataclass(kw_only=True)
 class S3Bucket(_ResourceT):
     bucket_name: str
     remove_on_delete: bool = field(default=True)
+    allowed_origins: list[str] = field(default_factory=list)
+    allowed_methods: list[str] = field(default_factory=list)
+    allowed_headers: list[str] = field(default_factory=list)
+    max_age: int = field(default=0)
     resource_type: Literal["s3_bucket"] = field(default="s3_bucket")
 
 
 @dataclass(kw_only=True)
 class RateSchedule(_ResourceT):
     schedule_name: str
     value: int | float
```

### Comparing `fluxional-0.1.8/fluxional/core/infrastructure/types.py` & `fluxional-0.1.9/fluxional/core/infrastructure/types.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.8/fluxional/core/logic.py` & `fluxional-0.1.9/fluxional/core/logic.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.8/fluxional/core/settings.py` & `fluxional-0.1.9/fluxional/core/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,18 @@
     enable_local: bool = field(default=False)
 
 
 @dataclass
 class StorageSettings:
     enable: bool = field(default=False)
     remove_on_delete: bool = field(default=True)
+    allowed_origins: list[str] = field(default_factory=list)
+    allowed_methods: list[str] = field(default_factory=list)
+    allowed_headers: list[str] = field(default_factory=list)
+    max_age: int = field(default=3600)
 
 
 @dataclass
 class Settings:
     stack_name: str = ""
     # Credentials
     credentials: CredentialsSettings = field(default_factory=CredentialsSettings)
```

### Comparing `fluxional-0.1.8/fluxional/core/tools.py` & `fluxional-0.1.9/fluxional/core/tools.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.8/fluxional/core/types.py` & `fluxional-0.1.9/fluxional/core/types.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.8/fluxional/deployment/constants.py` & `fluxional-0.1.9/fluxional/deployment/constants.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.8/fluxional/deployment/engine.py` & `fluxional-0.1.9/fluxional/deployment/engine.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.8/fluxional/dev/__init__.py` & `fluxional-0.1.9/fluxional/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.8/fluxional/dev/client.py` & `fluxional-0.1.9/fluxional/dev/client.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.8/fluxional/dev/runner.py` & `fluxional-0.1.9/fluxional/dev/runner.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.8/fluxional/utils.py` & `fluxional-0.1.9/fluxional/utils.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.8/pyproject.toml` & `fluxional-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fluxional"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["fluxional"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">= 3.10 < 4.0"
```

### Comparing `fluxional-0.1.8/PKG-INFO` & `fluxional-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxional
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 License: MIT
 Author: fluxional
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

