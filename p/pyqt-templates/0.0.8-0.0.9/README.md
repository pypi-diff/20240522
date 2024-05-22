# Comparing `tmp/pyqt_templates-0.0.8.tar.gz` & `tmp/pyqt_templates-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt_templates-0.0.8.tar", last modified: Fri Mar 29 12:58:39 2024, max compression
+gzip compressed data, was "pyqt_templates-0.0.9.tar", last modified: Tue May 21 10:13:19 2024, max compression
```

## Comparing `pyqt_templates-0.0.8.tar` & `pyqt_templates-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 12:58:39.242815 pyqt_templates-0.0.8/
--rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 pyqt_templates-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     4854 2024-03-29 12:58:39.242815 pyqt_templates-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3875 2024-03-29 12:56:47.000000 pyqt_templates-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-29 12:58:39.234821 pyqt_templates-0.0.8/pyqt_templates/
--rw-rw-rw-   0        0        0       63 2024-01-16 14:12:52.000000 pyqt_templates-0.0.8/pyqt_templates/__init__.py
--rw-rw-rw-   0        0        0     5645 2023-12-28 07:04:45.000000 pyqt_templates-0.0.8/pyqt_templates/from_t8.py
--rw-rw-rw-   0        0        0    17796 2024-02-07 11:29:07.000000 pyqt_templates-0.0.8/pyqt_templates/gui.py
--rw-rw-rw-   0        0        0     1213 2024-01-10 11:21:08.000000 pyqt_templates-0.0.8/pyqt_templates/signals.py
--rw-rw-rw-   0        0        0     3209 2024-01-16 14:18:43.000000 pyqt_templates-0.0.8/pyqt_templates/th.py
--rw-rw-rw-   0        0        0    14835 2024-03-29 12:45:17.000000 pyqt_templates-0.0.8/pyqt_templates/tm.py
--rw-rw-rw-   0        0        0      969 2024-01-16 13:12:55.000000 pyqt_templates-0.0.8/pyqt_templates/zero_stuff.py
-drwxrwxrwx   0        0        0        0 2024-03-29 12:58:39.242398 pyqt_templates-0.0.8/pyqt_templates.egg-info/
--rw-rw-rw-   0        0        0     4854 2024-03-29 12:58:39.000000 pyqt_templates-0.0.8/pyqt_templates.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2024-03-29 12:58:39.000000 pyqt_templates-0.0.8/pyqt_templates.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 12:58:39.000000 pyqt_templates-0.0.8/pyqt_templates.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-03-29 12:58:39.000000 pyqt_templates-0.0.8/pyqt_templates.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-29 12:58:39.243847 pyqt_templates-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 pyqt_templates-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 10:13:19.891057 pyqt_templates-0.0.9/
+-rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 pyqt_templates-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     4854 2024-05-21 10:13:19.891057 pyqt_templates-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3875 2024-05-21 10:12:27.000000 pyqt_templates-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 10:13:19.875545 pyqt_templates-0.0.9/pyqt_templates/
+-rw-rw-rw-   0        0        0       63 2024-01-16 14:12:52.000000 pyqt_templates-0.0.9/pyqt_templates/__init__.py
+-rw-rw-rw-   0        0        0     5645 2023-12-28 07:04:45.000000 pyqt_templates-0.0.9/pyqt_templates/from_t8.py
+-rw-rw-rw-   0        0        0    17796 2024-02-07 11:29:07.000000 pyqt_templates-0.0.9/pyqt_templates/gui.py
+-rw-rw-rw-   0        0        0     1213 2024-01-10 11:21:08.000000 pyqt_templates-0.0.9/pyqt_templates/signals.py
+-rw-rw-rw-   0        0        0     3209 2024-01-16 14:18:43.000000 pyqt_templates-0.0.9/pyqt_templates/th.py
+-rw-rw-rw-   0        0        0    14840 2024-05-21 10:12:10.000000 pyqt_templates-0.0.9/pyqt_templates/tm.py
+-rw-rw-rw-   0        0        0      969 2024-01-16 13:12:55.000000 pyqt_templates-0.0.9/pyqt_templates/zero_stuff.py
+drwxrwxrwx   0        0        0        0 2024-05-21 10:13:19.890056 pyqt_templates-0.0.9/pyqt_templates.egg-info/
+-rw-rw-rw-   0        0        0     4854 2024-05-21 10:13:19.000000 pyqt_templates-0.0.9/pyqt_templates.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2024-05-21 10:13:19.000000 pyqt_templates-0.0.9/pyqt_templates.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 10:13:19.000000 pyqt_templates-0.0.9/pyqt_templates.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-21 10:13:19.000000 pyqt_templates-0.0.9/pyqt_templates.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 10:13:19.892465 pyqt_templates-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 pyqt_templates-0.0.9/setup.py
```

### Comparing `pyqt_templates-0.0.8/LICENSE` & `pyqt_templates-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqt_templates-0.0.8/PKG-INFO` & `pyqt_templates-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqt_templates
-Version: 0.0.8
+Version: 0.0.9
 Summary: pyqt help examples and some other useful objects (overloaded pyqt classes)
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/pyqt_templates
 Keywords: pyqt,pyqt templates,pyqt guide,pyqt usage,pyqt examples,pyqt usage examples,pyqt help,pyqt help examples,pyqt signals
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# pyqt_templates (v0.0.8)
+# pyqt_templates (v0.0.9)
 
 ## DESCRIPTION_SHORT
 pyqt help examples and some other useful objects (overloaded pyqt classes)
 
 ## DESCRIPTION_LONG
 Designed for ...
