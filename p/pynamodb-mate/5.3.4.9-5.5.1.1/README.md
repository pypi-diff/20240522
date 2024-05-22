# Comparing `tmp/pynamodb_mate-5.3.4.9.tar.gz` & `tmp/pynamodb_mate-5.5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamodb_mate-5.3.4.9.tar", last modified: Mon May 15 05:54:30 2023, max compression
+gzip compressed data, was "pynamodb_mate-5.5.1.1.tar", last modified: Wed May 22 20:59:19 2024, max compression
```

## Comparing `pynamodb_mate-5.3.4.9.tar` & `pynamodb_mate-5.5.1.1.tar`

### file list

```diff
@@ -1,53 +1,82 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-15 05:54:30.926158 pynamodb_mate-5.3.4.9/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2022-12-26 12:25:06.000000 pynamodb_mate-5.3.4.9/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1123 2022-12-26 12:25:06.000000 pynamodb_mate-5.3.4.9/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      321 2022-12-26 13:43:20.000000 pynamodb_mate-5.3.4.9/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     6908 2023-05-15 05:54:30.926000 pynamodb_mate-5.3.4.9/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     5696 2023-02-17 04:31:53.000000 pynamodb_mate-5.3.4.9/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-15 05:54:30.921948 pynamodb_mate-5.3.4.9/pynamodb_mate/
--rw-r--r--   0 sanhehu    (501) staff       (20)     2528 2023-01-17 00:25:46.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       95 2023-05-15 04:52:11.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/_version.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-15 05:54:30.923203 pynamodb_mate-5.3.4.9/pynamodb_mate/attributes/
--rw-r--r--   0 sanhehu    (501) staff       (20)       60 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/attributes/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1894 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/attributes/compressed.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3694 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/attributes/encrypted.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5370 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/attributes/s3backed.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1764 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/cipher.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      336 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/compat.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-15 05:54:30.923342 pynamodb_mate-5.3.4.9/pynamodb_mate/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2022-12-26 12:25:06.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1321 2022-12-26 12:25:06.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/helpers.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    12065 2023-01-17 00:59:45.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/models.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-15 05:54:30.923523 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/
--rw-r--r--   0 sanhehu    (501) staff       (20)      109 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/__init__.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-15 05:54:30.924081 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/
--rw-r--r--   0 sanhehu    (501) staff       (20)      393 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3023 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/abstract.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-15 05:54:30.924484 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/backend/
--rw-r--r--   0 sanhehu    (501) staff       (20)       33 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/backend/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3561 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/backend/dynamodb.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1866 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/backend/in_memory.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/multi_layer.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      152 2023-01-16 16:26:52.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/utils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-15 05:54:30.924745 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/status_tracker/
--rw-r--r--   0 sanhehu    (501) staff       (20)      295 2023-02-17 04:31:53.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/status_tracker/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    27101 2023-05-15 04:51:28.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/status_tracker/impl.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-15 05:54:30.925688 pynamodb_mate-5.3.4.9/pynamodb_mate/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      208 2023-01-16 20:19:31.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      598 2023-01-16 20:34:26.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/tests/base.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1240 2022-12-26 13:46:07.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      370 2022-12-26 13:46:35.000000 pynamodb_mate-5.3.4.9/pynamodb_mate/tests/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-15 05:54:30.922660 pynamodb_mate-5.3.4.9/pynamodb_mate.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     6908 2023-05-15 05:54:30.000000 pynamodb_mate-5.3.4.9/pynamodb_mate.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1258 2023-05-15 05:54:30.000000 pynamodb_mate-5.3.4.9/pynamodb_mate.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-15 05:54:30.000000 pynamodb_mate-5.3.4.9/pynamodb_mate.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      378 2023-05-15 05:54:30.000000 pynamodb_mate-5.3.4.9/pynamodb_mate.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       14 2023-05-15 05:54:30.000000 pynamodb_mate-5.3.4.9/pynamodb_mate.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     6475 2023-05-15 04:53:41.000000 pynamodb_mate-5.3.4.9/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      208 2022-12-26 13:49:49.000000 pynamodb_mate-5.3.4.9/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      643 2022-12-26 13:50:07.000000 pynamodb_mate-5.3.4.9/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       13 2022-12-26 13:47:00.000000 pynamodb_mate-5.3.4.9/requirements-encrypt.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      189 2023-01-16 19:59:46.000000 pynamodb_mate-5.3.4.9/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      127 2023-01-16 17:39:27.000000 pynamodb_mate-5.3.4.9/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-15 05:54:30.926198 pynamodb_mate-5.3.4.9/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7555 2022-12-26 13:48:05.000000 pynamodb_mate-5.3.4.9/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-22 20:59:19.669370 pynamodb_mate-5.5.1.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      462 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1123 2024-04-08 05:32:11.000000 pynamodb_mate-5.5.1.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      367 2024-04-09 20:05:06.000000 pynamodb_mate-5.5.1.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     8933 2024-05-22 20:59:19.669131 pynamodb_mate-5.5.1.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6455 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-22 20:59:19.660320 pynamodb_mate-5.5.1.1/pynamodb_mate/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2970 2024-05-18 15:37:32.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       95 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1993 2024-05-18 15:33:23.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-22 20:59:19.661645 pynamodb_mate-5.5.1.1/pynamodb_mate/attributes/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       60 2024-04-08 05:32:11.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/attributes/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      776 2024-05-18 15:29:37.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/attributes/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1894 2024-04-08 05:32:11.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/attributes/compressed.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3694 2024-04-08 05:32:11.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/attributes/encrypted.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5986 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/attributes/s3backed.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1764 2024-04-08 05:32:11.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/cipher.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      336 2024-04-08 05:32:11.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/compat.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-22 20:59:19.661768 pynamodb_mate-5.5.1.1/pynamodb_mate/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2024-04-08 05:32:11.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2475 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/helpers.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    12465 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/models.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-22 20:59:19.662106 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       59 2024-05-18 14:16:08.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      205 2024-05-18 15:17:13.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-22 20:59:19.662790 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/cache/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       66 2024-05-18 15:15:58.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/cache/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3051 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/cache/abstract.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      467 2024-05-18 15:16:35.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/cache/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-22 20:59:19.663125 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/cache/backend/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       33 2024-04-08 05:32:11.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/cache/backend/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4064 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/cache/backend/dynamodb.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1866 2024-04-08 05:32:11.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/cache/backend/in_memory.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2024-04-08 05:32:11.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/cache/multi_layer.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      152 2024-04-08 05:32:11.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/cache/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-22 20:59:19.663449 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/large_attribute/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      343 2024-05-04 20:51:58.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/large_attribute/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      123 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/large_attribute/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    23287 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/large_attribute/impl.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-22 20:59:19.663891 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/relationship/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      324 2024-04-08 18:55:06.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/relationship/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      362 2024-04-08 15:34:36.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/relationship/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    17538 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/relationship/impl.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-22 20:59:19.664227 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/status_tracker/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      127 2024-05-18 14:15:32.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/status_tracker/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      262 2024-05-18 15:34:26.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/status_tracker/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    27127 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/status_tracker/impl.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      783 2024-04-08 18:48:51.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/type_hint.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-22 20:59:19.665591 pynamodb_mate-5.5.1.1/pynamodb_mate/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2024-05-21 18:27:32.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    16752 2022-01-07 07:50:09.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/vendor/decorator.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    13696 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/vendor/iterable.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      718 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/vendor/mark.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2556 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/vendor/mock_aws.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/pynamodb_mate/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-22 20:59:19.667650 pynamodb_mate-5.5.1.1/pynamodb_mate.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     8933 2024-05-22 20:59:19.000000 pynamodb_mate-5.5.1.1/pynamodb_mate.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2110 2024-05-22 20:59:19.000000 pynamodb_mate-5.5.1.1/pynamodb_mate.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2024-05-22 20:59:19.000000 pynamodb_mate-5.5.1.1/pynamodb_mate.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      565 2024-05-22 20:59:19.000000 pynamodb_mate-5.5.1.1/pynamodb_mate.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       14 2024-05-22 20:59:19.000000 pynamodb_mate-5.5.1.1/pynamodb_mate.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7999 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2024-04-08 05:32:11.000000 pynamodb_mate-5.5.1.1/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      391 2024-05-18 15:25:33.000000 pynamodb_mate-5.5.1.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      907 2024-04-08 05:32:11.000000 pynamodb_mate-5.5.1.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       28 2024-04-08 05:32:11.000000 pynamodb_mate-5.5.1.1/requirements-encrypt.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      128 2024-04-08 05:32:11.000000 pynamodb_mate-5.5.1.1/requirements-furo-sphinx-search.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      298 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      136 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2024-05-22 20:59:19.669407 pynamodb_mate-5.5.1.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7637 2024-05-04 16:38:08.000000 pynamodb_mate-5.5.1.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-22 20:59:19.667426 pynamodb_mate-5.5.1.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3293 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2749 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/tests/test_attr_compressed.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3080 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/tests/test_attr_encrypted.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4588 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/tests/test_attr_s3backed.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      875 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/tests/test_cipher.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      464 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/tests/test_helpers.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3071 2024-04-08 05:32:11.000000 pynamodb_mate-5.5.1.1/tests/test_import.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2240 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/tests/test_index.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5474 2024-05-22 20:55:21.000000 pynamodb_mate-5.5.1.1/tests/test_models.py
```

### Comparing `pynamodb_mate-5.3.4.9/LICENSE.txt` & `pynamodb_mate-5.5.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pynamodb_mate-5.3.4.9/PKG-INFO` & `pynamodb_mate-5.5.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pynamodb_mate
-Version: 5.3.4.9
+Version: 5.5.1.1
 Summary: Provide Additional Features for pynamodb.
 Home-page: https://github.com/MacHu-GWU/pynamodb_mate-project
