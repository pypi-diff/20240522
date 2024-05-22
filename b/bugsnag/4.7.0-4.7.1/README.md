# Comparing `tmp/bugsnag-4.7.0.tar.gz` & `tmp/bugsnag-4.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bugsnag-4.7.0.tar", last modified: Wed Apr 24 08:29:30 2024, max compression
+gzip compressed data, was "bugsnag-4.7.1.tar", last modified: Wed May 22 08:32:34 2024, max compression
```

## Comparing `bugsnag-4.7.0.tar` & `bugsnag-4.7.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-04-24 08:29:30.049447 bugsnag-4.7.0/
--rw-r--r--   0 joe.haines   (504) staff       (20)     1050 2022-10-04 14:38:17.000000 bugsnag-4.7.0/LICENSE.txt
--rw-r--r--   0 joe.haines   (504) staff       (20)     1363 2024-04-24 08:29:30.049516 bugsnag-4.7.0/PKG-INFO
--rw-r--r--   0 joe.haines   (504) staff       (20)     2025 2024-04-24 08:25:03.000000 bugsnag-4.7.0/README.md
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-04-24 08:29:30.041028 bugsnag-4.7.0/bugsnag/
--rw-r--r--   0 joe.haines   (504) staff       (20)     1523 2024-04-24 08:25:03.000000 bugsnag-4.7.0/bugsnag/__init__.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     4743 2022-10-04 14:38:17.000000 bugsnag-4.7.0/bugsnag/asgi.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     3389 2023-08-16 11:10:44.000000 bugsnag-4.7.0/bugsnag/breadcrumbs.py
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-04-24 08:29:30.042321 bugsnag-4.7.0/bugsnag/celery/
--rw-r--r--   0 joe.haines   (504) staff       (20)      977 2024-04-22 09:23:08.000000 bugsnag-4.7.0/bugsnag/celery/__init__.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    18533 2024-04-24 08:25:03.000000 bugsnag-4.7.0/bugsnag/client.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    20568 2024-04-24 08:25:03.000000 bugsnag-4.7.0/bugsnag/configuration.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     1683 2023-11-15 08:51:17.000000 bugsnag-4.7.0/bugsnag/context.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     5809 2024-04-24 08:25:03.000000 bugsnag-4.7.0/bugsnag/delivery.py
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-04-24 08:29:30.043273 bugsnag-4.7.0/bugsnag/django/
--rw-r--r--   0 joe.haines   (504) staff       (20)     3654 2023-09-01 09:33:43.000000 bugsnag-4.7.0/bugsnag/django/__init__.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     2087 2023-11-15 08:51:17.000000 bugsnag-4.7.0/bugsnag/django/middleware.py
--rw-r--r--   0 joe.haines   (504) staff       (20)      114 2022-10-26 12:09:12.000000 bugsnag-4.7.0/bugsnag/django/utils.py
--rw-r--r--   0 joe.haines   (504) staff       (20)      695 2022-10-04 14:38:17.000000 bugsnag-4.7.0/bugsnag/error.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    15555 2024-04-24 08:25:03.000000 bugsnag-4.7.0/bugsnag/event.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     2894 2023-11-15 08:51:17.000000 bugsnag-4.7.0/bugsnag/feature_flags.py
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-04-24 08:29:30.043552 bugsnag-4.7.0/bugsnag/flask/
--rw-r--r--   0 joe.haines   (504) staff       (20)     2368 2023-12-11 08:33:38.000000 bugsnag-4.7.0/bugsnag/flask/__init__.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     6512 2023-08-09 13:05:44.000000 bugsnag-4.7.0/bugsnag/handlers.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     5271 2024-04-24 08:25:03.000000 bugsnag-4.7.0/bugsnag/legacy.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     5336 2023-01-19 12:01:29.000000 bugsnag-4.7.0/bugsnag/middleware.py
--rw-r--r--   0 joe.haines   (504) staff       (20)      464 2022-10-04 14:38:17.000000 bugsnag-4.7.0/bugsnag/notification.py
--rw-r--r--   0 joe.haines   (504) staff       (20)      146 2024-04-24 08:25:03.000000 bugsnag-4.7.0/bugsnag/notifier.py
--rw-r--r--   0 joe.haines   (504) staff       (20)        0 2022-10-04 14:38:17.000000 bugsnag-4.7.0/bugsnag/py.typed
--rw-r--r--   0 joe.haines   (504) staff       (20)     1533 2024-04-24 08:25:03.000000 bugsnag-4.7.0/bugsnag/request_tracker.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     5628 2024-04-24 08:25:03.000000 bugsnag-4.7.0/bugsnag/sessiontracker.py
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-04-24 08:29:30.043821 bugsnag-4.7.0/bugsnag/tornado/
--rw-r--r--   0 joe.haines   (504) staff       (20)     5900 2023-11-15 08:51:17.000000 bugsnag-4.7.0/bugsnag/tornado/__init__.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    15245 2024-04-24 08:25:03.000000 bugsnag-4.7.0/bugsnag/utils.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     1096 2022-10-04 14:38:17.000000 bugsnag-4.7.0/bugsnag/uwsgi.py
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-04-24 08:29:30.044325 bugsnag-4.7.0/bugsnag/wsgi/
--rw-r--r--   0 joe.haines   (504) staff       (20)      147 2022-10-04 14:38:17.000000 bugsnag-4.7.0/bugsnag/wsgi/__init__.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     3822 2023-11-15 08:51:17.000000 bugsnag-4.7.0/bugsnag/wsgi/middleware.py
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-04-24 08:29:30.042155 bugsnag-4.7.0/bugsnag.egg-info/
--rw-r--r--   0 joe.haines   (504) staff       (20)     1363 2024-04-24 08:29:30.000000 bugsnag-4.7.0/bugsnag.egg-info/PKG-INFO
--rw-r--r--   0 joe.haines   (504) staff       (20)     1278 2024-04-24 08:29:30.000000 bugsnag-4.7.0/bugsnag.egg-info/SOURCES.txt
--rw-r--r--   0 joe.haines   (504) staff       (20)        1 2024-04-24 08:29:30.000000 bugsnag-4.7.0/bugsnag.egg-info/dependency_links.txt
--rw-r--r--   0 joe.haines   (504) staff       (20)       29 2024-04-24 08:29:30.000000 bugsnag-4.7.0/bugsnag.egg-info/requires.txt
--rw-r--r--   0 joe.haines   (504) staff       (20)        8 2024-04-24 08:29:30.000000 bugsnag-4.7.0/bugsnag.egg-info/top_level.txt
--rw-r--r--   0 joe.haines   (504) staff       (20)       76 2024-04-24 08:29:30.049744 bugsnag-4.7.0/setup.cfg
--rwxr-xr-x   0 joe.haines   (504) staff       (20)     1703 2024-04-24 08:25:03.000000 bugsnag-4.7.0/setup.py
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-04-24 08:29:30.049060 bugsnag-4.7.0/tests/
--rw-r--r--   0 joe.haines   (504) staff       (20)    11758 2023-11-15 08:51:17.000000 bugsnag-4.7.0/tests/test_breadcrumbs.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    68059 2024-04-24 08:25:03.000000 bugsnag-4.7.0/tests/test_client.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    24428 2024-03-05 09:31:55.000000 bugsnag-4.7.0/tests/test_configuration.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     4141 2023-11-15 08:51:17.000000 bugsnag-4.7.0/tests/test_context.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     6259 2024-04-24 08:25:03.000000 bugsnag-4.7.0/tests/test_delivery.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    18688 2023-11-15 08:51:17.000000 bugsnag-4.7.0/tests/test_event.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    14774 2023-12-11 08:33:38.000000 bugsnag-4.7.0/tests/test_exception_groups.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    10736 2023-11-15 08:51:17.000000 bugsnag-4.7.0/tests/test_feature_flags.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    24308 2023-12-11 08:33:38.000000 bugsnag-4.7.0/tests/test_handlers.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     4539 2022-11-02 11:51:55.000000 bugsnag-4.7.0/tests/test_middleware.py
--rw-r--r--   0 joe.haines   (504) staff       (20)      777 2022-10-04 14:38:17.000000 bugsnag-4.7.0/tests/test_notification.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    36483 2023-12-11 08:33:38.000000 bugsnag-4.7.0/tests/test_notify.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     3255 2022-10-04 14:38:17.000000 bugsnag-4.7.0/tests/test_path_encoding.py
--rw-r--r--   0 joe.haines   (504) staff       (20)      477 2022-10-04 14:38:17.000000 bugsnag-4.7.0/tests/test_request_config.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     1509 2024-04-24 08:25:03.000000 bugsnag-4.7.0/tests/test_request_tracker.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     2200 2022-10-04 14:38:17.000000 bugsnag-4.7.0/tests/test_sessionmiddleware.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     7408 2024-04-24 08:25:03.000000 bugsnag-4.7.0/tests/test_sessiontracker.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    22469 2023-11-16 15:02:21.000000 bugsnag-4.7.0/tests/test_utils.py
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-05-22 08:32:34.683006 bugsnag-4.7.1/
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1050 2022-10-04 14:38:17.000000 bugsnag-4.7.1/LICENSE.txt
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1464 2024-05-22 08:32:34.682897 bugsnag-4.7.1/PKG-INFO
+-rw-r--r--   0 joe.haines   (504) staff       (20)     2025 2024-04-24 08:48:29.000000 bugsnag-4.7.1/README.md
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-05-22 08:32:34.668679 bugsnag-4.7.1/bugsnag/
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1523 2024-04-24 08:25:03.000000 bugsnag-4.7.1/bugsnag/__init__.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     4743 2022-10-04 14:38:17.000000 bugsnag-4.7.1/bugsnag/asgi.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     3389 2023-08-16 11:10:44.000000 bugsnag-4.7.1/bugsnag/breadcrumbs.py
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-05-22 08:32:34.669741 bugsnag-4.7.1/bugsnag/celery/
+-rw-r--r--   0 joe.haines   (504) staff       (20)      977 2024-04-22 09:23:08.000000 bugsnag-4.7.1/bugsnag/celery/__init__.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    18533 2024-04-24 08:25:03.000000 bugsnag-4.7.1/bugsnag/client.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    20852 2024-05-22 08:30:51.000000 bugsnag-4.7.1/bugsnag/configuration.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1683 2023-11-15 08:51:17.000000 bugsnag-4.7.1/bugsnag/context.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     6224 2024-05-22 08:30:51.000000 bugsnag-4.7.1/bugsnag/delivery.py
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-05-22 08:32:34.670729 bugsnag-4.7.1/bugsnag/django/
+-rw-r--r--   0 joe.haines   (504) staff       (20)     3654 2023-09-01 09:33:43.000000 bugsnag-4.7.1/bugsnag/django/__init__.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     2087 2023-11-15 08:51:17.000000 bugsnag-4.7.1/bugsnag/django/middleware.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)      114 2022-10-26 12:09:12.000000 bugsnag-4.7.1/bugsnag/django/utils.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)      695 2022-10-04 14:38:17.000000 bugsnag-4.7.1/bugsnag/error.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    15555 2024-04-24 08:25:03.000000 bugsnag-4.7.1/bugsnag/event.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     2894 2023-11-15 08:51:17.000000 bugsnag-4.7.1/bugsnag/feature_flags.py
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-05-22 08:32:34.671015 bugsnag-4.7.1/bugsnag/flask/
+-rw-r--r--   0 joe.haines   (504) staff       (20)     2368 2023-12-11 08:33:38.000000 bugsnag-4.7.1/bugsnag/flask/__init__.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     6512 2023-08-09 13:05:44.000000 bugsnag-4.7.1/bugsnag/handlers.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     5271 2024-04-24 08:25:03.000000 bugsnag-4.7.1/bugsnag/legacy.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     5336 2023-01-19 12:01:29.000000 bugsnag-4.7.1/bugsnag/middleware.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)      464 2022-10-04 14:38:17.000000 bugsnag-4.7.1/bugsnag/notification.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)      146 2024-05-22 08:30:51.000000 bugsnag-4.7.1/bugsnag/notifier.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)        0 2022-10-04 14:38:17.000000 bugsnag-4.7.1/bugsnag/py.typed
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1533 2024-04-24 08:25:03.000000 bugsnag-4.7.1/bugsnag/request_tracker.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     5709 2024-05-22 08:30:51.000000 bugsnag-4.7.1/bugsnag/sessiontracker.py
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-05-22 08:32:34.671484 bugsnag-4.7.1/bugsnag/tornado/
+-rw-r--r--   0 joe.haines   (504) staff       (20)     5900 2023-11-15 08:51:17.000000 bugsnag-4.7.1/bugsnag/tornado/__init__.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    15245 2024-04-24 08:25:03.000000 bugsnag-4.7.1/bugsnag/utils.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1096 2022-10-04 14:38:17.000000 bugsnag-4.7.1/bugsnag/uwsgi.py
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-05-22 08:32:34.671988 bugsnag-4.7.1/bugsnag/wsgi/
+-rw-r--r--   0 joe.haines   (504) staff       (20)      147 2022-10-04 14:38:17.000000 bugsnag-4.7.1/bugsnag/wsgi/__init__.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     3822 2023-11-15 08:51:17.000000 bugsnag-4.7.1/bugsnag/wsgi/middleware.py
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-05-22 08:32:34.682441 bugsnag-4.7.1/bugsnag.egg-info/
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1464 2024-05-22 08:32:34.000000 bugsnag-4.7.1/bugsnag.egg-info/PKG-INFO
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1278 2024-05-22 08:32:34.000000 bugsnag-4.7.1/bugsnag.egg-info/SOURCES.txt
+-rw-r--r--   0 joe.haines   (504) staff       (20)        1 2024-05-22 08:32:34.000000 bugsnag-4.7.1/bugsnag.egg-info/dependency_links.txt
+-rw-r--r--   0 joe.haines   (504) staff       (20)       29 2024-05-22 08:32:34.000000 bugsnag-4.7.1/bugsnag.egg-info/requires.txt
+-rw-r--r--   0 joe.haines   (504) staff       (20)        8 2024-05-22 08:32:34.000000 bugsnag-4.7.1/bugsnag.egg-info/top_level.txt
+-rw-r--r--   0 joe.haines   (504) staff       (20)       76 2024-05-22 08:32:34.683333 bugsnag-4.7.1/setup.cfg
+-rwxr-xr-x   0 joe.haines   (504) staff       (20)     1703 2024-05-22 08:30:51.000000 bugsnag-4.7.1/setup.py
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-05-22 08:32:34.679106 bugsnag-4.7.1/tests/
+-rw-r--r--   0 joe.haines   (504) staff       (20)    11758 2024-05-17 08:58:12.000000 bugsnag-4.7.1/tests/test_breadcrumbs.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    68732 2024-05-22 08:30:51.000000 bugsnag-4.7.1/tests/test_client.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    24428 2024-03-05 09:31:55.000000 bugsnag-4.7.1/tests/test_configuration.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     4141 2023-11-15 08:51:17.000000 bugsnag-4.7.1/tests/test_context.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     6259 2024-05-21 05:51:21.000000 bugsnag-4.7.1/tests/test_delivery.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    18688 2023-11-15 08:51:17.000000 bugsnag-4.7.1/tests/test_event.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    14774 2023-12-11 08:33:38.000000 bugsnag-4.7.1/tests/test_exception_groups.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    10736 2023-11-15 08:51:17.000000 bugsnag-4.7.1/tests/test_feature_flags.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    24308 2023-12-11 08:33:38.000000 bugsnag-4.7.1/tests/test_handlers.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     4539 2022-11-02 11:51:55.000000 bugsnag-4.7.1/tests/test_middleware.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)      777 2022-10-04 14:38:17.000000 bugsnag-4.7.1/tests/test_notification.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    36483 2023-12-11 08:33:38.000000 bugsnag-4.7.1/tests/test_notify.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     3255 2022-10-04 14:38:17.000000 bugsnag-4.7.1/tests/test_path_encoding.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)      477 2022-10-04 14:38:17.000000 bugsnag-4.7.1/tests/test_request_config.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1509 2024-04-24 08:25:03.000000 bugsnag-4.7.1/tests/test_request_tracker.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     2200 2022-10-04 14:38:17.000000 bugsnag-4.7.1/tests/test_sessionmiddleware.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     7408 2024-04-24 08:25:03.000000 bugsnag-4.7.1/tests/test_sessiontracker.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    22469 2023-11-16 15:02:21.000000 bugsnag-4.7.1/tests/test_utils.py
```

### Comparing `bugsnag-4.7.0/LICENSE.txt` & `bugsnag-4.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/PKG-INFO` & `bugsnag-4.7.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bugsnag
-Version: 4.7.0
+Version: 4.7.1
 Summary: Automatic error monitoring for django, flask, etc.
 Home-page: https://bugsnag.com/
 Author: Simon Maynard
 Author-email: simon@bugsnag.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -20,16 +20,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Requires-Python: >=3.5, <4
