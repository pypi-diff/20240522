# Comparing `tmp/maji_passport-1.0.0.tar.gz` & `tmp/maji_passport-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maji_passport-1.0.0.tar", last modified: Wed May 22 08:41:57 2024, max compression
+gzip compressed data, was "maji_passport-1.0.1.tar", last modified: Wed May 22 09:08:57 2024, max compression
```

## Comparing `maji_passport-1.0.0.tar` & `maji_passport-1.0.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 08:41:57.456439 maji_passport-1.0.0/
--rw-rw-r--   0 teo       (1000) teo       (1000)     1073 2024-05-20 12:56:59.000000 maji_passport-1.0.0/LICENSE
--rw-r--r--   0 teo       (1000) teo       (1000)     3571 2024-05-22 08:41:57.456439 maji_passport-1.0.0/PKG-INFO
--rw-rw-r--   0 teo       (1000) teo       (1000)     2496 2024-05-21 13:19:25.000000 maji_passport-1.0.0/README.md
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 08:41:57.452439 maji_passport-1.0.0/maji_passport/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.0/maji_passport/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      406 2024-05-21 10:00:38.000000 maji_passport-1.0.0/maji_passport/admin.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      246 2024-05-21 10:09:31.000000 maji_passport-1.0.0/maji_passport/apps.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 08:41:57.452439 maji_passport-1.0.0/maji_passport/authentication/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.0/maji_passport/authentication/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     3046 2024-05-21 10:00:38.000000 maji_passport-1.0.0/maji_passport/authentication/backend.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 08:41:57.452439 maji_passport-1.0.0/maji_passport/management/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.0/maji_passport/management/__init__.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 08:41:57.452439 maji_passport-1.0.0/maji_passport/management/commands/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.0/maji_passport/management/commands/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      537 2024-05-21 10:00:38.000000 maji_passport-1.0.0/maji_passport/management/commands/kafka_consumer.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      861 2024-05-21 10:00:38.000000 maji_passport-1.0.0/maji_passport/management/commands/kafka_producer_test.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      236 2024-05-21 10:00:38.000000 maji_passport-1.0.0/maji_passport/management/commands/migrate_all_users_to_passport.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 08:41:57.456439 maji_passport-1.0.0/maji_passport/migrations/
--rw-rw-r--   0 teo       (1000) teo       (1000)     2234 2024-05-21 10:45:54.000000 maji_passport-1.0.0/maji_passport/migrations/0001_initial.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      526 2024-05-21 10:45:54.000000 maji_passport-1.0.0/maji_passport/migrations/0002_auto_20240418_1355.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      471 2024-05-21 10:45:54.000000 maji_passport-1.0.0/maji_passport/migrations/0003_accesstoken_passport_ac_token_cccee9_hash.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      536 2024-05-21 10:45:54.000000 maji_passport-1.0.0/maji_passport/migrations/0004_alter_accesstoken_passport_user.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      615 2024-05-21 10:47:34.000000 maji_passport-1.0.0/maji_passport/migrations/0005_auto_20240521_1047.py
--rw-rw-r--   0 teo       (1000) teo       (1000)     2480 2024-05-21 12:23:56.000000 maji_passport-1.0.0/maji_passport/migrations/0006_auto_20240521_1118.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.0/maji_passport/migrations/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     1824 2024-05-21 08:45:40.000000 maji_passport-1.0.0/maji_passport/models.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 08:41:57.456439 maji_passport-1.0.0/maji_passport/serializers/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.0/maji_passport/serializers/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     2397 2024-05-06 13:34:14.000000 maji_passport-1.0.0/maji_passport/serializers/exchange.py
--rw-rw-r--   0 teo       (1000) teo       (1000)     1852 2024-05-21 09:57:13.000000 maji_passport-1.0.0/maji_passport/serializers/kafka.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      519 2024-05-17 08:38:42.000000 maji_passport-1.0.0/maji_passport/serializers/passport.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 08:41:57.456439 maji_passport-1.0.0/maji_passport/services/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.0/maji_passport/services/__init__.py
--rw-rw-r--   0 teo       (1000) teo       (1000)     4490 2024-05-21 10:00:38.000000 maji_passport-1.0.0/maji_passport/services/auth.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     7023 2024-05-21 10:00:38.000000 maji_passport-1.0.0/maji_passport/services/exchange.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     2977 2024-05-21 09:04:04.000000 maji_passport-1.0.0/maji_passport/services/kafka.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      305 2024-05-21 10:00:38.000000 maji_passport-1.0.0/maji_passport/services/passport.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     2880 2024-05-21 08:32:10.000000 maji_passport-1.0.0/maji_passport/services/passport_migrate.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 08:41:57.456439 maji_passport-1.0.0/maji_passport/tests/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.0/maji_passport/tests/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     4010 2024-05-21 10:00:38.000000 maji_passport-1.0.0/maji_passport/tests/test_exchange.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     3026 2024-05-21 10:00:38.000000 maji_passport-1.0.0/maji_passport/tests/test_kafka.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      940 2024-05-21 10:10:15.000000 maji_passport-1.0.0/maji_passport/urls.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 08:41:57.456439 maji_passport-1.0.0/maji_passport/views/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.0/maji_passport/views/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     4806 2024-05-21 10:00:38.000000 maji_passport-1.0.0/maji_passport/views/exchange.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     3753 2024-05-21 10:00:38.000000 maji_passport-1.0.0/maji_passport/views/passport.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 08:41:57.452439 maji_passport-1.0.0/maji_passport.egg-info/
--rw-r--r--   0 teo       (1000) teo       (1000)     3571 2024-05-22 08:41:57.000000 maji_passport-1.0.0/maji_passport.egg-info/PKG-INFO
--rw-rw-r--   0 teo       (1000) teo       (1000)     1625 2024-05-22 08:41:57.000000 maji_passport-1.0.0/maji_passport.egg-info/SOURCES.txt
--rw-rw-r--   0 teo       (1000) teo       (1000)        1 2024-05-22 08:41:57.000000 maji_passport-1.0.0/maji_passport.egg-info/dependency_links.txt
--rw-rw-r--   0 teo       (1000) teo       (1000)      207 2024-05-22 08:41:57.000000 maji_passport-1.0.0/maji_passport.egg-info/requires.txt
--rw-rw-r--   0 teo       (1000) teo       (1000)       14 2024-05-22 08:41:57.000000 maji_passport-1.0.0/maji_passport.egg-info/top_level.txt
--rw-rw-r--   0 teo       (1000) teo       (1000)      668 2024-05-22 08:41:54.000000 maji_passport-1.0.0/pyproject.toml
--rw-rw-r--   0 teo       (1000) teo       (1000)       38 2024-05-22 08:41:57.456439 maji_passport-1.0.0/setup.cfg
--rw-rw-r--   0 teo       (1000) teo       (1000)     1018 2024-05-22 08:41:54.000000 maji_passport-1.0.0/setup.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 09:08:57.567430 maji_passport-1.0.1/
+-rw-rw-r--   0 teo       (1000) teo       (1000)     1073 2024-05-20 12:56:59.000000 maji_passport-1.0.1/LICENSE
+-rw-r--r--   0 teo       (1000) teo       (1000)     3571 2024-05-22 09:08:57.567430 maji_passport-1.0.1/PKG-INFO
+-rw-rw-r--   0 teo       (1000) teo       (1000)     2496 2024-05-21 13:19:25.000000 maji_passport-1.0.1/README.md
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 09:08:57.563430 maji_passport-1.0.1/maji_passport/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.1/maji_passport/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      406 2024-05-21 10:00:38.000000 maji_passport-1.0.1/maji_passport/admin.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      246 2024-05-21 10:09:31.000000 maji_passport-1.0.1/maji_passport/apps.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 09:08:57.567430 maji_passport-1.0.1/maji_passport/authentication/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.1/maji_passport/authentication/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     3046 2024-05-21 10:00:38.000000 maji_passport-1.0.1/maji_passport/authentication/backend.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 09:08:57.567430 maji_passport-1.0.1/maji_passport/management/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.1/maji_passport/management/__init__.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 09:08:57.567430 maji_passport-1.0.1/maji_passport/management/commands/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.1/maji_passport/management/commands/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      537 2024-05-21 10:00:38.000000 maji_passport-1.0.1/maji_passport/management/commands/kafka_consumer.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      861 2024-05-21 10:00:38.000000 maji_passport-1.0.1/maji_passport/management/commands/kafka_producer_test.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      236 2024-05-21 10:00:38.000000 maji_passport-1.0.1/maji_passport/management/commands/migrate_all_users_to_passport.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 09:08:57.567430 maji_passport-1.0.1/maji_passport/migrations/
+-rw-rw-r--   0 teo       (1000) teo       (1000)     2234 2024-05-21 10:45:54.000000 maji_passport-1.0.1/maji_passport/migrations/0001_initial.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)      526 2024-05-21 10:45:54.000000 maji_passport-1.0.1/maji_passport/migrations/0002_auto_20240418_1355.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)      471 2024-05-21 10:45:54.000000 maji_passport-1.0.1/maji_passport/migrations/0003_accesstoken_passport_ac_token_cccee9_hash.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)      536 2024-05-21 10:45:54.000000 maji_passport-1.0.1/maji_passport/migrations/0004_alter_accesstoken_passport_user.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)      615 2024-05-21 10:47:34.000000 maji_passport-1.0.1/maji_passport/migrations/0005_auto_20240521_1047.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)     2480 2024-05-21 12:23:56.000000 maji_passport-1.0.1/maji_passport/migrations/0006_auto_20240521_1118.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.1/maji_passport/migrations/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     1824 2024-05-21 08:45:40.000000 maji_passport-1.0.1/maji_passport/models.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 09:08:57.567430 maji_passport-1.0.1/maji_passport/serializers/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.1/maji_passport/serializers/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     2397 2024-05-06 13:34:14.000000 maji_passport-1.0.1/maji_passport/serializers/exchange.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)     1852 2024-05-21 09:57:13.000000 maji_passport-1.0.1/maji_passport/serializers/kafka.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      519 2024-05-17 08:38:42.000000 maji_passport-1.0.1/maji_passport/serializers/passport.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 09:08:57.567430 maji_passport-1.0.1/maji_passport/services/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.1/maji_passport/services/__init__.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)     4612 2024-05-22 09:08:55.000000 maji_passport-1.0.1/maji_passport/services/auth.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     7023 2024-05-21 10:00:38.000000 maji_passport-1.0.1/maji_passport/services/exchange.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     2977 2024-05-21 09:04:04.000000 maji_passport-1.0.1/maji_passport/services/kafka.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      305 2024-05-21 10:00:38.000000 maji_passport-1.0.1/maji_passport/services/passport.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     2880 2024-05-21 08:32:10.000000 maji_passport-1.0.1/maji_passport/services/passport_migrate.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 09:08:57.567430 maji_passport-1.0.1/maji_passport/tests/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.1/maji_passport/tests/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     4010 2024-05-21 10:00:38.000000 maji_passport-1.0.1/maji_passport/tests/test_exchange.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     3026 2024-05-21 10:00:38.000000 maji_passport-1.0.1/maji_passport/tests/test_kafka.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      940 2024-05-21 10:10:15.000000 maji_passport-1.0.1/maji_passport/urls.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 09:08:57.567430 maji_passport-1.0.1/maji_passport/views/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.1/maji_passport/views/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     4932 2024-05-22 09:07:59.000000 maji_passport-1.0.1/maji_passport/views/exchange.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     3753 2024-05-21 10:00:38.000000 maji_passport-1.0.1/maji_passport/views/passport.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 09:08:57.567430 maji_passport-1.0.1/maji_passport.egg-info/
+-rw-r--r--   0 teo       (1000) teo       (1000)     3571 2024-05-22 09:08:57.000000 maji_passport-1.0.1/maji_passport.egg-info/PKG-INFO
+-rw-rw-r--   0 teo       (1000) teo       (1000)     1625 2024-05-22 09:08:57.000000 maji_passport-1.0.1/maji_passport.egg-info/SOURCES.txt
+-rw-rw-r--   0 teo       (1000) teo       (1000)        1 2024-05-22 09:08:57.000000 maji_passport-1.0.1/maji_passport.egg-info/dependency_links.txt
+-rw-rw-r--   0 teo       (1000) teo       (1000)      207 2024-05-22 09:08:57.000000 maji_passport-1.0.1/maji_passport.egg-info/requires.txt
+-rw-rw-r--   0 teo       (1000) teo       (1000)       14 2024-05-22 09:08:57.000000 maji_passport-1.0.1/maji_passport.egg-info/top_level.txt
+-rw-rw-r--   0 teo       (1000) teo       (1000)      668 2024-05-22 09:08:54.000000 maji_passport-1.0.1/pyproject.toml
+-rw-rw-r--   0 teo       (1000) teo       (1000)       38 2024-05-22 09:08:57.567430 maji_passport-1.0.1/setup.cfg
+-rw-rw-r--   0 teo       (1000) teo       (1000)     1018 2024-05-22 09:08:54.000000 maji_passport-1.0.1/setup.py
```

### Comparing `maji_passport-1.0.0/LICENSE` & `maji_passport-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.0/PKG-INFO` & `maji_passport-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maji_passport
-Version: 1.0.0
+Version: 1.0.1
 Summary: Maji Passport With custom authorisation
 Home-page: https://passport.maji.la/
 Author: ViktorTeodorih
 Author-email: Viktor Ivanov <viktorteodorihivanov@gmail.com>
 Project-URL: Homepage, https://gitlab.com/argo-media/argo-media-backend-ecosystem/maji-passport-library
 Project-URL: Issues, https://gitlab.com/argo-media/argo-media-backend-ecosystem/maji-passport-library/issues
 Keywords: maji passport python
