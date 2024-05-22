# Comparing `tmp/fleekapi-0.2.5.tar.gz` & `tmp/fleekapi-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleekapi-0.2.5.tar", last modified: Mon May 20 22:07:26 2024, max compression
+gzip compressed data, was "fleekapi-0.2.6.tar", last modified: Wed May 22 08:19:10 2024, max compression
```

## Comparing `fleekapi-0.2.5.tar` & `fleekapi-0.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 22:07:26.276750 fleekapi-0.2.5/
--rw-r--r--   0 hasan     (1002) hasan     (1002)     2383 2024-05-20 22:07:26.276750 fleekapi-0.2.5/PKG-INFO
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 22:07:26.272750 fleekapi-0.2.5/fleekapi/
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       18 2024-05-20 22:07:21.000000 fleekapi-0.2.5/fleekapi/__init__.py
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 22:07:26.276750 fleekapi-0.2.5/fleekapi/src/
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       68 2024-05-20 21:58:20.000000 fleekapi-0.2.5/fleekapi/src/__init__.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     3803 2024-05-20 20:51:08.000000 fleekapi-0.2.5/fleekapi/src/app.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      674 2024-05-19 13:15:32.000000 fleekapi-0.2.5/fleekapi/src/middleware.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      972 2024-05-19 13:15:32.000000 fleekapi-0.2.5/fleekapi/src/response.py
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 22:07:26.276750 fleekapi-0.2.5/fleekapi.egg-info/
--rw-r--r--   0 hasan     (1002) hasan     (1002)     2383 2024-05-20 22:07:26.000000 fleekapi-0.2.5/fleekapi.egg-info/PKG-INFO
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      285 2024-05-20 22:07:26.000000 fleekapi-0.2.5/fleekapi.egg-info/SOURCES.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-20 22:07:26.000000 fleekapi-0.2.5/fleekapi.egg-info/dependency_links.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      138 2024-05-20 22:07:26.000000 fleekapi-0.2.5/fleekapi.egg-info/requires.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        9 2024-05-20 22:07:26.000000 fleekapi-0.2.5/fleekapi.egg-info/top_level.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-20 22:07:26.276750 fleekapi-0.2.5/setup.cfg
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     4013 2024-05-20 22:07:21.000000 fleekapi-0.2.5/setup.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-22 08:19:10.407117 fleekapi-0.2.6/
+-rw-r--r--   0 hasan     (1002) hasan     (1002)     2414 2024-05-22 08:19:10.403118 fleekapi-0.2.6/PKG-INFO
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-22 08:19:10.395117 fleekapi-0.2.6/fleekapi/
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-22 08:15:47.000000 fleekapi-0.2.6/fleekapi/__init__.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-22 08:19:10.403118 fleekapi-0.2.6/fleekapi/src/
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       69 2024-05-22 08:15:47.000000 fleekapi-0.2.6/fleekapi/src/__init__.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     3755 2024-05-22 08:15:47.000000 fleekapi-0.2.6/fleekapi/src/app.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      630 2024-05-22 08:15:47.000000 fleekapi-0.2.6/fleekapi/src/middleware.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      964 2024-05-22 08:15:47.000000 fleekapi-0.2.6/fleekapi/src/response.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-22 08:19:10.403118 fleekapi-0.2.6/fleekapi.egg-info/
+-rw-r--r--   0 hasan     (1002) hasan     (1002)     2414 2024-05-22 08:19:10.000000 fleekapi-0.2.6/fleekapi.egg-info/PKG-INFO
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      285 2024-05-22 08:19:10.000000 fleekapi-0.2.6/fleekapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-22 08:19:10.000000 fleekapi-0.2.6/fleekapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      154 2024-05-22 08:19:10.000000 fleekapi-0.2.6/fleekapi.egg-info/requires.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        9 2024-05-22 08:19:10.000000 fleekapi-0.2.6/fleekapi.egg-info/top_level.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-22 08:19:10.407117 fleekapi-0.2.6/setup.cfg
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     4036 2024-05-22 08:19:08.000000 fleekapi-0.2.6/setup.py
```

### Comparing `fleekapi-0.2.5/PKG-INFO` & `fleekapi-0.2.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: fleekapi
-Version: 0.2.5
+Version: 0.2.6
 Summary: My short description for my project.
-Home-page: https://github.com/under-script/FleekAPI
+Home-page: https://github.com/under-script/fleekapi
 Author: Yunusov Abdulmajid
 Author-email: abdulmajidyunusov18@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -18,14 +18,15 @@
 Requires-Dist: Jinja2==3.1.4
 Requires-Dist: parse==1.20.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests-wsgi-adapter==0.4.1
 Requires-Dist: WebOb==1.8.7
 Requires-Dist: whitenoise==6.6.0
 Requires-Dist: icecream==2.1.3
+Requires-Dist: Werkzeug==3.0.3
 
 
 # FleekAPI
 
 FleekAPI is a lightweight [WSGI][] web application framework. It is designed
 to make getting started quick and easy, with the ability to scale up to
 complex applications. It began as a simple wrapper around [Jinja][], and will become one of the most popular Python web