-Download-URL: https://pypi.python.org/pypi/pynamodb_mate/5.3.4.9#downloads
+Download-URL: https://pypi.python.org/pypi/pynamodb_mate/5.5.1.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -16,28 +16,53 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.7
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+Requires-Dist: pynamodb<6.0.0,>=5.5.1
+Requires-Dist: cached-property>=1.5.2; python_version < "3.8"
+Requires-Dist: dataclasses>=0.8; python_version == "3.6"
+Requires-Dist: iterproxy<1.0.0,>=0.3.1
 Provides-Extra: encrypt
+Requires-Dist: pycryptodome<4.0.0,>=3.18.0; extra == "encrypt"
 Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: boto3; extra == "tests"
+Requires-Dist: boto_session_manager<2.0.0,>=1.7.2; extra == "tests"
+Requires-Dist: s3pathlib<3.0.0,>=2.1.2; extra == "tests"
+Requires-Dist: pycryptodome<4.0.0,>=3.18.0; extra == "tests"
+Requires-Dist: moto<5.0.0,>=4.1.12; extra == "tests"
+Requires-Dist: moto[dynamodb,s3]<5.0.0,>=4.1.12; extra == "tests"
 Provides-Extra: docs
-License-File: LICENSE.txt
-License-File: AUTHORS.rst
+Requires-Dist: Sphinx==5.3.0; extra == "docs"
+Requires-Dist: sphinx-jinja==2.0.2; extra == "docs"
+Requires-Dist: sphinx-copybutton==0.5.1; extra == "docs"
+Requires-Dist: sphinx-design==0.5.0; extra == "docs"
+Requires-Dist: furo==2023.03.27; extra == "docs"
+Requires-Dist: nbsphinx==0.8.12; extra == "docs"
+Requires-Dist: rstobj==1.2.1; extra == "docs"
+Requires-Dist: pygments==2.15.1; extra == "docs"
+Requires-Dist: ipython==8.10.0; extra == "docs"
+Requires-Dist: docfly==2.0.3; extra == "docs"
+Requires-Dist: pycryptodome<4.0.0,>=3.18.0; extra == "docs"
 
 .. image:: https://readthedocs.org/projects/pynamodb_mate/badge/?version=latest
-    :target: https://pynamodb_mate.readthedocs.io/
+    :target: https://pynamodb-mate.readthedocs.io/
     :alt: Documentation Status
 
 .. image:: https://github.com/MacHu-GWU/pynamodb_mate-project/workflows/CI/badge.svg
     :target: https://github.com/MacHu-GWU/pynamodb_mate-project/actions?query=workflow:CI
 
 .. image:: https://codecov.io/gh/MacHu-GWU/pynamodb_mate-project/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/MacHu-GWU/pynamodb_mate-project
@@ -48,28 +73,32 @@
 .. image:: https://img.shields.io/pypi/l/pynamodb_mate.svg
     :target: https://pypi.python.org/pypi/pynamodb_mate
 
 .. image:: https://img.shields.io/pypi/pyversions/pynamodb_mate.svg
     :target: https://pypi.python.org/pypi/pynamodb_mate
 
 .. image:: https://img.shields.io/pypi/dm/pynamodb-mate.svg
+    :target: https://pypi.python.org/pypi/pynamodb_mate
+
+.. image:: https://img.shields.io/badge/Release_History!--None.svg?style=social
+    :target: https://github.com/MacHu-GWU/pynamodb_mate-project/blob/master/release-history.rst
 
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/pynamodb_mate-project
 
 ------
 
 .. image:: https://img.shields.io/badge/Link-Document-blue.svg
-      :target: https://pynamodb_mate.readthedocs.io/
+      :target: https://pynamodb-mate.readthedocs.io/
 
 .. image:: https://img.shields.io/badge/Link-API-blue.svg
-      :target: https://pynamodb_mate.readthedocs.io/py-modindex.html
+      :target: https://pynamodb-mate.readthedocs.io/py-modindex.html
 
 .. image:: https://img.shields.io/badge/Link-Source_Code-blue.svg
-      :target: https://pynamodb_mate.readthedocs.io/py-modindex.html
+      :target: https://pynamodb-mate.readthedocs.io/py-modindex.html
 
 .. image:: https://img.shields.io/badge/Link-Install-blue.svg
       :target: `install`_
 
 .. image:: https://img.shields.io/badge/Link-GitHub-blue.svg
       :target: https://github.com/MacHu-GWU/pynamodb_mate-project
 
@@ -81,48 +110,41 @@
 
 .. image:: https://img.shields.io/badge/Link-Download-blue.svg
       :target: https://pypi.org/pypi/pynamodb_mate#files
 
 
 Welcome to ``pynamodb_mate`` Documentation
 ==============================================================================
-📙 `Full Documentation is Here <https://pynamodb_mate.readthedocs.io/>`_
+📙 `Full Documentation is Here <https://pynamodb-mate.readthedocs.io/>`_
 
