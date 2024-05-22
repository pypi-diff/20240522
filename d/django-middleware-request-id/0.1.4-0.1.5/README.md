# Comparing `tmp/django-middleware-request-id-0.1.4.tar.gz` & `tmp/django-middleware-request-id-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-middleware-request-id-0.1.4.tar", last modified: Fri Sep 15 12:18:07 2023, max compression
+gzip compressed data, was "django-middleware-request-id-0.1.5.tar", last modified: Wed May 22 13:42:37 2024, max compression
```

## Comparing `django-middleware-request-id-0.1.4.tar` & `django-middleware-request-id-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-15 12:18:07.721912 django-middleware-request-id-0.1.4/
--rw-r--r--   0 test       (501) staff       (20)     1067 2022-09-07 02:01:49.000000 django-middleware-request-id-0.1.4/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      205 2022-09-07 02:02:12.000000 django-middleware-request-id-0.1.4/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     4892 2023-09-15 12:18:07.721797 django-middleware-request-id-0.1.4/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     4052 2023-09-15 12:17:25.000000 django-middleware-request-id-0.1.4/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-15 12:18:07.720714 django-middleware-request-id-0.1.4/django_middleware_request_id/
--rw-r--r--   0 test       (501) staff       (20)      554 2022-09-26 01:34:27.000000 django-middleware-request-id-0.1.4/django_middleware_request_id/__init__.py
--rw-r--r--   0 test       (501) staff       (20)      171 2022-09-07 02:08:00.000000 django-middleware-request-id-0.1.4/django_middleware_request_id/admin.py
--rw-r--r--   0 test       (501) staff       (20)      299 2022-09-07 02:07:57.000000 django-middleware-request-id-0.1.4/django_middleware_request_id/apps.py
--rw-r--r--   0 test       (501) staff       (20)     1462 2022-09-07 14:20:49.000000 django-middleware-request-id-0.1.4/django_middleware_request_id/log_filters.py
--rw-r--r--   0 test       (501) staff       (20)     1309 2022-10-17 02:56:33.000000 django-middleware-request-id-0.1.4/django_middleware_request_id/middlewares.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-15 12:18:07.721567 django-middleware-request-id-0.1.4/django_middleware_request_id/migrations/
--rw-r--r--   0 test       (501) staff       (20)      171 2022-09-07 02:08:09.000000 django-middleware-request-id-0.1.4/django_middleware_request_id/migrations/__init__.py
--rw-r--r--   0 test       (501) staff       (20)      171 2022-09-07 02:07:43.000000 django-middleware-request-id-0.1.4/django_middleware_request_id/models.py
--rw-r--r--   0 test       (501) staff       (20)      171 2022-09-07 02:07:45.000000 django-middleware-request-id-0.1.4/django_middleware_request_id/tests.py
--rw-r--r--   0 test       (501) staff       (20)      171 2022-09-07 02:07:48.000000 django-middleware-request-id-0.1.4/django_middleware_request_id/views.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-15 12:18:07.721449 django-middleware-request-id-0.1.4/django_middleware_request_id.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     4892 2023-09-15 12:18:07.000000 django-middleware-request-id-0.1.4/django_middleware_request_id.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      736 2023-09-15 12:18:07.000000 django-middleware-request-id-0.1.4/django_middleware_request_id.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-09-15 12:18:07.000000 django-middleware-request-id-0.1.4/django_middleware_request_id.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-09-15 12:18:07.000000 django-middleware-request-id-0.1.4/django_middleware_request_id.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)       40 2023-09-15 12:18:07.000000 django-middleware-request-id-0.1.4/django_middleware_request_id.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       29 2023-09-15 12:18:07.000000 django-middleware-request-id-0.1.4/django_middleware_request_id.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)       40 2022-09-07 02:26:41.000000 django-middleware-request-id-0.1.4/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2023-09-15 12:18:07.721946 django-middleware-request-id-0.1.4/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1902 2023-09-15 12:16:37.000000 django-middleware-request-id-0.1.4/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 13:42:37.870660 django-middleware-request-id-0.1.5/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-22 13:41:40.000000 django-middleware-request-id-0.1.5/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      205 2022-09-07 02:02:12.000000 django-middleware-request-id-0.1.5/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     4914 2024-05-22 13:42:37.870536 django-middleware-request-id-0.1.5/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     4113 2024-05-22 13:41:23.000000 django-middleware-request-id-0.1.5/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 13:42:37.869529 django-middleware-request-id-0.1.5/django_middleware_request_id/
+-rw-r--r--   0 test       (501) staff       (20)      554 2022-09-26 01:34:27.000000 django-middleware-request-id-0.1.5/django_middleware_request_id/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)      171 2022-09-07 02:08:00.000000 django-middleware-request-id-0.1.5/django_middleware_request_id/admin.py
+-rw-r--r--   0 test       (501) staff       (20)      299 2022-09-07 02:07:57.000000 django-middleware-request-id-0.1.5/django_middleware_request_id/apps.py
+-rw-r--r--   0 test       (501) staff       (20)     1462 2022-09-07 14:20:49.000000 django-middleware-request-id-0.1.5/django_middleware_request_id/log_filters.py
+-rw-r--r--   0 test       (501) staff       (20)     1309 2022-10-17 02:56:33.000000 django-middleware-request-id-0.1.5/django_middleware_request_id/middlewares.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 13:42:37.870339 django-middleware-request-id-0.1.5/django_middleware_request_id/migrations/
+-rw-r--r--   0 test       (501) staff       (20)      171 2022-09-07 02:08:09.000000 django-middleware-request-id-0.1.5/django_middleware_request_id/migrations/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)      171 2022-09-07 02:07:43.000000 django-middleware-request-id-0.1.5/django_middleware_request_id/models.py
+-rw-r--r--   0 test       (501) staff       (20)      171 2022-09-07 02:07:45.000000 django-middleware-request-id-0.1.5/django_middleware_request_id/tests.py
+-rw-r--r--   0 test       (501) staff       (20)      171 2022-09-07 02:07:48.000000 django-middleware-request-id-0.1.5/django_middleware_request_id/views.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 13:42:37.870218 django-middleware-request-id-0.1.5/django_middleware_request_id.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     4914 2024-05-22 13:42:37.000000 django-middleware-request-id-0.1.5/django_middleware_request_id.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      736 2024-05-22 13:42:37.000000 django-middleware-request-id-0.1.5/django_middleware_request_id.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-22 13:42:37.000000 django-middleware-request-id-0.1.5/django_middleware_request_id.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-22 13:42:37.000000 django-middleware-request-id-0.1.5/django_middleware_request_id.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)       40 2024-05-22 13:42:37.000000 django-middleware-request-id-0.1.5/django_middleware_request_id.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       29 2024-05-22 13:42:37.000000 django-middleware-request-id-0.1.5/django_middleware_request_id.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)       40 2022-09-07 02:26:41.000000 django-middleware-request-id-0.1.5/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-05-22 13:42:37.870702 django-middleware-request-id-0.1.5/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1812 2024-05-22 13:41:35.000000 django-middleware-request-id-0.1.5/setup.py
```

### Comparing `django-middleware-request-id-0.1.4/LICENSE` & `django-middleware-request-id-0.1.5/LICENSE`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 MIT License
 
-Copyright (c) 2022 zencore.cn
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `django-middleware-request-id-0.1.4/PKG-INFO` & `django-middleware-request-id-0.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-middleware-request-id
-Version: 0.1.4
+Version: 0.1.5
 Summary: The middleware detect if a client or the front reverse proxy server provides a X-Request-ID header, and get it as the request_id. If no such header is provided, it can provide a random value.