```

### Comparing `maji_passport-1.0.0/README.md` & `maji_passport-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.0/maji_passport/authentication/backend.py` & `maji_passport-1.0.1/maji_passport/authentication/backend.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.0/maji_passport/management/commands/kafka_consumer.py` & `maji_passport-1.0.1/maji_passport/management/commands/kafka_consumer.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.0/maji_passport/management/commands/kafka_producer_test.py` & `maji_passport-1.0.1/maji_passport/management/commands/kafka_producer_test.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.0/maji_passport/migrations/0001_initial.py` & `maji_passport-1.0.1/maji_passport/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.0/maji_passport/migrations/0002_auto_20240418_1355.py` & `maji_passport-1.0.1/maji_passport/migrations/0002_auto_20240418_1355.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.0/maji_passport/migrations/0004_alter_accesstoken_passport_user.py` & `maji_passport-1.0.1/maji_passport/migrations/0004_alter_accesstoken_passport_user.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.0/maji_passport/migrations/0005_auto_20240521_1047.py` & `maji_passport-1.0.1/maji_passport/migrations/0005_auto_20240521_1047.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.0/maji_passport/migrations/0006_auto_20240521_1118.py` & `maji_passport-1.0.1/maji_passport/migrations/0006_auto_20240521_1118.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.0/maji_passport/models.py` & `maji_passport-1.0.1/maji_passport/models.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.0/maji_passport/serializers/exchange.py` & `maji_passport-1.0.1/maji_passport/serializers/exchange.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.0/maji_passport/serializers/kafka.py` & `maji_passport-1.0.1/maji_passport/serializers/kafka.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.0/maji_passport/serializers/passport.py` & `maji_passport-1.0.1/maji_passport/serializers/passport.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.0/maji_passport/services/auth.py` & `maji_passport-1.0.1/maji_passport/services/auth.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import datetime
 
 import jwt
 from countries_plus.models import Country
 from django.contrib.auth import get_user_model
