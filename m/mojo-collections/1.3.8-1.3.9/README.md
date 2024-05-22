# Comparing `tmp/mojo_collections-1.3.8.tar.gz` & `tmp/mojo_collections-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_collections-1.3.8.tar", max compression
+gzip compressed data, was "mojo_collections-1.3.9.tar", max compression
```

## Comparing `mojo_collections-1.3.8.tar` & `mojo_collections-1.3.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1083 2024-01-26 02:55:06.310687 mojo_collections-1.3.8/LICENSE.txt
--rw-r--r--   0        0        0     1052 2024-01-28 00:27:21.997395 mojo_collections-1.3.8/README.rst
--rw-r--r--   0        0        0      663 2024-04-26 16:48:06.816356 mojo_collections-1.3.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-26 02:55:06.311771 mojo_collections-1.3.8/source/packages/mojo/collections/__init__.py
--rw-r--r--   0        0        0     5971 2024-01-26 02:55:06.311863 mojo_collections-1.3.8/source/packages/mojo/collections/caseinsensitivebytesdict.py
--rw-r--r--   0        0        0     5980 2024-01-26 02:55:06.311946 mojo_collections-1.3.8/source/packages/mojo/collections/caseinsensitivestringdict.py
--rw-r--r--   0        0        0    15470 2024-02-11 20:20:46.484714 mojo_collections-1.3.8/source/packages/mojo/collections/context.py
--rw-r--r--   0        0        0     5203 2024-04-26 16:47:44.206872 mojo_collections-1.3.8/source/packages/mojo/collections/contextpaths.py
--rw-r--r--   0        0        0      565 2024-01-26 02:55:06.312220 mojo_collections-1.3.8/source/packages/mojo/collections/contextuser.py
--rw-r--r--   0        0        0     1128 2024-01-26 02:55:06.312296 mojo_collections-1.3.8/source/packages/mojo/collections/helpers.py
--rw-r--r--   0        0        0     5913 2024-04-05 04:29:52.145043 mojo_collections-1.3.8/source/packages/mojo/collections/mergemap.py
--rw-r--r--   0        0        0     1057 2024-01-26 02:55:06.312475 mojo_collections-1.3.8/source/packages/mojo/collections/wellknown.py
--rw-r--r--   0        0        0     1680 1970-01-01 00:00:00.000000 mojo_collections-1.3.8/setup.py
--rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 mojo_collections-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-26 02:55:06.310687 mojo_collections-1.3.9/LICENSE.txt
+-rw-r--r--   0        0        0     1052 2024-01-28 00:27:21.997395 mojo_collections-1.3.9/README.rst
+-rw-r--r--   0        0        0      663 2024-05-05 23:55:46.501288 mojo_collections-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-26 02:55:06.311771 mojo_collections-1.3.9/source/packages/mojo/collections/__init__.py
+-rw-r--r--   0        0        0     5795 2024-05-02 02:56:25.269525 mojo_collections-1.3.9/source/packages/mojo/collections/caseinsensitivebytesdict.py
+-rw-r--r--   0        0        0     5804 2024-05-02 02:56:32.397558 mojo_collections-1.3.9/source/packages/mojo/collections/caseinsensitivestringdict.py
+-rw-r--r--   0        0        0    15293 2024-05-02 02:56:42.340247 mojo_collections-1.3.9/source/packages/mojo/collections/context.py
+-rw-r--r--   0        0        0     5298 2024-05-02 02:56:58.613454 mojo_collections-1.3.9/source/packages/mojo/collections/contextpaths.py
+-rw-r--r--   0        0        0      660 2024-05-02 02:57:06.014793 mojo_collections-1.3.9/source/packages/mojo/collections/contextuser.py
+-rw-r--r--   0        0        0      951 2024-05-02 02:57:14.914571 mojo_collections-1.3.9/source/packages/mojo/collections/helpers.py
+-rw-r--r--   0        0        0     5701 2024-05-05 23:48:36.594973 mojo_collections-1.3.9/source/packages/mojo/collections/mergemap.py
+-rw-r--r--   0        0        0     1153 2024-05-02 02:57:43.255068 mojo_collections-1.3.9/source/packages/mojo/collections/wellknown.py
+-rw-r--r--   0        0        0     1680 1970-01-01 00:00:00.000000 mojo_collections-1.3.9/setup.py
+-rw-r--r--   0        0        0     1637 1970-01-01 00:00:00.000000 mojo_collections-1.3.9/PKG-INFO
```

### Comparing `mojo_collections-1.3.8/LICENSE.txt` & `mojo_collections-1.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_collections-1.3.8/README.rst` & `mojo_collections-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `mojo_collections-1.3.8/pyproject.toml` & `mojo_collections-1.3.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "mojo-collections"
 description = "Mojo Collections Package"
-version = "1.3.8"
+version = "1.3.9"
 authors = []
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
 ]
 keywords = [
     "python"
 ]
 packages = [{include="mojo", from="source/packages"}]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.9,<4.0"
 
 [tool.poetry.group.dev.dependencies]
 myst-parser = "^0.18.1"
 sphinx = ">=1.6,<6"
 sphinx-rtd-theme = "^1.1.1"
 
 [tool.poetry.group.dbio.dependencies]
```

