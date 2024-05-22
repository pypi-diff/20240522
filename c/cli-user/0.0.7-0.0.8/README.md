# Comparing `tmp/cli_user-0.0.7.tar.gz` & `tmp/cli_user-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli_user-0.0.7.tar", last modified: Sun Jan 14 02:08:03 2024, max compression
+gzip compressed data, was "cli_user-0.0.8.tar", last modified: Wed May 22 08:46:45 2024, max compression
```

## Comparing `cli_user-0.0.7.tar` & `cli_user-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-01-14 02:08:03.571616 cli_user-0.0.7/
--rw-rw-rw-   0        0        0     1082 2024-01-13 20:24:42.000000 cli_user-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     3376 2024-01-14 02:08:03.570617 cli_user-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2495 2024-01-14 02:07:41.000000 cli_user-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-01-14 02:08:03.548628 cli_user-0.0.7/cli_user/
--rw-rw-rw-   0        0        0       21 2024-01-13 20:24:42.000000 cli_user-0.0.7/cli_user/__init__.py
--rw-rw-rw-   0        0        0    12001 2024-01-14 01:50:52.000000 cli_user-0.0.7/cli_user/main.py
-drwxrwxrwx   0        0        0        0 2024-01-14 02:08:03.567617 cli_user-0.0.7/cli_user.egg-info/
--rw-rw-rw-   0        0        0     3376 2024-01-14 02:08:03.000000 cli_user-0.0.7/cli_user.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-01-14 02:08:03.000000 cli_user-0.0.7/cli_user.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-14 02:08:03.000000 cli_user-0.0.7/cli_user.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-01-14 02:08:03.000000 cli_user-0.0.7/cli_user.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-14 02:08:03.576615 cli_user-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2656 2024-01-13 19:10:34.000000 cli_user-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:46:45.207679 cli_user-0.0.8/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 cli_user-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     3376 2024-05-22 08:46:45.207679 cli_user-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2495 2024-05-22 08:45:27.000000 cli_user-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 08:46:45.196454 cli_user-0.0.8/cli_user/
+-rw-rw-rw-   0        0        0      698 2024-05-22 08:44:05.000000 cli_user-0.0.8/cli_user/__init__.py
+-rw-rw-rw-   0        0        0    12007 2024-05-22 08:44:05.000000 cli_user-0.0.8/cli_user/main.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:46:45.206652 cli_user-0.0.8/cli_user.egg-info/
+-rw-rw-rw-   0        0        0     3376 2024-05-22 08:46:45.000000 cli_user-0.0.8/cli_user.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-05-22 08:46:45.000000 cli_user-0.0.8/cli_user.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 08:46:45.000000 cli_user-0.0.8/cli_user.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-22 08:46:45.000000 cli_user-0.0.8/cli_user.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 08:46:45.209814 cli_user-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 cli_user-0.0.8/setup.py
```

### Comparing `cli_user-0.0.7/LICENSE` & `cli_user-0.0.8/LICENSE`

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

### Comparing `cli_user-0.0.7/PKG-INFO` & `cli_user-0.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli_user
-Version: 0.0.7
+Version: 0.0.8
 Summary: send commands into system terminal
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/cli_user
 Keywords: cli,cli user,cli sender,os terminal,os terminal sender,os terminal user
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,21 +16,21 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# cli_user (v0.0.7)
+# cli_user (v0.0.8)
 
 ## DESCRIPTION_SHORT
-Send commands into system terminal
+send commands into system terminal
 
 ## DESCRIPTION_LONG
-designed to send commands into os terminal
+Designed to send commands into OS terminal
 
 
 ## Features
 1. send commands into OS terminal  
 2. check if cli commands are accessible (special utilities is installed)  
 3. access to standard parts of result in a simple ready-to-use form (stdout/stderr/retcode/full state)  
 4. use batch timeout for list
```

### Comparing `cli_user-0.0.7/README.md` & `cli_user-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# cli_user (v0.0.7)
+# cli_user (v0.0.8)
 
 ## DESCRIPTION_SHORT
-Send commands into system terminal
+send commands into system terminal
 
 ## DESCRIPTION_LONG
-designed to send commands into os terminal
+Designed to send commands into OS terminal
 
 
 ## Features
 1. send commands into OS terminal  
 2. check if cli commands are accessible (special utilities is installed)  
 3. access to standard parts of result in a simple ready-to-use form (stdout/stderr/retcode/full state)  
 4. use batch timeout for list
```

### Comparing `cli_user-0.0.7/cli_user/main.py` & `cli_user-0.0.8/cli_user/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import time
 
 from typing import *
 
 
 # =====================================================================================================================
 # TODO: is it necessary to add wait param in send? think not! but maybe use thread start?
+pass
 
 
 # =====================================================================================================================
 class Exx_CliNotAvailable(Exception):
     """CLI exx because of cli can not be available due to have not some of required commands.
     """
```

### Comparing `cli_user-0.0.7/cli_user.egg-info/PKG-INFO` & `cli_user-0.0.8/cli_user.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli_user
-Version: 0.0.7
+Version: 0.0.8
 Summary: send commands into system terminal
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/cli_user
 Keywords: cli,cli user,cli sender,os terminal,os terminal sender,os terminal user
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,21 +16,21 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# cli_user (v0.0.7)
+# cli_user (v0.0.8)
 
 ## DESCRIPTION_SHORT
-Send commands into system terminal
+send commands into system terminal
 
 ## DESCRIPTION_LONG
-designed to send commands into os terminal
+Designed to send commands into OS terminal
 
 
 ## Features
 1. send commands into OS terminal  
 2. check if cli commands are accessible (special utilities is installed)  
 3. access to standard parts of result in a simple ready-to-use form (stdout/stderr/retcode/full state)  
 4. use batch timeout for list
```