@@ -33,25 +34,26 @@
 
 FleekAPI offers suggestions, but doesn't enforce any dependencies or
 project layout. It is up to the developer to choose the tools and
 libraries they want to use. There are many extensions provided by the
 community that make adding new functionality easy.
 
 [WSGI]: https://wsgi.readthedocs.io/
-[Jinja]: https://jinja.palletsprojects.com/
 
+[Jinja]: https://jinja.palletsprojects.com/
 
 ## A Simple Example
 
 ```python
 # save this as app.py
 from fleekapi import FleekAPI
 
 app = FleekAPI()
 
+
 @app.route("/")
 def hello(req, resp):
     resp.text = "Hello, World!"
 ```
 
 ```
 $ gunicorn app:app
@@ -59,15 +61,14 @@
   [2024-05-21 01:34:43 +0500] [78175] [INFO] Listening at: http://127.0.0.1:8000 (78175)
   [2024-05-21 01:34:43 +0500] [78175] [INFO] Using worker: sync
   [2024-05-21 01:34:43 +0500] [78176] [INFO] Booting worker with pid: 7817
     
   * Running on http://127.0.0.1:8000/ (Press CTRL+C to quit)
 ```
 
-
 ## Donate
 
 The Avengers organization develops and supports FleekAPI. In order to grow the community of contributors and users, and
 allow the maintainers to devote more time to the projects, [please
 donate today][].
 
 [please donate today]: https://t.me/toEpamMiddle
```

### Comparing `fleekapi-0.2.5/fleekapi/src/app.py` & `fleekapi-0.2.6/fleekapi/src/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,27 @@
 from webob import Request
 from whitenoise import WhiteNoise
 
 from .middleware import Middleware
 from .response import Response
 
 
+def default_response(resp):
+    resp.status_code = 404
+    resp.text = "Page not found"
+
+    return resp
+
+
+def method_not_allowed(resp):
+    resp.status_code = 405
+    resp.text = "Method is not allowed"
+    return resp
+
+
 class FleekAPI:
     def __init__(self):
         self.routes = dict()
 
         self.template_env = Environment(
             loader=FileSystemLoader(os.path.abspath("templates"))
         )
@@ -30,70 +43,59 @@
 
         if path_info.startswith("/static"):
             return self.whitenoise(environ, start_response)
 
         return self.middleware(environ, start_response)
 
     def wsgi_app(self, environ, start_response):
-        request = Request(environ)
-        response = self.handle_request(request)
-        return response(environ, start_response)
-
-    def handle_request(self, request):
-        response = Response()
-        handler_data, kwargs = self.find_handler(request)
+        req = Request(environ)
+        resp = self.handle_request(req)
+        return resp(environ, start_response)
+
+    def handle_request(self, req):
+        resp = Response()
+        handler_data, kwargs = self.find_handler(req)
 
         if handler_data is not None:
             handler = handler_data["handler"]
             allowed_methods = handler_data["allowed_methods"]
 
             if inspect.isclass(handler):
-                handler = getattr(handler(), request.method.lower(), None)
+                handler = getattr(handler(), req.method.lower(), None)
 
                 if handler is None:
-                    return self.method_not_allowed(response)
+                    return method_not_allowed(resp)
             else:
-                if request.method.lower() not in allowed_methods:
-                    return self.method_not_allowed(response)
+                if req.method.lower() not in allowed_methods:
+                    return method_not_allowed(resp)
 
             try:
-                handler(request, response, **kwargs)
+                handler(req, resp, **kwargs)
             except Exception as e:
                 if self.exception_handler is not None:
-                    self.exception_handler(request, response, e)
+                    self.exception_handler(req, resp, e)
                 else:
                     raise e
         else:
-            self.default_response(response)
-        return response
-
-    def method_not_allowed(self, response):
-        response.status_code = 405
-        response.text = "Method is not allowed"
-        return response
+            default_response(resp)
+        return resp
 
-    def find_handler(self, request):
+    def find_handler(self, req):
         for path, handler_data in self.routes.items():
-            parsed_result = parse(path, request.path)
+            parsed_result = parse(path, req.path)
 
             if parsed_result is not None:
                 return handler_data, parsed_result.named
         return None, None
 
-    def default_response(self, response):
-        response.status_code = 404
-        response.text = "Page not found"
-
-        return response
-
     def add_route(self, path, handler, allowed_methods=None):
         assert path not in self.routes, "Duplicate route. Please change the URL."
 
         if allowed_methods is None:
-            allowed_methods = ["get", "post", "put", "delete", "head", "options", "patch", "connect", "trace"]
+            allowed_methods = ["get"]
 
         self.routes[path] = {
             "handler": handler,
             "allowed_methods": allowed_methods,
         }
 
     def route(self, path, allowed_methods=None):
@@ -114,8 +116,17 @@
         template = self.template_env.get_template(template_name).render(**context)
         return template
 
     def add_exception_handler(self, exception_handler):
         self.exception_handler = exception_handler
 
     def add_middleware(self, middleware_cls):
