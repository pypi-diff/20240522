# Comparing `tmp/faster-sam-0.8.0.tar.gz` & `tmp/faster-sam-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faster-sam-0.8.0.tar", last modified: Wed Mar 13 14:23:40 2024, max compression
+gzip compressed data, was "faster-sam-0.9.0.tar", last modified: Wed Mar 20 20:03:24 2024, max compression
```

## Comparing `faster-sam-0.8.0.tar` & `faster-sam-0.9.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:23:40.734917 faster-sam-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-13 14:23:34.000000 faster-sam-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-03-13 14:23:40.734917 faster-sam-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-13 14:23:34.000000 faster-sam-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:23:40.730917 faster-sam-0.8.0/faster_sam/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-13 14:23:34.000000 faster-sam-0.8.0/faster_sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-03-13 14:23:34.000000 faster-sam-0.8.0/faster_sam/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:23:40.730917 faster-sam-0.8.0/faster_sam/cache/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 14:23:34.000000 faster-sam-0.8.0/faster_sam/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-03-13 14:23:34.000000 faster-sam-0.8.0/faster_sam/cache/cache_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-03-13 14:23:34.000000 faster-sam-0.8.0/faster_sam/cache/redis_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-03-13 14:23:34.000000 faster-sam-0.8.0/faster_sam/cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-03-13 14:23:34.000000 faster-sam-0.8.0/faster_sam/lambda_event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:23:40.730917 faster-sam-0.8.0/faster_sam/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 14:23:34.000000 faster-sam-0.8.0/faster_sam/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12385 2024-03-13 14:23:34.000000 faster-sam-0.8.0/faster_sam/middlewares/lambda_authorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-03-13 14:23:34.000000 faster-sam-0.8.0/faster_sam/middlewares/remove_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-03-13 14:23:34.000000 faster-sam-0.8.0/faster_sam/middlewares/rewrite_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-03-13 14:23:34.000000 faster-sam-0.8.0/faster_sam/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-03-13 14:23:34.000000 faster-sam-0.8.0/faster_sam/routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-13 14:23:34.000000 faster-sam-0.8.0/faster_sam/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-03-13 14:23:34.000000 faster-sam-0.8.0/faster_sam/web_identity_providers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:23:40.734917 faster-sam-0.8.0/faster_sam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-03-13 14:23:40.000000 faster-sam-0.8.0/faster_sam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-13 14:23:40.000000 faster-sam-0.8.0/faster_sam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 14:23:40.000000 faster-sam-0.8.0/faster_sam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-13 14:23:40.000000 faster-sam-0.8.0/faster_sam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-13 14:23:40.000000 faster-sam-0.8.0/faster_sam.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-13 14:23:34.000000 faster-sam-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 14:23:40.734917 faster-sam-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:23:40.734917 faster-sam-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-03-13 14:23:34.000000 faster-sam-0.8.0/tests/test_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-03-13 14:23:34.000000 faster-sam-0.8.0/tests/test_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-03-13 14:23:34.000000 faster-sam-0.8.0/tests/test_lambda_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    18000 2024-03-13 14:23:34.000000 faster-sam-0.8.0/tests/test_middleware_lambda_authorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-13 14:23:34.000000 faster-sam-0.8.0/tests/test_middleware_remove_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-13 14:23:34.000000 faster-sam-0.8.0/tests/test_middleware_rewrite_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-03-13 14:23:34.000000 faster-sam-0.8.0/tests/test_openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-13 14:23:34.000000 faster-sam-0.8.0/tests/test_redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-03-13 14:23:34.000000 faster-sam-0.8.0/tests/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-13 14:23:34.000000 faster-sam-0.8.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-03-13 14:23:34.000000 faster-sam-0.8.0/tests/test_web_identity_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:03:24.343319 faster-sam-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-20 20:03:10.000000 faster-sam-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-03-20 20:03:24.343319 faster-sam-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-20 20:03:10.000000 faster-sam-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:03:24.339319 faster-sam-0.9.0/faster_sam/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-20 20:03:10.000000 faster-sam-0.9.0/faster_sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-03-20 20:03:10.000000 faster-sam-0.9.0/faster_sam/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:03:24.339319 faster-sam-0.9.0/faster_sam/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 20:03:10.000000 faster-sam-0.9.0/faster_sam/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-03-20 20:03:10.000000 faster-sam-0.9.0/faster_sam/cache/cache_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-03-20 20:03:10.000000 faster-sam-0.9.0/faster_sam/cache/redis_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-03-20 20:03:10.000000 faster-sam-0.9.0/faster_sam/cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-03-20 20:03:10.000000 faster-sam-0.9.0/faster_sam/lambda_event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:03:24.343319 faster-sam-0.9.0/faster_sam/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 20:03:10.000000 faster-sam-0.9.0/faster_sam/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12385 2024-03-20 20:03:10.000000 faster-sam-0.9.0/faster_sam/middlewares/lambda_authorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-03-20 20:03:10.000000 faster-sam-0.9.0/faster_sam/middlewares/remove_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-03-20 20:03:10.000000 faster-sam-0.9.0/faster_sam/middlewares/rewrite_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-03-20 20:03:10.000000 faster-sam-0.9.0/faster_sam/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-03-20 20:03:10.000000 faster-sam-0.9.0/faster_sam/routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-20 20:03:10.000000 faster-sam-0.9.0/faster_sam/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-03-20 20:03:10.000000 faster-sam-0.9.0/faster_sam/web_identity_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:03:24.343319 faster-sam-0.9.0/faster_sam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-03-20 20:03:24.000000 faster-sam-0.9.0/faster_sam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-20 20:03:24.000000 faster-sam-0.9.0/faster_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 20:03:24.000000 faster-sam-0.9.0/faster_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-20 20:03:24.000000 faster-sam-0.9.0/faster_sam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-20 20:03:24.000000 faster-sam-0.9.0/faster_sam.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-20 20:03:10.000000 faster-sam-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 20:03:24.343319 faster-sam-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:03:24.343319 faster-sam-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-03-20 20:03:10.000000 faster-sam-0.9.0/tests/test_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-03-20 20:03:10.000000 faster-sam-0.9.0/tests/test_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-03-20 20:03:10.000000 faster-sam-0.9.0/tests/test_lambda_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18000 2024-03-20 20:03:10.000000 faster-sam-0.9.0/tests/test_middleware_lambda_authorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-20 20:03:10.000000 faster-sam-0.9.0/tests/test_middleware_remove_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-20 20:03:10.000000 faster-sam-0.9.0/tests/test_middleware_rewrite_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-03-20 20:03:10.000000 faster-sam-0.9.0/tests/test_openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-20 20:03:10.000000 faster-sam-0.9.0/tests/test_redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-03-20 20:03:10.000000 faster-sam-0.9.0/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-20 20:03:10.000000 faster-sam-0.9.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-03-20 20:03:10.000000 faster-sam-0.9.0/tests/test_web_identity_providers.py
```

### Comparing `faster-sam-0.8.0/LICENSE` & `faster-sam-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `faster-sam-0.8.0/PKG-INFO` & `faster-sam-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster-sam
-Version: 0.8.0
+Version: 0.9.0
 Summary: An adapter to enable running APIs built with AWS SAM applications using FastAPI.
 Author-email: Dotz Developers <devs-dotz@dotz.com>
 License: MIT
 Keywords: utilities,fastapi,sam
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `faster-sam-0.8.0/README.md` & `faster-sam-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `faster-sam-0.8.0/faster_sam/adapter.py` & `faster-sam-0.9.0/faster_sam/adapter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from typing import Any, Dict, Optional
 
 from fastapi import FastAPI
 
 from faster_sam.cloudformation import CloudformationTemplate, NodeType
 from faster_sam.openapi import custom_openapi
-from faster_sam.routing import APIRoute, QueueRoute
+from faster_sam.routing import APIRoute, QueueRoute, ScheduleRoute
 
 ARN_PATTERN = r"^arn:aws:apigateway.*\${(\w+)\.Arn}/invocations$"
 
 
 class GatewayLookupError(LookupError):
     """
     Raised when performing API Gateway lookup, usually when multiple gateways
@@ -102,14 +102,31 @@
         app : FastAPI
             The FastAPI application instance to be configured.
         """
         routes = self.lambda_queue_mapper()
 
         self.register_routes(app, routes, QueueRoute)
 
+    def configure_schedule(
+        self,
+        app: FastAPI,
+    ) -> None:
+        """
+        Configures the FastAPI application with routes based on schedule defined
+        in cloudformation template.
+
+        Parameters
+        ----------
+        app : FastAPI
+            The FastAPI application instance to be configured.
+        """
+        routes = self.lambda_schedule_mapper()
+
+        self.register_routes(app, routes, ScheduleRoute)
+
     def openapi_mapper(self, openapi_schema: Dict[str, Any]) -> Dict[str, Any]:
         """
         Create a route map extracted from the given OpenAPI schema.
 
         Notice that this is an OpenAPI schema used by AWS SAM to configure
         an API Gateway, therefore it requires AWS extensions pointing to
         event consumers, most of the time Lambda Functions.
@@ -197,14 +214,48 @@
                 path = f"/{queue_name}"
                 endpoint = {"POST": {"handler": handler_path}}
 
                 routes.setdefault(path, {}).update(endpoint)
 
         return routes
 
+    def lambda_schedule_mapper(self) -> Dict[str, Any]:
+        """
+        Generate a route map extracted from the lambda functions that is a schedule consumer
+        using the name of the function name as path.
+
+        Returns
+        -------
+        Dict[str, Any]
+            Dictionary containing the routes.
+        """
+
+        routes: Dict[str, Any] = {}
+
+        for resource_id, function in self.template.functions.items():
+            if "Events" not in function["Properties"]:
+                continue
+
+            events = self.template.find_nodes(
+                function["Properties"]["Events"], NodeType.SCHEDULER_EVENT
+            )
+
+            if not events:
+                continue
+
+            function_name = function["Properties"]["FunctionName"].replace("_", "-")
+            handler_path = self.template.lambda_handler(resource_id)
+
+            path = f"/{function_name}"
+            endpoint = {"POST": {"handler": handler_path}}
+
+            routes.setdefault(path, {}).update(endpoint)
+
+        return routes
+
     def lambda_mapper(self, gateway_id: Optional[str]) -> Dict[str, Any]:
         """
         Generate a route map extracted from the lambda functions schema
         corresponding to the given gateway id.
 
         Parameters
         ----------
```

