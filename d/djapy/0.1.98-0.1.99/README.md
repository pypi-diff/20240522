# Comparing `tmp/djapy-0.1.98.tar.gz` & `tmp/djapy-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djapy-0.1.98.tar", last modified: Fri Mar 22 16:39:23 2024, max compression
+gzip compressed data, was "djapy-0.1.99.tar", last modified: Thu Mar 28 06:25:15 2024, max compression
```

## Comparing `djapy-0.1.98.tar` & `djapy-0.1.99.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-03-22 16:39:23.311723 djapy-0.1.98/
--rw-r--r--   0 codie     (1000) codie     (1000)     2209 2024-03-22 16:39:23.311723 djapy-0.1.98/PKG-INFO
--rw-r--r--   0 codie     (1000) codie     (1000)     1554 2024-03-16 02:12:56.000000 djapy-0.1.98/README.md
-drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-03-22 16:39:23.301723 djapy-0.1.98/djapy/
--rw-r--r--   0 codie     (1000) codie     (1000)      385 2024-03-07 04:59:47.000000 djapy-0.1.98/djapy/__init__.py
-drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-03-22 16:39:23.306723 djapy-0.1.98/djapy/core/
--rw-r--r--   0 codie     (1000) codie     (1000)        0 2024-02-27 12:33:41.000000 djapy-0.1.98/djapy/core/__init__.py
-drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-03-22 16:39:23.307723 djapy-0.1.98/djapy/core/auth/
--rw-r--r--   0 codie     (1000) codie     (1000)      276 2024-03-09 04:12:37.000000 djapy-0.1.98/djapy/core/auth/__init__.py
--rw-r--r--   0 codie     (1000) codie     (1000)     2065 2024-03-09 04:35:05.000000 djapy-0.1.98/djapy/core/auth/auth.py
--rw-r--r--   0 codie     (1000) codie     (1000)     1931 2024-03-09 04:28:51.000000 djapy-0.1.98/djapy/core/auth/dec.py
--rw-r--r--   0 codie     (1000) codie     (1000)    12347 2024-03-14 06:01:12.000000 djapy-0.1.98/djapy/core/dec.py
--rw-r--r--   0 codie     (1000) codie     (1000)      352 2024-03-09 04:13:00.000000 djapy-0.1.98/djapy/core/defaults.py
--rw-r--r--   0 codie     (1000) codie     (1000)      141 2024-02-27 12:36:19.000000 djapy-0.1.98/djapy/core/labels.py
--rw-r--r--   0 codie     (1000) codie     (1000)      896 2024-03-21 03:11:40.000000 djapy-0.1.98/djapy/core/mid.py
--rw-r--r--   0 codie     (1000) codie     (1000)     4283 2024-03-21 04:12:48.000000 djapy-0.1.98/djapy/core/parser.py
--rw-r--r--   0 codie     (1000) codie     (1000)      639 2024-02-27 12:36:06.000000 djapy-0.1.98/djapy/core/response.py
--rw-r--r--   0 codie     (1000) codie     (1000)     3739 2024-03-21 14:58:14.000000 djapy-0.1.98/djapy/core/type_check.py
--rw-r--r--   0 codie     (1000) codie     (1000)       55 2024-03-09 03:21:47.000000 djapy-0.1.98/djapy/core/typing_utils.py
-drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-03-22 16:39:23.308723 djapy-0.1.98/djapy/openapi/
--rw-r--r--   0 codie     (1000) codie     (1000)     5655 2024-03-21 12:22:02.000000 djapy-0.1.98/djapy/openapi/__init__.py
--rw-r--r--   0 codie     (1000) codie     (1000)      192 2024-02-28 04:37:25.000000 djapy-0.1.98/djapy/openapi/defaults.py
--rw-r--r--   0 codie     (1000) codie     (1000)     1341 2024-03-15 10:34:56.000000 djapy-0.1.98/djapy/openapi/icons.py
--rw-r--r--   0 codie     (1000) codie     (1000)      710 2024-03-15 12:02:27.000000 djapy-0.1.98/djapy/openapi/info.py
--rw-r--r--   0 codie     (1000) codie     (1000)     6925 2024-03-21 15:40:03.000000 djapy-0.1.98/djapy/openapi/openapi_path.py
-drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-03-22 16:39:23.310723 djapy-0.1.98/djapy/pagination/
--rw-r--r--   0 codie     (1000) codie     (1000)      350 2024-03-09 06:14:29.000000 djapy-0.1.98/djapy/pagination/__init__.py
--rw-r--r--   0 codie     (1000) codie     (1000)      310 2024-03-09 04:40:41.000000 djapy-0.1.98/djapy/pagination/base_pagination.py
--rw-r--r--   0 codie     (1000) codie     (1000)     2991 2024-03-11 03:32:52.000000 djapy-0.1.98/djapy/pagination/cursor_pagination.py
--rw-r--r--   0 codie     (1000) codie     (1000)     1490 2024-03-09 16:07:13.000000 djapy-0.1.98/djapy/pagination/dec.py
--rw-r--r--   0 codie     (1000) codie     (1000)     1899 2024-03-18 16:11:04.000000 djapy-0.1.98/djapy/pagination/offset_pagination.py
--rw-r--r--   0 codie     (1000) codie     (1000)     1770 2024-03-09 05:18:01.000000 djapy-0.1.98/djapy/pagination/page_number_pagination.py
-drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-03-22 16:39:23.310723 djapy-0.1.98/djapy/schema/
--rw-r--r--   0 codie     (1000) codie     (1000)      150 2024-03-21 04:21:21.000000 djapy-0.1.98/djapy/schema/__init__.py
--rw-r--r--   0 codie     (1000) codie     (1000)     1824 2024-03-21 04:34:39.000000 djapy-0.1.98/djapy/schema/handle.py
--rw-r--r--   0 codie     (1000) codie     (1000)     1081 2024-03-21 16:53:37.000000 djapy-0.1.98/djapy/schema/schema.py
--rw-r--r--   0 codie     (1000) codie     (1000)      451 2024-02-25 13:12:35.000000 djapy-0.1.98/djapy/schema/user.py
-drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-03-22 16:39:23.301723 djapy-0.1.98/djapy/templates/
-drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-03-22 16:39:23.310723 djapy-0.1.98/djapy/templates/djapy/
--rw-r--r--   0 codie     (1000) codie     (1000)     3395 2024-03-22 15:43:48.000000 djapy-0.1.98/djapy/templates/djapy/swagger_cdn.html
-drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-03-22 16:39:23.310723 djapy-0.1.98/djapy.egg-info/
--rw-r--r--   0 codie     (1000) codie     (1000)     2209 2024-03-22 16:39:23.000000 djapy-0.1.98/djapy.egg-info/PKG-INFO
--rw-r--r--   0 codie     (1000) codie     (1000)      920 2024-03-22 16:39:23.000000 djapy-0.1.98/djapy.egg-info/SOURCES.txt
--rw-r--r--   0 codie     (1000) codie     (1000)        1 2024-03-22 16:39:23.000000 djapy-0.1.98/djapy.egg-info/dependency_links.txt
--rw-r--r--   0 codie     (1000) codie     (1000)       16 2024-03-22 16:39:23.000000 djapy-0.1.98/djapy.egg-info/requires.txt
--rw-r--r--   0 codie     (1000) codie     (1000)        6 2024-03-22 16:39:23.000000 djapy-0.1.98/djapy.egg-info/top_level.txt
--rw-r--r--   0 codie     (1000) codie     (1000)       38 2024-03-22 16:39:23.311723 djapy-0.1.98/setup.cfg
--rw-r--r--   0 codie     (1000) codie     (1000)     1045 2024-03-22 16:38:37.000000 djapy-0.1.98/setup.py
+drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-03-28 06:25:15.079758 djapy-0.1.99/
+-rw-r--r--   0 codie     (1000) codie     (1000)     2209 2024-03-28 06:25:15.079758 djapy-0.1.99/PKG-INFO
+-rw-r--r--   0 codie     (1000) codie     (1000)     1554 2024-03-16 02:12:56.000000 djapy-0.1.99/README.md
+drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-03-28 06:25:15.076758 djapy-0.1.99/djapy/
+-rw-r--r--   0 codie     (1000) codie     (1000)      385 2024-03-07 04:59:47.000000 djapy-0.1.99/djapy/__init__.py
+drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-03-28 06:25:15.077758 djapy-0.1.99/djapy/core/
+-rw-r--r--   0 codie     (1000) codie     (1000)        0 2024-02-27 12:33:41.000000 djapy-0.1.99/djapy/core/__init__.py
+drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-03-28 06:25:15.077758 djapy-0.1.99/djapy/core/auth/
+-rw-r--r--   0 codie     (1000) codie     (1000)      276 2024-03-09 04:12:37.000000 djapy-0.1.99/djapy/core/auth/__init__.py
+-rw-r--r--   0 codie     (1000) codie     (1000)     2065 2024-03-09 04:35:05.000000 djapy-0.1.99/djapy/core/auth/auth.py
+-rw-r--r--   0 codie     (1000) codie     (1000)     1931 2024-03-09 04:28:51.000000 djapy-0.1.99/djapy/core/auth/dec.py
+-rw-r--r--   0 codie     (1000) codie     (1000)    12347 2024-03-14 06:01:12.000000 djapy-0.1.99/djapy/core/dec.py
+-rw-r--r--   0 codie     (1000) codie     (1000)      352 2024-03-09 04:13:00.000000 djapy-0.1.99/djapy/core/defaults.py
+-rw-r--r--   0 codie     (1000) codie     (1000)      141 2024-02-27 12:36:19.000000 djapy-0.1.99/djapy/core/labels.py
+-rw-r--r--   0 codie     (1000) codie     (1000)      896 2024-03-21 03:11:40.000000 djapy-0.1.99/djapy/core/mid.py
+-rw-r--r--   0 codie     (1000) codie     (1000)     4384 2024-03-28 06:24:13.000000 djapy-0.1.99/djapy/core/parser.py
+-rw-r--r--   0 codie     (1000) codie     (1000)      639 2024-02-27 12:36:06.000000 djapy-0.1.99/djapy/core/response.py
+-rw-r--r--   0 codie     (1000) codie     (1000)     3739 2024-03-21 14:58:14.000000 djapy-0.1.99/djapy/core/type_check.py
+-rw-r--r--   0 codie     (1000) codie     (1000)       55 2024-03-09 03:21:47.000000 djapy-0.1.99/djapy/core/typing_utils.py
+drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-03-28 06:25:15.078758 djapy-0.1.99/djapy/openapi/
+-rw-r--r--   0 codie     (1000) codie     (1000)     5655 2024-03-21 12:22:02.000000 djapy-0.1.99/djapy/openapi/__init__.py
+-rw-r--r--   0 codie     (1000) codie     (1000)      192 2024-02-28 04:37:25.000000 djapy-0.1.99/djapy/openapi/defaults.py
+-rw-r--r--   0 codie     (1000) codie     (1000)     1341 2024-03-15 10:34:56.000000 djapy-0.1.99/djapy/openapi/icons.py
+-rw-r--r--   0 codie     (1000) codie     (1000)      710 2024-03-15 12:02:27.000000 djapy-0.1.99/djapy/openapi/info.py
+-rw-r--r--   0 codie     (1000) codie     (1000)     6925 2024-03-21 15:40:03.000000 djapy-0.1.99/djapy/openapi/openapi_path.py
+drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-03-28 06:25:15.078758 djapy-0.1.99/djapy/pagination/
+-rw-r--r--   0 codie     (1000) codie     (1000)      350 2024-03-09 06:14:29.000000 djapy-0.1.99/djapy/pagination/__init__.py
+-rw-r--r--   0 codie     (1000) codie     (1000)      310 2024-03-09 04:40:41.000000 djapy-0.1.99/djapy/pagination/base_pagination.py
+-rw-r--r--   0 codie     (1000) codie     (1000)     2991 2024-03-11 03:32:52.000000 djapy-0.1.99/djapy/pagination/cursor_pagination.py
+-rw-r--r--   0 codie     (1000) codie     (1000)     1490 2024-03-09 16:07:13.000000 djapy-0.1.99/djapy/pagination/dec.py
+-rw-r--r--   0 codie     (1000) codie     (1000)     1899 2024-03-18 16:11:04.000000 djapy-0.1.99/djapy/pagination/offset_pagination.py
+-rw-r--r--   0 codie     (1000) codie     (1000)     1770 2024-03-09 05:18:01.000000 djapy-0.1.99/djapy/pagination/page_number_pagination.py
+drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-03-28 06:25:15.079758 djapy-0.1.99/djapy/schema/
+-rw-r--r--   0 codie     (1000) codie     (1000)      150 2024-03-21 04:21:21.000000 djapy-0.1.99/djapy/schema/__init__.py
+-rw-r--r--   0 codie     (1000) codie     (1000)     1824 2024-03-21 04:34:39.000000 djapy-0.1.99/djapy/schema/handle.py
+-rw-r--r--   0 codie     (1000) codie     (1000)     1081 2024-03-21 16:53:37.000000 djapy-0.1.99/djapy/schema/schema.py
+-rw-r--r--   0 codie     (1000) codie     (1000)      451 2024-02-25 13:12:35.000000 djapy-0.1.99/djapy/schema/user.py
+drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-03-28 06:25:15.076758 djapy-0.1.99/djapy/templates/
+drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-03-28 06:25:15.079758 djapy-0.1.99/djapy/templates/djapy/
+-rw-r--r--   0 codie     (1000) codie     (1000)     3395 2024-03-22 15:43:48.000000 djapy-0.1.99/djapy/templates/djapy/swagger_cdn.html
+drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-03-28 06:25:15.079758 djapy-0.1.99/djapy.egg-info/
+-rw-r--r--   0 codie     (1000) codie     (1000)     2209 2024-03-28 06:25:15.000000 djapy-0.1.99/djapy.egg-info/PKG-INFO
+-rw-r--r--   0 codie     (1000) codie     (1000)      920 2024-03-28 06:25:15.000000 djapy-0.1.99/djapy.egg-info/SOURCES.txt
+-rw-r--r--   0 codie     (1000) codie     (1000)        1 2024-03-28 06:25:15.000000 djapy-0.1.99/djapy.egg-info/dependency_links.txt
+-rw-r--r--   0 codie     (1000) codie     (1000)       16 2024-03-28 06:25:15.000000 djapy-0.1.99/djapy.egg-info/requires.txt
+-rw-r--r--   0 codie     (1000) codie     (1000)        6 2024-03-28 06:25:15.000000 djapy-0.1.99/djapy.egg-info/top_level.txt
+-rw-r--r--   0 codie     (1000) codie     (1000)       38 2024-03-28 06:25:15.079758 djapy-0.1.99/setup.cfg
+-rw-r--r--   0 codie     (1000) codie     (1000)     1045 2024-03-28 06:24:44.000000 djapy-0.1.99/setup.py
```

### Comparing `djapy-0.1.98/PKG-INFO` & `djapy-0.1.99/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djapy
-Version: 0.1.98
+Version: 0.1.99
 Summary: Write powerful APIs with Django and Pydantic; I/O validation, Swagger/OpenAPI docs, and more.
 Home-page: https://github.com/Bishwas-py/djapy
 Project-URL: Documentation, https://djapy.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `djapy-0.1.98/README.md` & `djapy-0.1.99/README.md`

 * *Files identical despite different names*

