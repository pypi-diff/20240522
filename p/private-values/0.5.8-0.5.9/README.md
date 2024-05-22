# Comparing `tmp/private_values-0.5.8.tar.gz` & `tmp/private_values-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "private_values-0.5.8.tar", last modified: Thu Jan 25 08:36:20 2024, max compression
+gzip compressed data, was "private_values-0.5.9.tar", last modified: Wed May 22 11:40:32 2024, max compression
```

## Comparing `private_values-0.5.8.tar` & `private_values-0.5.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-01-25 08:36:20.225773 private_values-0.5.8/
--rw-rw-rw-   0        0        0     1082 2023-10-25 07:24:19.000000 private_values-0.5.8/LICENSE
--rw-rw-rw-   0        0        0     5980 2024-01-25 08:36:20.224771 private_values-0.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     5083 2024-01-25 08:35:58.000000 private_values-0.5.8/README.md
-drwxrwxrwx   0        0        0        0 2024-01-25 08:36:20.219773 private_values-0.5.8/private_values/
--rw-rw-rw-   0        0        0      151 2023-12-08 07:20:48.000000 private_values-0.5.8/private_values/__init__.py
--rw-rw-rw-   0        0        0     1395 2024-01-17 14:26:06.000000 private_values-0.5.8/private_values/auto.py
--rw-rw-rw-   0        0        0     6466 2024-01-25 08:35:45.000000 private_values-0.5.8/private_values/base.py
--rw-rw-rw-   0        0        0     3046 2024-01-17 14:25:13.000000 private_values-0.5.8/private_values/csv.py
--rw-rw-rw-   0        0        0      747 2023-12-08 07:20:48.000000 private_values-0.5.8/private_values/derivatives.py
--rw-rw-rw-   0        0        0     1718 2024-01-17 14:19:03.000000 private_values-0.5.8/private_values/env.py
--rw-rw-rw-   0        0        0     1344 2024-01-17 14:19:03.000000 private_values-0.5.8/private_values/ini.py
--rw-rw-rw-   0        0        0     1224 2024-01-17 14:25:13.000000 private_values-0.5.8/private_values/json.py
-drwxrwxrwx   0        0        0        0 2024-01-25 08:36:20.224771 private_values-0.5.8/private_values.egg-info/
--rw-rw-rw-   0        0        0     5980 2024-01-25 08:36:20.000000 private_values-0.5.8/private_values.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2024-01-25 08:36:20.000000 private_values-0.5.8/private_values.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-25 08:36:20.000000 private_values-0.5.8/private_values.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-01-25 08:36:20.000000 private_values-0.5.8/private_values.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-25 08:36:20.225773 private_values-0.5.8/setup.cfg
--rw-rw-rw-   0        0        0     1709 2024-01-15 06:52:12.000000 private_values-0.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:40:32.935791 private_values-0.5.9/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 private_values-0.5.9/LICENSE
+-rw-rw-rw-   0        0        0     5992 2024-05-22 11:40:32.935791 private_values-0.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5095 2024-05-22 11:39:39.000000 private_values-0.5.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 11:40:32.930278 private_values-0.5.9/private_values/
+-rw-rw-rw-   0        0        0     1526 2024-05-22 11:33:02.000000 private_values-0.5.9/private_values/__init__.py
+-rw-rw-rw-   0        0        0     1395 2024-05-22 11:38:38.000000 private_values-0.5.9/private_values/auto.py
+-rw-rw-rw-   0        0        0     6506 2024-05-22 10:47:58.000000 private_values-0.5.9/private_values/base.py
+-rw-rw-rw-   0        0        0     3070 2024-05-22 11:38:38.000000 private_values-0.5.9/private_values/csv.py
+-rw-rw-rw-   0        0        0      785 2024-05-22 11:33:02.000000 private_values-0.5.9/private_values/derivatives.py
+-rw-rw-rw-   0        0        0     1742 2024-05-22 11:38:38.000000 private_values-0.5.9/private_values/env.py
+-rw-rw-rw-   0        0        0     1366 2024-05-22 11:38:38.000000 private_values-0.5.9/private_values/ini.py
+-rw-rw-rw-   0        0        0     1246 2024-05-22 11:38:38.000000 private_values-0.5.9/private_values/json.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:40:32.934788 private_values-0.5.9/private_values.egg-info/
+-rw-rw-rw-   0        0        0     5992 2024-05-22 11:40:32.000000 private_values-0.5.9/private_values.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2024-05-22 11:40:32.000000 private_values-0.5.9/private_values.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 11:40:32.000000 private_values-0.5.9/private_values.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-22 11:40:32.000000 private_values-0.5.9/private_values.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 11:40:32.936788 private_values-0.5.9/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 private_values-0.5.9/setup.py
```

### Comparing `private_values-0.5.8/LICENSE` & `private_values-0.5.9/LICENSE`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 Copyright (c) 2023 Andrei Starichenko
 
+IMPORTANT: SEE ADDITIONAL DEPENDANT LICENSES FROM LIST OF USED PROJECTS FROM REQUIREMENTS.TXT!
+
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
 the following conditions:
```