### Comparing `faster-sam-0.8.0/faster_sam/cache/cache_interface.py` & `faster-sam-0.9.0/faster_sam/cache/cache_interface.py`

 * *Files identical despite different names*

### Comparing `faster-sam-0.8.0/faster_sam/cache/redis_cache.py` & `faster-sam-0.9.0/faster_sam/cache/redis_cache.py`

 * *Files identical despite different names*

### Comparing `faster-sam-0.8.0/faster_sam/cloudformation.py` & `faster-sam-0.9.0/faster_sam/cloudformation.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,21 +42,24 @@
         Represents the "AWS::Serverless::Api" node type.
     LAMBDA : str
         Represents the "AWS::Serverless::Function" node type.
     QUEUE : str
         Represents the "AWS::SQS::Queue" node type.
     API_EVENT : str
         Represents the "Api" node type.
+    SCHEDULER_EVENT : str
+        Represents the "Schedule" node type.
     """
 
     API_GATEWAY = "AWS::Serverless::Api"
     LAMBDA = "AWS::Serverless::Function"
     QUEUE = "AWS::SQS::Queue"
     API_EVENT = "Api"
     SQS_EVENT = "SQS"
+    SCHEDULER_EVENT = "Schedule"
 
 
 def multi_constructor(loader: CFLoader, tag_suffix: str, node: yaml.nodes.Node) -> Dict[str, Any]:
     """
     Custom YAML node constructor.
 
     Handles AWS CloudFormation extensions for its short version of intrinsic functions.
