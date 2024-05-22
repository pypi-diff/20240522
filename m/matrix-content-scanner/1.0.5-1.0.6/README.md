# Comparing `tmp/matrix_content_scanner-1.0.5.tar.gz` & `tmp/matrix_content_scanner-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matrix_content_scanner-1.0.5.tar", last modified: Wed Nov 29 14:13:07 2023, max compression
+gzip compressed data, was "matrix_content_scanner-1.0.6.tar", last modified: Wed May 22 11:53:11 2024, max compression
```

## Comparing `matrix_content_scanner-1.0.5.tar` & `matrix_content_scanner-1.0.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 dmr       (1000) dmr       (1000)        0 2023-11-29 14:13:07.685222 matrix_content_scanner-1.0.5/
--rw-r--r--   0 dmr       (1000) dmr       (1000)    10174 2023-11-24 12:47:37.000000 matrix_content_scanner-1.0.5/LICENSE
--rw-r--r--   0 dmr       (1000) dmr       (1000)     5245 2023-11-29 14:13:07.685222 matrix_content_scanner-1.0.5/PKG-INFO
--rw-r--r--   0 dmr       (1000) dmr       (1000)     4152 2023-11-24 12:47:37.000000 matrix_content_scanner-1.0.5/README.md
--rw-r--r--   0 dmr       (1000) dmr       (1000)      169 2023-11-24 15:34:50.000000 matrix_content_scanner-1.0.5/pyproject.toml
--rw-r--r--   0 dmr       (1000) dmr       (1000)      835 2023-11-29 14:13:07.685222 matrix_content_scanner-1.0.5/setup.cfg
-drwxr-xr-x   0 dmr       (1000) dmr       (1000)        0 2023-11-29 14:13:07.676222 matrix_content_scanner-1.0.5/src/
-drwxr-xr-x   0 dmr       (1000) dmr       (1000)        0 2023-11-29 14:13:07.681222 matrix_content_scanner-1.0.5/src/matrix_content_scanner/
--rw-r--r--   0 dmr       (1000) dmr       (1000)      588 2023-11-24 12:47:37.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner/__init__.py
--rw-r--r--   0 dmr       (1000) dmr       (1000)     5933 2023-11-24 12:47:37.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner/config.py
--rw-r--r--   0 dmr       (1000) dmr       (1000)     4321 2023-11-27 13:11:40.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner/crypto.py
--rw-r--r--   0 dmr       (1000) dmr       (1000)     4792 2023-11-27 13:11:40.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner/httpserver.py
--rw-r--r--   0 dmr       (1000) dmr       (1000)     1516 2023-11-27 13:11:40.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner/logutils.py
--rw-r--r--   0 dmr       (1000) dmr       (1000)     3573 2023-11-24 12:47:37.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner/mcs.py
--rw-r--r--   0 dmr       (1000) dmr       (1000)        0 2023-11-24 12:47:37.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner/py.typed
-drwxr-xr-x   0 dmr       (1000) dmr       (1000)        0 2023-11-29 14:13:07.682222 matrix_content_scanner-1.0.5/src/matrix_content_scanner/scanner/
--rw-r--r--   0 dmr       (1000) dmr       (1000)      588 2023-11-24 12:47:37.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner/scanner/__init__.py
--rw-r--r--   0 dmr       (1000) dmr       (1000)    13205 2023-11-27 13:11:40.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner/scanner/file_downloader.py
--rw-r--r--   0 dmr       (1000) dmr       (1000)    22032 2023-11-29 14:08:36.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner/scanner/scanner.py
-drwxr-xr-x   0 dmr       (1000) dmr       (1000)        0 2023-11-29 14:13:07.683222 matrix_content_scanner-1.0.5/src/matrix_content_scanner/servlets/
--rw-r--r--   0 dmr       (1000) dmr       (1000)     7636 2023-11-24 13:34:16.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner/servlets/__init__.py
--rw-r--r--   0 dmr       (1000) dmr       (1000)     2093 2023-11-24 12:47:37.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner/servlets/download.py
--rw-r--r--   0 dmr       (1000) dmr       (1000)     1234 2023-11-24 12:47:37.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner/servlets/public_key.py
--rw-r--r--   0 dmr       (1000) dmr       (1000)     2178 2023-11-24 12:47:37.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner/servlets/scan.py
--rw-r--r--   0 dmr       (1000) dmr       (1000)     1458 2023-11-24 12:47:37.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner/servlets/thumbnail.py
-drwxr-xr-x   0 dmr       (1000) dmr       (1000)        0 2023-11-29 14:13:07.683222 matrix_content_scanner-1.0.5/src/matrix_content_scanner/utils/
--rw-r--r--   0 dmr       (1000) dmr       (1000)      588 2023-11-24 12:47:37.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner/utils/__init__.py
--rw-r--r--   0 dmr       (1000) dmr       (1000)     1385 2023-11-27 13:11:40.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner/utils/constants.py
--rw-r--r--   0 dmr       (1000) dmr       (1000)     3726 2023-11-24 12:47:37.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner/utils/encrypted_file_metadata.py
--rw-r--r--   0 dmr       (1000) dmr       (1000)     1938 2023-11-24 12:47:37.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner/utils/errors.py
--rw-r--r--   0 dmr       (1000) dmr       (1000)      927 2023-11-24 12:47:37.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner/utils/types.py
-drwxr-xr-x   0 dmr       (1000) dmr       (1000)        0 2023-11-29 14:13:07.684222 matrix_content_scanner-1.0.5/src/matrix_content_scanner.egg-info/
--rw-r--r--   0 dmr       (1000) dmr       (1000)     5245 2023-11-29 14:13:07.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner.egg-info/PKG-INFO
--rw-r--r--   0 dmr       (1000) dmr       (1000)     1216 2023-11-29 14:13:07.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner.egg-info/SOURCES.txt
--rw-r--r--   0 dmr       (1000) dmr       (1000)        1 2023-11-29 14:13:07.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner.egg-info/dependency_links.txt
--rw-r--r--   0 dmr       (1000) dmr       (1000)      273 2023-11-29 14:13:07.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner.egg-info/requires.txt
--rw-r--r--   0 dmr       (1000) dmr       (1000)       23 2023-11-29 14:13:07.000000 matrix_content_scanner-1.0.5/src/matrix_content_scanner.egg-info/top_level.txt
-drwxr-xr-x   0 dmr       (1000) dmr       (1000)        0 2023-11-29 14:13:07.684222 matrix_content_scanner-1.0.5/tests/
--rw-r--r--   0 dmr       (1000) dmr       (1000)     1521 2023-11-24 12:47:37.000000 matrix_content_scanner-1.0.5/tests/test_crypto.py
--rw-r--r--   0 dmr       (1000) dmr       (1000)     5122 2023-11-24 16:23:39.000000 matrix_content_scanner-1.0.5/tests/testutils.py
+drwxrwxr-x   0 erikj     (1000) erikj     (1000)        0 2024-05-22 11:53:11.606777 matrix_content_scanner-1.0.6/
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)    10174 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/LICENSE
+-rw-r--r--   0 erikj     (1000) erikj     (1000)     5245 2024-05-22 11:53:11.606777 matrix_content_scanner-1.0.6/PKG-INFO
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)     4152 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/README.md
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)      169 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/pyproject.toml
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)      835 2024-05-22 11:53:11.606777 matrix_content_scanner-1.0.6/setup.cfg
+drwxrwxr-x   0 erikj     (1000) erikj     (1000)        0 2024-05-22 11:53:11.602777 matrix_content_scanner-1.0.6/src/
+drwxrwxr-x   0 erikj     (1000) erikj     (1000)        0 2024-05-22 11:53:11.606777 matrix_content_scanner-1.0.6/src/matrix_content_scanner/
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)      588 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner/__init__.py
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)     5933 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner/config.py
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)     4321 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner/crypto.py
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)     5701 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner/httpserver.py
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)     1516 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner/logutils.py
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)     3573 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner/mcs.py
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)        0 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner/py.typed
+drwxrwxr-x   0 erikj     (1000) erikj     (1000)        0 2024-05-22 11:53:11.606777 matrix_content_scanner-1.0.6/src/matrix_content_scanner/scanner/
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)      588 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner/scanner/__init__.py
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)    13205 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner/scanner/file_downloader.py
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)    22032 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner/scanner/scanner.py
+drwxrwxr-x   0 erikj     (1000) erikj     (1000)        0 2024-05-22 11:53:11.606777 matrix_content_scanner-1.0.6/src/matrix_content_scanner/servlets/
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)     7636 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner/servlets/__init__.py
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)     2093 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner/servlets/download.py
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)     1234 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner/servlets/public_key.py
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)     2178 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner/servlets/scan.py
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)     1458 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner/servlets/thumbnail.py
+drwxrwxr-x   0 erikj     (1000) erikj     (1000)        0 2024-05-22 11:53:11.606777 matrix_content_scanner-1.0.6/src/matrix_content_scanner/utils/
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)      588 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner/utils/__init__.py
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)     1385 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner/utils/constants.py
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)     3726 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner/utils/encrypted_file_metadata.py
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)     1938 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner/utils/errors.py
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)      927 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner/utils/types.py
+drwxrwxr-x   0 erikj     (1000) erikj     (1000)        0 2024-05-22 11:53:11.606777 matrix_content_scanner-1.0.6/src/matrix_content_scanner.egg-info/
+-rw-r--r--   0 erikj     (1000) erikj     (1000)     5245 2024-05-22 11:53:11.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner.egg-info/PKG-INFO
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)     1216 2024-05-22 11:53:11.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner.egg-info/SOURCES.txt
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)        1 2024-05-22 11:53:11.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner.egg-info/dependency_links.txt
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)      273 2024-05-22 11:53:11.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner.egg-info/requires.txt
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)       23 2024-05-22 11:53:11.000000 matrix_content_scanner-1.0.6/src/matrix_content_scanner.egg-info/top_level.txt
+drwxrwxr-x   0 erikj     (1000) erikj     (1000)        0 2024-05-22 11:53:11.606777 matrix_content_scanner-1.0.6/tests/
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)     1521 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/tests/test_crypto.py
+-rw-rw-r--   0 erikj     (1000) erikj     (1000)     5122 2024-05-22 11:48:45.000000 matrix_content_scanner-1.0.6/tests/testutils.py
```

### Comparing `matrix_content_scanner-1.0.5/LICENSE` & `matrix_content_scanner-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `matrix_content_scanner-1.0.5/PKG-INFO` & `matrix_content_scanner-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matrix_content_scanner
-Version: 1.0.5
+Version: 1.0.6
 Summary: A web service for scanning media hosted by a Matrix media repository
 Home-page: https://github.com/vector-im/matrix-content-scanner-python
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs
```

