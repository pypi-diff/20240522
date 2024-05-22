# Comparing `tmp/oarepo_global_search-1.0.7.tar.gz` & `tmp/oarepo_global_search-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo_global_search-1.0.7.tar", last modified: Fri May 10 12:28:21 2024, max compression
+gzip compressed data, was "oarepo_global_search-1.0.8.tar", last modified: Wed May 22 14:15:29 2024, max compression
```

## Comparing `oarepo_global_search-1.0.7.tar` & `oarepo_global_search-1.0.8.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.140216 oarepo_global_search-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-10 12:28:21.136216 oarepo_global_search-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      194 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/format.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.132216 oarepo_global_search-1.0.7/oarepo_global_search/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.136216 oarepo_global_search-1.0.7/oarepo_global_search/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.136216 oarepo_global_search-1.0.7/oarepo_global_search/resources/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/resources/records/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/resources/records/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.136216 oarepo_global_search-1.0.7/oarepo_global_search/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.136216 oarepo_global_search-1.0.7/oarepo_global_search/services/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/services/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/services/records/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/services/records/params.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/services/records/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/services/records/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/services/records/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/services/records/user_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.136216 oarepo_global_search-1.0.7/oarepo_global_search/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/ui/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.132216 oarepo_global_search-1.0.7/oarepo_global_search/ui/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.132216 oarepo_global_search-1.0.7/oarepo_global_search/ui/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.136216 oarepo_global_search-1.0.7/oarepo_global_search/ui/templates/semantic-ui/global_search/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/ui/templates/semantic-ui/global_search/Search.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/ui/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.136216 oarepo_global_search-1.0.7/oarepo_global_search/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/views/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/oarepo_global_search/views/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:28:21.136216 oarepo_global_search-1.0.7/oarepo_global_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-10 12:28:21.000000 oarepo_global_search-1.0.7/oarepo_global_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-10 12:28:21.000000 oarepo_global_search-1.0.7/oarepo_global_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:28:21.000000 oarepo_global_search-1.0.7/oarepo_global_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-10 12:28:21.000000 oarepo_global_search-1.0.7/oarepo_global_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:25:10.000000 oarepo_global_search-1.0.7/oarepo_global_search.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-10 12:28:21.000000 oarepo_global_search-1.0.7/oarepo_global_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-10 12:28:21.000000 oarepo_global_search-1.0.7/oarepo_global_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      866 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-10 12:28:21.140216 oarepo_global_search-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-10 12:24:30.000000 oarepo_global_search-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.216615 oarepo_global_search-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-22 14:15:29.216615 oarepo_global_search-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      194 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/format.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.212615 oarepo_global_search-1.0.8/oarepo_global_search/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.212615 oarepo_global_search-1.0.8/oarepo_global_search/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.212615 oarepo_global_search-1.0.8/oarepo_global_search/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/resources/records/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/resources/records/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.212615 oarepo_global_search-1.0.8/oarepo_global_search/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.216615 oarepo_global_search-1.0.8/oarepo_global_search/services/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/services/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/services/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/services/records/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/services/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/services/records/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/services/records/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/services/records/user_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.216615 oarepo_global_search-1.0.8/oarepo_global_search/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/ui/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.208615 oarepo_global_search-1.0.8/oarepo_global_search/ui/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.208615 oarepo_global_search-1.0.8/oarepo_global_search/ui/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.216615 oarepo_global_search-1.0.8/oarepo_global_search/ui/templates/semantic-ui/global_search/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/ui/templates/semantic-ui/global_search/Search.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/ui/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.216615 oarepo_global_search-1.0.8/oarepo_global_search/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/views/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/oarepo_global_search/views/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:15:29.216615 oarepo_global_search-1.0.8/oarepo_global_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-22 14:15:29.000000 oarepo_global_search-1.0.8/oarepo_global_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-22 14:15:29.000000 oarepo_global_search-1.0.8/oarepo_global_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:15:29.000000 oarepo_global_search-1.0.8/oarepo_global_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-22 14:15:29.000000 oarepo_global_search-1.0.8/oarepo_global_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:12:25.000000 oarepo_global_search-1.0.8/oarepo_global_search.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-22 14:15:29.000000 oarepo_global_search-1.0.8/oarepo_global_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 14:15:29.000000 oarepo_global_search-1.0.8/oarepo_global_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      866 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-22 14:15:29.216615 oarepo_global_search-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-22 14:11:46.000000 oarepo_global_search-1.0.8/setup.py
```

### Comparing `oarepo_global_search-1.0.7/MANIFEST.in` & `oarepo_global_search-1.0.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.7/oarepo_global_search/ext.py` & `oarepo_global_search-1.0.8/oarepo_global_search/ext.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         app.extensions["global_search"] = self
 
     @functools.cached_property
     def model_services(self):
         # load all models from json files registered in oarepo.ui entry point
         ret = []
         eps = entry_points(group="oarepo.models")