+Home-page: UNKNOWN
 Author: Wang DongHao
-Author-email: wangdonghao@zencore.cn
 Maintainer: Wang DongHao
-Maintainer-email: wangdonghao@zencore.cn
 License: MIT
 Keywords: django-middleware-request-id
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -179,7 +179,13 @@
 ### v0.1.3
 
 - Doc update.
 
 ### v0.1.4
 
 - Unit test all passed.
+
+### v0.1.5
+
+- Add unit test for python-12 and django-5.0.6.
+
+
```

### Comparing `django-middleware-request-id-0.1.4/README.md` & `django-middleware-request-id-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -160,7 +160,11 @@
 ### v0.1.3
 
 - Doc update.
 
 ### v0.1.4
 
 - Unit test all passed.
+
+### v0.1.5
+
+- Add unit test for python-12 and django-5.0.6.
```

### Comparing `django-middleware-request-id-0.1.4/django_middleware_request_id/__init__.py` & `django-middleware-request-id-0.1.5/django_middleware_request_id/__init__.py`

 * *Files identical despite different names*

### Comparing `django-middleware-request-id-0.1.4/django_middleware_request_id/log_filters.py` & `django-middleware-request-id-0.1.5/django_middleware_request_id/log_filters.py`

 * *Files identical despite different names*

### Comparing `django-middleware-request-id-0.1.4/django_middleware_request_id/middlewares.py` & `django-middleware-request-id-0.1.5/django_middleware_request_id/middlewares.py`

 * *Files identical despite different names*

### Comparing `django-middleware-request-id-0.1.4/django_middleware_request_id.egg-info/PKG-INFO` & `django-middleware-request-id-0.1.5/django_middleware_request_id.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-middleware-request-id
-Version: 0.1.4
+Version: 0.1.5
 Summary: The middleware detect if a client or the front reverse proxy server provides a X-Request-ID header, and get it as the request_id. If no such header is provided, it can provide a random value.
+Home-page: UNKNOWN
 Author: Wang DongHao
-Author-email: wangdonghao@zencore.cn
 Maintainer: Wang DongHao
-Maintainer-email: wangdonghao@zencore.cn
 License: MIT
 Keywords: django-middleware-request-id
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -179,7 +179,13 @@
 ### v0.1.3
 
 - Doc update.
 
 ### v0.1.4
 
 - Unit test all passed.
+
+### v0.1.5
+
+- Add unit test for python-12 and django-5.0.6.
+
+
```

### Comparing `django-middleware-request-id-0.1.4/django_middleware_request_id.egg-info/SOURCES.txt` & `django-middleware-request-id-0.1.5/django_middleware_request_id.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-middleware-request-id-0.1.4/setup.py` & `django-middleware-request-id-0.1.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,22 +22,20 @@
 
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires = [x.strip() for x in fobj.readlines() if x.strip()]
 
 
 setup(
     name="django-middleware-request-id",
-    version="0.1.4",
+    version="0.1.5",
     description="The middleware detect if a client or the front reverse proxy server provides a X-Request-ID header, and get it as the request_id. If no such header is provided, it can provide a random value.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Wang DongHao",
-    author_email="wangdonghao@zencore.cn",
     maintainer="Wang DongHao",
-    maintainer_email="wangdonghao@zencore.cn",
     license="MIT",
     license_files=("LICENSE",),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
```

