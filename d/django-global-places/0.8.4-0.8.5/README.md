# Comparing `tmp/django_global_places-0.8.4.tar.gz` & `tmp/django_global_places-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_global_places-0.8.4.tar", last modified: Mon May  6 09:18:17 2024, max compression
+gzip compressed data, was "django_global_places-0.8.5.tar", last modified: Wed May 22 14:45:17 2024, max compression
```

## Comparing `django_global_places-0.8.4.tar` & `django_global_places-0.8.5.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 09:18:17.801533 django_global_places-0.8.4/
--rw-rw-rw-   0        0        0       63 2024-03-30 19:07:36.000000 django_global_places-0.8.4/AUTHORS
--rw-rw-rw-   0        0        0     1137 2024-03-30 19:22:19.000000 django_global_places-0.8.4/LICENSE
--rw-rw-rw-   0        0        0     4009 2024-05-06 09:18:17.800023 django_global_places-0.8.4/PKG-INFO
--rw-rw-rw-   0        0        0     3347 2024-03-30 19:07:36.000000 django_global_places-0.8.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 09:18:17.747264 django_global_places-0.8.4/django_global_places/
--rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/__init__.py
--rw-rw-rw-   0        0        0      429 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/__version__.py
--rw-rw-rw-   0        0        0     2157 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/abstract_models.py
--rw-rw-rw-   0        0        0     1217 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/admin.py
--rw-rw-rw-   0        0        0     1175 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/app_settings.py
--rw-rw-rw-   0        0        0      219 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/apps.py
-drwxrwxrwx   0        0        0        0 2024-05-06 09:18:17.783491 django_global_places-0.8.4/django_global_places/management/
--rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/management/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 09:18:17.786506 django_global_places-0.8.4/django_global_places/management/commands/
--rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/management/commands/__init__.py
--rw-rw-rw-   0        0        0    12320 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/management/commands/populate_global_places.py
-drwxrwxrwx   0        0        0        0 2024-05-06 09:18:17.787510 django_global_places-0.8.4/django_global_places/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/migrations/__init__.py
--rw-rw-rw-   0        0        0      739 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/models.py
-drwxrwxrwx   0        0        0        0 2024-05-06 09:18:17.793035 django_global_places-0.8.4/django_global_places/serializers/
--rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/serializers/__init__.py
--rw-rw-rw-   0        0        0      676 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/serializers/cities.py
--rw-rw-rw-   0        0        0      617 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/serializers/countries.py
--rw-rw-rw-   0        0        0      702 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/serializers/states.py
--rw-rw-rw-   0        0        0      711 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/urls.py
--rw-rw-rw-   0        0        0      662 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-06 09:18:17.799018 django_global_places-0.8.4/django_global_places/views/
--rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/views/__init__.py
--rw-rw-rw-   0        0        0     1438 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/views/cities.py
--rw-rw-rw-   0        0        0      999 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/views/countries.py
--rw-rw-rw-   0        0        0     1412 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/views/states.py
--rw-rw-rw-   0        0        0      859 2024-03-30 19:10:41.000000 django_global_places-0.8.4/django_global_places/viewsets_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-06 09:18:17.780207 django_global_places-0.8.4/django_global_places.egg-info/
--rw-rw-rw-   0        0        0     4009 2024-05-06 09:18:17.000000 django_global_places-0.8.4/django_global_places.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1168 2024-05-06 09:18:17.000000 django_global_places-0.8.4/django_global_places.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 09:18:17.000000 django_global_places-0.8.4/django_global_places.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-06 09:18:17.000000 django_global_places-0.8.4/django_global_places.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       43 2024-05-06 09:18:17.000000 django_global_places-0.8.4/django_global_places.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-05-06 09:18:17.000000 django_global_places-0.8.4/django_global_places.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 09:18:17.802550 django_global_places-0.8.4/setup.cfg
--rw-rw-rw-   0        0        0     1202 2024-03-30 19:07:36.000000 django_global_places-0.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:45:17.325307 django_global_places-0.8.5/
+-rw-rw-rw-   0        0        0       63 2024-03-30 19:07:36.000000 django_global_places-0.8.5/AUTHORS
+-rw-rw-rw-   0        0        0     1137 2024-03-30 19:22:19.000000 django_global_places-0.8.5/LICENSE
+-rw-rw-rw-   0        0        0     4009 2024-05-22 14:45:17.324293 django_global_places-0.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3347 2024-03-30 19:07:36.000000 django_global_places-0.8.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 14:45:17.267869 django_global_places-0.8.5/django_global_places/
+-rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/__init__.py
+-rw-rw-rw-   0        0        0      429 2024-05-22 13:46:18.000000 django_global_places-0.8.5/django_global_places/__version__.py
+-rw-rw-rw-   0        0        0     2157 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/abstract_models.py
+-rw-rw-rw-   0        0        0     1217 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/admin.py
+-rw-rw-rw-   0        0        0     1175 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/app_settings.py
+-rw-rw-rw-   0        0        0      219 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:45:17.304449 django_global_places-0.8.5/django_global_places/management/
+-rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/management/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:45:17.306708 django_global_places-0.8.5/django_global_places/management/commands/
+-rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/management/commands/__init__.py
+-rw-rw-rw-   0        0        0    12320 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/management/commands/populate_global_places.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:45:17.310707 django_global_places-0.8.5/django_global_places/migrations/
+-rw-rw-rw-   0        0        0     5205 2024-05-22 14:43:55.000000 django_global_places-0.8.5/django_global_places/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/migrations/__init__.py
+-rw-rw-rw-   0        0        0      739 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/models.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:45:17.316235 django_global_places-0.8.5/django_global_places/serializers/
+-rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/serializers/__init__.py
+-rw-rw-rw-   0        0        0      676 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/serializers/cities.py
+-rw-rw-rw-   0        0        0      617 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/serializers/countries.py
+-rw-rw-rw-   0        0        0      702 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/serializers/states.py
+-rw-rw-rw-   0        0        0      711 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/urls.py
+-rw-rw-rw-   0        0        0      662 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:45:17.322778 django_global_places-0.8.5/django_global_places/views/
+-rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/views/__init__.py
+-rw-rw-rw-   0        0        0     1438 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/views/cities.py
+-rw-rw-rw-   0        0        0      999 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/views/countries.py
+-rw-rw-rw-   0        0        0     1412 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/views/states.py
+-rw-rw-rw-   0        0        0      859 2024-03-30 19:10:41.000000 django_global_places-0.8.5/django_global_places/viewsets_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:45:17.302448 django_global_places-0.8.5/django_global_places.egg-info/
+-rw-rw-rw-   0        0        0     4009 2024-05-22 14:45:17.000000 django_global_places-0.8.5/django_global_places.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1216 2024-05-22 14:45:17.000000 django_global_places-0.8.5/django_global_places.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 14:45:17.000000 django_global_places-0.8.5/django_global_places.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-06 09:18:17.000000 django_global_places-0.8.5/django_global_places.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       43 2024-05-22 14:45:17.000000 django_global_places-0.8.5/django_global_places.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-22 14:45:17.000000 django_global_places-0.8.5/django_global_places.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 14:45:17.326308 django_global_places-0.8.5/setup.cfg
+-rw-rw-rw-   0        0        0     1202 2024-03-30 19:07:36.000000 django_global_places-0.8.5/setup.py
```

### Comparing `django_global_places-0.8.4/LICENSE` & `django_global_places-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.4/PKG-INFO` & `django_global_places-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_global_places
-Version: 0.8.4
+Version: 0.8.5
 Summary: Django Global Places is a simple Django app to provide a model for global places.
 Home-page: https://github.com/lucacitta/Django-GlobalPlaces
 Author: lucacitta
 Author-email: lucacitta.dev@gmail.com
 License: MIT
 Keywords: django global places
 Classifier: Framework :: Django