```

### Comparing `faster-sam-0.8.0/faster_sam/lambda_event.py` & `faster-sam-0.9.0/faster_sam/lambda_event.py`

 * *Files 8% similar despite different names*

```diff
@@ -164,14 +164,77 @@
                     "awsRegion": "us-east-2",
                 },
             ]
         }
         return event
 
 
+class Schedule(ResourceInterface):
+    def __init__(self, request: Request, endpoint: Handler):
+        """
+        Initializes the Schedule.
+
+        Parameters
+        ----------
+        request : Request
+            A request object.
+        endpoint : Handler
+            A callable object.
+        """
+        super().__init__(request, endpoint)
+
+    async def call_endpoint(self) -> Response:
+        """
+        Call event buider and retuns a custom response based
+        on the mapped event.
+
+        Returns
+        -------
+        Response
+            A response object.
+        """
+        event = await self.event_builder()
+        try:
+            result = self.endpoint(event, None)
+        except Exception as error:
+            logger.exception(error)
+            return CustomResponse({"body": "Error executing schedule function", "statusCode": 500})
+
+        return CustomResponse({"body": json.dumps(result), "statusCode": 200})
+
+    async def event_builder(self):
+        """
+        Builds an event of type schedule
+
+        It uses the given request object to fill the event details.
+
+        Returns
+        -------
+        Dict[str, Any]
+            An schedule event.
+        """
+
+        bytes_body = await self.request.body()
+        json_body = bytes_body.decode()
+        body = json.loads(json_body)
+        event = {
+            "version": "0",
+            "id": str(uuid4()),
+            "detail-type": "Scheduled Event",
+            "source": "aws.events",
+            "account": "",
+            "time": datetime.now(timezone.utc).strftime(r"%d/%b/%Y:%H:%M:%S %z"),
+            "region": "us-east-1",
+            "resources": [""],
+            "detail": body,
+        }
+
+        return event
+
+
 class ApiGateway(ResourceInterface):
     def __init__(self, request: Request, endpoint: Handler):
         """
         Initializes the ApiGateway.
 
         Parameters
         ----------
```

### Comparing `faster-sam-0.8.0/faster_sam/middlewares/lambda_authorizer.py` & `faster-sam-0.9.0/faster_sam/middlewares/lambda_authorizer.py`

 * *Files identical despite different names*

### Comparing `faster-sam-0.8.0/faster_sam/middlewares/remove_path.py` & `faster-sam-0.9.0/faster_sam/middlewares/remove_path.py`

 * *Files identical despite different names*

### Comparing `faster-sam-0.8.0/faster_sam/middlewares/rewrite_path.py` & `faster-sam-0.9.0/faster_sam/middlewares/rewrite_path.py`

 * *Files identical despite different names*

### Comparing `faster-sam-0.8.0/faster_sam/openapi.py` & `faster-sam-0.9.0/faster_sam/openapi.py`

 * *Files identical despite different names*

### Comparing `faster-sam-0.8.0/faster_sam/routing.py` & `faster-sam-0.9.0/faster_sam/routing.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from typing import Any, Awaitable, Callable, Dict
 
 from fastapi import Request, Response, routing
 
-from faster_sam.lambda_event import SQS, ApiGateway, ResourceInterface
+from faster_sam.lambda_event import SQS, ApiGateway, ResourceInterface, Schedule
 
 logger = logging.getLogger(__name__)
 
 Handler = Callable[[Dict[str, Any], Any], Dict[str, Any]]
 Endpoint = Callable[[Request], Awaitable[Response]]
 
 
@@ -99,7 +99,30 @@
             HTTP route path.
         endpoint : str
             Full module path.
         """
         handler_path = endpoint
         handler_func = import_handler(handler_path)
         super().__init__(path=path, endpoint=handler(handler_func, SQS), *args, **kwargs)
