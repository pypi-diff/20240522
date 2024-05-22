# Comparing `tmp/funcs_aux-0.2.0.tar.gz` & `tmp/funcs_aux-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcs_aux-0.2.0.tar", last modified: Tue May 21 10:03:17 2024, max compression
+gzip compressed data, was "funcs_aux-0.2.1.tar", last modified: Wed May 22 09:16:21 2024, max compression
```

## Comparing `funcs_aux-0.2.0.tar` & `funcs_aux-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 10:03:17.027619 funcs_aux-0.2.0/
--rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 funcs_aux-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     1883 2024-05-21 10:03:17.027120 funcs_aux-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      990 2024-05-21 10:02:53.000000 funcs_aux-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 10:03:17.019652 funcs_aux-0.2.0/funcs_aux/
--rw-rw-rw-   0        0        0      460 2024-05-21 07:34:52.000000 funcs_aux-0.2.0/funcs_aux/__init__.py
--rw-rw-rw-   0        0        0     1894 2024-03-01 08:49:51.000000 funcs_aux-0.2.0/funcs_aux/arrays.py
--rw-rw-rw-   0        0        0     9034 2024-05-20 09:17:18.000000 funcs_aux-0.2.0/funcs_aux/breeder_objects.py
--rw-rw-rw-   0        0        0     9791 2024-05-21 09:50:09.000000 funcs_aux-0.2.0/funcs_aux/breeder_str.py
--rw-rw-rw-   0        0        0     5211 2024-03-22 14:19:18.000000 funcs_aux-0.2.0/funcs_aux/iterables.py
--rw-rw-rw-   0        0        0     9678 2024-05-17 09:54:30.000000 funcs_aux-0.2.0/funcs_aux/results.py
--rw-rw-rw-   0        0        0     1920 2024-03-01 08:45:13.000000 funcs_aux-0.2.0/funcs_aux/strings.py
-drwxrwxrwx   0        0        0        0 2024-05-21 10:03:17.026076 funcs_aux-0.2.0/funcs_aux.egg-info/
--rw-rw-rw-   0        0        0     1883 2024-05-21 10:03:16.000000 funcs_aux-0.2.0/funcs_aux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-05-21 10:03:16.000000 funcs_aux-0.2.0/funcs_aux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 10:03:16.000000 funcs_aux-0.2.0/funcs_aux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-21 10:03:16.000000 funcs_aux-0.2.0/funcs_aux.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 10:03:17.028480 funcs_aux-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 funcs_aux-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:16:21.257413 funcs_aux-0.2.1/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 funcs_aux-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     1883 2024-05-22 09:16:21.256912 funcs_aux-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2024-05-22 09:15:48.000000 funcs_aux-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 09:16:21.248473 funcs_aux-0.2.1/funcs_aux/
+-rw-rw-rw-   0        0        0     1965 2024-05-22 09:14:12.000000 funcs_aux-0.2.1/funcs_aux/__init__.py
+-rw-rw-rw-   0        0        0     1894 2024-03-01 08:49:51.000000 funcs_aux-0.2.1/funcs_aux/arrays.py
+-rw-rw-rw-   0        0        0     9053 2024-05-21 13:43:03.000000 funcs_aux-0.2.1/funcs_aux/breeder_objects.py
+-rw-rw-rw-   0        0        0     9485 2024-05-22 07:23:49.000000 funcs_aux-0.2.1/funcs_aux/breeder_str.py
+-rw-rw-rw-   0        0        0     5221 2024-05-22 09:14:12.000000 funcs_aux-0.2.1/funcs_aux/iterables.py
+-rw-rw-rw-   0        0        0     9678 2024-05-17 09:54:30.000000 funcs_aux-0.2.1/funcs_aux/results.py
+-rw-rw-rw-   0        0        0     1918 2024-05-22 09:14:12.000000 funcs_aux-0.2.1/funcs_aux/strings.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:16:21.255488 funcs_aux-0.2.1/funcs_aux.egg-info/
+-rw-rw-rw-   0        0        0     1883 2024-05-22 09:16:21.000000 funcs_aux-0.2.1/funcs_aux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-05-22 09:16:21.000000 funcs_aux-0.2.1/funcs_aux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 09:16:21.000000 funcs_aux-0.2.1/funcs_aux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-22 09:16:21.000000 funcs_aux-0.2.1/funcs_aux.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 09:16:21.258426 funcs_aux-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 funcs_aux-0.2.1/setup.py
```

### Comparing `funcs_aux-0.2.0/LICENSE` & `funcs_aux-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.2.0/PKG-INFO` & `funcs_aux-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs_aux
-Version: 0.2.0
+Version: 0.2.1
 Summary: useful funcs in one place
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/funcs_aux
 Keywords: functions,auxiliary,auxiliary funcs,np funcs,collections funcs,strings funcs,result object
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# funcs_aux (v0.2.0)
+# funcs_aux (v0.2.1)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.2.0/README.md` & `funcs_aux-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# funcs_aux (v0.2.0)
+# funcs_aux (v0.2.1)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.2.0/funcs_aux/arrays.py` & `funcs_aux-0.2.1/funcs_aux/arrays.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.2.0/funcs_aux/breeder_objects.py` & `funcs_aux-0.2.1/funcs_aux/breeder_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,16 +76,16 @@
     # instance ---
     INDEX: int | None = None    # index used only in OBJECT INSTANCE
 
     def __init__(self, index: int):
         """
         init only when you need to do access to exact items!
         """