### Comparing `private_values-0.5.8/PKG-INFO` & `private_values-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: private_values
-Version: 0.5.8
+Version: 0.5.9
 Summary: update values into class attrs from OsEnvironment or Ini/Json File
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/private_values
 Keywords: environs,environment,private,rc,ini,csvjson
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,25 +16,25 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# private_values (v0.5.8)
+# private_values (v0.5.9)
 
 ## DESCRIPTION_SHORT
-Update values into class attrs from osenvironment or ini/json file
+update values into class attrs from OsEnvironment or Ini/Json File
 
 ## DESCRIPTION_LONG
-designed to use private data like username/pwd kept secure in osenvironment or ini/json-file for your several home projects at ones.  
-and not open it in public.  
+Designed to use private data like username/pwd kept secure in OsEnvironment or Ini/Json-File for your several home projects at ones.  
+    And not open it in public.  
 
-**caution:**  
-in requirements for other projects use fixed version! because it might be refactored so you would get exception soon.
+    **CAUTION:**  
+    in requirements for other projects use fixed version! because it might be refactored so you would get exception soon.
 
 
 ## Features
 1. load values to instance attrs from:  
 	- Environment  
 	- IniFile  
 	- JsonFile
```

### Comparing `private_values-0.5.8/README.md` & `private_values-0.5.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# private_values (v0.5.8)
+# private_values (v0.5.9)
 
 ## DESCRIPTION_SHORT
-Update values into class attrs from osenvironment or ini/json file
+update values into class attrs from OsEnvironment or Ini/Json File
 
 ## DESCRIPTION_LONG
-designed to use private data like username/pwd kept secure in osenvironment or ini/json-file for your several home projects at ones.  
-and not open it in public.  
+Designed to use private data like username/pwd kept secure in OsEnvironment or Ini/Json-File for your several home projects at ones.  
+    And not open it in public.  
 
-**caution:**  
-in requirements for other projects use fixed version! because it might be refactored so you would get exception soon.
+    **CAUTION:**  
+    in requirements for other projects use fixed version! because it might be refactored so you would get exception soon.
 
 
 ## Features
 1. load values to instance attrs from:  
 	- Environment  
 	- IniFile  
 	- JsonFile
```

### Comparing `private_values-0.5.8/private_values/auto.py` & `private_values-0.5.9/private_values/auto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from . import *
-
 from typing import *
 
 
 # =====================================================================================================================
 # TODO: add Csv???
 class PrivateAuto(PrivateJson, PrivateIni, PrivateEnv):
     """This class will try all variants in order Json-Ini-Env.
     and take values ONLY from FIRST ONE source with all needed values!
     It will not merge sources!
     """
-    def get_dict(self) -> Union[Type_PvDict, NoReturn]:
+    def get_dict(self) -> Union[TYPE__PV_DICT, NoReturn]:
         annots = self.annots_get_set()
         annots_lower = set(map(str.lower, annots))
 
         for cls in [PrivateAuto, PrivateJson, PrivateIni, PrivateCsv]:
             try:
                 self.FILENAME = super(cls, self).FILENAME
                 self._filepath_apply_new()
```

### Comparing `private_values-0.5.8/private_values/base.py` & `private_values-0.5.9/private_values/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+from typing import *
 import pathlib
 import abc
 
-from annot_attrs import *
+from annot_attrs import AnnotAttrs
 
 
 # =====================================================================================================================
 # TODO: add iter???
 
 
 # =====================================================================================================================
-Type_PvDict = Dict[str, Any]
-Type_Path = Union[str, pathlib.Path]
-Type_Value = Union[str, NoReturn, None]
+TYPE__PV_DICT = dict[str, Any]
+TYPE__PATH = Union[str, pathlib.Path]
+TYPE__VALUE = Union[str, NoReturn, None]
 
 
 # =====================================================================================================================
 class Exx_FileNotExists(Exception):
     """Any final exception when value can't be get.
     """
     pass
