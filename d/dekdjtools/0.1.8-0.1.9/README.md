# Comparing `tmp/dekdjtools-0.1.8.tar.gz` & `tmp/dekdjtools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dekdjtools-0.1.8.tar", last modified: Tue Apr 23 06:21:37 2024, max compression
+gzip compressed data, was "dekdjtools-0.1.9.tar", last modified: Tue Apr 23 06:52:41 2024, max compression
```

## Comparing `dekdjtools-0.1.8.tar` & `dekdjtools-0.1.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       25 2024-04-23 06:21:36.079005 dekdjtools-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-04-23 06:21:36.079005 dekdjtools-0.1.8/dekdjtools/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 06:21:36.079005 dekdjtools-0.1.8/dekdjtools/admin/__init__.py
--rw-r--r--   0        0        0     2215 2024-04-23 06:21:36.079005 dekdjtools-0.1.8/dekdjtools/admin/base/__init__.py
--rw-r--r--   0        0        0      152 2024-04-23 06:21:36.079005 dekdjtools-0.1.8/dekdjtools/apps.py
--rw-r--r--   0        0        0      217 2024-04-23 06:21:36.079005 dekdjtools-0.1.8/dekdjtools/console.py
--rw-r--r--   0        0        0      117 2024-04-23 06:21:36.079005 dekdjtools-0.1.8/dekdjtools/dekshellplugin/__init__.py
--rw-r--r--   0        0        0     1663 2024-04-23 06:21:36.079005 dekdjtools-0.1.8/dekdjtools/dekshellplugin/markers/__init__.py
--rw-r--r--   0        0        0       93 2024-04-23 06:21:36.079005 dekdjtools-0.1.8/dekdjtools/fields/__init__.py
--rw-r--r--   0        0        0     1982 2024-04-23 06:21:36.079005 dekdjtools-0.1.8/dekdjtools/fields/data.py
--rw-r--r--   0        0        0      484 2024-04-23 06:21:36.079005 dekdjtools-0.1.8/dekdjtools/fields/image.py
--rw-r--r--   0        0        0      966 2024-04-23 06:21:36.079005 dekdjtools-0.1.8/dekdjtools/fields/snowflake.py
--rw-r--r--   0        0        0      967 2024-04-23 06:21:36.079005 dekdjtools-0.1.8/dekdjtools/fields/snowflakeid.py
--rw-r--r--   0        0        0        0 2024-04-23 06:21:36.079005 dekdjtools-0.1.8/dekdjtools/management/__init__.py
--rw-r--r--   0        0        0      255 2024-04-23 06:21:36.079005 dekdjtools-0.1.8/dekdjtools/management/base/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 06:21:36.079005 dekdjtools-0.1.8/dekdjtools/management/commands/__init__.py
--rw-r--r--   0        0        0      328 2024-04-23 06:21:36.079005 dekdjtools-0.1.8/dekdjtools/management/commands/ddtdbreset.py
--rw-r--r--   0        0        0      782 2024-04-23 06:21:36.079005 dekdjtools-0.1.8/dekdjtools/management/commands/ddtdelmigrations.py
--rw-r--r--   0        0        0        0 2024-04-23 06:21:36.079005 dekdjtools-0.1.8/dekdjtools/migrations/__init__.py
--rw-r--r--   0        0        0       43 2024-04-23 06:21:36.079005 dekdjtools-0.1.8/dekdjtools/models/__init__.py
--rw-r--r--   0        0        0     2652 2024-04-23 06:21:36.079005 dekdjtools-0.1.8/dekdjtools/models/base/__init__.py
--rw-r--r--   0        0        0       34 2024-04-23 06:21:36.079005 dekdjtools-0.1.8/dekdjtools/settings.py
--rw-r--r--   0        0        0     1298 2024-04-23 06:21:36.079005 dekdjtools-0.1.8/dekdjtools/settings_app.py
--rw-r--r--   0        0        0     1664 2024-04-23 06:21:36.083005 dekdjtools-0.1.8/dekdjtools/settings_generate.py
--rw-r--r--   0        0        0     4473 2024-04-23 06:21:36.083005 dekdjtools-0.1.8/dekdjtools/snowflake.py
--rw-r--r--   0        0        0     1137 2024-04-23 06:21:36.083005 dekdjtools-0.1.8/dekdjtools/unionid.py
--rw-r--r--   0        0        0        0 2024-04-23 06:21:36.083005 dekdjtools-0.1.8/dekdjtools/utils/__init__.py
--rw-r--r--   0        0        0      558 2024-04-23 06:21:36.083005 dekdjtools-0.1.8/dekdjtools/utils/common.py
--rw-r--r--   0        0        0     1883 2024-04-23 06:21:36.083005 dekdjtools-0.1.8/dekdjtools/utils/finder.py
--rw-r--r--   0        0        0      862 2024-04-23 06:21:36.083005 dekdjtools-0.1.8/dekdjtools/utils/format.py
--rw-r--r--   0        0        0      914 2024-04-23 06:21:36.083005 dekdjtools-0.1.8/dekdjtools/utils/media.py
--rw-r--r--   0        0        0      799 2024-04-23 06:21:36.083005 dekdjtools-0.1.8/dekdjtools/utils/migration.py
--rw-r--r--   0        0        0     2918 2024-04-23 06:21:36.083005 dekdjtools-0.1.8/dekdjtools/utils/model.py
--rw-r--r--   0        0        0     2807 2024-04-23 06:21:36.083005 dekdjtools-0.1.8/dekdjtools/utils/query.py
--rw-r--r--   0        0        0     6473 2024-04-23 06:21:36.083005 dekdjtools-0.1.8/dekdjtools/utils/req.py
--rw-r--r--   0        0        0      441 2024-04-23 06:21:36.083005 dekdjtools-0.1.8/dekdjtools/utils/user.py
--rw-r--r--   0        0        0      655 2024-04-23 06:21:36.083005 dekdjtools-0.1.8/dekdjtools/validators.py
--rw-r--r--   0        0        0      632 2024-04-23 06:21:37.491010 dekdjtools-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 dekdjtools-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       25 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/admin/__init__.py
+-rw-r--r--   0        0        0     2215 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/admin/base/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/apps.py
+-rw-r--r--   0        0        0      217 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/console.py
+-rw-r--r--   0        0        0      117 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/dekshellplugin/__init__.py
+-rw-r--r--   0        0        0     1663 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/dekshellplugin/markers/__init__.py
+-rw-r--r--   0        0        0       93 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/fields/__init__.py
+-rw-r--r--   0        0        0     1982 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/fields/data.py
+-rw-r--r--   0        0        0      484 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/fields/image.py
+-rw-r--r--   0        0        0      966 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/fields/snowflake.py
+-rw-r--r--   0        0        0      967 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/fields/snowflakeid.py
+-rw-r--r--   0        0        0        0 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/management/__init__.py
+-rw-r--r--   0        0        0      255 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/management/base/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/management/commands/__init__.py
+-rw-r--r--   0        0        0      328 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/management/commands/ddtdbreset.py
+-rw-r--r--   0        0        0      782 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/management/commands/ddtdelmigrations.py
+-rw-r--r--   0        0        0        0 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/migrations/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/models/__init__.py
+-rw-r--r--   0        0        0     2652 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/models/base/__init__.py
+-rw-r--r--   0        0        0       34 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/settings.py
+-rw-r--r--   0        0        0     1298 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/settings_app.py
+-rw-r--r--   0        0        0     1780 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/settings_generate.py
+-rw-r--r--   0        0        0     4473 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/snowflake.py
+-rw-r--r--   0        0        0     1137 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/unionid.py
+-rw-r--r--   0        0        0        0 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/utils/__init__.py
+-rw-r--r--   0        0        0      558 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/utils/common.py
+-rw-r--r--   0        0        0     1883 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/utils/finder.py
+-rw-r--r--   0        0        0      862 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/utils/format.py
+-rw-r--r--   0        0        0      914 2024-04-23 06:52:40.335039 dekdjtools-0.1.9/dekdjtools/utils/media.py
+-rw-r--r--   0        0        0      799 2024-04-23 06:52:40.339039 dekdjtools-0.1.9/dekdjtools/utils/migration.py
+-rw-r--r--   0        0        0     2918 2024-04-23 06:52:40.339039 dekdjtools-0.1.9/dekdjtools/utils/model.py
+-rw-r--r--   0        0        0     2807 2024-04-23 06:52:40.339039 dekdjtools-0.1.9/dekdjtools/utils/query.py
+-rw-r--r--   0        0        0     6473 2024-04-23 06:52:40.339039 dekdjtools-0.1.9/dekdjtools/utils/req.py
+-rw-r--r--   0        0        0      441 2024-04-23 06:52:40.339039 dekdjtools-0.1.9/dekdjtools/utils/user.py
+-rw-r--r--   0        0        0      655 2024-04-23 06:52:40.339039 dekdjtools-0.1.9/dekdjtools/validators.py
+-rw-r--r--   0        0        0      632 2024-04-23 06:52:41.799043 dekdjtools-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 dekdjtools-0.1.9/PKG-INFO
```

### Comparing `dekdjtools-0.1.8/dekdjtools/admin/base/__init__.py` & `dekdjtools-0.1.9/dekdjtools/admin/base/__init__.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.8/dekdjtools/dekshellplugin/markers/__init__.py` & `dekdjtools-0.1.9/dekdjtools/dekshellplugin/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.8/dekdjtools/fields/data.py` & `dekdjtools-0.1.9/dekdjtools/fields/data.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.8/dekdjtools/fields/snowflake.py` & `dekdjtools-0.1.9/dekdjtools/fields/snowflake.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.8/dekdjtools/fields/snowflakeid.py` & `dekdjtools-0.1.9/dekdjtools/fields/snowflakeid.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.8/dekdjtools/management/commands/ddtdelmigrations.py` & `dekdjtools-0.1.9/dekdjtools/management/commands/ddtdelmigrations.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.8/dekdjtools/models/base/__init__.py` & `dekdjtools-0.1.9/dekdjtools/models/base/__init__.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.8/dekdjtools/settings_app.py` & `dekdjtools-0.1.9/dekdjtools/settings_app.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.8/dekdjtools/settings_generate.py` & `dekdjtools-0.1.9/dekdjtools/settings_generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,43 +16,45 @@
         "CLIENT_CLASS": "django_redis.client.DefaultClient",
     }
 }
 
 
 def generate_databases(s):
     result = {}
