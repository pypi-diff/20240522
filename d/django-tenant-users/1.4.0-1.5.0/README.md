# Comparing `tmp/django_tenant_users-1.4.0.tar.gz` & `tmp/django_tenant_users-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tenant_users-1.4.0.tar", max compression
+gzip compressed data, was "django_tenant_users-1.5.0.tar", max compression
```

## Comparing `django_tenant_users-1.4.0.tar` & `django_tenant_users-1.5.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1064 2021-12-17 15:19:01.356625 django_tenant_users-1.4.0/LICENSE
--rw-r--r--   0        0        0     2832 2023-09-15 20:47:08.781360 django_tenant_users-1.4.0/README.rst
--rw-r--r--   0        0        0     3417 2024-05-06 18:56:13.087663 django_tenant_users-1.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-12-17 15:19:01.362917 django_tenant_users-1.4.0/tenant_users/__init__.py
--rw-r--r--   0        0        0        0 2021-12-17 15:19:01.363033 django_tenant_users-1.4.0/tenant_users/permissions/__init__.py
--rw-r--r--   0        0        0     1036 2024-01-29 18:25:48.945680 django_tenant_users-1.4.0/tenant_users/permissions/backend.py
--rw-r--r--   0        0        0     1362 2024-01-29 18:25:48.946305 django_tenant_users-1.4.0/tenant_users/permissions/functional.py
--rw-r--r--   0        0        0     2942 2024-01-29 18:25:48.946835 django_tenant_users-1.4.0/tenant_users/permissions/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2021-12-17 15:19:01.363478 django_tenant_users-1.4.0/tenant_users/permissions/migrations/__init__.py
--rw-r--r--   0        0        0     5015 2024-01-29 22:22:06.353928 django_tenant_users-1.4.0/tenant_users/permissions/models.py
--rw-r--r--   0        0        0        0 2023-04-28 13:50:20.025905 django_tenant_users-1.4.0/tenant_users/tenants/__init__.py
--rw-r--r--   0        0        0      246 2023-09-13 21:56:22.327540 django_tenant_users-1.4.0/tenant_users/tenants/apps.py
--rw-r--r--   0        0        0        0 2024-05-06 18:35:34.990779 django_tenant_users-1.4.0/tenant_users/tenants/management/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:35:34.990900 django_tenant_users-1.4.0/tenant_users/tenants/management/commands/__init__.py
--rw-r--r--   0        0        0     1211 2024-05-06 18:35:34.991010 django_tenant_users-1.4.0/tenant_users/tenants/management/commands/create_public_tenant.py
--rw-r--r--   0        0        0        0 2021-12-17 15:19:01.364097 django_tenant_users-1.4.0/tenant_users/tenants/migrations/__init__.py
--rw-r--r--   0        0        0    14376 2024-02-03 15:47:21.153320 django_tenant_users-1.4.0/tenant_users/tenants/models.py
--rw-r--r--   0        0        0     4254 2024-02-03 15:47:21.154016 django_tenant_users-1.4.0/tenant_users/tenants/tasks.py
--rw-r--r--   0        0        0     3413 2024-02-03 15:47:21.154539 django_tenant_users-1.4.0/tenant_users/tenants/utils.py
--rw-r--r--   0        0        0     4122 1970-01-01 00:00:00.000000 django_tenant_users-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2021-12-17 15:19:01.356625 django_tenant_users-1.5.0/LICENSE
+-rw-r--r--   0        0        0     2832 2023-09-15 20:47:08.781360 django_tenant_users-1.5.0/README.rst
+-rw-r--r--   0        0        0     3417 2024-05-22 18:37:28.976063 django_tenant_users-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-12-17 15:19:01.362917 django_tenant_users-1.5.0/tenant_users/__init__.py
+-rw-r--r--   0        0        0        0 2021-12-17 15:19:01.363033 django_tenant_users-1.5.0/tenant_users/permissions/__init__.py
+-rw-r--r--   0        0        0     1036 2024-05-19 21:50:48.921700 django_tenant_users-1.5.0/tenant_users/permissions/backend.py
+-rw-r--r--   0        0        0     1362 2024-01-29 18:25:48.946305 django_tenant_users-1.5.0/tenant_users/permissions/functional.py
+-rw-r--r--   0        0        0     2942 2024-01-29 18:25:48.946835 django_tenant_users-1.5.0/tenant_users/permissions/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2021-12-17 15:19:01.363478 django_tenant_users-1.5.0/tenant_users/permissions/migrations/__init__.py
+-rw-r--r--   0        0        0     5015 2024-01-29 22:22:06.353928 django_tenant_users-1.5.0/tenant_users/permissions/models.py
+-rw-r--r--   0        0        0        0 2023-04-28 13:50:20.025905 django_tenant_users-1.5.0/tenant_users/tenants/__init__.py
+-rw-r--r--   0        0        0      246 2023-09-13 21:56:22.327540 django_tenant_users-1.5.0/tenant_users/tenants/apps.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:35:34.990779 django_tenant_users-1.5.0/tenant_users/tenants/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:35:34.990900 django_tenant_users-1.5.0/tenant_users/tenants/management/commands/__init__.py
+-rw-r--r--   0        0        0     1211 2024-05-06 18:35:34.991010 django_tenant_users-1.5.0/tenant_users/tenants/management/commands/create_public_tenant.py
+-rw-r--r--   0        0        0     2062 2024-05-19 21:50:25.994823 django_tenant_users-1.5.0/tenant_users/tenants/middleware.py
+-rw-r--r--   0        0        0        0 2021-12-17 15:19:01.364097 django_tenant_users-1.5.0/tenant_users/tenants/migrations/__init__.py
+-rw-r--r--   0        0        0    14376 2024-05-19 21:50:48.922390 django_tenant_users-1.5.0/tenant_users/tenants/models.py
+-rw-r--r--   0        0        0     4254 2024-02-03 15:47:21.154016 django_tenant_users-1.5.0/tenant_users/tenants/tasks.py
+-rw-r--r--   0        0        0     3413 2024-02-03 15:47:21.154539 django_tenant_users-1.5.0/tenant_users/tenants/utils.py
+-rw-r--r--   0        0        0     4122 1970-01-01 00:00:00.000000 django_tenant_users-1.5.0/PKG-INFO
```

### Comparing `django_tenant_users-1.4.0/LICENSE` & `django_tenant_users-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_tenant_users-1.4.0/README.rst` & `django_tenant_users-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `django_tenant_users-1.4.0/pyproject.toml` & `django_tenant_users-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 target-version = ['py38', 'py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
 
 
 [tool.poetry]
 name = "django-tenant-users"
 description = "A Django app to extend django-tenants to incorporate global multi-tenant users"
-version = "1.4.0"
+version = "1.5.0"
 license = "MIT License"
 
 packages = [
   { include = 'tenant_users' },
 ]
 
 authors = [
```