+
+
+class ScheduleRoute(routing.APIRoute):
+    """
+    Extends FastAPI Router class used to describe path operations.
+    This custom router class receives the endpoint parameter as a string with
+    the full module path instead of the actual callable.
+    """
+
+    def __init__(self, path: str, endpoint: str, *args, **kwargs):
+        """
+        Initializes the ScheduleRoute object.
+
+        Parameters
+        ----------
+        path : str
+            HTTP route path.
+        endpoint : str
+            Full module path.
+        """
+        handler_path = endpoint
+        handler_func = import_handler(handler_path)
+        super().__init__(path=path, endpoint=handler(handler_func, Schedule), *args, **kwargs)
```

### Comparing `faster-sam-0.8.0/faster_sam/utils.py` & `faster-sam-0.9.0/faster_sam/utils.py`

 * *Files identical despite different names*

### Comparing `faster-sam-0.8.0/faster_sam/web_identity_providers.py` & `faster-sam-0.9.0/faster_sam/web_identity_providers.py`

 * *Files identical despite different names*

### Comparing `faster-sam-0.8.0/faster_sam.egg-info/PKG-INFO` & `faster-sam-0.9.0/faster_sam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster-sam
-Version: 0.8.0
+Version: 0.9.0
 Summary: An adapter to enable running APIs built with AWS SAM applications using FastAPI.
 Author-email: Dotz Developers <devs-dotz@dotz.com>
 License: MIT
 Keywords: utilities,fastapi,sam
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `faster-sam-0.8.0/faster_sam.egg-info/SOURCES.txt` & `faster-sam-0.9.0/faster_sam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `faster-sam-0.8.0/pyproject.toml` & `faster-sam-0.9.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faster-sam"
-version = "0.8.0"
+version = "0.9.0"
 description = "An adapter to enable running APIs built with AWS SAM applications using FastAPI."
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [
     {name = "Dotz Developers", email = "devs-dotz@dotz.com"},
 ]
 license = {text = "MIT"}
 keywords = ["utilities", "fastapi", "sam"]