### Comparing `matrix_content_scanner-1.0.5/README.md` & `matrix_content_scanner-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `matrix_content_scanner-1.0.5/setup.cfg` & `matrix_content_scanner-1.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = matrix_content_scanner
 description = A web service for scanning media hosted by a Matrix media repository
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 1.0.5
+version = 1.0.6
 url = https://github.com/vector-im/matrix-content-scanner-python
 classifiers = 
 	License :: OSI Approved :: Apache Software License
 
 [options]
 package_dir = =src
 python_requires = >= 3.8
```

### Comparing `matrix_content_scanner-1.0.5/src/matrix_content_scanner/__init__.py` & `matrix_content_scanner-1.0.6/src/matrix_content_scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_content_scanner-1.0.5/src/matrix_content_scanner/config.py` & `matrix_content_scanner-1.0.6/src/matrix_content_scanner/config.py`

 * *Files identical despite different names*

### Comparing `matrix_content_scanner-1.0.5/src/matrix_content_scanner/crypto.py` & `matrix_content_scanner-1.0.6/src/matrix_content_scanner/crypto.py`

 * *Files identical despite different names*

### Comparing `matrix_content_scanner-1.0.5/src/matrix_content_scanner/httpserver.py` & `matrix_content_scanner-1.0.6/src/matrix_content_scanner/httpserver.py`

 * *Files 13% similar despite different names*

```diff
@@ -63,14 +63,39 @@
 
     # Run the request's handler and append CORS headers to it.
     response = await handler(request)
     response.headers.update(_CORS_HEADERS)
     return response
 
 