### Comparing `django_tenant_users-1.4.0/tenant_users/permissions/backend.py` & `django_tenant_users-1.5.0/tenant_users/permissions/backend.py`

 * *Files identical despite different names*

### Comparing `django_tenant_users-1.4.0/tenant_users/permissions/functional.py` & `django_tenant_users-1.5.0/tenant_users/permissions/functional.py`

 * *Files identical despite different names*

### Comparing `django_tenant_users-1.4.0/tenant_users/permissions/migrations/0001_initial.py` & `django_tenant_users-1.5.0/tenant_users/permissions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_tenant_users-1.4.0/tenant_users/permissions/models.py` & `django_tenant_users-1.5.0/tenant_users/permissions/models.py`

 * *Files identical despite different names*

### Comparing `django_tenant_users-1.4.0/tenant_users/tenants/management/commands/create_public_tenant.py` & `django_tenant_users-1.5.0/tenant_users/tenants/management/commands/create_public_tenant.py`

 * *Files identical despite different names*

### Comparing `django_tenant_users-1.4.0/tenant_users/tenants/models.py` & `django_tenant_users-1.5.0/tenant_users/tenants/models.py`

 * *Files identical despite different names*

### Comparing `django_tenant_users-1.4.0/tenant_users/tenants/tasks.py` & `django_tenant_users-1.5.0/tenant_users/tenants/tasks.py`

 * *Files identical despite different names*

### Comparing `django_tenant_users-1.4.0/tenant_users/tenants/utils.py` & `django_tenant_users-1.5.0/tenant_users/tenants/utils.py`

 * *Files identical despite different names*

### Comparing `django_tenant_users-1.4.0/PKG-INFO` & `django_tenant_users-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tenant-users
-Version: 1.4.0
+Version: 1.5.0
 Summary: A Django app to extend django-tenants to incorporate global multi-tenant users
 Home-page: https://www.github.com/Corvia/django-tenant-users
 License: MIT
 Keywords: django,django-tenant-users
 Author: Corvia Technologies, LLC
 Author-email: support@corvia.tech
 Requires-Python: >=3.8.1,<4.0.0
```

