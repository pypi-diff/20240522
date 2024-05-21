# Comparing `tmp/reflex-local-auth-0.1.2.tar.gz` & `tmp/reflex_local_auth-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-local-auth-0.1.2.tar", last modified: Thu Apr 11 13:59:23 2024, max compression
+gzip compressed data, was "reflex_local_auth-0.2.0.tar", last modified: Tue May 21 23:04:03 2024, max compression
```

## Comparing `reflex-local-auth-0.1.2.tar` & `reflex_local_auth-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:59:23.182590 reflex-local-auth-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-04-11 13:59:23.182590 reflex-local-auth-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-04-11 13:58:41.000000 reflex-local-auth-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:59:23.178590 reflex-local-auth-0.1.2/custom_components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:59:23.178590 reflex-local-auth-0.1.2/custom_components/reflex_local_auth/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-11 13:58:41.000000 reflex-local-auth-0.1.2/custom_components/reflex_local_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-11 13:58:41.000000 reflex-local-auth-0.1.2/custom_components/reflex_local_auth/auth_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-11 13:58:41.000000 reflex-local-auth-0.1.2/custom_components/reflex_local_auth/local_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-11 13:58:41.000000 reflex-local-auth-0.1.2/custom_components/reflex_local_auth/login.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:59:23.182590 reflex-local-auth-0.1.2/custom_components/reflex_local_auth/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-11 13:58:41.000000 reflex-local-auth-0.1.2/custom_components/reflex_local_auth/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-11 13:58:41.000000 reflex-local-auth-0.1.2/custom_components/reflex_local_auth/pages/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-11 13:58:41.000000 reflex-local-auth-0.1.2/custom_components/reflex_local_auth/pages/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-11 13:58:41.000000 reflex-local-auth-0.1.2/custom_components/reflex_local_auth/pages/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-11 13:58:41.000000 reflex-local-auth-0.1.2/custom_components/reflex_local_auth/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-11 13:58:41.000000 reflex-local-auth-0.1.2/custom_components/reflex_local_auth/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-11 13:58:41.000000 reflex-local-auth-0.1.2/custom_components/reflex_local_auth/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:59:23.182590 reflex-local-auth-0.1.2/custom_components/reflex_local_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-04-11 13:59:23.000000 reflex-local-auth-0.1.2/custom_components/reflex_local_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-11 13:59:23.000000 reflex-local-auth-0.1.2/custom_components/reflex_local_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:59:23.000000 reflex-local-auth-0.1.2/custom_components/reflex_local_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-11 13:59:23.000000 reflex-local-auth-0.1.2/custom_components/reflex_local_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 13:59:23.000000 reflex-local-auth-0.1.2/custom_components/reflex_local_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-11 13:58:41.000000 reflex-local-auth-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:59:23.182590 reflex-local-auth-0.1.2/setup.cfg
+drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-05-21 23:04:03.566234 reflex_local_auth-0.2.0/
+-rw-r--r--   0 masen      (502) staff       (20)     8119 2024-05-21 23:04:03.566054 reflex_local_auth-0.2.0/PKG-INFO
+-rw-r--r--   0 masen      (502) staff       (20)     7576 2024-05-09 02:46:02.000000 reflex_local_auth-0.2.0/README.md
+drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-05-21 23:04:03.562128 reflex_local_auth-0.2.0/custom_components/
+drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-05-21 23:04:03.564135 reflex_local_auth-0.2.0/custom_components/reflex_local_auth/
+-rw-r--r--   0 masen      (502) staff       (20)      447 2024-05-09 02:46:02.000000 reflex_local_auth-0.2.0/custom_components/reflex_local_auth/__init__.py
+-rw-r--r--   0 masen      (502) staff       (20)      512 2024-05-09 02:46:02.000000 reflex_local_auth-0.2.0/custom_components/reflex_local_auth/auth_session.py
+-rw-r--r--   0 masen      (502) staff       (20)     3397 2024-05-09 02:46:02.000000 reflex_local_auth-0.2.0/custom_components/reflex_local_auth/local_auth.py
+-rw-r--r--   0 masen      (502) staff       (20)     2946 2024-05-09 02:46:02.000000 reflex_local_auth-0.2.0/custom_components/reflex_local_auth/login.py
+drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-05-21 23:04:03.565554 reflex_local_auth-0.2.0/custom_components/reflex_local_auth/pages/
+-rw-r--r--   0 masen      (502) staff       (20)      152 2024-03-22 12:09:53.000000 reflex_local_auth-0.2.0/custom_components/reflex_local_auth/pages/__init__.py
+-rw-r--r--   0 masen      (502) staff       (20)      348 2024-05-09 02:45:36.000000 reflex_local_auth-0.2.0/custom_components/reflex_local_auth/pages/components.py
+-rw-r--r--   0 masen      (502) staff       (20)     1587 2024-05-09 02:46:02.000000 reflex_local_auth-0.2.0/custom_components/reflex_local_auth/pages/login.py
+-rw-r--r--   0 masen      (502) staff       (20)     1848 2024-05-09 02:46:02.000000 reflex_local_auth-0.2.0/custom_components/reflex_local_auth/pages/registration.py
+-rw-r--r--   0 masen      (502) staff       (20)     3258 2024-05-09 02:46:02.000000 reflex_local_auth-0.2.0/custom_components/reflex_local_auth/registration.py
+-rw-r--r--   0 masen      (502) staff       (20)      481 2024-03-22 12:15:18.000000 reflex_local_auth-0.2.0/custom_components/reflex_local_auth/routes.py
+-rw-r--r--   0 masen      (502) staff       (20)     1360 2024-05-09 02:46:02.000000 reflex_local_auth-0.2.0/custom_components/reflex_local_auth/user.py
+drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-05-21 23:04:03.565727 reflex_local_auth-0.2.0/custom_components/reflex_local_auth.egg-info/
+-rw-r--r--   0 masen      (502) staff       (20)     8119 2024-05-21 23:04:03.000000 reflex_local_auth-0.2.0/custom_components/reflex_local_auth.egg-info/PKG-INFO
+-rw-r--r--   0 masen      (502) staff       (20)      874 2024-05-21 23:04:03.000000 reflex_local_auth-0.2.0/custom_components/reflex_local_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 masen      (502) staff       (20)        1 2024-05-21 23:04:03.000000 reflex_local_auth-0.2.0/custom_components/reflex_local_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 masen      (502) staff       (20)       40 2024-05-21 23:04:03.000000 reflex_local_auth-0.2.0/custom_components/reflex_local_auth.egg-info/requires.txt
+-rw-r--r--   0 masen      (502) staff       (20)       18 2024-05-21 23:04:03.000000 reflex_local_auth-0.2.0/custom_components/reflex_local_auth.egg-info/top_level.txt
+-rw-r--r--   0 masen      (502) staff       (20)      728 2024-05-21 23:00:50.000000 reflex_local_auth-0.2.0/pyproject.toml
+-rw-r--r--   0 masen      (502) staff       (20)       38 2024-05-21 23:04:03.566267 reflex_local_auth-0.2.0/setup.cfg
```

### Comparing `reflex-local-auth-0.1.2/PKG-INFO` & `reflex_local_auth-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: reflex-local-auth
-Version: 0.1.2
+Version: 0.2.0
 Summary: Local DB user authentication for Reflex apps
 Author-email: Masen Furer <m_github@0x26.net>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/masenf/reflex-local-auth
 Keywords: reflex,reflex-custom-components
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: reflex>=0.4.2
+Requires-Dist: reflex>=0.5.0
 Requires-Dist: bcrypt
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # local-auth
```

### Comparing `reflex-local-auth-0.1.2/README.md` & `reflex_local_auth-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `reflex-local-auth-0.1.2/custom_components/reflex_local_auth/auth_session.py` & `reflex_local_auth-0.2.0/custom_components/reflex_local_auth/auth_session.py`

 * *Files identical despite different names*

