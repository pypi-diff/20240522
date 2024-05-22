# Comparing `tmp/testplans-0.3.2.tar.gz` & `tmp/testplans-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testplans-0.3.2.tar", last modified: Tue May 21 14:26:58 2024, max compression
+gzip compressed data, was "testplans-0.3.3.tar", last modified: Wed May 22 15:06:32 2024, max compression
```

## Comparing `testplans-0.3.2.tar` & `testplans-0.3.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 14:26:58.214276 testplans-0.3.2/
--rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 testplans-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     5494 2024-05-21 14:26:58.213277 testplans-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     4584 2024-05-21 14:26:20.000000 testplans-0.3.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-21 14:26:58.214276 testplans-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 testplans-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:26:58.206926 testplans-0.3.2/testplans/
--rw-rw-rw-   0        0        0      105 2024-02-01 12:13:36.000000 testplans-0.3.2/testplans/__init__.py
--rw-rw-rw-   0        0        0      776 2024-03-15 14:57:12.000000 testplans-0.3.2/testplans/_results.py
--rw-rw-rw-   0        0        0     3974 2024-05-08 07:37:04.000000 testplans-0.3.2/testplans/api.py
--rw-rw-rw-   0        0        0     4061 2024-05-21 12:55:18.000000 testplans-0.3.2/testplans/devices.py
--rw-rw-rw-   0        0        0     6659 2024-05-21 13:55:47.000000 testplans-0.3.2/testplans/gui.py
--rw-rw-rw-   0        0        0    12440 2024-05-21 12:55:18.000000 testplans-0.3.2/testplans/main.py
--rw-rw-rw-   0        0        0     1786 2024-05-13 13:45:51.000000 testplans-0.3.2/testplans/models.py
--rw-rw-rw-   0        0        0    13900 2024-05-21 14:21:43.000000 testplans-0.3.2/testplans/tc.py
--rw-rw-rw-   0        0        0    10008 2024-05-21 13:55:47.000000 testplans-0.3.2/testplans/tm.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:26:58.213277 testplans-0.3.2/testplans.egg-info/
--rw-rw-rw-   0        0        0     5494 2024-05-21 14:26:58.000000 testplans-0.3.2/testplans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-05-21 14:26:58.000000 testplans-0.3.2/testplans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 14:26:58.000000 testplans-0.3.2/testplans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-21 14:26:58.000000 testplans-0.3.2/testplans.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 15:06:32.846116 testplans-0.3.3/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 testplans-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     5494 2024-05-22 15:06:32.845616 testplans-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4584 2024-05-22 15:05:59.000000 testplans-0.3.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 15:06:32.847657 testplans-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 testplans-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 15:06:32.833168 testplans-0.3.3/testplans/
+-rw-rw-rw-   0        0        0     1657 2024-05-22 15:02:55.000000 testplans-0.3.3/testplans/__init__.py
+-rw-rw-rw-   0        0        0      776 2024-03-15 14:57:12.000000 testplans-0.3.3/testplans/_results.py
+-rw-rw-rw-   0        0        0     4000 2024-05-22 13:30:32.000000 testplans-0.3.3/testplans/api.py
+-rw-rw-rw-   0        0        0     4063 2024-05-22 14:48:19.000000 testplans-0.3.3/testplans/devices.py
+-rw-rw-rw-   0        0        0     6703 2024-05-22 14:56:01.000000 testplans-0.3.3/testplans/gui.py
+-rw-rw-rw-   0        0        0    12334 2024-05-22 14:48:19.000000 testplans-0.3.3/testplans/main.py
+-rw-rw-rw-   0        0        0     1786 2024-05-13 13:45:51.000000 testplans-0.3.3/testplans/models.py
+-rw-rw-rw-   0        0        0    13859 2024-05-22 14:56:01.000000 testplans-0.3.3/testplans/tc.py
+-rw-rw-rw-   0        0        0     9972 2024-05-22 14:48:19.000000 testplans-0.3.3/testplans/tm.py
+drwxrwxrwx   0        0        0        0 2024-05-22 15:06:32.844309 testplans-0.3.3/testplans.egg-info/
+-rw-rw-rw-   0        0        0     5494 2024-05-22 15:06:32.000000 testplans-0.3.3/testplans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-05-22 15:06:32.000000 testplans-0.3.3/testplans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 15:06:32.000000 testplans-0.3.3/testplans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-22 15:06:32.000000 testplans-0.3.3/testplans.egg-info/top_level.txt
```

### Comparing `testplans-0.3.2/LICENSE` & `testplans-0.3.3/LICENSE`

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

### Comparing `testplans-0.3.2/PKG-INFO` & `testplans-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testplans
-Version: 0.3.2
+Version: 0.3.3
 Summary: simple testplan framework for several DUTs
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/testplans
 Keywords: testplan,testplan structure framework,testplan gui,testplan multy dut,testplan several dut
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# testplans (v0.3.2)
+# testplans (v0.3.3)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```

### Comparing `testplans-0.3.2/README.md` & `testplans-0.3.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# testplans (v0.3.2)
+# testplans (v0.3.3)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```

### Comparing `testplans-0.3.2/setup.py` & `testplans-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `testplans-0.3.2/testplans/_results.py` & `testplans-0.3.3/testplans/_results.py`

 * *Files identical despite different names*

### Comparing `testplans-0.3.2/testplans/api.py` & `testplans-0.3.3/testplans/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import pathlib
 from typing import *
 from object_info import ObjectInfo
 