+
         for ep in eps:
             path = Path(obj_or_import_string(ep.module).__file__).parent / ep.attr
             model = json.loads(path.read_text())
             service_id = (
                 model.get("model", {}).get("service-config", {}).get("service-id")
             )
             if service_id and service_id in current_service_registry._services:
```

### Comparing `oarepo_global_search-1.0.7/oarepo_global_search/resources/records/config.py` & `oarepo_global_search-1.0.8/oarepo_global_search/resources/records/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,72 @@
+import copy
+
 from invenio_records_resources.resources.records.config import RecordResourceConfig
 from flask import current_app
 from invenio_base.utils import obj_or_import_string
 from flask_resources import ResponseHandler
+from flask import Response, make_response
+from flask_resources.context import resource_requestctx
+from .response import GlobalSearchResponseHandler
+import json
+
 
 
 class GlobalSearchResourceConfig(RecordResourceConfig):
     blueprint_name = "global_search"
     url_prefix = "/search"
     routes = {
         "list": "/",
     }
 
     @property
     def response_handlers(self):
         entrypoint_response_handlers = {}
 
         resource_defs = current_app.config.get("GLOBAL_SEARCH_MODELS")
-        api_resources = []
+        serializers = []
+
         for definition in resource_defs:
             api_resource = obj_or_import_string(definition["api_resource_config"])
-            api_resources.append(api_resource)
             handler = api_resource().response_handlers