### Comparing `mojo_collections-1.3.8/source/packages/mojo/collections/caseinsensitivebytesdict.py` & `mojo_collections-1.3.9/source/packages/mojo/collections/caseinsensitivebytesdict.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,15 @@
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
 
 from typing import Any
 
 class CaseInsensitiveBytesDict(dict):
     """
         The :class:`CaseInsensitiveBytesDict` is a dictionary that can store and
         recover values associated with a text based key in a case insensative
```

### Comparing `mojo_collections-1.3.8/source/packages/mojo/collections/caseinsensitivestringdict.py` & `mojo_collections-1.3.9/source/packages/mojo/collections/caseinsensitivestringdict.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,19 +6,15 @@
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
 
 from typing import Any
 
 
 class CaseInsensitiveStringDict(dict):
     """
         The :class:`CaseInsensitiveStringDict` is a dictionary that can store and
```

### Comparing `mojo_collections-1.3.8/source/packages/mojo/collections/context.py` & `mojo_collections-1.3.9/source/packages/mojo/collections/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,14 @@
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
 
 
 from typing import Any, List, Optional
 
 import re
 
 from collections import ChainMap
```

### Comparing `mojo_collections-1.3.8/source/packages/mojo/collections/contextpaths.py` & `mojo_collections-1.3.9/source/packages/mojo/collections/contextpaths.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,18 @@
     :platform: Darwin, Linux, Unix, Windows
     :synopsis: Module that contains the :class:`ContextPaths` enumeration which is an enumeration
                of wellknown context paths.
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
+__author__ = "Myron Walker"
+__copyright__ = "Copyright 2023, Myron W Walker"
+__credits__ = []
+
 from enum import Enum
 
 class ContextPaths(str, Enum):
 
     # ========================== environment paths ==============================
     BEHAVIORS_LOG_CONFIGURATION = "/environment/behaviors/log-configuration-declarations"
