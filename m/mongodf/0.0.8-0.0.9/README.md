# Comparing `tmp/mongodf-0.0.8.tar.gz` & `tmp/mongodf-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodf-0.0.8.tar", last modified: Thu Jan 20 16:07:15 2022, max compression
+gzip compressed data, was "mongodf-0.0.9.tar", last modified: Thu Jan 20 17:00:42 2022, max compression
```

## Comparing `mongodf-0.0.8.tar` & `mongodf-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 16:07:15.652630 mongodf-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-01-20 16:07:15.652630 mongodf-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-01-20 16:06:52.000000 mongodf-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 16:07:15.652630 mongodf-0.0.8/mongodf/
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-01-20 16:06:52.000000 mongodf-0.0.8/mongodf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2505 2022-01-20 16:06:52.000000 mongodf-0.0.8/mongodf/column.py
--rw-r--r--   0 runner    (1001) docker     (121)     3593 2022-01-20 16:06:52.000000 mongodf-0.0.8/mongodf/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-01-20 16:06:52.000000 mongodf-0.0.8/mongodf/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     3029 2022-01-20 16:06:52.000000 mongodf-0.0.8/mongodf/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 16:07:15.652630 mongodf-0.0.8/mongodf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-01-20 16:07:15.000000 mongodf-0.0.8/mongodf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-01-20 16:07:15.000000 mongodf-0.0.8/mongodf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-20 16:07:15.000000 mongodf-0.0.8/mongodf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-01-20 16:07:15.000000 mongodf-0.0.8/mongodf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-01-20 16:07:15.000000 mongodf-0.0.8/mongodf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-20 16:07:15.652630 mongodf-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-01-20 16:06:52.000000 mongodf-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 17:00:42.918441 mongodf-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-01-20 17:00:42.918441 mongodf-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      840 2022-01-20 17:00:25.000000 mongodf-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 17:00:42.918441 mongodf-0.0.9/mongodf/
+-rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-01-20 17:00:25.000000 mongodf-0.0.9/mongodf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2738 2022-01-20 17:00:25.000000 mongodf-0.0.9/mongodf/column.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3593 2022-01-20 17:00:25.000000 mongodf-0.0.9/mongodf/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-01-20 17:00:25.000000 mongodf-0.0.9/mongodf/exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3029 2022-01-20 17:00:25.000000 mongodf-0.0.9/mongodf/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 17:00:42.918441 mongodf-0.0.9/mongodf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-01-20 17:00:42.000000 mongodf-0.0.9/mongodf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-01-20 17:00:42.000000 mongodf-0.0.9/mongodf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-20 17:00:42.000000 mongodf-0.0.9/mongodf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-01-20 17:00:42.000000 mongodf-0.0.9/mongodf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-01-20 17:00:42.000000 mongodf-0.0.9/mongodf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-20 17:00:42.918441 mongodf-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      518 2022-01-20 17:00:25.000000 mongodf-0.0.9/setup.py
```

### Comparing `mongodf-0.0.8/PKG-INFO` & `mongodf-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongodf
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/VK/mongodf
 License: MIT
 Keywords: mongoDB pandas dataframe filter
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `mongodf-0.0.8/README.md` & `mongodf-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mongodf-0.0.8/mongodf/__init__.py` & `mongodf-0.0.9/mongodf/__init__.py`

 * *Files identical despite different names*

### Comparing `mongodf-0.0.8/mongodf/column.py` & `mongodf-0.0.9/mongodf/column.py`

 * *Files 9% similar despite different names*

```diff
@@ -65,18 +65,22 @@
                 "_id": None,
                 **{t: {pmap[t]: f"${self._name}"} for t in types}
             }}
         ])
 
         res = list(res)[0]
 
+        if res["median"] is None and "min" in res and res["min"] is not None:
+            res["median"] = res["min"]
+        if res["median"] is None and "max" in res and res["max"] is not None:
+            res["median"] = res["max"]
+
         def flatten(t, el):
             if isinstance(el, list):
                 a = _np.array(el)
-                a = a[_np.isfinite(a)]
+                a = a[_pd.notnull(a)]
                 return getattr(_np, t)(a)
             return el
 
-
         res = {k: flatten(k, v) for k, v in res.items() if k != "_id"}
 
         return _pd.Series(res, name=self._name)
```

### Comparing `mongodf-0.0.8/mongodf/dataframe.py` & `mongodf-0.0.9/mongodf/dataframe.py`

 * *Files identical despite different names*

### Comparing `mongodf-0.0.8/mongodf/filter.py` & `mongodf-0.0.9/mongodf/filter.py`

 * *Files identical despite different names*

### Comparing `mongodf-0.0.8/mongodf.egg-info/PKG-INFO` & `mongodf-0.0.9/mongodf.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongodf
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/VK/mongodf
 License: MIT
 Keywords: mongoDB pandas dataframe filter
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `mongodf-0.0.8/setup.py` & `mongodf-0.0.9/setup.py`

 * *Files identical despite different names*

