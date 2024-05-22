# Comparing `tmp/arccanet-0.0.5.tar.gz` & `tmp/arccanet-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arccanet-0.0.5.tar", last modified: Tue Mar 19 16:44:04 2024, max compression
+gzip compressed data, was "arccanet-0.0.6.tar", last modified: Wed May 22 19:00:07 2024, max compression
```

## Comparing `arccanet-0.0.5.tar` & `arccanet-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 16:44:04.213428 arccanet-0.0.5/
--rw-r--r--   0 root         (0) root         (0)      231 2024-03-19 16:44:04.212428 arccanet-0.0.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      437 2024-03-19 16:44:03.000000 arccanet-0.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 16:44:04.211428 arccanet-0.0.5/arccanet/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-19 16:44:03.000000 arccanet-0.0.5/arccanet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1691 2024-03-19 16:44:03.000000 arccanet-0.0.5/arccanet/conditionbuilder.py
--rw-rw-rw-   0 root         (0) root         (0)       54 2024-03-19 16:44:03.000000 arccanet-0.0.5/arccanet/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3476 2024-03-19 16:44:03.000000 arccanet-0.0.5/arccanet/general.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2024-03-19 16:44:03.000000 arccanet-0.0.5/arccanet/jwt.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2024-03-19 16:44:03.000000 arccanet-0.0.5/arccanet/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2024-03-19 16:44:03.000000 arccanet-0.0.5/arccanet/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)       45 2024-03-19 16:44:03.000000 arccanet-0.0.5/arccanet/response.py
--rw-rw-rw-   0 root         (0) root         (0)     3469 2024-03-19 16:44:03.000000 arccanet-0.0.5/arccanet/responsebuilder.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-19 16:44:03.000000 arccanet-0.0.5/arccanet/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2024-03-19 16:44:03.000000 arccanet-0.0.5/arccanet/test.py
--rw-rw-rw-   0 root         (0) root         (0)      335 2024-03-19 16:44:03.000000 arccanet-0.0.5/arccanet/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 16:44:04.212428 arccanet-0.0.5/arccanet.egg-info/
--rw-r--r--   0 root         (0) root         (0)      231 2024-03-19 16:44:04.000000 arccanet-0.0.5/arccanet.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      438 2024-03-19 16:44:04.000000 arccanet-0.0.5/arccanet.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-19 16:44:04.000000 arccanet-0.0.5/arccanet.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       79 2024-03-19 16:44:04.000000 arccanet-0.0.5/arccanet.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-19 16:44:04.000000 arccanet-0.0.5/arccanet.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-19 16:44:04.213428 arccanet-0.0.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      387 2024-03-19 16:44:03.000000 arccanet-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:00:07.376383 arccanet-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)      231 2024-05-22 19:00:07.375383 arccanet-0.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      437 2024-05-22 19:00:06.000000 arccanet-0.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:00:07.374383 arccanet-0.0.6/arccanet/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/conditionbuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)       54 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3476 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/general.py
+-rw-rw-rw-   0 root         (0) root         (0)      229 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/jwt.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)       45 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/response.py
+-rw-rw-rw-   0 root         (0) root         (0)     3469 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/responsebuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      335 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:00:07.375383 arccanet-0.0.6/arccanet.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      231 2024-05-22 19:00:07.000000 arccanet-0.0.6/arccanet.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-22 19:00:07.000000 arccanet-0.0.6/arccanet.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 19:00:07.000000 arccanet-0.0.6/arccanet.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2024-05-22 19:00:07.000000 arccanet-0.0.6/arccanet.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-22 19:00:07.000000 arccanet-0.0.6/arccanet.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 19:00:07.376383 arccanet-0.0.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      387 2024-05-22 19:00:06.000000 arccanet-0.0.6/setup.py
```

### Comparing `arccanet-0.0.5/arccanet/conditionbuilder.py` & `arccanet-0.0.6/arccanet/conditionbuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     if val is None:
         return ''
     return prepend + field + ' = ' + str(val)
 
 
 def profile_group(p, exclude_holding=True, prepend=''):
     if p is None:
-        return prepend + "h.value != 0" if exclude_holding else ''
-    if p.hierarchy.value == 0 and exclude_holding:
+        return prepend + "h.value > 0" if exclude_holding else ''
+    if p.hierarchy.value <= 0 and exclude_holding:
         return prepend + "false"
     return prepend + "pg.id = " + str(p.id)
 
 
 def uc_status(uc, prepend=''):
     if uc == '' or uc is None:
         return ""
```

### Comparing `arccanet-0.0.5/arccanet/general.py` & `arccanet-0.0.6/arccanet/general.py`

 * *Files identical despite different names*

### Comparing `arccanet-0.0.5/arccanet/responsebuilder.py` & `arccanet-0.0.6/arccanet/responsebuilder.py`

 * *Files identical despite different names*

