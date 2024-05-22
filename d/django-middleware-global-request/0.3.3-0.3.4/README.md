# Comparing `tmp/django-middleware-global-request-0.3.3.tar.gz` & `tmp/django-middleware-global-request-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-middleware-global-request-0.3.3.tar", last modified: Fri Sep 15 14:28:35 2023, max compression
+gzip compressed data, was "django-middleware-global-request-0.3.4.tar", last modified: Wed May 22 13:38:34 2024, max compression
```

## Comparing `django-middleware-global-request-0.3.3.tar` & `django-middleware-global-request-0.3.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-15 14:28:35.959265 django-middleware-global-request-0.3.3/
--rw-r--r--   0 test       (501) staff       (20)     1067 2022-06-16 07:38:43.000000 django-middleware-global-request-0.3.3/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      264 2022-06-16 07:41:13.000000 django-middleware-global-request-0.3.3/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     6300 2023-09-15 14:28:35.959131 django-middleware-global-request-0.3.3/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     5554 2023-09-15 13:12:20.000000 django-middleware-global-request-0.3.3/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-15 14:28:35.957366 django-middleware-global-request-0.3.3/django_middleware_global_request/
--rw-r--r--   0 test       (501) staff       (20)      430 2023-09-13 07:32:23.000000 django-middleware-global-request-0.3.3/django_middleware_global_request/__init__.py
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-13 07:32:24.000000 django-middleware-global-request-0.3.3/django_middleware_global_request/admin.py
--rw-r--r--   0 test       (501) staff       (20)      307 2022-09-07 09:33:15.000000 django-middleware-global-request-0.3.3/django_middleware_global_request/apps.py
--rw-r--r--   0 test       (501) staff       (20)     2206 2023-09-13 07:32:32.000000 django-middleware-global-request-0.3.3/django_middleware_global_request/middleware.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-15 14:28:35.958331 django-middleware-global-request-0.3.3/django_middleware_global_request/migrations/
--rw-r--r--   0 test       (501) staff       (20)      171 2022-09-07 09:34:04.000000 django-middleware-global-request-0.3.3/django_middleware_global_request/migrations/__init__.py
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-13 07:32:25.000000 django-middleware-global-request-0.3.3/django_middleware_global_request/models.py
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-13 07:32:05.000000 django-middleware-global-request-0.3.3/django_middleware_global_request/tests.py
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-13 07:32:02.000000 django-middleware-global-request-0.3.3/django_middleware_global_request/views.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-15 14:28:35.958166 django-middleware-global-request-0.3.3/django_middleware_global_request.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     6300 2023-09-15 14:28:35.000000 django-middleware-global-request-0.3.3/django_middleware_global_request.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      961 2023-09-15 14:28:35.000000 django-middleware-global-request-0.3.3/django_middleware_global_request.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-09-15 14:28:35.000000 django-middleware-global-request-0.3.3/django_middleware_global_request.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-09-15 14:28:35.000000 django-middleware-global-request-0.3.3/django_middleware_global_request.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)        7 2023-09-15 14:28:35.000000 django-middleware-global-request-0.3.3/django_middleware_global_request.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       74 2023-09-15 14:28:35.000000 django-middleware-global-request-0.3.3/django_middleware_global_request.egg-info/top_level.txt
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-15 14:28:35.955113 django-middleware-global-request-0.3.3/django_middleware_global_request_example/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-15 14:28:35.958590 django-middleware-global-request-0.3.3/django_middleware_global_request_example/management/
--rw-r--r--   0 test       (501) staff       (20)        0 2022-06-16 03:01:54.000000 django-middleware-global-request-0.3.3/django_middleware_global_request_example/management/__init__.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-15 14:28:35.958771 django-middleware-global-request-0.3.3/django_middleware_global_request_example/management/commands/
--rw-r--r--   0 test       (501) staff       (20)        0 2022-06-16 03:02:06.000000 django-middleware-global-request-0.3.3/django_middleware_global_request_example/management/commands/__init__.py
--rw-r--r--   0 test       (501) staff       (20)     1039 2023-09-15 13:01:09.000000 django-middleware-global-request-0.3.3/django_middleware_global_request_example/management/commands/create_books.py
--rw-r--r--   0 test       (501) staff       (20)        6 2022-06-15 12:47:54.000000 django-middleware-global-request-0.3.3/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2023-09-15 14:28:35.959303 django-middleware-global-request-0.3.3/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1881 2023-09-15 12:55:09.000000 django-middleware-global-request-0.3.3/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 13:38:34.339128 django-middleware-global-request-0.3.4/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-22 13:37:13.000000 django-middleware-global-request-0.3.4/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      264 2022-06-16 07:41:13.000000 django-middleware-global-request-0.3.4/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     6326 2024-05-22 13:38:34.339016 django-middleware-global-request-0.3.4/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     5615 2024-05-22 13:35:45.000000 django-middleware-global-request-0.3.4/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 13:38:34.337525 django-middleware-global-request-0.3.4/django_middleware_global_request/
+-rw-r--r--   0 test       (501) staff       (20)      430 2023-09-13 07:32:23.000000 django-middleware-global-request-0.3.4/django_middleware_global_request/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-13 07:32:24.000000 django-middleware-global-request-0.3.4/django_middleware_global_request/admin.py
+-rw-r--r--   0 test       (501) staff       (20)      307 2022-09-07 09:33:15.000000 django-middleware-global-request-0.3.4/django_middleware_global_request/apps.py
+-rw-r--r--   0 test       (501) staff       (20)     2206 2023-09-13 07:32:32.000000 django-middleware-global-request-0.3.4/django_middleware_global_request/middleware.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 13:38:34.338307 django-middleware-global-request-0.3.4/django_middleware_global_request/migrations/
+-rw-r--r--   0 test       (501) staff       (20)      171 2022-09-07 09:34:04.000000 django-middleware-global-request-0.3.4/django_middleware_global_request/migrations/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-13 07:32:25.000000 django-middleware-global-request-0.3.4/django_middleware_global_request/models.py
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-13 07:32:05.000000 django-middleware-global-request-0.3.4/django_middleware_global_request/tests.py
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-13 07:32:02.000000 django-middleware-global-request-0.3.4/django_middleware_global_request/views.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 13:38:34.338173 django-middleware-global-request-0.3.4/django_middleware_global_request.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     6326 2024-05-22 13:38:34.000000 django-middleware-global-request-0.3.4/django_middleware_global_request.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      961 2024-05-22 13:38:34.000000 django-middleware-global-request-0.3.4/django_middleware_global_request.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-22 13:38:34.000000 django-middleware-global-request-0.3.4/django_middleware_global_request.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-22 13:38:34.000000 django-middleware-global-request-0.3.4/django_middleware_global_request.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)        7 2024-05-22 13:38:34.000000 django-middleware-global-request-0.3.4/django_middleware_global_request.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       74 2024-05-22 13:38:34.000000 django-middleware-global-request-0.3.4/django_middleware_global_request.egg-info/top_level.txt
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 13:38:34.335810 django-middleware-global-request-0.3.4/django_middleware_global_request_example/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 13:38:34.338543 django-middleware-global-request-0.3.4/django_middleware_global_request_example/management/
+-rw-r--r--   0 test       (501) staff       (20)        0 2022-06-16 03:01:54.000000 django-middleware-global-request-0.3.4/django_middleware_global_request_example/management/__init__.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 13:38:34.338726 django-middleware-global-request-0.3.4/django_middleware_global_request_example/management/commands/
+-rw-r--r--   0 test       (501) staff       (20)        0 2022-06-16 03:02:06.000000 django-middleware-global-request-0.3.4/django_middleware_global_request_example/management/commands/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)     1039 2023-09-15 13:01:09.000000 django-middleware-global-request-0.3.4/django_middleware_global_request_example/management/commands/create_books.py
+-rw-r--r--   0 test       (501) staff       (20)        6 2022-06-15 12:47:54.000000 django-middleware-global-request-0.3.4/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-05-22 13:38:34.339170 django-middleware-global-request-0.3.4/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1795 2024-05-22 13:36:22.000000 django-middleware-global-request-0.3.4/setup.py
```

### Comparing `django-middleware-global-request-0.3.3/LICENSE` & `django-middleware-global-request-0.3.4/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 MIT License
 
