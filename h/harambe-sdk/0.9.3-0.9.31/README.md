# Comparing `tmp/harambe_sdk-0.9.3.tar.gz` & `tmp/harambe_sdk-0.9.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harambe_sdk-0.9.3.tar", max compression
+gzip compressed data, was "harambe_sdk-0.9.31.tar", max compression
```

## Comparing `harambe_sdk-0.9.3.tar` & `harambe_sdk-0.9.31.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     5141 2024-04-17 19:55:31.649222 harambe_sdk-0.9.3/README.md
--rw-r--r--   0        0        0      278 2024-04-17 19:55:31.649222 harambe_sdk-0.9.3/harambe/__init__.py
--rw-r--r--   0        0        0    12846 2024-04-17 19:55:31.649222 harambe_sdk-0.9.3/harambe/core.py
--rw-r--r--   0        0        0     2397 2024-04-17 19:55:31.649222 harambe_sdk-0.9.3/harambe/handlers.py
--rw-r--r--   0        0        0     1747 2024-04-17 19:55:31.649222 harambe_sdk-0.9.3/harambe/harness.py
--rw-r--r--   0        0        0     3038 2024-04-17 19:55:31.649222 harambe_sdk-0.9.3/harambe/meta.py
--rw-r--r--   0        0        0     2457 2024-04-17 19:55:31.649222 harambe_sdk-0.9.3/harambe/normalize_url.py
--rw-r--r--   0        0        0     5014 2024-04-17 19:55:31.653221 harambe_sdk-0.9.3/harambe/observer.py
--rw-r--r--   0        0        0     2269 2024-04-17 19:55:31.653221 harambe_sdk-0.9.3/harambe/parser/parser.py
--rw-r--r--   0        0        0        0 2024-04-17 19:55:31.653221 harambe_sdk-0.9.3/harambe/py.typed
--rw-r--r--   0        0        0     3907 2024-04-17 19:55:31.653221 harambe_sdk-0.9.3/harambe/tracker.py
--rw-r--r--   0        0        0      256 2024-04-17 19:55:31.653221 harambe_sdk-0.9.3/harambe/types.py
--rw-r--r--   0        0        0     3049 2024-04-17 19:55:31.653221 harambe_sdk-0.9.3/harambe/utils.py
--rw-r--r--   0        0        0     1189 2024-04-17 19:55:31.653221 harambe_sdk-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     5827 1970-01-01 00:00:00.000000 harambe_sdk-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     5141 2024-04-19 18:27:09.149939 harambe_sdk-0.9.31/README.md
+-rw-r--r--   0        0        0      278 2024-03-17 22:34:41.210967 harambe_sdk-0.9.31/harambe/__init__.py
+-rw-r--r--   0        0        0    12965 2024-04-19 18:27:11.183917 harambe_sdk-0.9.31/harambe/core.py
+-rw-r--r--   0        0        0     2397 2024-03-01 06:20:44.777193 harambe_sdk-0.9.31/harambe/handlers.py
+-rw-r--r--   0        0        0     1747 2024-04-19 18:27:09.150654 harambe_sdk-0.9.31/harambe/harness.py
+-rw-r--r--   0        0        0     3038 2024-03-01 05:38:05.074579 harambe_sdk-0.9.31/harambe/meta.py
+-rw-r--r--   0        0        0     2457 2024-03-17 23:05:42.149184 harambe_sdk-0.9.31/harambe/normalize_url.py
+-rw-r--r--   0        0        0     5014 2024-04-19 18:27:09.150952 harambe_sdk-0.9.31/harambe/observer.py
+-rw-r--r--   0        0        0     2269 2024-04-19 18:27:09.151432 harambe_sdk-0.9.31/harambe/parser/parser.py
+-rw-r--r--   0        0        0        0 2023-11-16 20:05:34.307080 harambe_sdk-0.9.31/harambe/py.typed
+-rw-r--r--   0        0        0     7067 2024-04-19 18:27:11.184055 harambe_sdk-0.9.31/harambe/test.py
+-rw-r--r--   0        0        0     3907 2024-03-01 05:38:05.074901 harambe_sdk-0.9.31/harambe/tracker.py
+-rw-r--r--   0        0        0      256 2024-03-01 05:38:05.075229 harambe_sdk-0.9.31/harambe/types.py
+-rw-r--r--   0        0        0     3049 2024-03-01 05:43:34.226033 harambe_sdk-0.9.31/harambe/utils.py
+-rw-r--r--   0        0        0     1190 2024-04-19 18:27:24.817124 harambe_sdk-0.9.31/pyproject.toml
+-rw-r--r--   0        0        0     5828 1970-01-01 00:00:00.000000 harambe_sdk-0.9.31/PKG-INFO
```

### Comparing `harambe_sdk-0.9.3/README.md` & `harambe_sdk-0.9.31/README.md`

 * *Files identical despite different names*

### Comparing `harambe_sdk-0.9.3/harambe/core.py` & `harambe_sdk-0.9.31/harambe/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         # Create a temporary file to save the download
         with tempfile.NamedTemporaryFile() as temp_file:
             await download.save_as(temp_file.name)
             with open(temp_file.name, "rb") as f:
                 content = f.read()
 
         res = await self._notify_observers(
-            "on_download", download.url, download.suggested_filename, content
+            "on_download", download.url, download.suggested_filename, content, check_duplication=False
         )
         return res[0]
 
     async def capture_pdf(
         self,
     ) -> DownloadMeta:
         """
@@ -208,26 +208,29 @@
         file_name = PAGE_PDF_FILENAME
         res = await self._notify_observers(
             "on_download", self.page.url, file_name, pdf_content
         )
         return res[0]
 
     async def _notify_observers(
-        self, method: ObservationTrigger, *args: Any, **kwargs: Any
+        self, method: ObservationTrigger, *args: Any, check_duplication: bool = True, **kwargs: Any
     ) -> Any:
         """
         Notify all observers of an event. This will call the method on each observer that is subscribed. Note that
         the first observer is the stop pagination observer, so it will always be called separately so that we can stop
         pagination if needed.
         :param method: observation trigger
         :param args: arguments to pass to the method
         :param kwargs: keyword arguments to pass to the method
         :return: the result of the method call
         """
-        duplicated = await getattr(self._deduper, method)(*args, **kwargs)
+        duplicated = False
+        if check_duplication:
+            duplicated = await getattr(self._deduper, method)(*args, **kwargs)
+
         if not duplicated:
             return await asyncio.gather(
                 *[getattr(o, method)(*args, **kwargs) for o in self._observers]
             )
 
     @staticmethod
     async def run(
```

### Comparing `harambe_sdk-0.9.3/harambe/handlers.py` & `harambe_sdk-0.9.31/harambe/handlers.py`

 * *Files identical despite different names*

### Comparing `harambe_sdk-0.9.3/harambe/harness.py` & `harambe_sdk-0.9.31/harambe/harness.py`

 * *Files identical despite different names*

### Comparing `harambe_sdk-0.9.3/harambe/meta.py` & `harambe_sdk-0.9.31/harambe/meta.py`

 * *Files identical despite different names*

### Comparing `harambe_sdk-0.9.3/harambe/normalize_url.py` & `harambe_sdk-0.9.31/harambe/normalize_url.py`

 * *Files identical despite different names*

### Comparing `harambe_sdk-0.9.3/harambe/observer.py` & `harambe_sdk-0.9.31/harambe/observer.py`

 * *Files identical despite different names*

### Comparing `harambe_sdk-0.9.3/harambe/parser/parser.py` & `harambe_sdk-0.9.31/harambe/parser/parser.py`

 * *Files identical despite different names*

### Comparing `harambe_sdk-0.9.3/harambe/tracker.py` & `harambe_sdk-0.9.31/harambe/tracker.py`

 * *Files identical despite different names*

### Comparing `harambe_sdk-0.9.3/harambe/utils.py` & `harambe_sdk-0.9.31/harambe/utils.py`

 * *Files identical despite different names*

### Comparing `harambe_sdk-0.9.3/pyproject.toml` & `harambe_sdk-0.9.31/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "harambe-sdk"
-version = "0.9.3"
+version = "0.9.31"
 description = "Data extraction SDK for Playwright 🐒🍌"
 authors = ["awtkns <hello@awtkns.com>"]
 readme = "README.md"
 packages = [
     { include = "harambe", from = "." },
 ]
```

### Comparing `harambe_sdk-0.9.3/PKG-INFO` & `harambe_sdk-0.9.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harambe-sdk
-Version: 0.9.3
+Version: 0.9.31
 Summary: Data extraction SDK for Playwright 🐒🍌
 Author: awtkns
 Author-email: hello@awtkns.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

