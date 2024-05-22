# Comparing `tmp/todoist_api_python-2.1.4.tar.gz` & `tmp/todoist_api_python-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "todoist_api_python-2.1.4.tar", max compression
+gzip compressed data, was "todoist_api_python-2.1.5.tar", max compression
```

## Comparing `todoist_api_python-2.1.4.tar` & `todoist_api_python-2.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2024-05-07 13:43:04.045588 todoist_api_python-2.1.4/LICENSE
--rw-r--r--   0        0        0     2906 2024-05-07 13:43:04.045588 todoist_api_python-2.1.4/README.md
--rw-r--r--   0        0        0     4880 2024-05-07 13:43:04.045588 todoist_api_python-2.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-07 13:43:04.049588 todoist_api_python-2.1.4/todoist_api_python/__init__.py
--rw-r--r--   0        0        0     9394 2024-05-07 13:43:04.049588 todoist_api_python-2.1.4/todoist_api_python/api.py
--rw-r--r--   0        0        0     5595 2024-05-07 13:43:04.049588 todoist_api_python-2.1.4/todoist_api_python/api_async.py
--rw-r--r--   0        0        0     2002 2024-05-07 13:43:04.049588 todoist_api_python-2.1.4/todoist_api_python/authentication.py
--rw-r--r--   0        0        0     1103 2024-05-07 13:43:04.049588 todoist_api_python-2.1.4/todoist_api_python/endpoints.py
--rw-r--r--   0        0        0      645 2024-05-07 13:43:04.049588 todoist_api_python-2.1.4/todoist_api_python/headers.py
--rw-r--r--   0        0        0     1414 2024-05-07 13:43:04.049588 todoist_api_python-2.1.4/todoist_api_python/http_requests.py
--rw-r--r--   0        0        0    11615 2024-05-07 13:43:04.049588 todoist_api_python-2.1.4/todoist_api_python/models.py
--rw-r--r--   0        0        0        0 2024-05-07 13:43:04.049588 todoist_api_python-2.1.4/todoist_api_python/py.typed
--rw-r--r--   0        0        0      436 2024-05-07 13:43:04.049588 todoist_api_python-2.1.4/todoist_api_python/utils.py
--rw-r--r--   0        0        0     3842 1970-01-01 00:00:00.000000 todoist_api_python-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-22 06:45:19.606107 todoist_api_python-2.1.5/LICENSE
+-rw-r--r--   0        0        0     2906 2024-05-22 06:45:19.606107 todoist_api_python-2.1.5/README.md
+-rw-r--r--   0        0        0     4880 2024-05-22 06:45:19.606107 todoist_api_python-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-22 06:45:19.610107 todoist_api_python-2.1.5/todoist_api_python/__init__.py
+-rw-r--r--   0        0        0     9394 2024-05-22 06:45:19.610107 todoist_api_python-2.1.5/todoist_api_python/api.py
+-rw-r--r--   0        0        0     5595 2024-05-22 06:45:19.610107 todoist_api_python-2.1.5/todoist_api_python/api_async.py
+-rw-r--r--   0        0        0     2002 2024-05-22 06:45:19.610107 todoist_api_python-2.1.5/todoist_api_python/authentication.py
+-rw-r--r--   0        0        0     1103 2024-05-22 06:45:19.610107 todoist_api_python-2.1.5/todoist_api_python/endpoints.py
+-rw-r--r--   0        0        0      645 2024-05-22 06:45:19.610107 todoist_api_python-2.1.5/todoist_api_python/headers.py
+-rw-r--r--   0        0        0     1414 2024-05-22 06:45:19.610107 todoist_api_python-2.1.5/todoist_api_python/http_requests.py
+-rw-r--r--   0        0        0    11619 2024-05-22 06:45:19.610107 todoist_api_python-2.1.5/todoist_api_python/models.py
+-rw-r--r--   0        0        0        0 2024-05-22 06:45:19.610107 todoist_api_python-2.1.5/todoist_api_python/py.typed
+-rw-r--r--   0        0        0      436 2024-05-22 06:45:19.610107 todoist_api_python-2.1.5/todoist_api_python/utils.py
+-rw-r--r--   0        0        0     3842 1970-01-01 00:00:00.000000 todoist_api_python-2.1.5/PKG-INFO
```

### Comparing `todoist_api_python-2.1.4/LICENSE` & `todoist_api_python-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `todoist_api_python-2.1.4/README.md` & `todoist_api_python-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `todoist_api_python-2.1.4/pyproject.toml` & `todoist_api_python-2.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "todoist_api_python"
-version = "2.1.4"
+version = "2.1.5"
 description = "Official Python SDK for the Todoist REST API."
 readme = "README.md"
 homepage = "https://github.com/Doist/todoist-api-python"
 repository = "https://github.com/Doist/todoist-api-python"
 documentation = "https://developer.todoist.com/rest/"
 authors = ["Doist Developers <dev@doist.com>"]
 keywords = ["todoist", "rest", "api", "python"]
```

### Comparing `todoist_api_python-2.1.4/todoist_api_python/api.py` & `todoist_api_python-2.1.5/todoist_api_python/api.py`

 * *Files identical despite different names*

### Comparing `todoist_api_python-2.1.4/todoist_api_python/api_async.py` & `todoist_api_python-2.1.5/todoist_api_python/api_async.py`

 * *Files identical despite different names*

### Comparing `todoist_api_python-2.1.4/todoist_api_python/authentication.py` & `todoist_api_python-2.1.5/todoist_api_python/authentication.py`

 * *Files identical despite different names*

### Comparing `todoist_api_python-2.1.4/todoist_api_python/endpoints.py` & `todoist_api_python-2.1.5/todoist_api_python/endpoints.py`

 * *Files identical despite different names*

### Comparing `todoist_api_python-2.1.4/todoist_api_python/headers.py` & `todoist_api_python-2.1.5/todoist_api_python/headers.py`

 * *Files identical despite different names*

### Comparing `todoist_api_python-2.1.4/todoist_api_python/http_requests.py` & `todoist_api_python-2.1.5/todoist_api_python/http_requests.py`

 * *Files identical despite different names*

### Comparing `todoist_api_python-2.1.4/todoist_api_python/models.py` & `todoist_api_python-2.1.5/todoist_api_python/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             color=obj["color"],
             comment_count=obj["comment_count"],
             id=obj["id"],
             is_favorite=obj["is_favorite"],
             is_inbox_project=obj.get("is_inbox_project"),
             is_shared=obj["is_shared"],
             is_team_inbox=obj.get("is_team_inbox"),
-            can_assign_tasks=obj["can_assign_tasks"],
+            can_assign_tasks=obj.get("can_assign_tasks"),
             name=obj["name"],
             order=obj.get("order"),
             parent_id=obj.get("parent_id"),
             url=obj["url"],
             view_style=obj["view_style"],
         )
```

### Comparing `todoist_api_python-2.1.4/PKG-INFO` & `todoist_api_python-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: todoist_api_python
-Version: 2.1.4
+Version: 2.1.5
 Summary: Official Python SDK for the Todoist REST API.
 Home-page: https://github.com/Doist/todoist-api-python
 License: MIT
 Keywords: todoist,rest,api,python
 Author: Doist Developers
 Author-email: dev@doist.com
 Requires-Python: >=3.9,<4.0
```