@@ -33,28 +34,28 @@
     -----
     if you dont need RAISE when no value get for exact annotated name - just define None!
     """
     DONT_CHECK_VALUES_EXISTS: Optional[bool] = None
 
     SECTION: Optional[str] = None
 
-    DIRPATH: Optional[Type_Path] = pathlib.Path.home()
+    DIRPATH: Optional[TYPE__PATH] = pathlib.Path.home()
     FILENAME: Optional[str] = None
 
     _text: Optional[str] = None     # TODO: need tests!!!
     dict: Dict[str, Any] = None
 
     # -----------------------------------------------------------------------------------------------------------------
     def __init__(
             self,
             _section: Optional[str] = None,
 
-            _dirpath: Type_Path = None,
+            _dirpath: TYPE__PATH = None,
             _filename: str = None,
-            _filepath: Type_Path = None,
+            _filepath: TYPE__PATH = None,
 
             _text: Optional[str] = None,                # instead of file
             _dict: Optional[Dict[str, Any]] = None,     # instead of file
 
             _dont_check_values_exists: Optional[bool] = None
     ):
         super().__init__()
@@ -95,17 +96,17 @@
         else:
             result += f"\ndata=None"
         return result
 
     # -----------------------------------------------------------------------------------------------------------------
     def _filepath_apply_new(
             self,
-            _dirpath: Type_Path = None,
+            _dirpath: TYPE__PATH = None,
             _filename: str = None,
-            _filepath: Type_Path = None
+            _filepath: TYPE__PATH = None
     ) -> Optional[NoReturn]:
         """apply new file destination
         """
         if not _filepath:
             self.DIRPATH = pathlib.Path(_dirpath or self.DIRPATH)
             self.FILENAME = _filename or self.FILENAME
         else:
```

### Comparing `private_values-0.5.8/private_values/csv.py` & `private_values-0.5.9/private_values/csv.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from . import *
+from typing import *
 import re
 
 
 # =====================================================================================================================
 class Exx_SameKeys(Exception):
     """Same keys NOT allowed!
     """
@@ -47,15 +48,15 @@
     SEPARATOR: str = ":"
     SPACE_IN_KEYS: str = "_"
     RAISE_SAME_KEYS: bool = True
     LINE_SKIP__FIRST: Optional[int] = None
     LINE_SKIP__LAST: Optional[int] = None
     LINE_SKIP__REGEXP: Optional[str] = None
 
-    def get_dict(self) -> Union[Type_PvDict, NoReturn]:
+    def get_dict(self) -> Union[TYPE__PV_DICT, NoReturn]:
         result = {}
         lines = self._text.splitlines()[self.LINE_SKIP__FIRST:]
         if self.LINE_SKIP__LAST:
             lines = lines[:-self.LINE_SKIP__LAST]
 
         for line in lines:
             if self.SEPARATOR not in line:
```

### Comparing `private_values-0.5.8/private_values/derivatives.py` & `private_values-0.5.9/private_values/derivatives.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # =====================================================================================================================
+# DONOT apply PrivateBase nesting!
+
 class PrivateAuth:
     """Typical structure for AUTH
 
     :ivar USER: user login name
     :ivar PWD: password
     """
     USER: str
```

### Comparing `private_values-0.5.8/private_values/env.py` & `private_values-0.5.9/private_values/env.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from .base import *
-
+from typing import *
 import os
 
 
 # =====================================================================================================================
 class PrivateEnv(PrivateBase):
     """
     read exact environs from Os Environment
     """
-    def get_dict(self, _prefix: Optional[str] = None) -> Type_PvDict:
+    def get_dict(self, _prefix: Optional[str] = None) -> TYPE__PV_DICT:
         """
         directly using result - mainly it is only for PRINTing and debugging! don't use result!
 
         NOTE: be careful to use result as dict! especially if you have lowercase letters!
 
         REASON:
             import os