```

### Comparing `django_global_places-0.8.4/README.md` & `django_global_places-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.4/django_global_places/abstract_models.py` & `django_global_places-0.8.5/django_global_places/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.4/django_global_places/admin.py` & `django_global_places-0.8.5/django_global_places/admin.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.4/django_global_places/app_settings.py` & `django_global_places-0.8.5/django_global_places/app_settings.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.4/django_global_places/management/commands/populate_global_places.py` & `django_global_places-0.8.5/django_global_places/management/commands/populate_global_places.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.4/django_global_places/models.py` & `django_global_places-0.8.5/django_global_places/models.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.4/django_global_places/serializers/cities.py` & `django_global_places-0.8.5/django_global_places/serializers/cities.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.4/django_global_places/serializers/countries.py` & `django_global_places-0.8.5/django_global_places/serializers/countries.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.4/django_global_places/serializers/states.py` & `django_global_places-0.8.5/django_global_places/serializers/states.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.4/django_global_places/urls.py` & `django_global_places-0.8.5/django_global_places/urls.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.4/django_global_places/utils.py` & `django_global_places-0.8.5/django_global_places/utils.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.4/django_global_places/views/cities.py` & `django_global_places-0.8.5/django_global_places/views/cities.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.4/django_global_places/views/countries.py` & `django_global_places-0.8.5/django_global_places/views/countries.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.4/django_global_places/views/states.py` & `django_global_places-0.8.5/django_global_places/views/states.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.4/django_global_places/viewsets_utils.py` & `django_global_places-0.8.5/django_global_places/viewsets_utils.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.4/django_global_places.egg-info/PKG-INFO` & `django_global_places-0.8.5/django_global_places.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-global-places
-Version: 0.8.4
+Version: 0.8.5
 Summary: Django Global Places is a simple Django app to provide a model for global places.
 Home-page: https://github.com/lucacitta/Django-GlobalPlaces
 Author: lucacitta
 Author-email: lucacitta.dev@gmail.com
 License: MIT
 Keywords: django global places
 Classifier: Framework :: Django
```

### Comparing `django_global_places-0.8.4/django_global_places.egg-info/SOURCES.txt` & `django_global_places-0.8.5/django_global_places.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 django_global_places.egg-info/dependency_links.txt
 django_global_places.egg-info/not-zip-safe
 django_global_places.egg-info/requires.txt
 django_global_places.egg-info/top_level.txt
 django_global_places/management/__init__.py
 django_global_places/management/commands/__init__.py
 django_global_places/management/commands/populate_global_places.py
+django_global_places/migrations/0001_initial.py
 django_global_places/migrations/__init__.py
 django_global_places/serializers/__init__.py
 django_global_places/serializers/cities.py
 django_global_places/serializers/countries.py
 django_global_places/serializers/states.py
 django_global_places/views/__init__.py
 django_global_places/views/cities.py
```

### Comparing `django_global_places-0.8.4/setup.py` & `django_global_places-0.8.5/setup.py`

 * *Files identical despite different names*