### Comparing `djapy-0.1.98/djapy/core/auth/auth.py` & `djapy-0.1.99/djapy/core/auth/auth.py`

 * *Files identical despite different names*

### Comparing `djapy-0.1.98/djapy/core/auth/dec.py` & `djapy-0.1.99/djapy/core/auth/dec.py`

 * *Files identical despite different names*

### Comparing `djapy-0.1.98/djapy/core/dec.py` & `djapy-0.1.99/djapy/core/dec.py`

 * *Files identical despite different names*

### Comparing `djapy-0.1.98/djapy/core/mid.py` & `djapy-0.1.99/djapy/core/mid.py`

 * *Files identical despite different names*

### Comparing `djapy-0.1.98/djapy/core/parser.py` & `djapy-0.1.99/djapy/core/parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,25 +24,26 @@
         self.data = {}
 
     def parse_request_data(self):
         """
         Parse the request data and validate it with the data model.
         """
         self.set_request_data()
+        context = {"request": self.request}
         if self.single_data_schema:
-            validated_obj = self.single_data_schema.validate(self.data)
+            validated_obj = self.single_data_schema.model_validate(self.data, context=context)
             destructured_data_dict = {self.single_data_key: validated_obj}
         else:
-            data = self.data_schema.model_validate(self.data)
+            data = self.data_schema.model_validate(self.data, context=context)
             destructured_data_dict = data.__dict__
 
         query_data = self.query_schema.model_validate({
             **self.query_data,
             **self.line_kwargs
-        })
+        }, context=context)
         destructured_object_data = {
             **query_data.__dict__,
             **destructured_data_dict
         }
         return destructured_object_data
 
     def set_request_data(self):