-Provides-Extra: flask
 License-File: LICENSE.txt
+Requires-Dist: webob
+Provides-Extra: flask
+Requires-Dist: flask; extra == "flask"
+Requires-Dist: blinker; extra == "flask"
 
 
 Bugsnag
 =======
 
 The official Python notifier for `Bugsnag <https://bugsnag.com/>`_.
 Provides support for automatically capturing and sending exceptions
```

### Comparing `bugsnag-4.7.0/README.md` & `bugsnag-4.7.1/README.md`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/bugsnag/__init__.py` & `bugsnag-4.7.1/bugsnag/__init__.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/bugsnag/asgi.py` & `bugsnag-4.7.1/bugsnag/asgi.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/bugsnag/breadcrumbs.py` & `bugsnag-4.7.1/bugsnag/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/bugsnag/celery/__init__.py` & `bugsnag-4.7.1/bugsnag/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/bugsnag/client.py` & `bugsnag-4.7.1/bugsnag/client.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/bugsnag/configuration.py` & `bugsnag-4.7.1/bugsnag/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,15 +275,19 @@
             self._delivery = value
 
             # deliver_sessions is _technically_ optional in that if you disable
             # session tracking it will never be called
             # this should be made mandatory in the next major release
             if (
                 hasattr(value, 'deliver_sessions') and
-                callable(value.deliver_sessions)
+                callable(value.deliver_sessions) and
+                # Mock objects don't allow accessing or mocking '__code__' so
+                # ensure it exists before attempting to read it
+                # __code__ should always be present in a real delivery object
+                hasattr(value.deliver_sessions, '__code__')
             ):
                 parameter_names = value.deliver_sessions.__code__.co_varnames
 
                 if 'options' not in parameter_names:
                     warnings.warn(
                         'delivery.deliver_sessions should accept an ' +
                         '"options" parameter to allow for synchronous ' +
```