-Copyright (c) 2017 zencore.cn
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `django-middleware-global-request-0.3.3/PKG-INFO` & `django-middleware-global-request-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-middleware-global-request
-Version: 0.3.3
+Version: 0.3.4
 Summary: Django middleware that keep request instance for every thread.
+Home-page: UNKNOWN
 Author: Wang Liang
-Author-email: wangliang@zencore.cn
 Maintainer: Wang Liang
-Maintainer-email: wangliang@zencore.cn
 License: MIT
 Keywords: django extensions,django middleware global request
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires: django
@@ -222,7 +222,13 @@
 ### v0.3.2
 
 - Doc update.
 
 ### v0.3.3
 
 - All unit test passed.
+
+### v0.3.4
+
+- Add unit tests for python12 and django-5.0.6.
+
+
```

### Comparing `django-middleware-global-request-0.3.3/README.md` & `django-middleware-global-request-0.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -202,7 +202,11 @@
 ### v0.3.2
 
 - Doc update.
 
 ### v0.3.3
 
 - All unit test passed.
+
+### v0.3.4
+
+- Add unit tests for python12 and django-5.0.6.
```

### Comparing `django-middleware-global-request-0.3.3/django_middleware_global_request/middleware.py` & `django-middleware-global-request-0.3.4/django_middleware_global_request/middleware.py`

 * *Files identical despite different names*

### Comparing `django-middleware-global-request-0.3.3/django_middleware_global_request.egg-info/PKG-INFO` & `django-middleware-global-request-0.3.4/django_middleware_global_request.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-middleware-global-request
-Version: 0.3.3
+Version: 0.3.4
 Summary: Django middleware that keep request instance for every thread.
+Home-page: UNKNOWN
 Author: Wang Liang
-Author-email: wangliang@zencore.cn
 Maintainer: Wang Liang
-Maintainer-email: wangliang@zencore.cn
 License: MIT
 Keywords: django extensions,django middleware global request
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires: django
@@ -222,7 +222,13 @@
 ### v0.3.2
 
 - Doc update.
 
 ### v0.3.3
 
 - All unit test passed.
+
+### v0.3.4
+
+- Add unit tests for python12 and django-5.0.6.
+
+
```

### Comparing `django-middleware-global-request-0.3.3/django_middleware_global_request.egg-info/SOURCES.txt` & `django-middleware-global-request-0.3.4/django_middleware_global_request.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-middleware-global-request-0.3.3/django_middleware_global_request_example/management/commands/create_books.py` & `django-middleware-global-request-0.3.4/django_middleware_global_request_example/management/commands/create_books.py`

 * *Files identical despite different names*

### Comparing `django-middleware-global-request-0.3.3/setup.py` & `django-middleware-global-request-0.3.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,22 +21,20 @@
     long_description = fobj.read()
 
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires = [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="django-middleware-global-request",
-    version="0.3.3",
+    version="0.3.4",
     description="Django middleware that keep request instance for every thread.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Wang Liang",
-    author_email="wangliang@zencore.cn",
     maintainer="Wang Liang",
-    maintainer_email="wangliang@zencore.cn",
     license="MIT",
     license_files=("LICENSE",),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
```