```

### Comparing `djapy-0.1.98/djapy/core/response.py` & `djapy-0.1.99/djapy/core/response.py`

 * *Files identical despite different names*

### Comparing `djapy-0.1.98/djapy/core/type_check.py` & `djapy-0.1.99/djapy/core/type_check.py`

 * *Files identical despite different names*

### Comparing `djapy-0.1.98/djapy/openapi/__init__.py` & `djapy-0.1.99/djapy/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `djapy-0.1.98/djapy/openapi/icons.py` & `djapy-0.1.99/djapy/openapi/icons.py`

 * *Files identical despite different names*

### Comparing `djapy-0.1.98/djapy/openapi/info.py` & `djapy-0.1.99/djapy/openapi/info.py`

 * *Files identical despite different names*

### Comparing `djapy-0.1.98/djapy/openapi/openapi_path.py` & `djapy-0.1.99/djapy/openapi/openapi_path.py`

 * *Files identical despite different names*

### Comparing `djapy-0.1.98/djapy/pagination/cursor_pagination.py` & `djapy-0.1.99/djapy/pagination/cursor_pagination.py`

 * *Files identical despite different names*

### Comparing `djapy-0.1.98/djapy/pagination/dec.py` & `djapy-0.1.99/djapy/pagination/dec.py`

 * *Files identical despite different names*