-.. contents::
-    :class: this-will-duplicate-information-and-it-is-still-useful-here
-    :depth: 1
-    :local:
+.. image:: https://pynamodb-mate.readthedocs.io/en/latest/_static/pynamodb_mate-logo.png
+    :target: https://pynamodb-mate.readthedocs.io/
 
 
 Overview
 ------------------------------------------------------------------------------
-``pynamodb_mate`` provides advanced best practice using DynamoDB in python. Built on top of `pynamodb <https://pynamodb.readthedocs.io/en/latest/>`_ python library. It maintain the compatibility to major version of ``pynamodb`` library. For example ``pynamodb_mate>=5.0.0,<6.0.0`` is compatible to ``pynamodb>=5.0.0,<6.0.0``.
+``pynamodb_mate`` provides advanced best practice using DynamoDB in python. Built on top of `pynamodb <https://pynamodb.readthedocs.io/en/latest/>`_ python library. It maintain the compatibility to major version of ``pynamodb`` library. For example ``pynamodb_mate>=5.0.0,<6.0.0`` is compatible to ``pynamodb>=5.0.0,<6.0.0``, ``pynamodb_mate==5.5.1.X`` is compatible to ``pynamodb>=5.5.1,<6.0.0``, ``pynamodb_mate==6.0.0.X`` is compatible to ``pynamodb>=6.0.0,<7.0.0``.
 
 
 Disclaimer
 ------------------------------------------------------------------------------
 Even though the author is a Dynamodb Subject Matter Expert from AWS, but this project is NOT an AWS official project, and it is a personal open source project for the Python community.
 
 
 Features
 ------------------------------------------------------------------------------
-Click on the link below to see detailed tutorial and examples.
-
-- ⭐ `Store Large Object in DynamoDB <https://github.com/MacHu-GWU/pynamodb_mate-project/blob/master/examples/Store-Large-Object-in-DynamoDB.ipynb>`_: This feature allows you to store any Python object and arbitrary big data in DynamoDB that can exceed the 400KB limit.
-- ⭐ `Client Side Encryption <https://github.com/MacHu-GWU/pynamodb_mate-project/blob/master/examples/Client-Side-Encryption.ipynb>`_: This feature allows you to use your own encryption key to encrypt your data before it is sent to the DynamoDB.
-- ⭐ `Compressed Attribute <https://github.com/MacHu-GWU/pynamodb_mate-project/blob/master/examples/Compressed-Attribute.ipynb>`_: This feature can automatically compress the data before it is sent to the DynamoDB.
-- ⭐ `AWS DynamoDB Console Url <https://github.com/MacHu-GWU/pynamodb_mate-project/blob/master/examples/AWS-DynamoDB-Console-Url.ipynb>`_: This feature can print the AWS DynamoDB console url for the table, items. You can use this in you log to quickly jump to the console to debug.
-
-
-DynamoDB Patterns
-------------------------------------------------------------------------------
-``pynamodb_mate`` also provides some commonly used patterns. It is based on the author's experience providing solutions to many customers from different industries. Click on the link below to see detailed tutorial and examples.
+``pynamodb_mate`` provides some commonly used patterns. It is based on the author's experience providing solutions to many customers from different industries. Click on the link below to see detailed tutorial and examples.
 
-- 🎉 `Cache <https://github.com/MacHu-GWU/pynamodb_mate-project/blob/master/examples/patterns/cache.ipynb>`_: This feature gives you a "Redis" liked, serverless, Zero-ops, auto-scaling, high performance, pay-as-you-go cache layer based on DynamoDB.
-- 🎉 `Status Tracker <https://github.com/MacHu-GWU/pynamodb_mate-project/blob/master/examples/patterns/status-tracker.ipynb>`_: This feature gives you the ability to track status of each task, and error-handling, retry, concurrency control out-of-the-box.
+- ⭐ `Store Large Object in DynamoDB <https://pynamodb-mate.readthedocs.io/en/latest/01-Store-Large-Object-in-DynamoDB/index.html>`_: This feature allows you to store any Python object and arbitrary big data in DynamoDB that can exceed the 400KB limit. It also handles data consistency and data integrity between DynamoDB and S3.
+- ⭐ `Client Side Encryption <https://pynamodb-mate.readthedocs.io/en/latest/02-Client-Side-Encryption/index.html>`_: This feature allows you to use your own encryption key to encrypt your data before it is sent to the DynamoDB.
+- ⭐ `Compressed Attribute <https://pynamodb-mate.readthedocs.io/en/latest/03-Compressed-Attribute/index.html>`_: This feature can automatically compress the data before it is sent to the DynamoDB, it would save you a lot of money if you use JSON attribute in DynamoDB.
+- ⭐ `AWS DynamoDB Console Url <https://pynamodb-mate.readthedocs.io/en/latest/04-DynamoDB-Consule-Url/index.html>`_: This feature can print the AWS DynamoDB console url for the table, items. You can use this in you log to quickly jump to the console to debug.
+- ⭐ `Use DynamoDB as a Cache Backend <https://pynamodb-mate.readthedocs.io/en/latest/05-Use-DynamoDB-as-Cache-Backend/index.html>`_: This feature gives you a "Redis" liked, serverless, Zero-ops, auto-scaling, high performance, pay-as-you-go cache layer based on DynamoDB.
+- ⭐ `Enable status tracking for business critical application using Amazon DynamoDB <https://pynamodb-mate.readthedocs.io/en/latest/06-Status-Tracker/index.html>`_: This feature gives you the ability to track status of each task, and error-handling, retry, concurrency control out-of-the-box.
+- ⭐ `Modeling Relational Data in DynamoDB <https://pynamodb-mate.readthedocs.io/en/latest/07-Modeling-Relational-Data-in-DynamoDB/index.html>`_: This feature allow you to manage mass amount entity and one-to-many, many-to-many relationship in DynamoDB using the ultimate data modeling strategy that has high performance and scales well. Made data modeling in DynamoDB deadly simple.
 
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 ``pynamodb_mate`` is released on PyPI, so all you need is:
```

### Comparing `pynamodb_mate-5.3.4.9/README.rst` & `pynamodb_mate-5.5.1.1/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. image:: https://readthedocs.org/projects/pynamodb_mate/badge/?version=latest
-    :target: https://pynamodb_mate.readthedocs.io/
+    :target: https://pynamodb-mate.readthedocs.io/
     :alt: Documentation Status
 
 .. image:: https://github.com/MacHu-GWU/pynamodb_mate-project/workflows/CI/badge.svg
     :target: https://github.com/MacHu-GWU/pynamodb_mate-project/actions?query=workflow:CI
 
 .. image:: https://codecov.io/gh/MacHu-GWU/pynamodb_mate-project/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/MacHu-GWU/pynamodb_mate-project
@@ -14,28 +14,32 @@
 .. image:: https://img.shields.io/pypi/l/pynamodb_mate.svg
     :target: https://pypi.python.org/pypi/pynamodb_mate
 
 .. image:: https://img.shields.io/pypi/pyversions/pynamodb_mate.svg
     :target: https://pypi.python.org/pypi/pynamodb_mate
 
 .. image:: https://img.shields.io/pypi/dm/pynamodb-mate.svg
+    :target: https://pypi.python.org/pypi/pynamodb_mate
+
+.. image:: https://img.shields.io/badge/Release_History!--None.svg?style=social
+    :target: https://github.com/MacHu-GWU/pynamodb_mate-project/blob/master/release-history.rst
 
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/pynamodb_mate-project
 
 ------
 
 .. image:: https://img.shields.io/badge/Link-Document-blue.svg