+@web.middleware
+async def json_errors_middleware(
+    request: web.Request,
+    handler: Callable[[web.Request], Awaitable[web.StreamResponse]],
+) -> web.StreamResponse:
+    """A simple aiohttp middleware that converts 404/405 errors into Matrix JSON error.
+
+    Args:
+        request: The request to handle.
+        handler: The handler for this request.
+
+    Returns:
+        The original response OR a JSON error response.
+    """
+    # Run the request's handler and append CORS headers to it.
+    try:
+        return await handler(request)
+    except (web.HTTPNotFound, web.HTTPMethodNotAllowed) as ex:
+        # Return the proper JSON response.
+        return web.json_response(
+            {"errcode": "M_UNRECOGNIZED", "error": "Unrecognized request"},
+            status=ex.status,
+        )
+
+
 class HTTPServer:
     def __init__(self, mcs: "MatrixContentScanner"):
         self._mcs = mcs
         self._bind_address = mcs.config.web.host
         self._bind_port = mcs.config.web.port
 
         self._app = self._build_app()
@@ -113,14 +138,16 @@
         root = web.Application(
             # Apply middlewares. This will also apply to subapps.
             middlewares=[
                 # Handle trailing slashes.
                 web.normalize_path_middleware(),
                 # Handler CORS.
                 simple_cors_middleware,
+                # Convert unknown routes/methods into JSON errors.
+                json_errors_middleware,
             ],
         )
         root.add_subapp("/_matrix/media_proxy/unstable", app)
 
         return root
 
     def start(self) -> None:
```

### Comparing `matrix_content_scanner-1.0.5/src/matrix_content_scanner/logutils.py` & `matrix_content_scanner-1.0.6/src/matrix_content_scanner/logutils.py`

 * *Files identical despite different names*

### Comparing `matrix_content_scanner-1.0.5/src/matrix_content_scanner/mcs.py` & `matrix_content_scanner-1.0.6/src/matrix_content_scanner/mcs.py`

 * *Files identical despite different names*

### Comparing `matrix_content_scanner-1.0.5/src/matrix_content_scanner/scanner/__init__.py` & `matrix_content_scanner-1.0.6/src/matrix_content_scanner/scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_content_scanner-1.0.5/src/matrix_content_scanner/scanner/file_downloader.py` & `matrix_content_scanner-1.0.6/src/matrix_content_scanner/scanner/file_downloader.py`

 * *Files identical despite different names*

### Comparing `matrix_content_scanner-1.0.5/src/matrix_content_scanner/scanner/scanner.py` & `matrix_content_scanner-1.0.6/src/matrix_content_scanner/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `matrix_content_scanner-1.0.5/src/matrix_content_scanner/servlets/__init__.py` & `matrix_content_scanner-1.0.6/src/matrix_content_scanner/servlets/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_content_scanner-1.0.5/src/matrix_content_scanner/servlets/download.py` & `matrix_content_scanner-1.0.6/src/matrix_content_scanner/servlets/download.py`

 * *Files identical despite different names*

### Comparing `matrix_content_scanner-1.0.5/src/matrix_content_scanner/servlets/public_key.py` & `matrix_content_scanner-1.0.6/src/matrix_content_scanner/servlets/public_key.py`

 * *Files identical despite different names*

### Comparing `matrix_content_scanner-1.0.5/src/matrix_content_scanner/servlets/scan.py` & `matrix_content_scanner-1.0.6/src/matrix_content_scanner/servlets/scan.py`

 * *Files identical despite different names*

### Comparing `matrix_content_scanner-1.0.5/src/matrix_content_scanner/servlets/thumbnail.py` & `matrix_content_scanner-1.0.6/src/matrix_content_scanner/servlets/thumbnail.py`

 * *Files identical despite different names*

### Comparing `matrix_content_scanner-1.0.5/src/matrix_content_scanner/utils/__init__.py` & `matrix_content_scanner-1.0.6/src/matrix_content_scanner/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_content_scanner-1.0.5/src/matrix_content_scanner/utils/constants.py` & `matrix_content_scanner-1.0.6/src/matrix_content_scanner/utils/constants.py`

 * *Files identical despite different names*

### Comparing `matrix_content_scanner-1.0.5/src/matrix_content_scanner/utils/encrypted_file_metadata.py` & `matrix_content_scanner-1.0.6/src/matrix_content_scanner/utils/encrypted_file_metadata.py`

 * *Files identical despite different names*

### Comparing `matrix_content_scanner-1.0.5/src/matrix_content_scanner/utils/errors.py` & `matrix_content_scanner-1.0.6/src/matrix_content_scanner/utils/errors.py`

 * *Files identical despite different names*

### Comparing `matrix_content_scanner-1.0.5/src/matrix_content_scanner/utils/types.py` & `matrix_content_scanner-1.0.6/src/matrix_content_scanner/utils/types.py`

 * *Files identical despite different names*

### Comparing `matrix_content_scanner-1.0.5/src/matrix_content_scanner.egg-info/PKG-INFO` & `matrix_content_scanner-1.0.6/src/matrix_content_scanner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: matrix-content-scanner
-Version: 1.0.5
+Name: matrix_content_scanner
+Version: 1.0.6
 Summary: A web service for scanning media hosted by a Matrix media repository
 Home-page: https://github.com/vector-im/matrix-content-scanner-python
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs
```

### Comparing `matrix_content_scanner-1.0.5/src/matrix_content_scanner.egg-info/SOURCES.txt` & `matrix_content_scanner-1.0.6/src/matrix_content_scanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `matrix_content_scanner-1.0.5/tests/test_crypto.py` & `matrix_content_scanner-1.0.6/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `matrix_content_scanner-1.0.5/tests/testutils.py` & `matrix_content_scanner-1.0.6/tests/testutils.py`

 * *Files identical despite different names*