-        self.middleware.add(middleware_cls)
+        self.middleware.add(middleware_cls)
+
+    def include_router(self, router):
+        self.routes.update(**router.routes)
+
+
+class Router(FleekAPI):
+    def __init__(self):
+        super().__init__()
+        self.routes = dict()
```

### Comparing `fleekapi-0.2.5/fleekapi/src/middleware.py` & `fleekapi-0.2.6/fleekapi/src/middleware.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
     def process_request(self, req):
         pass
 
     def process_response(self, req, resp):
         pass
 
-    def handle_request(self, request):
-        self.process_request(request)
-        response = self.app.handle_request(request)
-        self.process_response(request, response)
-        return response
+    def handle_request(self, req):
+        self.process_request(req)
+        resp = self.app.handle_request(req)
+        self.process_response(req, resp)
+        return resp
 
     def __call__(self, environ, start_response):
-        request = Request(environ)
-        response = self.app.handle_request(request)
-        return response(environ, start_response)
+        req = Request(environ)
+        resp = self.app.handle_request(req)
+        return resp(environ, start_response)
```

### Comparing `fleekapi-0.2.5/fleekapi/src/response.py` & `fleekapi-0.2.6/fleekapi/src/response.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,13 +22,13 @@
         elif self.text is not None:
             self.body = self.text
             self.content_type = "text/plain"
 
     def __call__(self, environ, start_response):
         self.set_body_and_content_type()
 
-        response = WebResponse(
+        resp = WebResponse(
             body=self.body,
             content_type=self.content_type,
             status=self.status_code,
         )
-        return response(environ, start_response)
+        return resp(environ, start_response)
```

### Comparing `fleekapi-0.2.5/fleekapi.egg-info/PKG-INFO` & `fleekapi-0.2.6/fleekapi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: fleekapi
-Version: 0.2.5
+Version: 0.2.6
 Summary: My short description for my project.
-Home-page: https://github.com/under-script/FleekAPI
+Home-page: https://github.com/under-script/fleekapi
 Author: Yunusov Abdulmajid
 Author-email: abdulmajidyunusov18@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -18,14 +18,15 @@
 Requires-Dist: Jinja2==3.1.4
 Requires-Dist: parse==1.20.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests-wsgi-adapter==0.4.1
 Requires-Dist: WebOb==1.8.7
 Requires-Dist: whitenoise==6.6.0
 Requires-Dist: icecream==2.1.3
+Requires-Dist: Werkzeug==3.0.3
 
 
 # FleekAPI
 
 FleekAPI is a lightweight [WSGI][] web application framework. It is designed
 to make getting started quick and easy, with the ability to scale up to
 complex applications. It began as a simple wrapper around [Jinja][], and will become one of the most popular Python web
@@ -33,25 +34,26 @@
 
 FleekAPI offers suggestions, but doesn't enforce any dependencies or
 project layout. It is up to the developer to choose the tools and
 libraries they want to use. There are many extensions provided by the
 community that make adding new functionality easy.
 
 [WSGI]: https://wsgi.readthedocs.io/
-[Jinja]: https://jinja.palletsprojects.com/
 
+[Jinja]: https://jinja.palletsprojects.com/
 
 ## A Simple Example
 
 ```python
 # save this as app.py
 from fleekapi import FleekAPI
 
 app = FleekAPI()
 
+
 @app.route("/")
 def hello(req, resp):
     resp.text = "Hello, World!"
 ```
 
 ```
 $ gunicorn app:app
@@ -59,15 +61,14 @@
   [2024-05-21 01:34:43 +0500] [78175] [INFO] Listening at: http://127.0.0.1:8000 (78175)
   [2024-05-21 01:34:43 +0500] [78175] [INFO] Using worker: sync
   [2024-05-21 01:34:43 +0500] [78176] [INFO] Booting worker with pid: 7817
     
   * Running on http://127.0.0.1:8000/ (Press CTRL+C to quit)
 ```
 
-
 ## Donate
 
 The Avengers organization develops and supports FleekAPI. In order to grow the community of contributors and users, and
 allow the maintainers to devote more time to the projects, [please
 donate today][].
 
 [please donate today]: https://t.me/toEpamMiddle
```

### Comparing `fleekapi-0.2.5/setup.py` & `fleekapi-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,31 +10,32 @@
 from shutil import rmtree
 
 from setuptools import find_packages, setup, Command
 
 # Package meta-data.
 NAME = 'fleekapi'
 DESCRIPTION = 'My short description for my project.'
-URL = 'https://github.com/under-script/FleekAPI'
+URL = 'https://github.com/under-script/fleekapi'
 EMAIL = 'abdulmajidyunusov18@gmail.com'
 AUTHOR = 'Yunusov Abdulmajid'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.2.05'
+VERSION = '0.2.06'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
     "gunicorn==22.0.0",
     "Jinja2==3.1.4",
     "parse==1.20.1",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
     "WebOb==1.8.7",
     "whitenoise==6.6.0",
     "icecream==2.1.3",
+    "Werkzeug==3.0.3",
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