```

### Comparing `pyqt_templates-0.0.8/README.md` & `pyqt_templates-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pyqt_templates (v0.0.8)
+# pyqt_templates (v0.0.9)
 
 ## DESCRIPTION_SHORT
 pyqt help examples and some other useful objects (overloaded pyqt classes)
 
 ## DESCRIPTION_LONG
 Designed for ...
```

### Comparing `pyqt_templates-0.0.8/pyqt_templates/from_t8.py` & `pyqt_templates-0.0.9/pyqt_templates/from_t8.py`

 * *Files identical despite different names*

### Comparing `pyqt_templates-0.0.8/pyqt_templates/gui.py` & `pyqt_templates-0.0.9/pyqt_templates/gui.py`

 * *Files identical despite different names*

### Comparing `pyqt_templates-0.0.8/pyqt_templates/signals.py` & `pyqt_templates-0.0.9/pyqt_templates/signals.py`

 * *Files identical despite different names*

### Comparing `pyqt_templates-0.0.8/pyqt_templates/th.py` & `pyqt_templates-0.0.9/pyqt_templates/th.py`

 * *Files identical despite different names*

### Comparing `pyqt_templates-0.0.8/pyqt_templates/tm.py` & `pyqt_templates-0.0.9/pyqt_templates/tm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import *
 
 from PyQt5.QtCore import *
 from PyQt5.QtGui import *
 from PyQt5.QtWidgets import *
 
-from funcs_aux import NamesIndexed_Base, NamesIndexed_Templated
+from funcs_aux import BreederStrSeries, BreederStrStack
 
 from .zero_stuff import Data_
 
 
 # =====================================================================================================================
-class Headers(NamesIndexed_Base):
-    NAME = 0
-    BATCH = NamesIndexed_Templated(1, 4)
+class Headers(BreederStrStack):
+    NAME: int = 0
+    BATCH: BreederStrSeries = BreederStrSeries(1, 4)
 
 
 # =====================================================================================================================
 class TableModelTemplate(QAbstractTableModel):
     DATA: Data_
-    HEADERS: NamesIndexed_Base = Headers()
+    HEADERS: BreederStrStack = Headers()
 
     # METHODS USER ----------------------------------------------------------------------------------------------------
     def __init__(self, data: Optional[Any] = None):
         super().__init__(parent=None)
         self.DATA = data
 
     def _data_reread(self) -> None:
```

### Comparing `pyqt_templates-0.0.8/pyqt_templates/zero_stuff.py` & `pyqt_templates-0.0.9/pyqt_templates/zero_stuff.py`

 * *Files identical despite different names*

### Comparing `pyqt_templates-0.0.8/pyqt_templates.egg-info/PKG-INFO` & `pyqt_templates-0.0.9/pyqt_templates.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqt_templates
-Version: 0.0.8
+Version: 0.0.9
 Summary: pyqt help examples and some other useful objects (overloaded pyqt classes)
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/pyqt_templates
 Keywords: pyqt,pyqt templates,pyqt guide,pyqt usage,pyqt examples,pyqt usage examples,pyqt help,pyqt help examples,pyqt signals
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# pyqt_templates (v0.0.8)
+# pyqt_templates (v0.0.9)
 
 ## DESCRIPTION_SHORT
 pyqt help examples and some other useful objects (overloaded pyqt classes)
 
 ## DESCRIPTION_LONG
 Designed for ...
```

### Comparing `pyqt_templates-0.0.8/setup.py` & `pyqt_templates-0.0.9/setup.py`

 * *Files identical despite different names*