### Comparing `djapy-0.1.98/djapy/pagination/offset_pagination.py` & `djapy-0.1.99/djapy/pagination/offset_pagination.py`

 * *Files identical despite different names*

### Comparing `djapy-0.1.98/djapy/pagination/page_number_pagination.py` & `djapy-0.1.99/djapy/pagination/page_number_pagination.py`

 * *Files identical despite different names*

### Comparing `djapy-0.1.98/djapy/schema/handle.py` & `djapy-0.1.99/djapy/schema/handle.py`

 * *Files identical despite different names*

### Comparing `djapy-0.1.98/djapy/schema/schema.py` & `djapy-0.1.99/djapy/schema/schema.py`

 * *Files identical despite different names*

### Comparing `djapy-0.1.98/djapy/templates/djapy/swagger_cdn.html` & `djapy-0.1.99/djapy/templates/djapy/swagger_cdn.html`

 * *Files identical despite different names*

### Comparing `djapy-0.1.98/djapy.egg-info/PKG-INFO` & `djapy-0.1.99/djapy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djapy
-Version: 0.1.98
+Version: 0.1.99
 Summary: Write powerful APIs with Django and Pydantic; I/O validation, Swagger/OpenAPI docs, and more.
 Home-page: https://github.com/Bishwas-py/djapy
 Project-URL: Documentation, https://djapy.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `djapy-0.1.98/djapy.egg-info/SOURCES.txt` & `djapy-0.1.99/djapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djapy-0.1.98/setup.py` & `djapy-0.1.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="djapy",
-    version="0.1.98",
+    version="0.1.99",
     description="Write powerful APIs with Django and Pydantic; I/O validation, Swagger/OpenAPI docs, and more.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Bishwas-py/djapy",
     py_modules=["djapy"],
     packages=find_packages(include=["djapy", "djapy.*"]),
     package_data={
```

