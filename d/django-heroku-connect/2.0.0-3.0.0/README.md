# Comparing `tmp/django_heroku_connect-2.0.0.tar.gz` & `tmp/django_heroku_connect-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_heroku_connect-2.0.0.tar", max compression
+gzip compressed data, was "django_heroku_connect-3.0.0.tar", max compression
```

## Comparing `django_heroku_connect-2.0.0.tar` & `django_heroku_connect-3.0.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    11357 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/LICENSE
--rw-r--r--   0        0        0     1019 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/README.rst
--rw-r--r--   0        0        0      370 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/__init__.py
--rw-r--r--   0        0        0     6630 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/admin.py
--rw-r--r--   0        0        0      462 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/apps.py
--rw-r--r--   0        0        0     3752 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/checks.py
--rw-r--r--   0        0        0     2773 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/conf.py
--rw-r--r--   0        0        0        0 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/contrib/__init__.py
--rw-r--r--   0        0        0      384 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/contrib/heroku_connect_health_check/__init__.py
--rw-r--r--   0        0        0      312 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/contrib/heroku_connect_health_check/apps.py
--rw-r--r--   0        0        0     1516 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/contrib/heroku_connect_health_check/backends.py
--rw-r--r--   0        0        0        0 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/db/__init__.py
--rw-r--r--   0        0        0        0 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/db/backends/__init__.py
--rw-r--r--   0        0        0        0 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/db/backends/base/__init__.py
--rw-r--r--   0        0        0      497 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/db/backends/base/base.py
--rw-r--r--   0        0        0      604 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/db/backends/base/creation.py
--rw-r--r--   0        0        0        0 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/db/backends/postgis/__init__.py
--rw-r--r--   0        0        0      291 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/db/backends/postgis/base.py
--rw-r--r--   0        0        0        0 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/db/backends/postgresql/__init__.py
--rw-r--r--   0        0        0      270 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/db/backends/postgresql/base.py
--rw-r--r--   0        0        0      193 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/db/exceptions.py
--rw-r--r--   0        0        0       89 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/db/models/__init__.py
--rw-r--r--   0        0        0    10967 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/db/models/base.py
--rw-r--r--   0        0        0     8854 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/db/models/fields.py
--rw-r--r--   0        0        0      700 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/db/models/related.py
--rw-r--r--   0        0        0     1221 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/db/router.py
--rw-r--r--   0        0        0        0 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/management/__init__.py
--rw-r--r--   0        0        0        0 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/management/commands/__init__.py
--rw-r--r--   0        0        0     1347 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/management/commands/create_development_schema.py
--rw-r--r--   0        0        0     5088 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/management/commands/import_mappings.py
--rw-r--r--   0        0        0     2924 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/management/commands/load_remote_schema.py
--rw-r--r--   0        0        0      980 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/management/commands/makemappings.py
--rw-r--r--   0        0        0     6410 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/migrations/__init__.py
--rw-r--r--   0        0        0    15167 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/models.py
--rw-r--r--   0        0        0      462 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/test/__init__.py
--rw-r--r--   0        0        0     2224 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/test/utils.py
--rw-r--r--   0        0        0     9535 2023-09-05 08:49:53.318993 django_heroku_connect-2.0.0/heroku_connect/utils.py
--rw-r--r--   0        0        0     1723 2023-09-05 08:50:09.955285 django_heroku_connect-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     2255 1970-01-01 00:00:00.000000 django_heroku_connect-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-22 11:33:55.586321 django_heroku_connect-3.0.0/LICENSE
+-rw-r--r--   0        0        0     1019 2024-05-22 11:33:55.586321 django_heroku_connect-3.0.0/README.rst
+-rw-r--r--   0        0        0      370 2024-05-22 11:33:55.586321 django_heroku_connect-3.0.0/heroku_connect/__init__.py
+-rw-r--r--   0        0        0     6630 2024-05-22 11:33:55.586321 django_heroku_connect-3.0.0/heroku_connect/admin.py
+-rw-r--r--   0        0        0      462 2024-05-22 11:33:55.586321 django_heroku_connect-3.0.0/heroku_connect/apps.py
+-rw-r--r--   0        0        0     3752 2024-05-22 11:33:55.586321 django_heroku_connect-3.0.0/heroku_connect/checks.py
+-rw-r--r--   0        0        0     2773 2024-05-22 11:33:55.586321 django_heroku_connect-3.0.0/heroku_connect/conf.py
+-rw-r--r--   0        0        0        0 2024-05-22 11:33:55.586321 django_heroku_connect-3.0.0/heroku_connect/contrib/__init__.py
+-rw-r--r--   0        0        0      384 2024-05-22 11:33:55.586321 django_heroku_connect-3.0.0/heroku_connect/contrib/heroku_connect_health_check/__init__.py
+-rw-r--r--   0        0        0      312 2024-05-22 11:33:55.586321 django_heroku_connect-3.0.0/heroku_connect/contrib/heroku_connect_health_check/apps.py
+-rw-r--r--   0        0        0     1516 2024-05-22 11:33:55.586321 django_heroku_connect-3.0.0/heroku_connect/contrib/heroku_connect_health_check/backends.py
+-rw-r--r--   0        0        0        0 2024-05-22 11:33:55.586321 django_heroku_connect-3.0.0/heroku_connect/db/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 11:33:55.586321 django_heroku_connect-3.0.0/heroku_connect/db/backends/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 11:33:55.586321 django_heroku_connect-3.0.0/heroku_connect/db/backends/base/__init__.py
+-rw-r--r--   0        0        0      497 2024-05-22 11:33:55.586321 django_heroku_connect-3.0.0/heroku_connect/db/backends/base/base.py
+-rw-r--r--   0        0        0      604 2024-05-22 11:33:55.586321 django_heroku_connect-3.0.0/heroku_connect/db/backends/base/creation.py
+-rw-r--r--   0        0        0        0 2024-05-22 11:33:55.586321 django_heroku_connect-3.0.0/heroku_connect/db/backends/postgis/__init__.py
+-rw-r--r--   0        0        0      291 2024-05-22 11:33:55.586321 django_heroku_connect-3.0.0/heroku_connect/db/backends/postgis/base.py
+-rw-r--r--   0        0        0        0 2024-05-22 11:33:55.586321 django_heroku_connect-3.0.0/heroku_connect/db/backends/postgresql/__init__.py
+-rw-r--r--   0        0        0      270 2024-05-22 11:33:55.586321 django_heroku_connect-3.0.0/heroku_connect/db/backends/postgresql/base.py
+-rw-r--r--   0        0        0      193 2024-05-22 11:33:55.586321 django_heroku_connect-3.0.0/heroku_connect/db/exceptions.py
+-rw-r--r--   0        0        0       89 2024-05-22 11:33:55.586321 django_heroku_connect-3.0.0/heroku_connect/db/models/__init__.py
+-rw-r--r--   0        0        0    10967 2024-05-22 11:33:55.590321 django_heroku_connect-3.0.0/heroku_connect/db/models/base.py
+-rw-r--r--   0        0        0     8854 2024-05-22 11:33:55.590321 django_heroku_connect-3.0.0/heroku_connect/db/models/fields.py
+-rw-r--r--   0        0        0      700 2024-05-22 11:33:55.590321 django_heroku_connect-3.0.0/heroku_connect/db/models/related.py
+-rw-r--r--   0        0        0     1221 2024-05-22 11:33:55.590321 django_heroku_connect-3.0.0/heroku_connect/db/router.py
+-rw-r--r--   0        0        0        0 2024-05-22 11:33:55.590321 django_heroku_connect-3.0.0/heroku_connect/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 11:33:55.590321 django_heroku_connect-3.0.0/heroku_connect/management/commands/__init__.py
+-rw-r--r--   0        0        0     1347 2024-05-22 11:33:55.590321 django_heroku_connect-3.0.0/heroku_connect/management/commands/create_development_schema.py
+-rw-r--r--   0        0        0     5088 2024-05-22 11:33:55.590321 django_heroku_connect-3.0.0/heroku_connect/management/commands/import_mappings.py
+-rw-r--r--   0        0        0     2924 2024-05-22 11:33:55.590321 django_heroku_connect-3.0.0/heroku_connect/management/commands/load_remote_schema.py
+-rw-r--r--   0        0        0      980 2024-05-22 11:33:55.590321 django_heroku_connect-3.0.0/heroku_connect/management/commands/makemappings.py
+-rw-r--r--   0        0        0     6410 2024-05-22 11:33:55.590321 django_heroku_connect-3.0.0/heroku_connect/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-22 11:33:55.590321 django_heroku_connect-3.0.0/heroku_connect/migrations/__init__.py
+-rw-r--r--   0        0        0    15167 2024-05-22 11:33:55.590321 django_heroku_connect-3.0.0/heroku_connect/models.py
+-rw-r--r--   0        0        0      462 2024-05-22 11:33:55.590321 django_heroku_connect-3.0.0/heroku_connect/test/__init__.py
+-rw-r--r--   0        0        0     2224 2024-05-22 11:33:55.590321 django_heroku_connect-3.0.0/heroku_connect/test/utils.py
+-rw-r--r--   0        0        0     9535 2024-05-22 11:33:55.590321 django_heroku_connect-3.0.0/heroku_connect/utils.py
+-rw-r--r--   0        0        0     1723 2024-05-22 11:34:09.694288 django_heroku_connect-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2306 1970-01-01 00:00:00.000000 django_heroku_connect-3.0.0/PKG-INFO
```

### Comparing `django_heroku_connect-2.0.0/LICENSE` & `django_heroku_connect-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_heroku_connect-2.0.0/README.rst` & `django_heroku_connect-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `django_heroku_connect-2.0.0/heroku_connect/admin.py` & `django_heroku_connect-3.0.0/heroku_connect/admin.py`

 * *Files identical despite different names*

