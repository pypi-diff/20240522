# Comparing `tmp/server_templates-0.3.1.tar.gz` & `tmp/server_templates-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "server_templates-0.3.1.tar", last modified: Tue May 21 10:31:33 2024, max compression
+gzip compressed data, was "server_templates-0.3.2.tar", last modified: Tue May 21 15:00:33 2024, max compression
```

## Comparing `server_templates-0.3.1.tar` & `server_templates-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 10:31:33.529430 server_templates-0.3.1/
--rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 server_templates-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     1970 2024-05-21 10:31:33.528431 server_templates-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1115 2024-05-21 10:31:13.000000 server_templates-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 10:31:33.518472 server_templates-0.3.1/server_templates/
--rw-rw-rw-   0        0        0      241 2024-04-24 11:47:38.000000 server_templates-0.3.1/server_templates/__init__.py
--rw-rw-rw-   0        0        0     7122 2024-05-21 10:31:13.000000 server_templates-0.3.1/server_templates/client_requests.py
-drwxrwxrwx   0        0        0        0 2024-05-21 10:31:33.523469 server_templates-0.3.1/server_templates/server_aiohttp/
--rw-rw-rw-   0        0        0       19 2024-01-29 15:35:36.000000 server_templates-0.3.1/server_templates/server_aiohttp/__init__.py
--rw-rw-rw-   0        0        0    10646 2024-04-25 06:41:35.000000 server_templates-0.3.1/server_templates/server_aiohttp/main.py
-drwxrwxrwx   0        0        0        0 2024-05-21 10:31:33.526024 server_templates-0.3.1/server_templates/server_fastapi/
--rw-rw-rw-   0        0        0       19 2024-01-29 15:35:36.000000 server_templates-0.3.1/server_templates/server_fastapi/__init__.py
--rw-rw-rw-   0        0        0    23007 2024-05-14 12:59:21.000000 server_templates-0.3.1/server_templates/server_fastapi/main.py
--rw-rw-rw-   0        0        0     1353 2024-05-14 13:08:49.000000 server_templates-0.3.1/server_templates/url.py
-drwxrwxrwx   0        0        0        0 2024-05-21 10:31:33.528431 server_templates-0.3.1/server_templates.egg-info/
--rw-rw-rw-   0        0        0     1970 2024-05-21 10:31:33.000000 server_templates-0.3.1/server_templates.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2024-05-21 10:31:33.000000 server_templates-0.3.1/server_templates.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 10:31:33.000000 server_templates-0.3.1/server_templates.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-21 10:31:33.000000 server_templates-0.3.1/server_templates.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 10:31:33.530418 server_templates-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2092 2024-01-30 06:52:17.000000 server_templates-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:00:33.218770 server_templates-0.3.2/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 server_templates-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     1970 2024-05-21 15:00:33.217186 server_templates-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1115 2024-05-21 14:59:39.000000 server_templates-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 15:00:33.091547 server_templates-0.3.2/server_templates/
+-rw-rw-rw-   0        0        0      241 2024-04-24 11:47:38.000000 server_templates-0.3.2/server_templates/__init__.py
+-rw-rw-rw-   0        0        0     7320 2024-05-21 14:59:38.000000 server_templates-0.3.2/server_templates/client_requests.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:00:33.137850 server_templates-0.3.2/server_templates/server_aiohttp/
+-rw-rw-rw-   0        0        0       19 2024-01-29 15:35:36.000000 server_templates-0.3.2/server_templates/server_aiohttp/__init__.py
+-rw-rw-rw-   0        0        0    10646 2024-04-25 06:41:35.000000 server_templates-0.3.2/server_templates/server_aiohttp/main.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:00:33.154901 server_templates-0.3.2/server_templates/server_fastapi/
+-rw-rw-rw-   0        0        0       19 2024-01-29 15:35:36.000000 server_templates-0.3.2/server_templates/server_fastapi/__init__.py
+-rw-rw-rw-   0        0        0    23007 2024-05-14 12:59:21.000000 server_templates-0.3.2/server_templates/server_fastapi/main.py
+-rw-rw-rw-   0        0        0     1353 2024-05-14 13:08:49.000000 server_templates-0.3.2/server_templates/url.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:00:33.216116 server_templates-0.3.2/server_templates.egg-info/
+-rw-rw-rw-   0        0        0     1970 2024-05-21 15:00:32.000000 server_templates-0.3.2/server_templates.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2024-05-21 15:00:33.000000 server_templates-0.3.2/server_templates.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 15:00:32.000000 server_templates-0.3.2/server_templates.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-21 15:00:32.000000 server_templates-0.3.2/server_templates.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 15:00:33.220714 server_templates-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     2092 2024-01-30 06:52:17.000000 server_templates-0.3.2/setup.py
```

### Comparing `server_templates-0.3.1/LICENSE` & `server_templates-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `server_templates-0.3.1/PKG-INFO` & `server_templates-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: server_templates
-Version: 0.3.1
+Version: 0.3.2
 Summary: templates for servers
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/server_templates
 Keywords: api,api server,http server,aiohttp,FastApi
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# server_templates (v0.3.1)
+# server_templates (v0.3.2)
 
 ## DESCRIPTION_SHORT
 templates for servers
 
 ## DESCRIPTION_LONG
 designed for keep all servers templates in one place
```