```

### Comparing `mojo_collections-1.3.8/source/packages/mojo/collections/helpers.py` & `mojo_collections-1.3.9/source/packages/mojo/collections/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,19 +5,14 @@
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
 
 
 from typing import Any
 
 
 def insert_into_ordered_list_ascending(ordered_list: list, item: Any):
     """
```

### Comparing `mojo_collections-1.3.8/source/packages/mojo/collections/mergemap.py` & `mojo_collections-1.3.9/source/packages/mojo/collections/mergemap.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,19 +7,15 @@
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
 
 from typing import Iterable, List, Optional, MutableMapping
 
 import json
 
 import reprlib
 
@@ -107,64 +103,64 @@
         if kfound is not None:
             raise KeyError(f'Key not found in the first mapping: {key!r}')
 
         return
 
     def __getitem__(self, key: str):
 
-        merge_val = None
+        rtnval = None
 
-        for mapping in self.maps:
-            if key in mapping:
-                nm = mapping[key]          # can't use 'key in mapping' with defaultdict
-                if merge_val is None:
-                    if isinstance(nm, dict):
-                        merge_val = MergeMap(nm)
-                    else:
-                        merge_val = [nm]
-                elif isinstance(merge_val, list):
-                    merge_val.append(nm)
-                else:
-                    merge_val.maps.append(nm)
+        candidates = []
 
-        if merge_val is None:
-            self.__missing__(key)  # support subclasses that define __missing__
+        for nxtmap in self.maps:
+            if key in nxtmap:
+                mval = nxtmap[key]
+                candidates.append(mval)
+
+        if len(candidates) == 0:
+            self.__missing__(key)
+        elif len(candidates) == 1:
+            rtnval = candidates[0]
+        else:
+
+            # Check to see if the mapping values at this level are the same type and can be merged
+            common_type = type(candidates[0])
+
+            if common_type == list or common_type == tuple:
+                has_common_type = True
+
+                for nxtitem in candidates:
+                    nxttype = type(nxtitem)
+                    if nxttype != common_type:
+                        has_common_type = False
+                        break
+
+                if has_common_type:
+                    # If we made it here, we can merge
+                    cmplist = []
+                    merged_list = []
+                    for nxtcand in candidates:
+                        for nxtval in nxtcand:
+                            cmpval = nxtval
+                            if isinstance(cmpval, dict):
+                                cmpval = json.dumps(nxtval, sort_keys=True)
+                            elif isinstance(cmpval, list) or isinstance(nxtval, tuple):
+                                cmpval = json.dumps(cmpval.sort())
+                            
+                            if cmpval not in cmplist:
+                                cmplist.append(cmpval)
+                                merged_list.append(nxtval)
 
-        if isinstance(merge_val, list):
-            all_lists = True
-            for nxtval in merge_val:
-                if not isinstance(nxtval, list):
-                    all_lists = False
-                    break
-
-            if all_lists and len(merge_val) > 1:
-                merged_compare = []
-                merged_lists = []
-
-                for nxtlist in merge_val:
-                    for nxtitem in nxtlist:
-                        nxtcmp = None
-
-                        if isinstance(nxtitem, dict):
-                            nxtcmp = json.dumps(nxtitem, sort_keys=True)
-                        elif isinstance(nxtitem, list):
-                            nxtitem.sort()
-                            nxtcmp = json.dumps(nxtitem, sort_keys=True)
-                        else:
-                            nxtcmp = nxtitem
-
-                        if nxtcmp not in merged_compare:
-                            merged_compare.append(nxtcmp)
-                            merged_lists.append(nxtitem)
-                
-                merge_val = merged_lists
+                    rtnval = merged_list
+                else:
+                    rtnval = candidates[0]
             else:
-                merge_val = merge_val[0]
+                rtnval = candidates[0]
 
-        return merge_val         
+        return rtnval         
 
     def __iter__(self):
         mks = self.keys()
         return iter(mks)
 
     def __len__(self):
         """
```

### Comparing `mojo_collections-1.3.8/source/packages/mojo/collections/wellknown.py` & `mojo_collections-1.3.9/source/packages/mojo/collections/wellknown.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 .. module:: wellknown
     :platform: Darwin, Linux, Unix, Windows
     :synopsis: Module that contains the :class:`Context` singleton instance and factory.
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
+__author__ = "Myron Walker"
+__copyright__ = "Copyright 2023, Myron W Walker"
+__credits__ = []
+
+
 from threading import RLock
 
 from mojo.collections.context import Context
 
 CONTEXT_SINGLETON = None
 
 SINGLETON_LOCK = RLock()
```

### Comparing `mojo_collections-1.3.8/setup.py` & `mojo_collections-1.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 ['mojo', 'mojo.collections']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'mojo-collections',
-    'version': '1.3.8',
+    'version': '1.3.9',
     'description': 'Mojo Collections Package',
     'long_description': "===================================\nAutomation Mojo Collections Package\n===================================\nA package that contains specialized collections used for automation and configuration.\n\n===========================\nFeatures of this Repository\n===========================\n* Machine Setup\n* Virtual Environment Setup (Poetry)\n* PyPi Publishing\n* Sphinx Documentation\n\n=================\nCode Organization\n=================\n* .vscode - Common tasks\n* development - This is where the runtime environment scripts are located\n* repository-setup - Scripts for homing your repository and to your checkout and machine setup\n* userguide - Where you put your user guide\n* source/packages - Put your root folder here 'source/packages/(root-module-folder)'\n* source/sphinx - This is the Sphinx documentation folder\n* workspaces - This is where you add VSCode workspaces templates and where workspaces show up when homed.\n\n==========\nReferences\n==========\n\n- `User Guide <userguide/userguide.rst>`\n- `Coding Standards <userguide/10-00-coding-standards.rst>`\n",
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `mojo_collections-1.3.8/PKG-INFO` & `mojo_collections-1.3.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: mojo-collections
-Version: 1.3.8
+Version: 1.3.9
 Summary: Mojo Collections Package
 License: LICENSE.txt
 Keywords: python
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
 
 ===================================
```

