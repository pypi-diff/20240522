# Comparing `tmp/whaox-wapi-1.1.3.tar.gz` & `tmp/whaox-wapi-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whaox-wapi-1.1.3.tar", last modified: Sat May 18 05:09:41 2024, max compression
+gzip compressed data, was "whaox-wapi-1.1.4.tar", last modified: Wed May 22 18:46:59 2024, max compression
```

## Comparing `whaox-wapi-1.1.3.tar` & `whaox-wapi-1.1.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 05:09:41.251245 whaox-wapi-1.1.3/
--rw-rw-rw-   0        0        0     1083 2024-04-11 20:02:10.000000 whaox-wapi-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     3072 2024-05-18 05:09:41.250174 whaox-wapi-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2663 2024-05-16 18:13:06.000000 whaox-wapi-1.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-18 05:09:41.251824 whaox-wapi-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      932 2024-05-18 05:09:39.000000 whaox-wapi-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-18 05:09:41.192316 whaox-wapi-1.1.3/wapi/
--rw-rw-rw-   0        0        0       27 2024-04-15 09:31:56.000000 whaox-wapi-1.1.3/wapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 05:09:41.207352 whaox-wapi-1.1.3/wapi/features/
--rw-rw-rw-   0        0        0      669 2024-05-16 17:54:49.000000 whaox-wapi-1.1.3/wapi/features/DELETE.py
--rw-rw-rw-   0        0        0      663 2024-05-16 18:00:57.000000 whaox-wapi-1.1.3/wapi/features/GET.py
--rw-rw-rw-   0        0        0      667 2024-05-16 17:54:49.000000 whaox-wapi-1.1.3/wapi/features/PATCH.py
--rw-rw-rw-   0        0        0      659 2024-05-16 18:00:57.000000 whaox-wapi-1.1.3/wapi/features/POST.py
--rw-rw-rw-   0        0        0      663 2024-05-16 17:54:49.000000 whaox-wapi-1.1.3/wapi/features/PUT.py
--rw-rw-rw-   0        0        0      837 2024-05-09 11:47:35.000000 whaox-wapi-1.1.3/wapi/features/Route.py
--rw-rw-rw-   0        0        0      148 2024-05-16 18:00:57.000000 whaox-wapi-1.1.3/wapi/features/__init__.py
--rw-rw-rw-   0        0        0     1293 2024-05-18 05:09:39.000000 whaox-wapi-1.1.3/wapi/features/request.py
-drwxrwxrwx   0        0        0        0 2024-05-18 05:09:41.212447 whaox-wapi-1.1.3/wapi/static/
--rw-rw-rw-   0        0        0       48 2024-04-11 20:01:35.000000 whaox-wapi-1.1.3/wapi/static/T.py
--rw-rw-rw-   0        0        0        0 2024-04-15 09:20:58.000000 whaox-wapi-1.1.3/wapi/static/__init__.py
--rw-rw-rw-   0        0        0      118 2024-05-16 16:57:54.000000 whaox-wapi-1.1.3/wapi/static/methods.py
--rw-rw-rw-   0        0        0      440 2024-05-16 17:01:19.000000 whaox-wapi-1.1.3/wapi/static/params.py
-drwxrwxrwx   0        0        0        0 2024-05-18 05:09:41.225053 whaox-wapi-1.1.3/wapi/utils/
--rw-rw-rw-   0        0        0        0 2024-04-15 09:21:14.000000 whaox-wapi-1.1.3/wapi/utils/__init__.py
--rw-rw-rw-   0        0        0      299 2024-05-14 15:31:03.000000 whaox-wapi-1.1.3/wapi/utils/get_path.py
--rw-rw-rw-   0        0        0      252 2024-05-16 17:25:56.000000 whaox-wapi-1.1.3/wapi/utils/get_used_vars.py
--rw-rw-rw-   0        0        0       54 2024-05-09 11:47:35.000000 whaox-wapi-1.1.3/wapi/utils/is_class.py
--rw-rw-rw-   0        0        0      124 2024-04-11 20:01:35.000000 whaox-wapi-1.1.3/wapi/utils/is_dataclass.py
--rw-rw-rw-   0        0        0       59 2024-05-09 09:32:44.000000 whaox-wapi-1.1.3/wapi/utils/is_object.py
--rw-rw-rw-   0        0        0      311 2024-05-14 15:31:03.000000 whaox-wapi-1.1.3/wapi/utils/merge_paths.py
--rw-rw-rw-   0        0        0      242 2024-05-14 15:31:57.000000 whaox-wapi-1.1.3/wapi/utils/set_path.py
-drwxrwxrwx   0        0        0        0 2024-05-18 05:09:41.249651 whaox-wapi-1.1.3/whaox_wapi.egg-info/
--rw-rw-rw-   0        0        0     3072 2024-05-18 05:09:41.000000 whaox-wapi-1.1.3/whaox_wapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      680 2024-05-18 05:09:41.000000 whaox-wapi-1.1.3/whaox_wapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 05:09:41.000000 whaox-wapi-1.1.3/whaox_wapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-18 05:09:41.000000 whaox-wapi-1.1.3/whaox_wapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-18 05:09:41.000000 whaox-wapi-1.1.3/whaox_wapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 18:46:59.383000 whaox-wapi-1.1.4/
+-rw-rw-rw-   0        0        0     1083 2024-04-11 20:02:10.000000 whaox-wapi-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     3072 2024-05-22 18:46:59.381430 whaox-wapi-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2663 2024-05-16 18:13:06.000000 whaox-wapi-1.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 18:46:59.383000 whaox-wapi-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      932 2024-05-22 18:46:42.000000 whaox-wapi-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:46:59.322908 whaox-wapi-1.1.4/wapi/
+-rw-rw-rw-   0        0        0       27 2024-04-15 09:31:56.000000 whaox-wapi-1.1.4/wapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:46:59.332761 whaox-wapi-1.1.4/wapi/features/
+-rw-rw-rw-   0        0        0      669 2024-05-16 17:54:49.000000 whaox-wapi-1.1.4/wapi/features/DELETE.py
+-rw-rw-rw-   0        0        0      663 2024-05-16 18:00:57.000000 whaox-wapi-1.1.4/wapi/features/GET.py
+-rw-rw-rw-   0        0        0      667 2024-05-16 17:54:49.000000 whaox-wapi-1.1.4/wapi/features/PATCH.py
+-rw-rw-rw-   0        0        0      659 2024-05-16 18:00:57.000000 whaox-wapi-1.1.4/wapi/features/POST.py
+-rw-rw-rw-   0        0        0      663 2024-05-16 17:54:49.000000 whaox-wapi-1.1.4/wapi/features/PUT.py
+-rw-rw-rw-   0        0        0      946 2024-05-22 18:46:42.000000 whaox-wapi-1.1.4/wapi/features/Route.py
+-rw-rw-rw-   0        0        0      148 2024-05-16 18:00:57.000000 whaox-wapi-1.1.4/wapi/features/__init__.py
+-rw-rw-rw-   0        0        0     1293 2024-05-18 05:09:39.000000 whaox-wapi-1.1.4/wapi/features/request.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:46:59.336634 whaox-wapi-1.1.4/wapi/static/
+-rw-rw-rw-   0        0        0       48 2024-04-11 20:01:35.000000 whaox-wapi-1.1.4/wapi/static/T.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 09:20:58.000000 whaox-wapi-1.1.4/wapi/static/__init__.py
+-rw-rw-rw-   0        0        0      118 2024-05-16 16:57:54.000000 whaox-wapi-1.1.4/wapi/static/methods.py
+-rw-rw-rw-   0        0        0      440 2024-05-16 17:01:19.000000 whaox-wapi-1.1.4/wapi/static/params.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:46:59.345610 whaox-wapi-1.1.4/wapi/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-15 09:21:14.000000 whaox-wapi-1.1.4/wapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      299 2024-05-14 15:31:03.000000 whaox-wapi-1.1.4/wapi/utils/get_path.py
+-rw-rw-rw-   0        0        0      252 2024-05-16 17:25:56.000000 whaox-wapi-1.1.4/wapi/utils/get_used_vars.py
+-rw-rw-rw-   0        0        0       54 2024-05-09 11:47:35.000000 whaox-wapi-1.1.4/wapi/utils/is_class.py
+-rw-rw-rw-   0        0        0      124 2024-04-11 20:01:35.000000 whaox-wapi-1.1.4/wapi/utils/is_dataclass.py
+-rw-rw-rw-   0        0        0       59 2024-05-09 09:32:44.000000 whaox-wapi-1.1.4/wapi/utils/is_object.py
+-rw-rw-rw-   0        0        0      311 2024-05-14 15:31:03.000000 whaox-wapi-1.1.4/wapi/utils/merge_paths.py
+-rw-rw-rw-   0        0        0      242 2024-05-14 15:31:57.000000 whaox-wapi-1.1.4/wapi/utils/set_path.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:46:59.380279 whaox-wapi-1.1.4/whaox_wapi.egg-info/
+-rw-rw-rw-   0        0        0     3072 2024-05-22 18:46:59.000000 whaox-wapi-1.1.4/whaox_wapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      680 2024-05-22 18:46:59.000000 whaox-wapi-1.1.4/whaox_wapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 18:46:59.000000 whaox-wapi-1.1.4/whaox_wapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-22 18:46:59.000000 whaox-wapi-1.1.4/whaox_wapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-22 18:46:59.000000 whaox-wapi-1.1.4/whaox_wapi.egg-info/top_level.txt
```

### Comparing `whaox-wapi-1.1.3/LICENSE` & `whaox-wapi-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.1.3/PKG-INFO` & `whaox-wapi-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whaox-wapi
-Version: 1.1.3
+Version: 1.1.4
 Summary: Web-Library for Python
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
 Keywords: python,web,api,requests,post,get,put,patch,delete,rest
 Description-Content-Type: text/markdown