### Comparing `server_templates-0.3.1/README.md` & `server_templates-0.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# server_templates (v0.3.1)
+# server_templates (v0.3.2)
 
 ## DESCRIPTION_SHORT
 templates for servers
 
 ## DESCRIPTION_LONG
 designed for keep all servers templates in one place
```

### Comparing `server_templates-0.3.1/server_templates/client_requests.py` & `server_templates-0.3.2/server_templates/client_requests.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     # SETTINGS -------------------------------------
     START_ON_INIT: bool = None      # DONT DELETE!!! useful for delayed/pending requests
     TIMEOUT_SEND: float = 1
 
     RETRY_LIMIT: int | None = 1
     RETRY_TIMEOUT: float = 0.5
     retry_index: int = 0
+    SUCCESS_IF_FAIL_CODE: bool | None = None    # need to separate timedout and fail statuscode
 
     METHOD: ResponseMethod = ResponseMethod.POST
 
     # INIT ------------------------------------------
     BODY: Optional[Type__RequestBody]
     # REQUEST: Optional[requests.Request]
     RESPONSE: Optional[requests.Response]
@@ -95,15 +96,17 @@
             self.__class__.INDEX = 0
         else:
             self.__class__.INDEX += 1
 
         self.INDEX = self.__class__.INDEX
 
     def check_success(self) -> bool:
-        result = self.RESPONSE is not None and self.RESPONSE.ok
+        result = self.RESPONSE is not None
+        if not self.SUCCESS_IF_FAIL_CODE:
+            result &= self.RESPONSE.ok
         # self.LOGGER.debug(result)
         return result
 
     def __str__(self) -> str:
         return f"[{self.INDEX=}/len={self.__class__.INDEX+1}/{self.retry_index=}/{self.check_success()=}]{self.EXX=}/{self.RESPONSE=}"
 
     def __repr__(self) -> str:
@@ -120,23 +123,24 @@
             super().start(*args)
 
     def run(self) -> None:
         self.LOGGER.debug("run")
         while True:
             self._send()
 
-            # CHECK EXIT -------------------------------
+            # CHECK EXIT ----------------------------------------------
             if self.check_success():
                 return
 
+            # retry LIMIT ---------------------
             if self.RETRY_LIMIT and self.retry_index == self.RETRY_LIMIT - 1:
                 return
-            else:
-                time.sleep(self.RETRY_TIMEOUT)
-                self.retry_index += 1
+
+            self.retry_index += 1
+            time.sleep(self.RETRY_TIMEOUT)
 
     def _send(self) -> None:
         self.TIMESTAMP = time.time()
         self.RESPONSE = None
         self.EXX = None
 
         url = self.URL_create()
```

### Comparing `server_templates-0.3.1/server_templates/server_aiohttp/main.py` & `server_templates-0.3.2/server_templates/server_aiohttp/main.py`

 * *Files identical despite different names*

### Comparing `server_templates-0.3.1/server_templates/server_fastapi/main.py` & `server_templates-0.3.2/server_templates/server_fastapi/main.py`

 * *Files identical despite different names*

### Comparing `server_templates-0.3.1/server_templates/url.py` & `server_templates-0.3.2/server_templates/url.py`

 * *Files identical despite different names*

### Comparing `server_templates-0.3.1/server_templates.egg-info/PKG-INFO` & `server_templates-0.3.2/server_templates.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: server_templates
-Version: 0.3.1
+Version: 0.3.2
 Summary: templates for servers
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/server_templates
 Keywords: api,api server,http server,aiohttp,FastApi
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# server_templates (v0.3.1)
+# server_templates (v0.3.2)
 
 ## DESCRIPTION_SHORT
 templates for servers
 
 ## DESCRIPTION_LONG
 designed for keep all servers templates in one place
```

### Comparing `server_templates-0.3.1/setup.py` & `server_templates-0.3.2/setup.py`

 * *Files identical despite different names*