### Comparing `reflex-local-auth-0.1.2/custom_components/reflex_local_auth/local_auth.py` & `reflex_local_auth-0.2.0/custom_components/reflex_local_auth/local_auth.py`

 * *Files identical despite different names*

### Comparing `reflex-local-auth-0.1.2/custom_components/reflex_local_auth/login.py` & `reflex_local_auth-0.2.0/custom_components/reflex_local_auth/login.py`

 * *Files identical despite different names*

### Comparing `reflex-local-auth-0.1.2/custom_components/reflex_local_auth/pages/login.py` & `reflex_local_auth-0.2.0/custom_components/reflex_local_auth/pages/login.py`

 * *Files identical despite different names*

### Comparing `reflex-local-auth-0.1.2/custom_components/reflex_local_auth/pages/registration.py` & `reflex_local_auth-0.2.0/custom_components/reflex_local_auth/pages/registration.py`

 * *Files identical despite different names*

### Comparing `reflex-local-auth-0.1.2/custom_components/reflex_local_auth/registration.py` & `reflex_local_auth-0.2.0/custom_components/reflex_local_auth/registration.py`

 * *Files identical despite different names*

### Comparing `reflex-local-auth-0.1.2/custom_components/reflex_local_auth/user.py` & `reflex_local_auth-0.2.0/custom_components/reflex_local_auth/user.py`

 * *Files identical despite different names*

### Comparing `reflex-local-auth-0.1.2/custom_components/reflex_local_auth.egg-info/PKG-INFO` & `reflex_local_auth-0.2.0/custom_components/reflex_local_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: reflex-local-auth
-Version: 0.1.2
+Version: 0.2.0
 Summary: Local DB user authentication for Reflex apps
 Author-email: Masen Furer <m_github@0x26.net>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/masenf/reflex-local-auth
 Keywords: reflex,reflex-custom-components
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: reflex>=0.4.2
+Requires-Dist: reflex>=0.5.0
 Requires-Dist: bcrypt
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # local-auth
```

### Comparing `reflex-local-auth-0.1.2/custom_components/reflex_local_auth.egg-info/SOURCES.txt` & `reflex_local_auth-0.2.0/custom_components/reflex_local_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reflex-local-auth-0.1.2/pyproject.toml` & `reflex_local_auth-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
     "setuptools",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reflex-local-auth"
-version = "0.1.2"
+version = "0.2.0"
 description = "Local DB user authentication for Reflex apps"
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.8"
 authors = [{ name = "Masen Furer", email = "m_github@0x26.net" }]
 keywords = [
     "reflex",
     "reflex-custom-components"]
 
 dependencies = [
-    "reflex>=0.4.2",
+    "reflex>=0.5.0",
     "bcrypt",
 ]
 
 classifiers = [
   "Development Status :: 4 - Beta",
 ]
```