```

### Comparing `whaox-wapi-1.1.3/README.md` & `whaox-wapi-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.1.3/setup.py` & `whaox-wapi-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 """
 :authors: WHAOX
 :license: MIT License, see LICENSE file
 :copyright: (c) 2024 WHAOX
 """
 
-version = '1.1.3'
+version = '1.1.4'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='whaox-wapi',
     version=version,
```

### Comparing `whaox-wapi-1.1.3/wapi/features/DELETE.py` & `whaox-wapi-1.1.4/wapi/features/DELETE.py`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.1.3/wapi/features/GET.py` & `whaox-wapi-1.1.4/wapi/features/GET.py`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.1.3/wapi/features/PATCH.py` & `whaox-wapi-1.1.4/wapi/features/PATCH.py`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.1.3/wapi/features/POST.py` & `whaox-wapi-1.1.4/wapi/features/POST.py`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.1.3/wapi/features/PUT.py` & `whaox-wapi-1.1.4/wapi/features/PUT.py`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.1.3/wapi/features/Route.py` & `whaox-wapi-1.1.4/wapi/features/Route.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,17 +15,20 @@
 
             set_path(obj)
 
             return obj
 
         @wraps(obj)
         def func_wrapper(self, *args, **kwargs):
-            if hasattr(obj.__wrapped__, 'path'):
-                obj.__wrapped__.path = path + obj.__wrapped__.path
-            else:
+            # if hasattr(obj.__wrapped__, 'path'):
+            #     obj.__wrapped__.path = path + obj.__wrapped__.path
+            # else:
+            #     obj.__wrapped__.path = path
+
+            if not hasattr(obj.__wrapped__, 'path'):
                 obj.__wrapped__.path = path
 
             return obj(self, *args, **kwargs)
 
         if is_class(obj):
             return class_wrapper()
         return func_wrapper
```

### Comparing `whaox-wapi-1.1.3/wapi/features/request.py` & `whaox-wapi-1.1.4/wapi/features/request.py`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.1.3/whaox_wapi.egg-info/PKG-INFO` & `whaox-wapi-1.1.4/whaox_wapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whaox-wapi
-Version: 1.1.3
+Version: 1.1.4
 Summary: Web-Library for Python
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
 Keywords: python,web,api,requests,post,get,put,patch,delete,rest
 Description-Content-Type: text/markdown
```

### Comparing `whaox-wapi-1.1.3/whaox_wapi.egg-info/SOURCES.txt` & `whaox-wapi-1.1.4/whaox_wapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