-from server_templates import ServerAiohttpBase, decorator__log_request_response, web
 from server_templates import *
+from aiohttp import web
+from fastapi import FastAPI, Response
+from fastapi.responses import RedirectResponse
 
 from .models import *
 
 
 # =====================================================================================================================
 class TpApi_Aiohttp(ServerAiohttpBase):
     async def response_get_html__(self, request) -> web.Response:
```

### Comparing `testplans-0.3.2/testplans/devices.py` & `testplans-0.3.3/testplans/devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import *
 import uuid
 from enum import Enum, auto
 
+from funcs_aux import BreederObjectList
+
 from .tc import TestCaseBase
 from .models import *
-from funcs_aux import BreederObjectList
 
 
 # =====================================================================================================================
 class DeviceBase:
     # AUX -----------------------------------
     conn: Any = None
     INDEX: int = None
```

### Comparing `testplans-0.3.2/testplans/gui.py` & `testplans-0.3.3/testplans/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-# from . import *
-from .tc import TestCaseBase
-# from .tp import TpMultyDutBase
-from .tm import TpTableModel
+from typing import *
 
-import time
+from PyQt5.QtCore import *
+from PyQt5.QtGui import *
+from PyQt5.QtWidgets import *
 
 from pyqt_templates import *
 
+from .tc import TestCaseBase
+from .tm import TpTableModel
+
 
 # =====================================================================================================================
 class TpGuiBase(Gui):
     # OVERWRITTEN -----------------------------------
     START = False
 
     TITLE = "[TestPlan] Title"
```

### Comparing `testplans-0.3.2/testplans/main.py` & `testplans-0.3.3/testplans/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,32 +5,30 @@
 
 
 # =====================================================================================================================
 # from . import *
 from .tc import TestCaseBase
 from .devices import DutBase, DeviceBase, DevicesBreeder_WithDut, DevicesBreeder_Example
 from .gui import TpGuiBase
-from .api import TpApi_Aiohttp, TpApi_FastApi
+from .api import TpApi_FastApi
 from .models import *
 
 from typing import *
 import json
 from pathlib import Path
-from PyQt5.QtCore import QThread
+from PyQt5.QtCore import QThread, pyqtSignal
 from importlib import import_module
-import asyncio
 from pydantic import BaseModel
 
 from pyqt_templates import *
-from server_templates import ServerAiohttpBase, Client_RequestItem, Client_RequestsStack, ServerFastApi_Thread
+from logger_aux import *
+from server_templates import *
 from object_info import ObjectInfo
 from private_values import PrivateJson
 
-from logger_aux import Logger
-
 
 # =====================================================================================================================
 class Exx__TcsPathNotExists(Exception):
     pass
 
 
 class Exx__TcItemNotFound(Exception):
```

### Comparing `testplans-0.3.2/testplans/models.py` & `testplans-0.3.3/testplans/models.py`

 * *Files identical despite different names*

### Comparing `testplans-0.3.2/testplans/tc.py` & `testplans-0.3.3/testplans/tc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import pathlib
 from typing import *
 import json
-from enum import Enum, auto
-from PyQt5.QtCore import QThread
+import time
+from PyQt5.QtCore import QThread, pyqtSignal
 
 from pyqt_templates import *
 from private_values import PrivateJson
 
-# from .devices import DevicesBreeder
-from .models import *
-
 from logger_aux import Logger
 from funcs_aux import ResultExpect_Base
 
+from .models import *
+
 
 # =====================================================================================================================
 TYPE__RESULT = Union[None, bool, ResultExpect_Base]
 
 
 # =====================================================================================================================
 class _TestCaseBase0(Logger):
@@ -324,15 +323,15 @@
 
     @classmethod
     def teardown__cls__wrapped(cls) -> TYPE__RESULT:
         return True
 
 
 # =====================================================================================================================
-class Info(_TestCaseBase):
+class _Info(_TestCaseBase):
     """
     separated class for gen results/info by models!
     """
     # =================================================================================================================
     def info_pretty(self) -> str:
         # fixme: ref from info_get
         result = ""
@@ -395,13 +394,13 @@
     def results__get_all(cls) -> List[Dict[str, Any]]:
         results = []
         for tc_inst in cls.TCS__LIST:
             results.append(tc_inst.get__results().dict())
         return results
 
 
-class TestCaseBase(Info):
+class TestCaseBase(_Info):
     """
     """
 
 
 # =====================================================================================================================
```

### Comparing `testplans-0.3.2/testplans/tm.py` & `testplans-0.3.3/testplans/tm.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 from PyQt5.QtCore import *
 from PyQt5.QtGui import *
 
 from pyqt_templates import TableModelTemplate
 from funcs_aux import BreederStrSeries, BreederStrStack, ResultExpect_Base
 
-# from .tp import TpMultyDutBase
-
 
 # =====================================================================================================================
 class TpTableModel(TableModelTemplate):
     DATA: "TpMultyDutBase"
     HEADERS: "Headers"
 
     # AUX -------------------------------------------
```

### Comparing `testplans-0.3.2/testplans.egg-info/PKG-INFO` & `testplans-0.3.3/testplans.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testplans
-Version: 0.3.2
+Version: 0.3.3
 Summary: simple testplan framework for several DUTs
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/testplans
 Keywords: testplan,testplan structure framework,testplan gui,testplan multy dut,testplan several dut
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# testplans (v0.3.2)
+# testplans (v0.3.3)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```