-      :target: https://pynamodb_mate.readthedocs.io/
+      :target: https://pynamodb-mate.readthedocs.io/
 
 .. image:: https://img.shields.io/badge/Link-API-blue.svg
-      :target: https://pynamodb_mate.readthedocs.io/py-modindex.html
+      :target: https://pynamodb-mate.readthedocs.io/py-modindex.html
 
 .. image:: https://img.shields.io/badge/Link-Source_Code-blue.svg
-      :target: https://pynamodb_mate.readthedocs.io/py-modindex.html
+      :target: https://pynamodb-mate.readthedocs.io/py-modindex.html
 
 .. image:: https://img.shields.io/badge/Link-Install-blue.svg
       :target: `install`_
 
 .. image:: https://img.shields.io/badge/Link-GitHub-blue.svg
       :target: https://github.com/MacHu-GWU/pynamodb_mate-project
 
@@ -47,48 +51,41 @@
 
 .. image:: https://img.shields.io/badge/Link-Download-blue.svg
       :target: https://pypi.org/pypi/pynamodb_mate#files
 
 
 Welcome to ``pynamodb_mate`` Documentation
 ==============================================================================
-📙 `Full Documentation is Here <https://pynamodb_mate.readthedocs.io/>`_
+📙 `Full Documentation is Here <https://pynamodb-mate.readthedocs.io/>`_
 
-.. contents::
-    :class: this-will-duplicate-information-and-it-is-still-useful-here
-    :depth: 1
-    :local:
+.. image:: https://pynamodb-mate.readthedocs.io/en/latest/_static/pynamodb_mate-logo.png
+    :target: https://pynamodb-mate.readthedocs.io/
 
 
 Overview
 ------------------------------------------------------------------------------
-``pynamodb_mate`` provides advanced best practice using DynamoDB in python. Built on top of `pynamodb <https://pynamodb.readthedocs.io/en/latest/>`_ python library. It maintain the compatibility to major version of ``pynamodb`` library. For example ``pynamodb_mate>=5.0.0,<6.0.0`` is compatible to ``pynamodb>=5.0.0,<6.0.0``.
+``pynamodb_mate`` provides advanced best practice using DynamoDB in python. Built on top of `pynamodb <https://pynamodb.readthedocs.io/en/latest/>`_ python library. It maintain the compatibility to major version of ``pynamodb`` library. For example ``pynamodb_mate>=5.0.0,<6.0.0`` is compatible to ``pynamodb>=5.0.0,<6.0.0``, ``pynamodb_mate==5.5.1.X`` is compatible to ``pynamodb>=5.5.1,<6.0.0``, ``pynamodb_mate==6.0.0.X`` is compatible to ``pynamodb>=6.0.0,<7.0.0``.
 
 
 Disclaimer
 ------------------------------------------------------------------------------
 Even though the author is a Dynamodb Subject Matter Expert from AWS, but this project is NOT an AWS official project, and it is a personal open source project for the Python community.
 
 
 Features
 ------------------------------------------------------------------------------
-Click on the link below to see detailed tutorial and examples.
-
-- ⭐ `Store Large Object in DynamoDB <https://github.com/MacHu-GWU/pynamodb_mate-project/blob/master/examples/Store-Large-Object-in-DynamoDB.ipynb>`_: This feature allows you to store any Python object and arbitrary big data in DynamoDB that can exceed the 400KB limit.
-- ⭐ `Client Side Encryption <https://github.com/MacHu-GWU/pynamodb_mate-project/blob/master/examples/Client-Side-Encryption.ipynb>`_: This feature allows you to use your own encryption key to encrypt your data before it is sent to the DynamoDB.
-- ⭐ `Compressed Attribute <https://github.com/MacHu-GWU/pynamodb_mate-project/blob/master/examples/Compressed-Attribute.ipynb>`_: This feature can automatically compress the data before it is sent to the DynamoDB.
-- ⭐ `AWS DynamoDB Console Url <https://github.com/MacHu-GWU/pynamodb_mate-project/blob/master/examples/AWS-DynamoDB-Console-Url.ipynb>`_: This feature can print the AWS DynamoDB console url for the table, items. You can use this in you log to quickly jump to the console to debug.
-
-
-DynamoDB Patterns
-------------------------------------------------------------------------------
-``pynamodb_mate`` also provides some commonly used patterns. It is based on the author's experience providing solutions to many customers from different industries. Click on the link below to see detailed tutorial and examples.
+``pynamodb_mate`` provides some commonly used patterns. It is based on the author's experience providing solutions to many customers from different industries. Click on the link below to see detailed tutorial and examples.
 
-- 🎉 `Cache <https://github.com/MacHu-GWU/pynamodb_mate-project/blob/master/examples/patterns/cache.ipynb>`_: This feature gives you a "Redis" liked, serverless, Zero-ops, auto-scaling, high performance, pay-as-you-go cache layer based on DynamoDB.
-- 🎉 `Status Tracker <https://github.com/MacHu-GWU/pynamodb_mate-project/blob/master/examples/patterns/status-tracker.ipynb>`_: This feature gives you the ability to track status of each task, and error-handling, retry, concurrency control out-of-the-box.
+- ⭐ `Store Large Object in DynamoDB <https://pynamodb-mate.readthedocs.io/en/latest/01-Store-Large-Object-in-DynamoDB/index.html>`_: This feature allows you to store any Python object and arbitrary big data in DynamoDB that can exceed the 400KB limit. It also handles data consistency and data integrity between DynamoDB and S3.
+- ⭐ `Client Side Encryption <https://pynamodb-mate.readthedocs.io/en/latest/02-Client-Side-Encryption/index.html>`_: This feature allows you to use your own encryption key to encrypt your data before it is sent to the DynamoDB.
+- ⭐ `Compressed Attribute <https://pynamodb-mate.readthedocs.io/en/latest/03-Compressed-Attribute/index.html>`_: This feature can automatically compress the data before it is sent to the DynamoDB, it would save you a lot of money if you use JSON attribute in DynamoDB.
+- ⭐ `AWS DynamoDB Console Url <https://pynamodb-mate.readthedocs.io/en/latest/04-DynamoDB-Consule-Url/index.html>`_: This feature can print the AWS DynamoDB console url for the table, items. You can use this in you log to quickly jump to the console to debug.
+- ⭐ `Use DynamoDB as a Cache Backend <https://pynamodb-mate.readthedocs.io/en/latest/05-Use-DynamoDB-as-Cache-Backend/index.html>`_: This feature gives you a "Redis" liked, serverless, Zero-ops, auto-scaling, high performance, pay-as-you-go cache layer based on DynamoDB.
+- ⭐ `Enable status tracking for business critical application using Amazon DynamoDB <https://pynamodb-mate.readthedocs.io/en/latest/06-Status-Tracker/index.html>`_: This feature gives you the ability to track status of each task, and error-handling, retry, concurrency control out-of-the-box.
+- ⭐ `Modeling Relational Data in DynamoDB <https://pynamodb-mate.readthedocs.io/en/latest/07-Modeling-Relational-Data-in-DynamoDB/index.html>`_: This feature allow you to manage mass amount entity and one-to-many, many-to-many relationship in DynamoDB using the ultimate data modeling strategy that has high performance and scales well. Made data modeling in DynamoDB deadly simple.
 
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 ``pynamodb_mate`` is released on PyPI, so all you need is:
```

### Comparing `pynamodb_mate-5.3.4.9/pynamodb_mate/__init__.py` & `pynamodb_mate-5.5.1.1/pynamodb_mate/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -60,29 +60,48 @@
     from pynamodb.signals import pre_dynamodb_send, post_dynamodb_send
 except ImportError as e:  # pragma: no cover
     print(e)
     pass
 except:  # pragma: no cover
     raise
 