### Comparing `bugsnag-4.7.0/bugsnag/context.py` & `bugsnag-4.7.1/bugsnag/context.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/bugsnag/delivery.py` & `bugsnag-4.7.1/bugsnag/delivery.py`

 * *Files 14% similar despite different names*

```diff
@@ -89,15 +89,14 @@
                               'No sessions will be sent to Bugsnag.')
                 self.sent_session_warning = True
         else:
             if options is None:
                 options = {}
 
             options['endpoint'] = config.session_endpoint
-            options['success'] = 202
 
             self.deliver(config, payload, options)
 
     def queue_request(self, request: Callable, config, options: Dict):
         post_delivery_callback = _marshall_post_delivery_callback(
             options.pop('post_delivery_callback', None)
         )
@@ -147,18 +146,22 @@
             else:
                 opener = build_opener()
 
             resp = opener.open(req)
             status = resp.getcode()
 
             if 'success' in options:
-                success = options['success']
+                # if an expected status code has been given then it must match
+                # exactly with the actual status code
+                success = status == options['success']
             else:
-                success = 200
-            if status != success:
+                # warn if we don't get a 2xx status code by default
+                success = status >= 200 and status < 300
+
+            if not success:
                 config.logger.warning(
                     'Delivery to %s failed, status %d' % (uri, status)
                 )
 
         self.queue_request(request, config, options)
 
 
@@ -180,18 +183,22 @@
                 req_options['proxies'] = {
                     'https': config.proxy_host,
                     'http': config.proxy_host
                 }
 
             response = requests.post(uri, **req_options)
             status = response.status_code
+
             if 'success' in options:
-                success = options['success']
+                # if an expected status code has been given then it must match
+                # exactly with the actual status code
+                success = status == options['success']
             else:
-                success = requests.codes.ok
+                # warn if we don't get a 2xx status code by default
+                success = status >= 200 and status < 300
 
-            if status != success:
+            if not success:
                 config.logger.warning(
                     'Delivery to %s failed, status %d' % (uri, status)
                 )
 
         self.queue_request(request, config, options)
```