### Comparing `django_heroku_connect-2.0.0/heroku_connect/checks.py` & `django_heroku_connect-3.0.0/heroku_connect/checks.py`

 * *Files identical despite different names*

### Comparing `django_heroku_connect-2.0.0/heroku_connect/conf.py` & `django_heroku_connect-3.0.0/heroku_connect/conf.py`

 * *Files identical despite different names*

### Comparing `django_heroku_connect-2.0.0/heroku_connect/contrib/heroku_connect_health_check/backends.py` & `django_heroku_connect-3.0.0/heroku_connect/contrib/heroku_connect_health_check/backends.py`

 * *Files identical despite different names*

### Comparing `django_heroku_connect-2.0.0/heroku_connect/db/backends/base/creation.py` & `django_heroku_connect-3.0.0/heroku_connect/db/backends/base/creation.py`

 * *Files identical despite different names*

### Comparing `django_heroku_connect-2.0.0/heroku_connect/db/models/base.py` & `django_heroku_connect-3.0.0/heroku_connect/db/models/base.py`

 * *Files identical despite different names*

### Comparing `django_heroku_connect-2.0.0/heroku_connect/db/models/fields.py` & `django_heroku_connect-3.0.0/heroku_connect/db/models/fields.py`

 * *Files identical despite different names*