+            service_def = obj_or_import_string(definition["model_service"])
+            service_cfg = obj_or_import_string(definition["service_config"])
+            service = service_def(service_cfg())
+            serializers.append({"schema": service.record_cls.schema.value,
+                                "serializer": handler["application/vnd.inveniordm.v1+json"].serializer})
 
         return {
-            "application/vnd.inveniordm.v1+json": ResponseHandler(
-                handler["application/vnd.inveniordm.v1+json"].serializer
+            "application/vnd.inveniordm.v1+json": GlobalSearchResponseHandler(
+                serializers
             ),
             **super().response_handlers,
             **entrypoint_response_handlers,
         }
-
 class GlobalUserSearchResourceConfig(RecordResourceConfig):
     blueprint_name = "global_user_search"
     url_prefix = "/user/search"
     routes = {
         "list": "/",
     }
 
     @property
     def response_handlers(self):
         entrypoint_response_handlers = {}
 
         resource_defs = current_app.config.get("GLOBAL_SEARCH_MODELS")
-        api_resources = []
+        serializers = []
+
         for definition in resource_defs:
             api_resource = obj_or_import_string(definition["api_resource_config"])
-            api_resources.append(api_resource)
             handler = api_resource().response_handlers
+            service_def = obj_or_import_string(definition["model_service"])
+            service_cfg = obj_or_import_string(definition["service_config"])
+            service = service_def(service_cfg())
+            serializers.append({"schema": service.record_cls.schema.value,"serializer": handler["application/vnd.inveniordm.v1+json"].serializer })
 
-        # todo own Handler class
         return {
-            "application/vnd.inveniordm.v1+json": ResponseHandler(
-                handler["application/vnd.inveniordm.v1+json"].serializer
+            "application/vnd.inveniordm.v1+json": GlobalSearchResponseHandler(
+                serializers
             ),
             **super().response_handlers,
             **entrypoint_response_handlers,
-        }
+        }
```

### Comparing `oarepo_global_search-1.0.7/oarepo_global_search/resources/records/resource.py` & `oarepo_global_search-1.0.8/oarepo_global_search/resources/records/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.7/oarepo_global_search/services/records/params.py` & `oarepo_global_search-1.0.8/oarepo_global_search/services/records/params.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.7/oarepo_global_search/services/records/results.py` & `oarepo_global_search-1.0.8/oarepo_global_search/services/records/results.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,26 @@
     RecordList as BaseRecordList,
 )
 
 
 class GlobalSearchResultList(BaseRecordList):
     services = []
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    @property
+    def aggregations(self):
+        """Get the search result aggregations."""
+        # TODO: have a way to label or not label
+        try:
+            return self._results.labelled_facets.to_dict()
+        except AttributeError:
+            return None
+
     @property
     def hits(self):
         """Iterator over the hits."""
         records = []
         hits_array = []
         order = []
         for hit in self._results:
```

### Comparing `oarepo_global_search-1.0.7/oarepo_global_search/services/records/user_service.py` & `oarepo_global_search-1.0.8/oarepo_global_search/services/records/user_service.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from oarepo_global_search.proxies import current_global_search
 from oarepo_global_search.services.records.service import GlobalSearchService
 
 
 class GlobalUserSearchService(GlobalSearchService):
     """GlobalSearchRecord service."""
+    components_def = True
 
     def indices(self):
         indices = []
         for s in current_global_search.model_services:
             indices.append(s.record_cls.index.search_alias)
             if getattr(s, "draft_cls", None):
                 indices.append(s.draft_cls.index.search_alias)
```

### Comparing `oarepo_global_search-1.0.7/oarepo_global_search/views/api.py` & `oarepo_global_search-1.0.8/oarepo_global_search/views/api.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.7/oarepo_global_search/views/app.py` & `oarepo_global_search-1.0.8/oarepo_global_search/views/app.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.7/oarepo_global_search.egg-info/SOURCES.txt` & `oarepo_global_search-1.0.8/oarepo_global_search.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 oarepo_global_search.egg-info/not-zip-safe
 oarepo_global_search.egg-info/requires.txt
 oarepo_global_search.egg-info/top_level.txt
 oarepo_global_search/resources/__init__.py
 oarepo_global_search/resources/records/__init__.py
 oarepo_global_search/resources/records/config.py
 oarepo_global_search/resources/records/resource.py
+oarepo_global_search/resources/records/response.py
 oarepo_global_search/services/__init__.py
 oarepo_global_search/services/records/__init__.py
 oarepo_global_search/services/records/api.py
 oarepo_global_search/services/records/params.py
 oarepo_global_search/services/records/permissions.py
 oarepo_global_search/services/records/results.py
 oarepo_global_search/services/records/service.py
```

### Comparing `oarepo_global_search-1.0.7/oarepo_global_search.egg-info/entry_points.txt` & `oarepo_global_search-1.0.8/oarepo_global_search.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.7/run-tests.sh` & `oarepo_global_search-1.0.8/run-tests.sh`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.7/setup.cfg` & `oarepo_global_search-1.0.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-global-search
-version = 1.0.7
+version = 1.0.8
 description = "A model builder plugin for global search"
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = invenio relations model builder
 license = MIT
 author = Alzbeta Pokorna
 author_email = Alzbeta.Pokorna@cesnet.cz
```