### Comparing `bugsnag-4.7.0/bugsnag/django/__init__.py` & `bugsnag-4.7.1/bugsnag/django/__init__.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/bugsnag/django/middleware.py` & `bugsnag-4.7.1/bugsnag/django/middleware.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/bugsnag/error.py` & `bugsnag-4.7.1/bugsnag/error.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/bugsnag/event.py` & `bugsnag-4.7.1/bugsnag/event.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/bugsnag/feature_flags.py` & `bugsnag-4.7.1/bugsnag/feature_flags.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/bugsnag/flask/__init__.py` & `bugsnag-4.7.1/bugsnag/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/bugsnag/handlers.py` & `bugsnag-4.7.1/bugsnag/handlers.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/bugsnag/legacy.py` & `bugsnag-4.7.1/bugsnag/legacy.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/bugsnag/middleware.py` & `bugsnag-4.7.1/bugsnag/middleware.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/bugsnag/request_tracker.py` & `bugsnag-4.7.1/bugsnag/request_tracker.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/bugsnag/sessiontracker.py` & `bugsnag-4.7.1/bugsnag/sessiontracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,18 @@
                 keyword_filters=self.config.params_filters
             )
 
             encoded_payload = encoder.encode(payload)
 
             deliver = self.config.delivery.deliver_sessions
 
