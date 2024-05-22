# Comparing `tmp/stac_fastapi_api-3.0.0a0.tar.gz` & `tmp/stac_fastapi_api-3.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_api-3.0.0a0.tar", last modified: Mon May  6 16:07:40 2024, max compression
+gzip compressed data, was "stac_fastapi_api-3.0.0a1.tar", last modified: Wed May 22 11:04:04 2024, max compression
```

## Comparing `stac_fastapi_api-3.0.0a0.tar` & `stac_fastapi_api-3.0.0a1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:40.282728 stac_fastapi_api-3.0.0a0/
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-06 16:07:40.282728 stac_fastapi_api-3.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-06 16:07:40.282728 stac_fastapi_api-3.0.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:40.274727 stac_fastapi_api-3.0.0a0/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:40.278728 stac_fastapi_api-3.0.0a0/stac_fastapi/api/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/stac_fastapi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16992 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/stac_fastapi/api/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/stac_fastapi/api/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/stac_fastapi/api/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/stac_fastapi/api/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/stac_fastapi/api/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/stac_fastapi/api/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/stac_fastapi/api/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/stac_fastapi/api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:40.278728 stac_fastapi_api-3.0.0a0/stac_fastapi.api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-06 16:07:40.000000 stac_fastapi_api-3.0.0a0/stac_fastapi.api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-06 16:07:40.000000 stac_fastapi_api-3.0.0a0/stac_fastapi.api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:07:40.000000 stac_fastapi_api-3.0.0a0/stac_fastapi.api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:07:40.000000 stac_fastapi_api-3.0.0a0/stac_fastapi.api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-06 16:07:40.000000 stac_fastapi_api-3.0.0a0/stac_fastapi.api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-06 16:07:40.000000 stac_fastapi_api-3.0.0a0/stac_fastapi.api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:40.278728 stac_fastapi_api-3.0.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/tests/test_app_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:04:04.536846 stac_fastapi_api-3.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-22 11:04:04.536846 stac_fastapi_api-3.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-22 11:04:04.536846 stac_fastapi_api-3.0.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:04:04.532846 stac_fastapi_api-3.0.0a1/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:04:04.536846 stac_fastapi_api-3.0.0a1/stac_fastapi/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/stac_fastapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/stac_fastapi/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/stac_fastapi/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/stac_fastapi/api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/stac_fastapi/api/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/stac_fastapi/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/stac_fastapi/api/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/stac_fastapi/api/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/stac_fastapi/api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:04:04.536846 stac_fastapi_api-3.0.0a1/stac_fastapi.api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-22 11:04:04.000000 stac_fastapi_api-3.0.0a1/stac_fastapi.api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-22 11:04:04.000000 stac_fastapi_api-3.0.0a1/stac_fastapi.api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:04:04.000000 stac_fastapi_api-3.0.0a1/stac_fastapi.api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:04:04.000000 stac_fastapi_api-3.0.0a1/stac_fastapi.api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-22 11:04:04.000000 stac_fastapi_api-3.0.0a1/stac_fastapi.api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 11:04:04.000000 stac_fastapi_api-3.0.0a1/stac_fastapi.api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:04:04.536846 stac_fastapi_api-3.0.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/tests/test_app_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/tests/test_models.py
```

### Comparing `stac_fastapi_api-3.0.0a0/PKG-INFO` & `stac_fastapi_api-3.0.0a1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.api
-Version: 3.0.0a0
+Version: 3.0.0a1
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
@@ -23,14 +23,13 @@
 Provides-Extra: dev
 Requires-Dist: httpx; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: requests; extra == "dev"
-Requires-Dist: pystac[validation]==1.*; extra == "dev"
 Provides-Extra: benchmark
 Requires-Dist: pytest-benchmark; extra == "benchmark"
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: pdocs; extra == "docs"
```

### Comparing `stac_fastapi_api-3.0.0a0/setup.py` & `stac_fastapi_api-3.0.0a1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     "dev": [
         "httpx",
         "pytest",
         "pytest-cov",
         "pytest-asyncio",
         "pre-commit",
         "requests",
-        "pystac[validation]==1.*",
     ],
     "benchmark": [
         "pytest-benchmark",
     ],
     "docs": ["mkdocs", "mkdocs-material", "pdocs"],
 }