-from django.core.exceptions import ObjectDoesNotExist
+from django.core.exceptions import ObjectDoesNotExist, PermissionDenied
 from django.db import IntegrityError
 from django.conf import settings
-from jwt import InvalidAlgorithmError, ExpiredSignatureError
+from jwt import InvalidAlgorithmError, ExpiredSignatureError, InvalidSignatureError
 from loguru import logger
 
 from maji_passport.models import PassportUser, AccessToken, TargetAccess
 
 User = get_user_model()
 
 
@@ -133,9 +133,11 @@
         try:
             decoded = jwt.decode(token, public_key, algorithms=["RS256"])
         except InvalidAlgorithmError as e:
             logger.warning(f"Can't decode token: {token}")
             raise InvalidAlgorithmError(e)
         except ExpiredSignatureError as e:
             raise ExpiredSignatureError(e)
+        except InvalidSignatureError as e:
+            raise PermissionDenied(e)
 
         return decoded
```

### Comparing `maji_passport-1.0.0/maji_passport/services/exchange.py` & `maji_passport-1.0.1/maji_passport/services/exchange.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.0/maji_passport/services/kafka.py` & `maji_passport-1.0.1/maji_passport/services/kafka.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.0/maji_passport/services/passport_migrate.py` & `maji_passport-1.0.1/maji_passport/services/passport_migrate.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.0/maji_passport/tests/test_exchange.py` & `maji_passport-1.0.1/maji_passport/tests/test_exchange.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.0/maji_passport/tests/test_kafka.py` & `maji_passport-1.0.1/maji_passport/tests/test_kafka.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.0/maji_passport/urls.py` & `maji_passport-1.0.1/maji_passport/urls.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.0/maji_passport/views/exchange.py` & `maji_passport-1.0.1/maji_passport/views/exchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,18 @@
         """
         serializer = AccessTokenSerializer(data=request.data)
         serializer.is_valid(raise_exception=True)
         data = dict(serializer.data)
         ExchangeTokenService.auto_continue_flow(data["access_token"])
         return Response(status=status.HTTP_204_NO_CONTENT)
 
+    @swagger_auto_schema(
+        request_body=AccessTokenSerializer,
+        responses={204: AccessTokenSerializer()},
+    )
     @action(
         detail=False,
         methods=["POST"],
     )
     def update_token(self, request):
         """
         Made server-server request for update token