-            if 'options' in deliver.__code__.co_varnames:
+            if (
+                hasattr(deliver, '__code__') and
+                'options' in deliver.__code__.co_varnames
+            ):
                 try:
                     post_delivery_callback = self._request_tracker.new_request()
 
                     deliver(
                         self.config,
                         encoded_payload,
                         options={
```

### Comparing `bugsnag-4.7.0/bugsnag/tornado/__init__.py` & `bugsnag-4.7.1/bugsnag/tornado/__init__.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/bugsnag/utils.py` & `bugsnag-4.7.1/bugsnag/utils.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/bugsnag/uwsgi.py` & `bugsnag-4.7.1/bugsnag/uwsgi.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/bugsnag/wsgi/middleware.py` & `bugsnag-4.7.1/bugsnag/wsgi/middleware.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/bugsnag.egg-info/PKG-INFO` & `bugsnag-4.7.1/bugsnag.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bugsnag
-Version: 4.7.0
+Version: 4.7.1
 Summary: Automatic error monitoring for django, flask, etc.
 Home-page: https://bugsnag.com/
 Author: Simon Maynard
 Author-email: simon@bugsnag.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -20,16 +20,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Requires-Python: >=3.5, <4
-Provides-Extra: flask
 License-File: LICENSE.txt
+Requires-Dist: webob
+Provides-Extra: flask
+Requires-Dist: flask; extra == "flask"
+Requires-Dist: blinker; extra == "flask"
 
 
 Bugsnag
 =======
 
 The official Python notifier for `Bugsnag <https://bugsnag.com/>`_.
 Provides support for automatically capturing and sending exceptions
```

### Comparing `bugsnag-4.7.0/bugsnag.egg-info/SOURCES.txt` & `bugsnag-4.7.1/bugsnag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/setup.py` & `bugsnag-4.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 and solve your bugs as fast as possible.
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name='bugsnag',
-    version='4.7.0',
+    version='4.7.1',
     description='Automatic error monitoring for django, flask, etc.',
     long_description=__doc__,
     author='Simon Maynard',
     author_email='simon@bugsnag.com',
     url='https://bugsnag.com/',
     license='MIT',
     python_requires='>=3.5, <4',
```

### Comparing `bugsnag-4.7.0/tests/test_breadcrumbs.py` & `bugsnag-4.7.1/tests/test_breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/tests/test_client.py` & `bugsnag-4.7.1/tests/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Client,
     Configuration,
     BreadcrumbType,
     Breadcrumb,
     FeatureFlag
 )
 
+from bugsnag.delivery import Delivery
 import bugsnag.legacy as legacy
 from tests.utils import (
     BrokenDelivery,
     IntegrationTest,
     QueueingDelivery,
     ScaryException,
 )
@@ -120,14 +121,30 @@
 
         c.configure(delivery=FooDelivery(), api_key='abc')
         client = Client(c)
         client.notify(Exception('Oh no'))
         self.assertTrue(self.called)
         del self.called
 
+    # test for a regression caused by reading '__code__', which does not exist
+    # on Mock objects, nor can it be mocked
+    # see: https://github.com/bugsnag/bugsnag-python/commit/77e11747c293ba715bc764d17b49fb32918c030a#r142130768  # noqa: E501
+    def test_delivery_can_be_mocked(self):
+        delivery = Mock(spec=Delivery)
+
+        client = Client(delivery=delivery, api_key='abc')
+        client.notify(Exception('Oh no'))
+
+        assert delivery.deliver.call_count == 1
+
+        client.session_tracker.start_session()
+        client.session_tracker.send_sessions()
+
+        assert delivery.deliver_sessions.call_count == 1
+
     # Capture
 
     def test_notify_capture(self):
         try:
             with self.client.capture():
                 raise Exception('Testing Notify Context')
         except Exception:
```

### Comparing `bugsnag-4.7.0/tests/test_configuration.py` & `bugsnag-4.7.1/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/tests/test_context.py` & `bugsnag-4.7.1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/tests/test_delivery.py` & `bugsnag-4.7.1/tests/test_delivery.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/tests/test_event.py` & `bugsnag-4.7.1/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/tests/test_exception_groups.py` & `bugsnag-4.7.1/tests/test_exception_groups.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/tests/test_feature_flags.py` & `bugsnag-4.7.1/tests/test_feature_flags.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/tests/test_handlers.py` & `bugsnag-4.7.1/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/tests/test_middleware.py` & `bugsnag-4.7.1/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/tests/test_notification.py` & `bugsnag-4.7.1/tests/test_notification.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/tests/test_notify.py` & `bugsnag-4.7.1/tests/test_notify.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/tests/test_path_encoding.py` & `bugsnag-4.7.1/tests/test_path_encoding.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/tests/test_request_tracker.py` & `bugsnag-4.7.1/tests/test_request_tracker.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/tests/test_sessionmiddleware.py` & `bugsnag-4.7.1/tests/test_sessionmiddleware.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/tests/test_sessiontracker.py` & `bugsnag-4.7.1/tests/test_sessiontracker.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.7.0/tests/test_utils.py` & `bugsnag-4.7.1/tests/test_utils.py`

 * *Files identical despite different names*