```

### Comparing `stac_fastapi_api-3.0.0a0/stac_fastapi/api/app.py` & `stac_fastapi_api-3.0.0a1/stac_fastapi/api/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,22 +168,22 @@
         Returns:
             None
         """
         self.router.add_api_route(
             name="Conformance Classes",
             path="/conformance",
             response_model=(
-                api.ConformanceClasses if self.settings.enable_response_models else None
+                api.Conformance if self.settings.enable_response_models else None
             ),
             responses={
                 200: {
                     "content": {
                         MimeTypes.json.value: {},
                     },
-                    "model": api.ConformanceClasses,
+                    "model": api.Conformance,
                 },
             },
             response_class=self.response_class,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=create_async_endpoint(self.client.conformance, EmptyRequest),
```

### Comparing `stac_fastapi_api-3.0.0a0/stac_fastapi/api/config.py` & `stac_fastapi_api-3.0.0a1/stac_fastapi/api/config.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-3.0.0a0/stac_fastapi/api/errors.py` & `stac_fastapi_api-3.0.0a1/stac_fastapi/api/errors.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-3.0.0a0/stac_fastapi/api/middleware.py` & `stac_fastapi_api-3.0.0a1/stac_fastapi/api/middleware.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-3.0.0a0/stac_fastapi/api/models.py` & `stac_fastapi_api-3.0.0a1/stac_fastapi/api/models.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-3.0.0a0/stac_fastapi/api/openapi.py` & `stac_fastapi_api-3.0.0a1/stac_fastapi/api/openapi.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-3.0.0a0/stac_fastapi/api/routes.py` & `stac_fastapi_api-3.0.0a1/stac_fastapi/api/routes.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-3.0.0a0/stac_fastapi.api.egg-info/PKG-INFO` & `stac_fastapi_api-3.0.0a1/stac_fastapi.api.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.api
-Version: 3.0.0a0
+Version: 3.0.0a1
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
@@ -23,14 +23,13 @@
 Provides-Extra: dev
 Requires-Dist: httpx; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: requests; extra == "dev"
-Requires-Dist: pystac[validation]==1.*; extra == "dev"
 Provides-Extra: benchmark
 Requires-Dist: pytest-benchmark; extra == "benchmark"
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: pdocs; extra == "docs"
```

### Comparing `stac_fastapi_api-3.0.0a0/stac_fastapi.api.egg-info/SOURCES.txt` & `stac_fastapi_api-3.0.0a1/stac_fastapi.api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-3.0.0a0/tests/test_api.py` & `stac_fastapi_api-3.0.0a1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-3.0.0a0/tests/test_app.py` & `stac_fastapi_api-3.0.0a1/tests/test_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,16 @@
     )
     test_app.app.openapi()
     components = ["LandingPage", "Collection", "Collections", "Item", "ItemCollection"]
     for component in components:
         assert component in test_app.app.openapi_schema["components"]["schemas"]
 
 
-def test_filter_extension(TestCoreClient, item_dict):
+@pytest.mark.parametrize("validate", [True, False])
+def test_filter_extension(validate, TestCoreClient, item_dict):
     """Test if Filter Parameters are passed correctly."""
 
     class FilterClient(TestCoreClient):
         def post_search(
             self, search_request: BaseSearchPostRequest, **kwargs
         ) -> stac.ItemCollection:
             search_request.collections = ["test"]
@@ -155,21 +156,23 @@
             return stac.ItemCollection(
                 type="FeatureCollection", features=[stac.Item(**item_dict)]
             )
 
     post_request_model = create_post_request_model([FilterExtension()])
 
     test_app = app.StacApi(
-        settings=ApiSettings(),
+        settings=ApiSettings(enable_response_models=validate),
         client=FilterClient(post_request_model=post_request_model),
         search_get_request_model=create_get_request_model([FilterExtension()]),
         search_post_request_model=post_request_model,
+        extensions=[FilterExtension()],
     )
 
     with TestClient(test_app.app) as client:
+        landing = client.get("/")
         get_search = client.get(
             "/search",
             params={
                 "filter": "TEST",
                 "filter-crs": "EPSG:4326",
                 "filter-lang": "cql2-text",
             },
@@ -180,9 +183,10 @@
                 "collections": ["test"],
                 "filter": {},
                 "filter-crs": "EPSG:4326",
                 "filter-lang": "cql2-text",
             },
         )
 
+    assert landing.status_code == 200, landing.text
     assert get_search.status_code == 200, get_search.text
     assert post_search.status_code == 200, post_search.text
```

### Comparing `stac_fastapi_api-3.0.0a0/tests/test_app_prefix.py` & `stac_fastapi_api-3.0.0a1/tests/test_app_prefix.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-3.0.0a0/tests/test_middleware.py` & `stac_fastapi_api-3.0.0a1/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-3.0.0a0/tests/test_models.py` & `stac_fastapi_api-3.0.0a1/tests/test_models.py`

 * *Files identical despite different names*

