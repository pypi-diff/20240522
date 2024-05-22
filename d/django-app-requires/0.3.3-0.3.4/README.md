# Comparing `tmp/django-app-requires-0.3.3.tar.gz` & `tmp/django-app-requires-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-app-requires-0.3.3.tar", last modified: Sun May 12 14:14:31 2024, max compression
+gzip compressed data, was "django-app-requires-0.3.4.tar", last modified: Wed May 22 12:44:31 2024, max compression
```

## Comparing `django-app-requires-0.3.3.tar` & `django-app-requires-0.3.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 14:14:31.453507 django-app-requires-0.3.3/
--rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-12 14:09:22.000000 django-app-requires-0.3.3/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      308 2022-09-13 02:41:33.000000 django-app-requires-0.3.3/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     3348 2024-05-12 14:14:31.453393 django-app-requires-0.3.3/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     2504 2024-05-12 14:09:14.000000 django-app-requires-0.3.3/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 14:14:31.450680 django-app-requires-0.3.3/django_app_requires/
--rw-r--r--   0 test       (501) staff       (20)      100 2022-06-01 13:00:11.000000 django-app-requires-0.3.3/django_app_requires/__init__.py
--rw-r--r--   0 test       (501) staff       (20)     3331 2023-09-13 06:50:31.000000 django-app-requires-0.3.3/django_app_requires/utils.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 14:14:31.451412 django-app-requires-0.3.3/django_app_requires.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     3348 2024-05-12 14:14:31.000000 django-app-requires-0.3.3/django_app_requires.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     1057 2024-05-12 14:14:31.000000 django-app-requires-0.3.3/django_app_requires.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 14:14:31.000000 django-app-requires-0.3.3/django_app_requires.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 14:14:31.000000 django-app-requires-0.3.3/django_app_requires.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)       16 2024-05-12 14:14:31.000000 django-app-requires-0.3.3/django_app_requires.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       95 2024-05-12 14:14:31.000000 django-app-requires-0.3.3/django_app_requires.egg-info/top_level.txt
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 14:14:31.452248 django-app-requires-0.3.3/django_app_requires_first_placeholder/
--rw-r--r--   0 test       (501) staff       (20)      107 2022-06-05 13:04:20.000000 django-app-requires-0.3.3/django_app_requires_first_placeholder/__init__.py
--rw-r--r--   0 test       (501) staff       (20)       63 2022-06-05 13:03:42.000000 django-app-requires-0.3.3/django_app_requires_first_placeholder/admin.py
--rw-r--r--   0 test       (501) staff       (20)     2408 2023-09-13 06:50:46.000000 django-app-requires-0.3.3/django_app_requires_first_placeholder/apps.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 14:14:31.452370 django-app-requires-0.3.3/django_app_requires_first_placeholder/migrations/
--rw-r--r--   0 test       (501) staff       (20)        0 2022-06-05 13:03:42.000000 django-app-requires-0.3.3/django_app_requires_first_placeholder/migrations/__init__.py
--rw-r--r--   0 test       (501) staff       (20)       57 2022-06-05 13:03:42.000000 django-app-requires-0.3.3/django_app_requires_first_placeholder/models.py
--rw-r--r--   0 test       (501) staff       (20)       60 2022-06-05 13:03:42.000000 django-app-requires-0.3.3/django_app_requires_first_placeholder/tests.py
--rw-r--r--   0 test       (501) staff       (20)       63 2022-06-05 13:03:42.000000 django-app-requires-0.3.3/django_app_requires_first_placeholder/views.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 14:14:31.453122 django-app-requires-0.3.3/django_app_requires_last_placeholder/
--rw-r--r--   0 test       (501) staff       (20)      105 2022-06-05 07:49:41.000000 django-app-requires-0.3.3/django_app_requires_last_placeholder/__init__.py
--rw-r--r--   0 test       (501) staff       (20)       63 2022-06-05 07:46:24.000000 django-app-requires-0.3.3/django_app_requires_last_placeholder/admin.py
--rw-r--r--   0 test       (501) staff       (20)      799 2023-09-13 06:50:39.000000 django-app-requires-0.3.3/django_app_requires_last_placeholder/apps.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 14:14:31.453244 django-app-requires-0.3.3/django_app_requires_last_placeholder/migrations/
--rw-r--r--   0 test       (501) staff       (20)        0 2022-06-05 07:46:24.000000 django-app-requires-0.3.3/django_app_requires_last_placeholder/migrations/__init__.py
--rw-r--r--   0 test       (501) staff       (20)       57 2022-06-05 07:46:24.000000 django-app-requires-0.3.3/django_app_requires_last_placeholder/models.py
--rw-r--r--   0 test       (501) staff       (20)       60 2022-06-05 07:46:24.000000 django-app-requires-0.3.3/django_app_requires_last_placeholder/tests.py
--rw-r--r--   0 test       (501) staff       (20)       63 2022-06-05 07:46:24.000000 django-app-requires-0.3.3/django_app_requires_last_placeholder/views.py
--rw-r--r--   0 test       (501) staff       (20)       20 2023-09-13 06:50:51.000000 django-app-requires-0.3.3/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2024-05-12 14:14:31.453556 django-app-requires-0.3.3/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1615 2024-05-12 14:08:48.000000 django-app-requires-0.3.3/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 12:44:31.091498 django-app-requires-0.3.4/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-12 14:09:22.000000 django-app-requires-0.3.4/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      308 2022-09-13 02:41:33.000000 django-app-requires-0.3.4/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     3379 2024-05-22 12:44:31.091383 django-app-requires-0.3.4/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     2535 2024-05-22 12:44:12.000000 django-app-requires-0.3.4/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 12:44:31.087419 django-app-requires-0.3.4/django_app_requires/
+-rw-r--r--   0 test       (501) staff       (20)      100 2022-06-01 13:00:11.000000 django-app-requires-0.3.4/django_app_requires/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)     3331 2023-09-13 06:50:31.000000 django-app-requires-0.3.4/django_app_requires/utils.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 12:44:31.088200 django-app-requires-0.3.4/django_app_requires.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     3379 2024-05-22 12:44:31.000000 django-app-requires-0.3.4/django_app_requires.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     1057 2024-05-22 12:44:31.000000 django-app-requires-0.3.4/django_app_requires.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-22 12:44:31.000000 django-app-requires-0.3.4/django_app_requires.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-22 12:44:31.000000 django-app-requires-0.3.4/django_app_requires.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)       16 2024-05-22 12:44:31.000000 django-app-requires-0.3.4/django_app_requires.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       95 2024-05-22 12:44:31.000000 django-app-requires-0.3.4/django_app_requires.egg-info/top_level.txt
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 12:44:31.089398 django-app-requires-0.3.4/django_app_requires_first_placeholder/
+-rw-r--r--   0 test       (501) staff       (20)      107 2022-06-05 13:04:20.000000 django-app-requires-0.3.4/django_app_requires_first_placeholder/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)       63 2022-06-05 13:03:42.000000 django-app-requires-0.3.4/django_app_requires_first_placeholder/admin.py
+-rw-r--r--   0 test       (501) staff       (20)     2408 2023-09-13 06:50:46.000000 django-app-requires-0.3.4/django_app_requires_first_placeholder/apps.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 12:44:31.089835 django-app-requires-0.3.4/django_app_requires_first_placeholder/migrations/
+-rw-r--r--   0 test       (501) staff       (20)        0 2022-06-05 13:03:42.000000 django-app-requires-0.3.4/django_app_requires_first_placeholder/migrations/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)       57 2022-06-05 13:03:42.000000 django-app-requires-0.3.4/django_app_requires_first_placeholder/models.py
+-rw-r--r--   0 test       (501) staff       (20)       60 2022-06-05 13:03:42.000000 django-app-requires-0.3.4/django_app_requires_first_placeholder/tests.py
+-rw-r--r--   0 test       (501) staff       (20)       63 2022-06-05 13:03:42.000000 django-app-requires-0.3.4/django_app_requires_first_placeholder/views.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 12:44:31.091061 django-app-requires-0.3.4/django_app_requires_last_placeholder/
+-rw-r--r--   0 test       (501) staff       (20)      105 2022-06-05 07:49:41.000000 django-app-requires-0.3.4/django_app_requires_last_placeholder/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)       63 2022-06-05 07:46:24.000000 django-app-requires-0.3.4/django_app_requires_last_placeholder/admin.py
+-rw-r--r--   0 test       (501) staff       (20)      799 2023-09-13 06:50:39.000000 django-app-requires-0.3.4/django_app_requires_last_placeholder/apps.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 12:44:31.091238 django-app-requires-0.3.4/django_app_requires_last_placeholder/migrations/
+-rw-r--r--   0 test       (501) staff       (20)        0 2022-06-05 07:46:24.000000 django-app-requires-0.3.4/django_app_requires_last_placeholder/migrations/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)       57 2022-06-05 07:46:24.000000 django-app-requires-0.3.4/django_app_requires_last_placeholder/models.py
+-rw-r--r--   0 test       (501) staff       (20)       60 2022-06-05 07:46:24.000000 django-app-requires-0.3.4/django_app_requires_last_placeholder/tests.py
+-rw-r--r--   0 test       (501) staff       (20)       63 2022-06-05 07:46:24.000000 django-app-requires-0.3.4/django_app_requires_last_placeholder/views.py
+-rw-r--r--   0 test       (501) staff       (20)       20 2023-09-13 06:50:51.000000 django-app-requires-0.3.4/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-05-22 12:44:31.091541 django-app-requires-0.3.4/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1615 2024-05-22 12:44:21.000000 django-app-requires-0.3.4/setup.py
```

### Comparing `django-app-requires-0.3.3/LICENSE` & `django-app-requires-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-app-requires-0.3.3/PKG-INFO` & `django-app-requires-0.3.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-app-requires
-Version: 0.3.3
+Version: 0.3.4
 Summary: A simple tool that allows you to specify app dependencies and middleware dependencies in your application, and also allow you to add default values for your additional configurations, after then load all your application settings into your project's settings.
 Home-page: UNKNOWN
 Author: Jin MinXiang
 Maintainer: Jin MinXiang
 License: MIT
 Keywords: django utils
 Platform: UNKNOWN
