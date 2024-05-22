# Comparing `tmp/singleton_meta-0.1.2.tar.gz` & `tmp/singleton_meta-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singleton_meta-0.1.2.tar", last modified: Wed Mar 27 08:40:43 2024, max compression
+gzip compressed data, was "singleton_meta-0.1.3.tar", last modified: Wed May 22 13:48:50 2024, max compression
```

## Comparing `singleton_meta-0.1.2.tar` & `singleton_meta-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 08:40:43.319337 singleton_meta-0.1.2/
--rw-rw-rw-   0        0        0     1082 2024-03-27 07:26:28.000000 singleton_meta-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     2835 2024-03-27 08:40:43.319337 singleton_meta-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1969 2024-03-27 08:38:40.000000 singleton_meta-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-03-27 08:40:43.320334 singleton_meta-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 singleton_meta-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-27 08:40:43.310037 singleton_meta-0.1.2/singleton_meta/
--rw-rw-rw-   0        0        0       21 2024-03-27 07:26:28.000000 singleton_meta-0.1.2/singleton_meta/__init__.py
--rw-rw-rw-   0        0        0     8042 2024-03-27 07:26:28.000000 singleton_meta-0.1.2/singleton_meta/main.py
-drwxrwxrwx   0        0        0        0 2024-03-27 08:40:43.318333 singleton_meta-0.1.2/singleton_meta.egg-info/
--rw-rw-rw-   0        0        0     2835 2024-03-27 08:40:43.000000 singleton_meta-0.1.2/singleton_meta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-03-27 08:40:43.000000 singleton_meta-0.1.2/singleton_meta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 08:40:43.000000 singleton_meta-0.1.2/singleton_meta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-03-27 08:40:43.000000 singleton_meta-0.1.2/singleton_meta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 13:48:50.408886 singleton_meta-0.1.3/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 singleton_meta-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2835 2024-05-22 13:48:50.408355 singleton_meta-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1969 2024-05-22 13:48:05.000000 singleton_meta-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 13:48:50.410580 singleton_meta-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 singleton_meta-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:48:50.393686 singleton_meta-0.1.3/singleton_meta/
+-rw-rw-rw-   0        0        0      992 2024-05-22 13:47:33.000000 singleton_meta-0.1.3/singleton_meta/__init__.py
+-rw-rw-rw-   0        0        0     8042 2024-03-27 07:26:28.000000 singleton_meta-0.1.3/singleton_meta/main.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:48:50.407055 singleton_meta-0.1.3/singleton_meta.egg-info/
+-rw-rw-rw-   0        0        0     2835 2024-05-22 13:48:50.000000 singleton_meta-0.1.3/singleton_meta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-22 13:48:50.000000 singleton_meta-0.1.3/singleton_meta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 13:48:50.000000 singleton_meta-0.1.3/singleton_meta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-22 13:48:50.000000 singleton_meta-0.1.3/singleton_meta.egg-info/top_level.txt
```

### Comparing `singleton_meta-0.1.2/LICENSE` & `singleton_meta-0.1.3/LICENSE`

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

### Comparing `singleton_meta-0.1.2/PKG-INFO` & `singleton_meta-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singleton_meta
-Version: 0.1.2
+Version: 0.1.3
 Summary: create perfect singletons
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/singleton_meta
 Keywords: singleton,singleton meta,singleton call,singleton new
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# singleton_meta (v0.1.2)
+# singleton_meta (v0.1.3)
 
 ## DESCRIPTION_SHORT
 create perfect singletons
 
 ## DESCRIPTION_LONG
 designed for singletons creation
```

### Comparing `singleton_meta-0.1.2/README.md` & `singleton_meta-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# singleton_meta (v0.1.2)
+# singleton_meta (v0.1.3)
 
 ## DESCRIPTION_SHORT
 create perfect singletons
 
 ## DESCRIPTION_LONG
 designed for singletons creation
```

### Comparing `singleton_meta-0.1.2/setup.py` & `singleton_meta-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `singleton_meta-0.1.2/singleton_meta/main.py` & `singleton_meta-0.1.3/singleton_meta/main.py`

 * *Files identical despite different names*

### Comparing `singleton_meta-0.1.2/singleton_meta.egg-info/PKG-INFO` & `singleton_meta-0.1.3/singleton_meta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singleton_meta
-Version: 0.1.2
+Version: 0.1.3
 Summary: create perfect singletons
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/singleton_meta
 Keywords: singleton,singleton meta,singleton call,singleton new
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# singleton_meta (v0.1.2)
+# singleton_meta (v0.1.3)
 
 ## DESCRIPTION_SHORT
 create perfect singletons
 
 ## DESCRIPTION_LONG
 designed for singletons creation
```

