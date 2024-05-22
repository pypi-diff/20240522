# Comparing `tmp/buzz_client-1.1.0.tar.gz` & `tmp/buzz_client-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buzz_client-1.1.0.tar", max compression
+gzip compressed data, was "buzz_client-1.1.1.tar", max compression
```

## Comparing `buzz_client-1.1.0.tar` & `buzz_client-1.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2288 2024-05-21 10:16:10.377792 buzz_client-1.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-16 12:39:43.660459 buzz_client-1.1.0/buzz_client/__init__.py
--rwxr-xr-x   0        0        0     5050 2024-05-21 10:35:55.428345 buzz_client-1.1.0/buzz_client/cli.py
--rw-r--r--   0        0        0     2617 2024-05-21 09:18:17.969995 buzz_client-1.1.0/buzz_client/client.py
--rw-r--r--   0        0        0      451 2024-05-22 08:06:32.308072 buzz_client-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2933 1970-01-01 00:00:00.000000 buzz_client-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2288 2024-05-21 10:16:10.377792 buzz_client-1.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-22 08:29:59.906130 buzz_client-1.1.1/buzz_client/__init__.py
+-rwxr-xr-x   0        0        0     5223 2024-05-22 09:04:07.954604 buzz_client-1.1.1/buzz_client/cli.py
+-rw-r--r--   0        0        0     2617 2024-05-22 09:00:42.371384 buzz_client-1.1.1/buzz_client/client.py
+-rw-r--r--   0        0        0      451 2024-05-22 08:16:59.189809 buzz_client-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2933 1970-01-01 00:00:00.000000 buzz_client-1.1.1/PKG-INFO
```

### Comparing `buzz_client-1.1.0/README.md` & `buzz_client-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `buzz_client-1.1.0/buzz_client/cli.py` & `buzz_client-1.1.1/buzz_client/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-#  buzz [--server URL] [--token TOKEN] list
 """
 
 Buzz client
 
 Usage:
     buzz [options] list
     buzz [options] version
@@ -36,21 +35,30 @@
                        Example: http://sesame@localhost:8000
 
 """
 import sys
 import signal
 import time
 from docopt import docopt
-from buzz_client.client import BuzzClient
+# from buzz_client.client import BuzzClient
+try:
+    from buzz_client.client import BuzzClient
+except ImportError:
+    from client import BuzzClient
 from scriptonite.configuration import Configuration
 from scriptonite.logging import Logger
 
+import importlib.metadata
+
 log = Logger(level="INFO")
 
-VERSION = "1.0.4"
+try:
+    VERSION = importlib.metadata.version("buzz_client")
+except ImportError:
+    VERSION = "dev"
 
 
 def shutdown(sig, frame):
     print("\nAye, aye! See you...")
     sys.exit(0)
```

### Comparing `buzz_client-1.1.0/buzz_client/client.py` & `buzz_client-1.1.1/buzz_client/client.py`

 * *Files identical despite different names*

### Comparing `buzz_client-1.1.0/PKG-INFO` & `buzz_client-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buzz-client
-Version: 1.1.0
+Version: 1.1.1
 Summary: A client for Buzz API
 License: GPL
 Author: Andrea Mistrali
 Author-email: andrea@mistrali.pw
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: buzz-client Version: 1.1.0 Summary: A client for
+Metadata-Version: 2.1 Name: buzz-client Version: 1.1.1 Summary: A client for
 Buzz API License: GPL Author: Andrea Mistrali Author-email: andrea@mistrali.pw
 Requires-Python: >=3.10,<4.0 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: docopt-ng
 (>=0.9.0,<0.10.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist:
 requests (>=2.31.0,<3.0.0) Requires-Dist: scriptonite (>=1.0.3,<2.0.0)
```