```

### Comparing `faster-sam-0.8.0/tests/test_adapter.py` & `faster-sam-0.9.0/tests/test_adapter.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,14 +56,23 @@
         sam = SAM("tests/fixtures/templates/example6.yml")
 
         self.assertEqual(len(app.routes), 4)
 
         sam.configure_queues(app)
         self.assertEqual(len(app.routes), 5)
 
+    def test_configure_schedule(self):
+        app = FastAPI()
+        sam = SAM("tests/fixtures/templates/example7.yml")
+
+        self.assertEqual(len(app.routes), 4)
+
+        sam.configure_schedule(app)
+        self.assertEqual(len(app.routes), 5)
+
     def test_configure_api_raises_gateway_lookup_error(self):
         error = "^Missing required gateway ID. Found: ApiGateway, ApiGatewayTwo"
 
         with self.assertRaisesRegex(GatewayLookupError, error):
             app = FastAPI()
             sam = SAM(self.templates[3])
             sam.configure_api(app)
```

### Comparing `faster-sam-0.8.0/tests/test_cloudformation.py` & `faster-sam-0.9.0/tests/test_cloudformation.py`

 * *Files identical despite different names*

### Comparing `faster-sam-0.8.0/tests/test_lambda_event.py` & `faster-sam-0.9.0/tests/test_lambda_event.py`

 * *Files 16% similar despite different names*

```diff
@@ -65,14 +65,35 @@
         "client": ("127.0.0.1", 80),
         "app": FastAPI(),
     }
 
     return Request(scope, receive)
 
 
+def build_request_schedule():
+
+    async def receive():
+        body = {}
+        return {"type": "http.request", "body": json.dumps(body).encode()}
+
+    scope = {
+        "type": "http",
+        "http_version": "1.1",
+        "root_path": "",
+        "path": "/test",
+        "method": "GET",
+        "query_string": [],
+        "path_params": {},
+        "client": ("127.0.0.1", 80),
+        "app": FastAPI(),
+    }
+
+    return Request(scope, receive)
+
+
 class TestCustomResponse(unittest.TestCase):
     def setUp(self):
         self.data = {
             "statusCode": HTTPStatus.OK.value,
             "body": '{"message": "test"}',
             "headers": {"content-type": "application/json"},
         }
@@ -142,7 +163,33 @@
 
         sqs = faster_sam.lambda_event.SQS(request, handler)
 
         event = await sqs.event_builder()
 
         self.assertIsInstance(event, dict)
         self.assertEqual(set(event["Records"][0].keys()), expected_key)