@@ -25,15 +25,15 @@
 
             print(os.environ[name_lowercase])   # name_lowercase
             print(os.environ[name_lowercase.upper()])   # name_lowercase
 
             print(dict(os.environ)[name_lowercase])     # KeyError: 'name_lowercase'
         """
         envs_all = os.environ
-        result: Type_PvDict = {}
+        result: TYPE__PV_DICT = {}
 
         # filter ---------------
         for name, value in envs_all.items():
             if not _prefix or (_prefix and name.upper().startswith(_prefix.upper())):
                 result.update({name: value})
 
         # print ---------------
```

### Comparing `private_values-0.5.8/private_values/ini.py` & `private_values-0.5.9/private_values/ini.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from . import *
-
+from typing import *
 from configparser import ConfigParser
 
 
 # =====================================================================================================================
 class PrivateIni(PrivateBase):
     """Get values from Ini file.
     Not recommended using DEFAULT SECTION!
     """
     FILENAME: str = "pv.ini"
 
-    def get_dict(self) -> Union[Type_PvDict, NoReturn]:
+    def get_dict(self) -> Union[TYPE__PV_DICT, NoReturn]:
         ini = ConfigParser()
 
         try:
             ini.read_string(self._text)
         except Exception as exx:
             msg = f"[CRITICAL] incorrect format file!\n{exx!r}"
             print(msg)
```

### Comparing `private_values-0.5.8/private_values/json.py` & `private_values-0.5.9/private_values/json.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from . import *
-
+from typing import *
 import json
 
 
 # =====================================================================================================================
 class PrivateJson(PrivateBase):
     FILENAME: str = "pv.json"
 
-    def get_dict(self) -> Union[Type_PvDict, NoReturn]:
+    def get_dict(self) -> Union[TYPE__PV_DICT, NoReturn]:
         """
         section only in first level!
         """
         try:
             json_data = json.loads(self._text)
         except Exception as exx:
             msg = f"[CRITICAL] incorrect format file!\n{exx!r}"
```

### Comparing `private_values-0.5.8/private_values.egg-info/PKG-INFO` & `private_values-0.5.9/private_values.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: private_values
-Version: 0.5.8
+Version: 0.5.9
 Summary: update values into class attrs from OsEnvironment or Ini/Json File
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/private_values
 Keywords: environs,environment,private,rc,ini,csvjson
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,25 +16,25 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# private_values (v0.5.8)
+# private_values (v0.5.9)
 
 ## DESCRIPTION_SHORT
-Update values into class attrs from osenvironment or ini/json file
+update values into class attrs from OsEnvironment or Ini/Json File
 
 ## DESCRIPTION_LONG
-designed to use private data like username/pwd kept secure in osenvironment or ini/json-file for your several home projects at ones.  
-and not open it in public.  
+Designed to use private data like username/pwd kept secure in OsEnvironment or Ini/Json-File for your several home projects at ones.  
+    And not open it in public.  
 
-**caution:**  
-in requirements for other projects use fixed version! because it might be refactored so you would get exception soon.
+    **CAUTION:**  
+    in requirements for other projects use fixed version! because it might be refactored so you would get exception soon.
 
 
 ## Features
 1. load values to instance attrs from:  
 	- Environment  
 	- IniFile  
 	- JsonFile
```

### Comparing `private_values-0.5.8/setup.py` & `private_values-0.5.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,27 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 from PROJECT import PROJECT
 
 
 # =====================================================================================================================
-with open("README.md", "r") as f:
+# VERSION = (0, 0, 1)   # use find_packages to keep all internal pkgs for pypi
+VERSION = (0, 0, 2)   # fix ability to read russian text in readme
+
+
+# =====================================================================================================================
+with open("README.md", mode="r", encoding="utf8") as f:
     readme = f.read()
 
 
+packages = [PROJECT.NAME_IMPORT, ]
+pkgs_internal = find_packages(where=PROJECT.NAME_IMPORT)
+for name in pkgs_internal:
+    packages.append(f"{PROJECT.NAME_IMPORT}.{name}")
+
+
 # =====================================================================================================================
 setup(
   version=PROJECT.VERSION_STR,
   description=PROJECT.DESCRIPTION_SHORT,
   keywords=PROJECT.KEYWORDS,
   classifiers=[
     # "Topic :: ________________",
@@ -38,14 +49,14 @@
 
   url=PROJECT.AUTHOR_HOMEPAGE,  # HOMEPAGE
   project_urls={
     # "Documentation": f"https://github.com/centroid457/{NAME}/blob/main/GUIDE.md",
     "Source": f"https://github.com/centroid457/{PROJECT.NAME_IMPORT}",
   },
 
-  packages=[PROJECT.NAME_IMPORT, ],
+  packages=packages,
   install_requires=[],
   python_requires=">=3.6"
 )
 
 
 # =====================================================================================================================
```