```

### Comparing `maji_passport-1.0.0/maji_passport/views/passport.py` & `maji_passport-1.0.1/maji_passport/views/passport.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.0/maji_passport.egg-info/PKG-INFO` & `maji_passport-1.0.1/maji_passport.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maji-passport
-Version: 1.0.0
+Version: 1.0.1
 Summary: Maji Passport With custom authorisation
 Home-page: https://passport.maji.la/
 Author: ViktorTeodorih
 Author-email: Viktor Ivanov <viktorteodorihivanov@gmail.com>
 Project-URL: Homepage, https://gitlab.com/argo-media/argo-media-backend-ecosystem/maji-passport-library
 Project-URL: Issues, https://gitlab.com/argo-media/argo-media-backend-ecosystem/maji-passport-library/issues
 Keywords: maji passport python
```

### Comparing `maji_passport-1.0.0/maji_passport.egg-info/SOURCES.txt` & `maji_passport-1.0.1/maji_passport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.0/pyproject.toml` & `maji_passport-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "maji_passport"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Viktor Ivanov", email="viktorteodorihivanov@gmail.com" },
 ]
 description = "Maji Passport With custom authorisation"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `maji_passport-1.0.0/setup.py` & `maji_passport-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 
 setup(
   name='maji_passport',
-  version='1.0.0',
+  version='1.0.1',
   author='ViktorTeodorih',
   author_email='viktorteodorihivanov@gmail.com',
   description='Maji Passport With custom authorisation',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://passport.maji.la/',
   packages=find_packages(),
```