-    db_name, s = s.split('::')
-    if db_name:
-        db_name_options = {'NAME': db_name}
-    else:
-        db_name_options = {}
-    for item in s.split(','):
-        item = item.strip()
-        if not item:
-            continue
-        name, host = item.split(':')
-        result[name] = {**default_db_options, **{'HOST': host}, **db_name_options}
+    if s:
+        db_name, s = s.split('::')
+        if db_name:
+            db_name_options = {'NAME': db_name}
+        else:
+            db_name_options = {}
+        for item in s.split(','):
+            item = item.strip()
+            if not item:
+                continue
+            name, host = item.split(':')
+            result[name] = {**default_db_options, **{'HOST': host}, **db_name_options}
     return result
 
 
 def generate_caches(s):
     result = {}
-    for item in s.split(','):
-        item = item.strip()
-        if not item:
-            continue
-        name, host, index = item.split(':')
-        result[name] = {
-            **default_cache_options,
-            **{
-                'LOCATION': default_cache_options['LOCATION'] % (
-                    "123456", host, 6379, index or 0,
-                )
+    if s:
+        for item in s.split(','):
+            item = item.strip()
+            if not item:
+                continue
+            name, host, index = item.split(':')
+            result[name] = {
+                **default_cache_options,
+                **{
+                    'LOCATION': default_cache_options['LOCATION'] % (
+                        "123456", host, 6379, index or 0,
+                    )
+                }
             }
-        }
     return result
 
 
 extra_databases = generate_databases(os.getenv("DJANGO_PRESET_DATABASES", ""))
 extra_caches = generate_caches(os.getenv("DJANGO_PRESET_CACHES", ""))
```

### Comparing `dekdjtools-0.1.8/dekdjtools/snowflake.py` & `dekdjtools-0.1.9/dekdjtools/snowflake.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.8/dekdjtools/unionid.py` & `dekdjtools-0.1.9/dekdjtools/unionid.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.8/dekdjtools/utils/common.py` & `dekdjtools-0.1.9/dekdjtools/utils/common.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.8/dekdjtools/utils/finder.py` & `dekdjtools-0.1.9/dekdjtools/utils/finder.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.8/dekdjtools/utils/format.py` & `dekdjtools-0.1.9/dekdjtools/utils/format.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.8/dekdjtools/utils/media.py` & `dekdjtools-0.1.9/dekdjtools/utils/media.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.8/dekdjtools/utils/migration.py` & `dekdjtools-0.1.9/dekdjtools/utils/migration.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.8/dekdjtools/utils/model.py` & `dekdjtools-0.1.9/dekdjtools/utils/model.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.8/dekdjtools/utils/query.py` & `dekdjtools-0.1.9/dekdjtools/utils/query.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.8/dekdjtools/utils/req.py` & `dekdjtools-0.1.9/dekdjtools/utils/req.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.8/dekdjtools/validators.py` & `dekdjtools-0.1.9/dekdjtools/validators.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.8/pyproject.toml` & `dekdjtools-0.1.9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dekdjtools"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = [
     { name = "sanzenwin", email = "sanzenwin@gmail.com" },
 ]
 dependencies = [
     "django<=3.2.18",
     "django-extensions<=2.1.6",
```