@@ -158,8 +158,12 @@
 - Doc update.
 - Use zenutils.
 
 ### v0.3.3
 
 - Doc update.
 
+### v0.3.4
+
+- Fix unit tests.
+
```

### Comparing `django-app-requires-0.3.3/README.md` & `django-app-requires-0.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -138,7 +138,11 @@
 
 - Doc update.
 - Use zenutils.
 
 ### v0.3.3
 
 - Doc update.
+
+### v0.3.4
+
+- Fix unit tests.
```

### Comparing `django-app-requires-0.3.3/django_app_requires/utils.py` & `django-app-requires-0.3.4/django_app_requires/utils.py`

 * *Files identical despite different names*

### Comparing `django-app-requires-0.3.3/django_app_requires.egg-info/PKG-INFO` & `django-app-requires-0.3.4/django_app_requires.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-app-requires
-Version: 0.3.3
+Version: 0.3.4
 Summary: A simple tool that allows you to specify app dependencies and middleware dependencies in your application, and also allow you to add default values for your additional configurations, after then load all your application settings into your project's settings.
 Home-page: UNKNOWN
 Author: Jin MinXiang
 Maintainer: Jin MinXiang
 License: MIT
 Keywords: django utils
 Platform: UNKNOWN
@@ -158,8 +158,12 @@
 - Doc update.
 - Use zenutils.
 
 ### v0.3.3
 
 - Doc update.
 
+### v0.3.4
+
+- Fix unit tests.
+
```

### Comparing `django-app-requires-0.3.3/django_app_requires.egg-info/SOURCES.txt` & `django-app-requires-0.3.4/django_app_requires.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-app-requires-0.3.3/django_app_requires_first_placeholder/apps.py` & `django-app-requires-0.3.4/django_app_requires_first_placeholder/apps.py`

 * *Files identical despite different names*

### Comparing `django-app-requires-0.3.3/django_app_requires_last_placeholder/apps.py` & `django-app-requires-0.3.4/django_app_requires_last_placeholder/apps.py`

 * *Files identical despite different names*

### Comparing `django-app-requires-0.3.3/setup.py` & `django-app-requires-0.3.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires = [x.strip() for x in fobj.readlines() if x.strip()]
 
 
 setup(
     name="django-app-requires",
-    version="0.3.3",
+    version="0.3.4",
     description="A simple tool that allows you to specify app dependencies and middleware dependencies in your application, and also allow you to add default values for your additional configurations, after then load all your application settings into your project's settings.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Jin MinXiang",
     maintainer="Jin MinXiang",
     license="MIT",
     classifiers=[
```

