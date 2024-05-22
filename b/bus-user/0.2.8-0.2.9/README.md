# Comparing `tmp/bus_user-0.2.8.tar.gz` & `tmp/bus_user-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bus_user-0.2.8.tar", last modified: Tue Mar 19 08:32:39 2024, max compression
+gzip compressed data, was "bus_user-0.2.9.tar", last modified: Tue Mar 19 09:20:17 2024, max compression
```

## Comparing `bus_user-0.2.8.tar` & `bus_user-0.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 08:32:39.970240 bus_user-0.2.8/
--rw-rw-rw-   0        0        0     1082 2023-12-11 08:31:15.000000 bus_user-0.2.8/LICENSE
--rw-rw-rw-   0        0        0     4094 2024-03-19 08:32:39.970240 bus_user-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     3129 2024-03-19 08:28:44.000000 bus_user-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-19 08:32:39.963385 bus_user-0.2.8/bus_user/
--rw-rw-rw-   0        0        0      301 2024-03-19 06:40:12.000000 bus_user-0.2.8/bus_user/__init__.py
--rw-rw-rw-   0        0        0     3366 2023-12-14 12:44:59.000000 bus_user-0.2.8/bus_user/history.py
--rw-rw-rw-   0        0        0     3759 2024-01-31 08:51:20.000000 bus_user-0.2.8/bus_user/i2c_client.py
--rw-rw-rw-   0        0        0    35212 2024-03-19 08:32:12.000000 bus_user-0.2.8/bus_user/serial_client.py
--rw-rw-rw-   0        0        0      697 2024-03-19 06:40:12.000000 bus_user-0.2.8/bus_user/serial_derivatives.py
--rw-rw-rw-   0        0        0    23517 2024-03-19 07:22:28.000000 bus_user-0.2.8/bus_user/serial_server.py
-drwxrwxrwx   0        0        0        0 2024-03-19 08:32:39.969242 bus_user-0.2.8/bus_user.egg-info/
--rw-rw-rw-   0        0        0     4094 2024-03-19 08:32:39.000000 bus_user-0.2.8/bus_user.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2024-03-19 08:32:39.000000 bus_user-0.2.8/bus_user.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 08:32:39.000000 bus_user-0.2.8/bus_user.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-19 08:32:39.000000 bus_user-0.2.8/bus_user.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-19 08:32:39.971241 bus_user-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 bus_user-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-19 09:20:17.435155 bus_user-0.2.9/
+-rw-rw-rw-   0        0        0     1082 2023-12-11 08:31:15.000000 bus_user-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0     4094 2024-03-19 09:20:17.434563 bus_user-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3129 2024-03-19 08:55:33.000000 bus_user-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2024-03-19 09:20:17.423863 bus_user-0.2.9/bus_user/
+-rw-rw-rw-   0        0        0      301 2024-03-19 06:40:12.000000 bus_user-0.2.9/bus_user/__init__.py
+-rw-rw-rw-   0        0        0     3366 2023-12-14 12:44:59.000000 bus_user-0.2.9/bus_user/history.py
+-rw-rw-rw-   0        0        0     3759 2024-01-31 08:51:20.000000 bus_user-0.2.9/bus_user/i2c_client.py
+-rw-rw-rw-   0        0        0    35352 2024-03-19 09:17:30.000000 bus_user-0.2.9/bus_user/serial_client.py
+-rw-rw-rw-   0        0        0      697 2024-03-19 06:40:12.000000 bus_user-0.2.9/bus_user/serial_derivatives.py
+-rw-rw-rw-   0        0        0    23919 2024-03-19 09:18:31.000000 bus_user-0.2.9/bus_user/serial_server.py
+drwxrwxrwx   0        0        0        0 2024-03-19 09:20:17.432957 bus_user-0.2.9/bus_user.egg-info/
+-rw-rw-rw-   0        0        0     4094 2024-03-19 09:20:17.000000 bus_user-0.2.9/bus_user.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2024-03-19 09:20:17.000000 bus_user-0.2.9/bus_user.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-19 09:20:17.000000 bus_user-0.2.9/bus_user.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-03-19 09:20:17.000000 bus_user-0.2.9/bus_user.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-03-19 09:20:17.436686 bus_user-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 bus_user-0.2.9/setup.py
```

### Comparing `bus_user-0.2.8/LICENSE` & `bus_user-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bus_user-0.2.8/PKG-INFO` & `bus_user-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bus_user
-Version: 0.2.8
+Version: 0.2.9
 Summary: work with equipment over buses like Serial/i2c/... as client and server
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/bus_user
 Keywords: serial,serial bus,pyserial,serial port,com port,comport,rs232,UART,TTL,serial client,serial server,serial emulator,i2c
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# bus_user (v0.2.8)
+# bus_user (v0.2.9)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
 ### !. MOST APPROPRIATE COMMAND PROTOCOL
 other protocols mot recommended
```

### Comparing `bus_user-0.2.8/README.md` & `bus_user-0.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# bus_user (v0.2.8)
+# bus_user (v0.2.9)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
 ### !. MOST APPROPRIATE COMMAND PROTOCOL
 other protocols mot recommended