+try:
+    from .type_hint import (
+        REQUIRED_STR,
+        OPTIONAL_STR,
+        REQUIRED_INT,
+        OPTIONAL_INT,
+        REQUIRED_FLOAT,
+        OPTIONAL_FLOAT,
+        REQUIRED_BOOL,
+        OPTIONAL_BOOL,
+        REQUIRED_BINARY,
+        OPTIONAL_BINARY,
+        REQUIRED_DATETIME,
+        OPTIONAL_DATETIME,
+    )
+except ImportError as e:  # pragma: no cover
+    pass
+except:  # pragma: no cover
+    raise
 
 try:
     from .attributes.s3backed import (
         S3BackedAttribute,
         S3BackedBigBinaryAttribute,
         S3BackedBigTextAttribute,
         S3BackedJsonDictAttribute,
     )
     from .attributes.compressed import (
         CompressedAttribute,
         CompressedUnicodeAttribute,
         CompressedBinaryAttribute,
         CompressedJSONDictAttribute,
     )
-    from .models import Model
+    from .models import Model, T_MODEL
 except ImportError as e:  # pragma: no cover
     pass
 except:  # pragma: no cover
     raise
 
 
 try:
@@ -96,12 +115,12 @@
 except ImportError as e:  # pragma: no cover
     pass
 except:  # pragma: no cover
     raise
 
 
 try:
-    from . import patterns
+    from .patterns import api as patterns
 except ImportError as e:  # pragma: no cover
     pass
 except:  # pragma: no cover
     raise
```

### Comparing `pynamodb_mate-5.3.4.9/pynamodb_mate/attributes/compressed.py` & `pynamodb_mate-5.5.1.1/pynamodb_mate/attributes/compressed.py`

 * *Files identical despite different names*

### Comparing `pynamodb_mate-5.3.4.9/pynamodb_mate/attributes/encrypted.py` & `pynamodb_mate-5.5.1.1/pynamodb_mate/attributes/encrypted.py`

 * *Files identical despite different names*

### Comparing `pynamodb_mate-5.3.4.9/pynamodb_mate/attributes/s3backed.py` & `pynamodb_mate-5.5.1.1/pynamodb_mate/attributes/s3backed.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 """
 Store big binary or text in S3 and store the s3 object path in DynamoDB.
 """
 
 import typing as T
 import gzip
 import json
+import warnings
 
+import boto3
 from pynamodb.attributes import (
     UnicodeAttribute,
 )
 from ..helpers import sha256, join_s3_uri, split_s3_uri, is_s3_object_exists
 
-if T.TYPE_CHECKING:
-    import boto3
-    from botocore.client import BaseClient
+if T.TYPE_CHECKING:  # pragma: no cover
+    from mypy_boto3_s3.client import S3Client
 
 
 class S3BackedAttribute(UnicodeAttribute):
     """
     S3BackedAttribute will store the original data on S3 and store the S3 uri
     in DynamoDB.
 
@@ -31,29 +32,42 @@
     :param key_template: the template of the S3 key. It must contain "{fingerprint}",
         and the {fingerprint} is the sha256 of the data
     :param compressed: whether to compress the data before storing it on S3.
     :param s3_client: the boto3 s3 client to read/write data to S3, it is useful
         if you want to use multiple s3 bucket that with different AWS credential.
 
     Other parameters are the same as ``pynamodb.attributes.UnicodeAttribute``.
+
+    .. deprecated:: 5.5.1.1
     """
 
     def __init__(
         self,
         bucket_name: str,
         key_template: str = "pynamodb-mate/s3backed/{fingerprint}",
         compressed: bool = True,
-        s3_client: T.Optional["BaseClient"] = None,
+        s3_client: T.Optional["S3Client"] = None,
         hash_key: bool = False,
         range_key: bool = False,
         null: T.Optional[bool] = None,
         default: T.Optional[T.Callable] = None,
         default_for_new: T.Optional[T.Callable] = None,
         attr_name: T.Optional[str] = None,
     ):