+
+    async def test_event_builder_schedule(self):
+        request = build_request_schedule()
+        expected_keys = {
+            "version",
+            "id",
+            "detail-type",
+            "source",
+            "account",
+            "time",
+            "region",
+            "resources",
+            "detail",
+        }
+
+        module_name = "tests.fixtures.handlers.lambda_handler"
+        handler_name = "handler"
+        handler_path = f"{module_name}.{handler_name}"
+        handler = faster_sam.routing.import_handler(handler_path)
+
+        schedule = faster_sam.lambda_event.Schedule(request, handler)
+
+        event = await schedule.event_builder()
+
+        self.assertIsInstance(event, dict)
+        self.assertEqual(set(event.keys()), expected_keys)
```

### Comparing `faster-sam-0.8.0/tests/test_middleware_lambda_authorizer.py` & `faster-sam-0.9.0/tests/test_middleware_lambda_authorizer.py`

 * *Files identical despite different names*

### Comparing `faster-sam-0.8.0/tests/test_middleware_remove_path.py` & `faster-sam-0.9.0/tests/test_middleware_remove_path.py`

 * *Files identical despite different names*

### Comparing `faster-sam-0.8.0/tests/test_middleware_rewrite_path.py` & `faster-sam-0.9.0/tests/test_middleware_rewrite_path.py`

 * *Files identical despite different names*

### Comparing `faster-sam-0.8.0/tests/test_openapi.py` & `faster-sam-0.9.0/tests/test_openapi.py`

 * *Files identical despite different names*

### Comparing `faster-sam-0.8.0/tests/test_redis.py` & `faster-sam-0.9.0/tests/test_redis.py`

 * *Files identical despite different names*

### Comparing `faster-sam-0.8.0/tests/test_routing.py` & `faster-sam-0.9.0/tests/test_routing.py`

 * *Files 11% similar despite different names*

```diff
@@ -64,14 +64,35 @@
         "client": ("127.0.0.1", 80),
         "app": FastAPI(),
     }
 
     return Request(scope, receive)
 
 
+def build_request_schedule():
+
+    async def receive():
+        body = {"x": "y"}
+        return {"type": "http.request", "body": json.dumps(body).encode()}
+
+    scope = {
+        "type": "http",
+        "http_version": "1.1",
+        "root_path": "",
+        "path": "/test",
+        "method": "GET",
+        "query_string": [],
+        "path_params": {},
+        "client": ("127.0.0.1", 80),
+        "app": FastAPI(),
+    }
+
+    return Request(scope, receive)
+
+
 class TestAPIRoute(unittest.TestCase):
     def test_route(self):
         endpoint = "tests.fixtures.handlers.lambda_handler.handler"
 
         route = faster_sam.routing.APIRoute(path="/test", name="test", endpoint=endpoint)
 
         self.assertEqual(route.path, "/test")
@@ -163,7 +184,31 @@
 
         self.assertIsInstance(response, Response)
         self.assertEqual(response.status_code, HTTPStatus.INTERNAL_SERVER_ERROR.value)
         self.assertEqual(
             response.body.decode(),
             '{"statusCode": 500, "body": "hello", "batchItemFailures": "foo"}',
         )
+
+    async def test_schedule_handler(self):
+        request = build_request_schedule()
+
+        def echo(event, _):
+            return {
+                "statusCode": HTTPStatus.OK.value,
+                "body": event["detail"],
+            }
+
+        cases = {
+            "none_as_return": {"func": lambda event, _: None, "response": "null"},
+            "dict_as_return": {"func": echo, "response": '{"statusCode": 200, "body": {"x": "y"}}'},
+        }
+
+        for case, value in cases.items():
+            with self.subTest(case=case):
+                endpoint = faster_sam.routing.handler(
+                    value["func"], faster_sam.lambda_event.Schedule
+                )
+                response = await endpoint(request)
+                self.assertIsInstance(response, Response)
+                self.assertEqual(response.status_code, HTTPStatus.OK.value)
+                self.assertEqual(response.body.decode(), value["response"])
```

### Comparing `faster-sam-0.8.0/tests/test_utils.py` & `faster-sam-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `faster-sam-0.8.0/tests/test_web_identity_providers.py` & `faster-sam-0.9.0/tests/test_web_identity_providers.py`

 * *Files identical despite different names*