```

### Comparing `bus_user-0.2.8/bus_user/history.py` & `bus_user-0.2.9/bus_user/history.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.2.8/bus_user/i2c_client.py` & `bus_user-0.2.9/bus_user/i2c_client.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.2.8/bus_user/serial_client.py` & `bus_user-0.2.9/bus_user/serial_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,14 +172,16 @@
         # apply settings
         # self._SERIAL.interCharTimeout = 0.8
         self._SERIAL.baudrate = self.BAUDRATE
         self._SERIAL.timeout = self.TIMEOUT__READ
         # self._SERIAL.write_timeout = self._TIMEOUT__WRITE
 
         # self.addresses_system__detect()   # DONT USE in init!!!
+        # self.addresses_shorted__detect()   # DONT USE in init!!!
+        # self.addresses_paired__detect()   # DONT USE in init!!!
 
     def __del__(self):
         self.disconnect()
 
     # MSG =============================================================================================================
     def msg_log(self, msg: str = None) -> None:
         msg = f"[{self._SERIAL.port}]{msg}"
@@ -590,15 +592,15 @@
 
         SerialClient.ADDRESSES__PAIRED = result
         print(f"{cls.ADDRESSES__PAIRED=}")
         return result
 
     def addresses_paired__get_used(self) -> Optional[Tuple[str, str]]:
         for pair in self.addresses_paired__detect():
-            if self.ADDRESS in pair:
+            if self._SERIAL.port in pair:
                 return pair
 
     # COUNTS -----------------------------------------
     @classmethod
     def addresses_system__count(cls) -> int:
         return len(cls.addresses_system__detect())
```

### Comparing `bus_user-0.2.8/bus_user/serial_derivatives.py` & `bus_user-0.2.9/bus_user/serial_derivatives.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.2.8/bus_user/serial_server.py` & `bus_user-0.2.9/bus_user/serial_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .serial_client import SerialClient, AddressAutoAcceptVariant
+from .serial_client import SerialClient, AddressAutoAcceptVariant, TYPE__ADDRESS
 
 from typing import *
 import time
 import re
 from enum import Enum
 from object_info import ObjectInfo
 from PyQt5.QtCore import QThread
@@ -269,17 +269,19 @@
 
 # =====================================================================================================================
 class SerialServer_Base(QThread):
     # TODO: not realized - ACCESS RULES for PARAMS - may be not need in this case of class/situation!!!
     # TODO: not realised list access - best way to use pattern "name/index" and change same access with Dict "name/key"
 
     # SETTINGS ------------------------------------------------
-    SERIAL_CLIENT: SerialClient = SerialClient()
+    _SERIAL_CLIENT__CLS: Type[SerialClient] = SerialClient  # usually not redefines!
+    SERIAL_CLIENT: SerialClient
+    ADDRESS: str = None     # DON'T DEPRECATE! usually use only as exact port or keep NONE!
 
-    HELLO_MSG__SEND_ON_START: bool = True   # dont set here on True! use it only as overwritten if needed!!!
+    HELLO_MSG__SEND_ON_START: bool = True   # don't set here on True! use it only as overwritten if needed!!!
     HELLO_MSG: List[str] = [
         "SerialServer_Base HELLO line 1",
         "SerialServer_Base hello line 2",
     ]
 
     PARAMS: Dict[str, Union[Any, Dict[Union[str, int], Any]]] = None
     ANSWER: Type[AnswerVariants] = AnswerVariants
@@ -352,16 +354,19 @@
         elif not self.PARAMS:
             self.PARAMS = {}
         else:
             pass
 
         self._init_lists()
 
+        self.SERIAL_CLIENT = self._SERIAL_CLIENT__CLS()
         self.SERIAL_CLIENT.RAISE_READ_FAIL_PATTERN = False
         self.SERIAL_CLIENT.TIMEOUT__READ = None
+        if self.ADDRESS:
+            self.SERIAL_CLIENT.ADDRESS = self.ADDRESS
         if not self.SERIAL_CLIENT.ADDRESS:
             self.SERIAL_CLIENT.ADDRESS = AddressAutoAcceptVariant.FIRST_FREE__PAIRED_FOR_EMU   # here keep only FIRST_FREE__PAIRED_FOR_EMU! as default!
 
     def _init_lists(self) -> None:
         self._LIST__CMDS = []
         self._LIST__SCRIPTS = []
 
@@ -376,14 +381,15 @@
     def run(self) -> None:
         if not self.SERIAL_CLIENT.connect(_raise=False):
             msg = f"[ERROR]NOT STARTED={self.__class__.__name__}"
             print(msg)
             return
 
         if self.HELLO_MSG__SEND_ON_START:
+            self.HELLO_MSG.append(f"Started on [{self.SERIAL_CLIENT._SERIAL.port}]")
             self.SERIAL_CLIENT._write_line("")
             self.SERIAL_CLIENT._write_line("="*50)
             # self._execute_line("hello")
             self.SERIAL_CLIENT._write_line(self.HELLO_MSG)
 
         while True:
             self.MONITOR_READY = True
```

### Comparing `bus_user-0.2.8/bus_user.egg-info/PKG-INFO` & `bus_user-0.2.9/bus_user.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bus_user
-Version: 0.2.8
+Version: 0.2.9
 Summary: work with equipment over buses like Serial/i2c/... as client and server
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/bus_user
 Keywords: serial,serial bus,pyserial,serial port,com port,comport,rs232,UART,TTL,serial client,serial server,serial emulator,i2c
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# bus_user (v0.2.8)
+# bus_user (v0.2.9)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
 ### !. MOST APPROPRIATE COMMAND PROTOCOL
 other protocols mot recommended
```

### Comparing `bus_user-0.2.8/setup.py` & `bus_user-0.2.9/setup.py`

 * *Files identical despite different names*