+        self.INDEX = index      # need first!
         super().__init__()
-        self.INDEX = index
         # self.generate__objects()
 
     # -----------------------------------------------------------------------------------------------------------------
     @classmethod
     def generate__objects(cls) -> None:
         """exact and only one method to Gen all objects - dont forget to call it!
         """
```

### Comparing `funcs_aux-0.2.0/funcs_aux/breeder_str.py` & `funcs_aux-0.2.1/funcs_aux/breeder_str.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import *
+from annot_attrs import AnnotsNested
 
 
 # =====================================================================================================================
 class Exx__IndexOverlayed(Exception):
     pass
 
 
@@ -121,15 +122,15 @@
                 else:
                     result += 1
         else:
             raise Exx__ItemNotExists()
 
 
 # =====================================================================================================================
-class BreederStrStack:
+class BreederStrStack(AnnotsNested):
     """
     created specially for applying in Gui tableModels (PyQt5) as header structure
 
     VULNERABILITIES # FIXME:
     ------------------------
     1. if exists same names cause of patterns - it would return always first index!
         class BreederStrStack_Example2(BreederStrStack):
@@ -268,27 +269,14 @@
                 continue
 
             if index - index_prev != 1:
                 msg = f"index [{index-1}]"
                 raise Exx__IndexNotSet(msg)
             index_prev = index
 
-    @classmethod
-    def annotations__get_nested(cls) -> dict[str, Any]:
-        """
-        get all annotations in correct order!
-        """
-        result = {}
-        for cls_i in cls.__mro__:
-            if cls_i == BreederStrStack:
-                break
-
-            result = dict(**cls_i.__annotations__, **result)
-        return result
-
 
 # =====================================================================================================================
 class BreederStrStack_Example(BreederStrStack):
     name0: int = 0
     name1: int = 1
     TAIL: BreederStrSeries = BreederStrSeries(2, 2, "%s")
```

### Comparing `funcs_aux-0.2.0/funcs_aux/results.py` & `funcs_aux-0.2.1/funcs_aux/results.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.2.0/funcs_aux/strings.py` & `funcs_aux-0.2.1/funcs_aux/strings.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 )
 TYPES_ELEMENTARY_COLLECTION: tuple = (
     tuple, list,
     set, dict,
 )
 TYPES_ELEMENTARY: tuple = (*TYPES_ELEMENTARY_SINGLE, *TYPES_ELEMENTARY_COLLECTION,)
 
-TYPE__ELEMENTARY = Union[*TYPES_ELEMENTARY]
+TYPE_ELEMENTARY = Union[*TYPES_ELEMENTARY]
 
 
 # =====================================================================================================================
 class Strings:
     SOURCE: str
 
     def __init__(self, source: Optional[str] = None):
         self.SOURCE = source
 
-    def try_convert_to__elementary(self, source: Optional[Any] = None) -> TYPE__ELEMENTARY:
+    def try_convert_to__elementary(self, source: Optional[Any] = None) -> TYPE_ELEMENTARY:
         """
         by now it works correct only with single elementary values like INT/FLOAT/BOOL/NONE
         for collections it may work but may not work correctly!!! so use it by your own risk and conscious choice!!
         """
         # FIXME: this is not work FULL and CORRECT!!!! need FIX!!!
 
         # INIT source -------------
```

### Comparing `funcs_aux-0.2.0/funcs_aux.egg-info/PKG-INFO` & `funcs_aux-0.2.1/funcs_aux.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs_aux
-Version: 0.2.0
+Version: 0.2.1
 Summary: useful funcs in one place
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/funcs_aux
 Keywords: functions,auxiliary,auxiliary funcs,np funcs,collections funcs,strings funcs,result object
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# funcs_aux (v0.2.0)
+# funcs_aux (v0.2.1)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.2.0/setup.py` & `funcs_aux-0.2.1/setup.py`

 * *Files identical despite different names*