### Comparing `django_heroku_connect-2.0.0/heroku_connect/db/models/related.py` & `django_heroku_connect-3.0.0/heroku_connect/db/models/related.py`

 * *Files identical despite different names*

### Comparing `django_heroku_connect-2.0.0/heroku_connect/db/router.py` & `django_heroku_connect-3.0.0/heroku_connect/db/router.py`

 * *Files identical despite different names*

### Comparing `django_heroku_connect-2.0.0/heroku_connect/management/commands/create_development_schema.py` & `django_heroku_connect-3.0.0/heroku_connect/management/commands/create_development_schema.py`

 * *Files identical despite different names*

### Comparing `django_heroku_connect-2.0.0/heroku_connect/management/commands/import_mappings.py` & `django_heroku_connect-3.0.0/heroku_connect/management/commands/import_mappings.py`

 * *Files identical despite different names*

### Comparing `django_heroku_connect-2.0.0/heroku_connect/management/commands/load_remote_schema.py` & `django_heroku_connect-3.0.0/heroku_connect/management/commands/load_remote_schema.py`

 * *Files identical despite different names*

### Comparing `django_heroku_connect-2.0.0/heroku_connect/management/commands/makemappings.py` & `django_heroku_connect-3.0.0/heroku_connect/management/commands/makemappings.py`

 * *Files identical despite different names*

### Comparing `django_heroku_connect-2.0.0/heroku_connect/migrations/0001_initial.py` & `django_heroku_connect-3.0.0/heroku_connect/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_heroku_connect-2.0.0/heroku_connect/models.py` & `django_heroku_connect-3.0.0/heroku_connect/models.py`

 * *Files identical despite different names*

### Comparing `django_heroku_connect-2.0.0/heroku_connect/test/utils.py` & `django_heroku_connect-3.0.0/heroku_connect/test/utils.py`

 * *Files identical despite different names*

### Comparing `django_heroku_connect-2.0.0/heroku_connect/utils.py` & `django_heroku_connect-3.0.0/heroku_connect/utils.py`

 * *Files identical despite different names*

### Comparing `django_heroku_connect-2.0.0/pyproject.toml` & `django_heroku_connect-3.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "django-heroku-connect"
 # just a dummy version
 # will be overwritten from the git tag,
 # see https://github.com/mtkennerly/poetry-dynamic-versioning
-version = "2.0.0"
+version = "3.0.0"
 description = "Django integration Salesforce using Heroku Connect."
 authors = ["thermondo <opensource@thermondo.de>"]
 readme = "README.rst"
 repository = "https://github.com/thermondo/django-heroku-connect"
 documentation = "https://django-heroku-connect.readthedocs.io/"
 license = "Apache-2.0"
 keywords = ["heroku", "salesforce", "django"]
@@ -22,15 +22,15 @@
   "Programming Language :: Python :: 3",
   "Framework :: Django",
 ]
 packages = [{ include = "heroku_connect" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
-django = ">=3.2,<4.3"
+django = ">=4.2,<5.1"
 django-appconf = "~1"
 requests = "~2"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "!=1.6.3,!=1.7.0"
 black = "*"
 coverage = "*"
```

### Comparing `django_heroku_connect-2.0.0/PKG-INFO` & `django_heroku_connect-3.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-heroku-connect
-Version: 2.0.0
+Version: 3.0.0
 Summary: Django integration Salesforce using Heroku Connect.
 Home-page: https://github.com/thermondo/django-heroku-connect
 License: Apache-2.0
 Keywords: heroku,salesforce,django
 Author: thermondo
 Author-email: opensource@thermondo.de
 Requires-Python: >=3.8,<4.0
@@ -17,15 +17,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: django (>=3.2,<4.3)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: django (>=4.2,<5.1)
 Requires-Dist: django-appconf (>=1,<2)
 Requires-Dist: requests (>=2,<3)
 Project-URL: Documentation, https://django-heroku-connect.readthedocs.io/
 Project-URL: Repository, https://github.com/thermondo/django-heroku-connect
 Description-Content-Type: text/x-rst
 
 |version| |ci| |coverage| |license|
```