+        warnings.warn(
+            (
+                "pynamodb_mate.attributes.s3backed.S3BackedAttribute, "
+                "pynamodb_mate.attributes.s3backed.S3BackedBigBinaryAttribute, "
+                "pynamodb_mate.attributes.s3backed.S3BackedBigTextAttribute, "
+                "pynamodb_mate.attributes.s3backed.S3BackedJsonDictAttribute "
+                "are deprecated, they will be removed in 6.X. You should use "
+                "pynamodb_mate.patterns.large_attribute.api instead."
+            ),
+            DeprecationWarning,
+        )
         super().__init__(
             hash_key=hash_key,
             range_key=range_key,
             null=null,
             default=default,
             default_for_new=default_for_new,
             attr_name=attr_name,
```

### Comparing `pynamodb_mate-5.3.4.9/pynamodb_mate/cipher.py` & `pynamodb_mate-5.5.1.1/pynamodb_mate/cipher.py`

 * *Files identical despite different names*

### Comparing `pynamodb_mate-5.3.4.9/pynamodb_mate/models.py` & `pynamodb_mate-5.5.1.1/pynamodb_mate/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,14 +110,26 @@
         """
         if copy:
             return copy_lib.deepcopy(self.attribute_values)
         else:
             return self.attribute_values
 
     @classmethod
+    def make_one(
+        cls,
+        hash_key: T.Any,
+        range_key: T.Optional[T.Any] = None,
+        **attributes: T.Any,
+    ):
+        key_attributes = {cls._hash_keyname: hash_key}
+        if range_key is not None:
+            key_attributes[cls._range_keyname] = range_key
+        return cls(**key_attributes, **attributes)
+
+    @classmethod
     def get_one_or_none(
         cls,
         hash_key: T.Any,
         range_key: T.Optional[T.Any] = None,
         consistent_read: bool = False,
         attributes_to_get: T.Optional[T.Sequence[str]] = None,
         settings: OperationSettings = OperationSettings.default,
@@ -362,7 +374,10 @@
                 limit=limit,
                 last_evaluated_key=last_evaluated_key,
                 attributes_to_get=attributes_to_get,
                 page_size=page_size,
                 rate_limit=rate_limit,
             )
         )
+
+
+T_MODEL = T.TypeVar("T_MODEL", bound=Model)
```

### Comparing `pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/abstract.py` & `pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/cache/abstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     :param key: the cache key
     :param value: the binary view of the original value
     :param expire: cache expire time, in seconds
     :param update_ts: last update timestamp
     """
 
     value: bytes
-    expire: int
-    update_ts: int
+    expire: T.Union[int, float]
+    update_ts: T.Union[int, float]
 
     __slots__ = ("value", "expire", "update_ts")
 
 
 class AbstractCache(
     ABC,
     T.Generic[VALUE], # the type of the cached value
@@ -93,15 +93,15 @@
         :param key: cache key.
         :param value: the object you stored in cache.
         :param expire: Time-to-live in seconds.
         """
         record = CacheRecord(
             value=self.serialize(value),
             expire=expire,
-            update_ts=int(utc_now().timestamp()),
+            update_ts=utc_now().timestamp(),
         )
         self._set_record_to_backend(key, record)
 
     def get(
         self,
         key: str,
     ) -> T.Optional[VALUE]:
@@ -109,14 +109,15 @@
         Get object from cache.
 
         :param key: cache key
 
         :return: the cached object.
         """
         record = self._get_record_from_backend(key)
+
         if record is None:
             return None
 
         if record.expire:
             now = utc_now()
             if (now.timestamp() - record.update_ts) < record.expire:
                 return self.deserialize(record.value)
```

### Comparing `pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/backend/dynamodb.py` & `pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/cache/backend/dynamodb.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 DynamoDB backend for cache.
 """
 
 import typing as T
 import json
 
-from pynamodb.models import PAY_PER_REQUEST_BILLING_MODE
+from pynamodb.constants import PAY_PER_REQUEST_BILLING_MODE
 from pynamodb.attributes import (
     UnicodeAttribute,
     BinaryAttribute,
     NumberAttribute,
 )
 
 from ....models import Model
@@ -24,14 +24,23 @@
 class DynamoDBBackend(
     AbstractCache,
     T.Generic[VALUE],
 ):
     """
     Base class for DynamoDB cache backend. You have to implement your own
     ``serialize()`` and ``deserialize()`` methods before use.
+
+    :param table_name: DynamoDB table name
+    :param region: aws region
+    :param billing_mode: billing model to use when creating the table
+    :param write_capacity_units: WCU configuration when creating the table
+    :param read_capacity_units: RCU configuration when creating the table
+    :param create: if True, create the table when initializing the backend,
+        if table already exists, then do nothing. if False, you should create
+        the table manually before using the backend.
     """
 
     def __init__(
         self,
         table_name: str,
         region: T.Optional[str] = None,
         billing_mode: T.Optional[str] = PAY_PER_REQUEST_BILLING_MODE,
```

### Comparing `pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/backend/in_memory.py` & `pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/cache/backend/in_memory.py`

 * *Files identical despite different names*

### Comparing `pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/cache/multi_layer.py` & `pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/cache/multi_layer.py`

 * *Files identical despite different names*

### Comparing `pynamodb_mate-5.3.4.9/pynamodb_mate/patterns/status_tracker/impl.py` & `pynamodb_mate-5.5.1.1/pynamodb_mate/patterns/status_tracker/impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -803,15 +803,16 @@
             status_list = status
         else:
             status_list = [status]
         processed_status_list = [ensure_status_value(status) for status in status_list]
 
         # use index to query by status and aggregate the results
         for status in processed_status_list:
-            yield from cls._get_status_index().query(
+            index = cls._get_status_index()
+            yield from index.query(
                 hash_key=cls.make_value(status, JOB_ID),
                 scan_index_forward=older_task_first,
                 limit=limit,
             )
 
     @classmethod
     def query_by_status(
```

### Comparing `pynamodb_mate-5.3.4.9/pynamodb_mate.egg-info/PKG-INFO` & `pynamodb_mate-5.5.1.1/pynamodb_mate.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: pynamodb-mate
-Version: 5.3.4.9
+Name: pynamodb_mate
+Version: 5.5.1.1
 Summary: Provide Additional Features for pynamodb.
 Home-page: https://github.com/MacHu-GWU/pynamodb_mate-project
-Download-URL: https://pypi.python.org/pypi/pynamodb_mate/5.3.4.9#downloads
+Download-URL: https://pypi.python.org/pypi/pynamodb_mate/5.5.1.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -16,28 +16,53 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.7
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+Requires-Dist: pynamodb<6.0.0,>=5.5.1
+Requires-Dist: cached-property>=1.5.2; python_version < "3.8"
+Requires-Dist: dataclasses>=0.8; python_version == "3.6"
+Requires-Dist: iterproxy<1.0.0,>=0.3.1
 Provides-Extra: encrypt
+Requires-Dist: pycryptodome<4.0.0,>=3.18.0; extra == "encrypt"
 Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: boto3; extra == "tests"
+Requires-Dist: boto_session_manager<2.0.0,>=1.7.2; extra == "tests"
+Requires-Dist: s3pathlib<3.0.0,>=2.1.2; extra == "tests"
+Requires-Dist: pycryptodome<4.0.0,>=3.18.0; extra == "tests"
+Requires-Dist: moto<5.0.0,>=4.1.12; extra == "tests"
+Requires-Dist: moto[dynamodb,s3]<5.0.0,>=4.1.12; extra == "tests"
 Provides-Extra: docs
-License-File: LICENSE.txt
-License-File: AUTHORS.rst
+Requires-Dist: Sphinx==5.3.0; extra == "docs"
+Requires-Dist: sphinx-jinja==2.0.2; extra == "docs"
+Requires-Dist: sphinx-copybutton==0.5.1; extra == "docs"
+Requires-Dist: sphinx-design==0.5.0; extra == "docs"
+Requires-Dist: furo==2023.03.27; extra == "docs"
+Requires-Dist: nbsphinx==0.8.12; extra == "docs"
+Requires-Dist: rstobj==1.2.1; extra == "docs"
+Requires-Dist: pygments==2.15.1; extra == "docs"
+Requires-Dist: ipython==8.10.0; extra == "docs"
+Requires-Dist: docfly==2.0.3; extra == "docs"
+Requires-Dist: pycryptodome<4.0.0,>=3.18.0; extra == "docs"
 
 .. image:: https://readthedocs.org/projects/pynamodb_mate/badge/?version=latest
-    :target: https://pynamodb_mate.readthedocs.io/
+    :target: https://pynamodb-mate.readthedocs.io/
     :alt: Documentation Status
 
 .. image:: https://github.com/MacHu-GWU/pynamodb_mate-project/workflows/CI/badge.svg
     :target: https://github.com/MacHu-GWU/pynamodb_mate-project/actions?query=workflow:CI
 
 .. image:: https://codecov.io/gh/MacHu-GWU/pynamodb_mate-project/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/MacHu-GWU/pynamodb_mate-project
@@ -48,28 +73,32 @@
 .. image:: https://img.shields.io/pypi/l/pynamodb_mate.svg
     :target: https://pypi.python.org/pypi/pynamodb_mate
 
 .. image:: https://img.shields.io/pypi/pyversions/pynamodb_mate.svg
     :target: https://pypi.python.org/pypi/pynamodb_mate
 
 .. image:: https://img.shields.io/pypi/dm/pynamodb-mate.svg
+    :target: https://pypi.python.org/pypi/pynamodb_mate
+
+.. image:: https://img.shields.io/badge/Release_History!--None.svg?style=social
+    :target: https://github.com/MacHu-GWU/pynamodb_mate-project/blob/master/release-history.rst
 
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/pynamodb_mate-project
 
 ------
 
 .. image:: https://img.shields.io/badge/Link-Document-blue.svg
-      :target: https://pynamodb_mate.readthedocs.io/
+      :target: https://pynamodb-mate.readthedocs.io/
 
 .. image:: https://img.shields.io/badge/Link-API-blue.svg
-      :target: https://pynamodb_mate.readthedocs.io/py-modindex.html
+      :target: https://pynamodb-mate.readthedocs.io/py-modindex.html
 
 .. image:: https://img.shields.io/badge/Link-Source_Code-blue.svg
-      :target: https://pynamodb_mate.readthedocs.io/py-modindex.html
+      :target: https://pynamodb-mate.readthedocs.io/py-modindex.html
 
 .. image:: https://img.shields.io/badge/Link-Install-blue.svg
       :target: `install`_
 
 .. image:: https://img.shields.io/badge/Link-GitHub-blue.svg
       :target: https://github.com/MacHu-GWU/pynamodb_mate-project
 
@@ -81,48 +110,41 @@
 
 .. image:: https://img.shields.io/badge/Link-Download-blue.svg
       :target: https://pypi.org/pypi/pynamodb_mate#files
 
 
 Welcome to ``pynamodb_mate`` Documentation
 ==============================================================================
-📙 `Full Documentation is Here <https://pynamodb_mate.readthedocs.io/>`_
+📙 `Full Documentation is Here <https://pynamodb-mate.readthedocs.io/>`_
 
-.. contents::
-    :class: this-will-duplicate-information-and-it-is-still-useful-here
-    :depth: 1
-    :local:
+.. image:: https://pynamodb-mate.readthedocs.io/en/latest/_static/pynamodb_mate-logo.png
+    :target: https://pynamodb-mate.readthedocs.io/
 
 
 Overview
 ------------------------------------------------------------------------------
-``pynamodb_mate`` provides advanced best practice using DynamoDB in python. Built on top of `pynamodb <https://pynamodb.readthedocs.io/en/latest/>`_ python library. It maintain the compatibility to major version of ``pynamodb`` library. For example ``pynamodb_mate>=5.0.0,<6.0.0`` is compatible to ``pynamodb>=5.0.0,<6.0.0``.
+``pynamodb_mate`` provides advanced best practice using DynamoDB in python. Built on top of `pynamodb <https://pynamodb.readthedocs.io/en/latest/>`_ python library. It maintain the compatibility to major version of ``pynamodb`` library. For example ``pynamodb_mate>=5.0.0,<6.0.0`` is compatible to ``pynamodb>=5.0.0,<6.0.0``, ``pynamodb_mate==5.5.1.X`` is compatible to ``pynamodb>=5.5.1,<6.0.0``, ``pynamodb_mate==6.0.0.X`` is compatible to ``pynamodb>=6.0.0,<7.0.0``.
 
 
 Disclaimer
 ------------------------------------------------------------------------------
 Even though the author is a Dynamodb Subject Matter Expert from AWS, but this project is NOT an AWS official project, and it is a personal open source project for the Python community.
 
 
 Features
 ------------------------------------------------------------------------------
-Click on the link below to see detailed tutorial and examples.
-
-- ⭐ `Store Large Object in DynamoDB <https://github.com/MacHu-GWU/pynamodb_mate-project/blob/master/examples/Store-Large-Object-in-DynamoDB.ipynb>`_: This feature allows you to store any Python object and arbitrary big data in DynamoDB that can exceed the 400KB limit.
-- ⭐ `Client Side Encryption <https://github.com/MacHu-GWU/pynamodb_mate-project/blob/master/examples/Client-Side-Encryption.ipynb>`_: This feature allows you to use your own encryption key to encrypt your data before it is sent to the DynamoDB.
-- ⭐ `Compressed Attribute <https://github.com/MacHu-GWU/pynamodb_mate-project/blob/master/examples/Compressed-Attribute.ipynb>`_: This feature can automatically compress the data before it is sent to the DynamoDB.
-- ⭐ `AWS DynamoDB Console Url <https://github.com/MacHu-GWU/pynamodb_mate-project/blob/master/examples/AWS-DynamoDB-Console-Url.ipynb>`_: This feature can print the AWS DynamoDB console url for the table, items. You can use this in you log to quickly jump to the console to debug.
-
-
-DynamoDB Patterns
-------------------------------------------------------------------------------
-``pynamodb_mate`` also provides some commonly used patterns. It is based on the author's experience providing solutions to many customers from different industries. Click on the link below to see detailed tutorial and examples.
+``pynamodb_mate`` provides some commonly used patterns. It is based on the author's experience providing solutions to many customers from different industries. Click on the link below to see detailed tutorial and examples.
 
-- 🎉 `Cache <https://github.com/MacHu-GWU/pynamodb_mate-project/blob/master/examples/patterns/cache.ipynb>`_: This feature gives you a "Redis" liked, serverless, Zero-ops, auto-scaling, high performance, pay-as-you-go cache layer based on DynamoDB.
-- 🎉 `Status Tracker <https://github.com/MacHu-GWU/pynamodb_mate-project/blob/master/examples/patterns/status-tracker.ipynb>`_: This feature gives you the ability to track status of each task, and error-handling, retry, concurrency control out-of-the-box.
+- ⭐ `Store Large Object in DynamoDB <https://pynamodb-mate.readthedocs.io/en/latest/01-Store-Large-Object-in-DynamoDB/index.html>`_: This feature allows you to store any Python object and arbitrary big data in DynamoDB that can exceed the 400KB limit. It also handles data consistency and data integrity between DynamoDB and S3.
+- ⭐ `Client Side Encryption <https://pynamodb-mate.readthedocs.io/en/latest/02-Client-Side-Encryption/index.html>`_: This feature allows you to use your own encryption key to encrypt your data before it is sent to the DynamoDB.
+- ⭐ `Compressed Attribute <https://pynamodb-mate.readthedocs.io/en/latest/03-Compressed-Attribute/index.html>`_: This feature can automatically compress the data before it is sent to the DynamoDB, it would save you a lot of money if you use JSON attribute in DynamoDB.
+- ⭐ `AWS DynamoDB Console Url <https://pynamodb-mate.readthedocs.io/en/latest/04-DynamoDB-Consule-Url/index.html>`_: This feature can print the AWS DynamoDB console url for the table, items. You can use this in you log to quickly jump to the console to debug.
+- ⭐ `Use DynamoDB as a Cache Backend <https://pynamodb-mate.readthedocs.io/en/latest/05-Use-DynamoDB-as-Cache-Backend/index.html>`_: This feature gives you a "Redis" liked, serverless, Zero-ops, auto-scaling, high performance, pay-as-you-go cache layer based on DynamoDB.
+- ⭐ `Enable status tracking for business critical application using Amazon DynamoDB <https://pynamodb-mate.readthedocs.io/en/latest/06-Status-Tracker/index.html>`_: This feature gives you the ability to track status of each task, and error-handling, retry, concurrency control out-of-the-box.
+- ⭐ `Modeling Relational Data in DynamoDB <https://pynamodb-mate.readthedocs.io/en/latest/07-Modeling-Relational-Data-in-DynamoDB/index.html>`_: This feature allow you to manage mass amount entity and one-to-many, many-to-many relationship in DynamoDB using the ultimate data modeling strategy that has high performance and scales well. Made data modeling in DynamoDB deadly simple.
 
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 ``pynamodb_mate`` is released on PyPI, so all you need is:
```

### Comparing `pynamodb_mate-5.3.4.9/pynamodb_mate.egg-info/SOURCES.txt` & `pynamodb_mate-5.5.1.1/pynamodb_mate.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,67 @@
 AUTHORS.rst
 LICENSE.txt
 MANIFEST.in
 README.rst
 release-history.rst
+requirements-automation.txt
 requirements-dev.txt
 requirements-doc.txt
 requirements-encrypt.txt
+requirements-furo-sphinx-search.txt
 requirements-test.txt
 requirements.txt
 setup.py
 pynamodb_mate/__init__.py
 pynamodb_mate/_version.py
+pynamodb_mate/api.py
 pynamodb_mate/cipher.py
 pynamodb_mate/compat.py
 pynamodb_mate/helpers.py
 pynamodb_mate/models.py
+pynamodb_mate/paths.py
+pynamodb_mate/type_hint.py
 pynamodb_mate.egg-info/PKG-INFO
 pynamodb_mate.egg-info/SOURCES.txt
 pynamodb_mate.egg-info/dependency_links.txt
 pynamodb_mate.egg-info/requires.txt
 pynamodb_mate.egg-info/top_level.txt
 pynamodb_mate/attributes/__init__.py
+pynamodb_mate/attributes/api.py
 pynamodb_mate/attributes/compressed.py
 pynamodb_mate/attributes/encrypted.py
 pynamodb_mate/attributes/s3backed.py
 pynamodb_mate/docs/__init__.py
 pynamodb_mate/patterns/__init__.py
+pynamodb_mate/patterns/api.py
 pynamodb_mate/patterns/cache/__init__.py
 pynamodb_mate/patterns/cache/abstract.py
+pynamodb_mate/patterns/cache/api.py
 pynamodb_mate/patterns/cache/multi_layer.py
 pynamodb_mate/patterns/cache/utils.py
 pynamodb_mate/patterns/cache/backend/__init__.py
 pynamodb_mate/patterns/cache/backend/dynamodb.py
 pynamodb_mate/patterns/cache/backend/in_memory.py
+pynamodb_mate/patterns/large_attribute/__init__.py
+pynamodb_mate/patterns/large_attribute/api.py
+pynamodb_mate/patterns/large_attribute/impl.py
+pynamodb_mate/patterns/relationship/__init__.py
+pynamodb_mate/patterns/relationship/api.py
+pynamodb_mate/patterns/relationship/impl.py
 pynamodb_mate/patterns/status_tracker/__init__.py
+pynamodb_mate/patterns/status_tracker/api.py
 pynamodb_mate/patterns/status_tracker/impl.py
-pynamodb_mate/tests/__init__.py
-pynamodb_mate/tests/base.py
-pynamodb_mate/tests/helper.py
-pynamodb_mate/tests/paths.py
+pynamodb_mate/vendor/__init__.py
+pynamodb_mate/vendor/decorator.py
+pynamodb_mate/vendor/iterable.py
+pynamodb_mate/vendor/mark.py
+pynamodb_mate/vendor/mock_aws.py
+pynamodb_mate/vendor/pytest_cov_helper.py
+tests/test_api.py
+tests/test_attr_compressed.py
+tests/test_attr_encrypted.py
+tests/test_attr_s3backed.py
+tests/test_cipher.py
+tests/test_helpers.py
+tests/test_import.py
+tests/test_index.py
+tests/test_models.py
```

### Comparing `pynamodb_mate-5.3.4.9/release-history.rst` & `pynamodb_mate-5.5.1.1/release-history.rst`

 * *Files 18% similar despite different names*

```diff
@@ -8,28 +8,55 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - add automatically rollback if one of the DynamoDB write or S3 write failed.
 - add an option to delete the S3 object as well when the DynamoDB item is deleted.
 - add lazy load option for S3BackedAttribute.
 - add ``clear_expired()`` method to DynamoDB cache backend.
+- add ``large_attribute`` pattern.
 
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+5.5.1.1 (2024-05-22)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Background**
+
+- The ``pynamodb`` implementation relies on some ``botocore`` private API. And one of the private API is changed from ``botocore`` 1.33.2 that breaks the ``pynamodb`` implementation. ``pynamodb`` 5.5.1 fixed the compatibility issue, so that ``pynamodb_mate`` also got upgraded to ``5.5.1.X``.
+
+**Features and Improvements**
+
+- add :mod:`pynamodb_mate.patterns.relationship` Pattern, allow you to manage mass amount entity and one-to-many, many-to-many relationship in DynamoDB using the ultimate data modeling strategy.
+- add :mod:`pynamodb_mate.patterns.large_attribute` Pattern, it re-implements the ``pynamodb_mate.attributes.s3backed`` to provide better consistency model across DynamoDB and S3, and it also support updating multiple large attributes in one API. The old ``pynamodb_mate.attibutes.s3backed`` module is marked as deprecated, and it will be removed in 6.X version.
+- rework the import structure of the library, now we recommend using ``import pynamodb_mate.api as pm`` instead of ``import pynamodb_mate as pm``. Old public API is still available in ``import pynamodb_mate as pm`` name space. And these API is scheduled to be deleted in 6.X version.
+
+**Minor Improvements**
+
+- Rework the unit test, now it uses both mock and real AWS DynamoDB table for testing.
+- Rework the documentation site.
+
+**Miscellaneous**
+
+- add Python3.12 support.
+
+
 5.3.4.9 (2023-05-15)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Bugfixes**
 
 - fix a but that some usages of :meth:`~pynamodb_mate.patterns.status_tracker.impl.BaseStatusTracker.make_value` are missing the parameter job_id.
 
+**Miscellaneous**
+
+- add Python3.11 support.
+
 
 5.3.4.8 (2023-02-03)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - :class:`~pynamodb_mate.patterns.status_tracker.impl.BaseStatusTracker` added ``create_time`` attribute.
 - :class:`~pynamodb_mate.patterns.status_tracker.impl.StatusAndCreateTimeIndex` is renamed to :class:`~pynamodb_mate.patterns.status_tracker.impl.StatusAndUpdateTimeIndex`, and the index now uses ``update_time`` as the range key, and it now uses IncludeProjection.
@@ -48,18 +75,14 @@
 - :class:`~pynamodb_mate.patterns.status_tracker.impl.StatusAndTaskIdIndex` is renamed to :class:`~pynamodb_mate.patterns.status_tracker.impl.StatusAndCreateTimeIndex`, and the index now uses ``create_time`` as the range key, and it now uses AllProjection.
 - :meth:`pynamodb_mate.patterns.status_tracker.impl.BaseStatusTracker.query_by_status` add ``older_task_first`` parameter.
 
 **Minor Improvements**
 
 - improve logging in :meth:`pynamodb_mate.patterns.status_tracker.impl.BaseStatusTracker.start`.
 
-**Bugfixes**
-
-**Miscellaneous**
-
 
 5.3.4.6 (2023-01-16)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - Use iterproxy for Model query and scan, enable type hint in result iterator.
 - Use iterproxy for Model query and scan, enable type hint in result iterator.
```

### Comparing `pynamodb_mate-5.3.4.9/setup.py` & `pynamodb_mate-5.5.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,20 +114,20 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS",
         "Operating System :: Unix",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ]
     """
     Full list can be found at: https://pypi.python.org/pypi?%3Aaction=list_classifiers
     """
 
 
     def read_requirements_file(path):
@@ -182,14 +182,15 @@
         package_data=PACKAGE_DATA,
         py_modules=PY_MODULES,
         url=URL,
         download_url=DOWNLOAD_URL,
         classifiers=CLASSIFIERS,
         platforms=PLATFORMS,
         license=LICENSE,
+        python_requires=">=3.7",
         install_requires=REQUIRES,
         extras_require=EXTRA_REQUIRE,
     )
 
 """
 Appendix
 --------
@@ -233,14 +234,15 @@
     "Operating System :: Unix",
 
     "Programming Language :: Python",
     "Programming Language :: Python :: 2",
     "Programming Language :: Python :: 2.7",
     "Programming Language :: Python :: 2 :: Only",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.4",
-    "Programming Language :: Python :: 3.5",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
 ]
 """
```

