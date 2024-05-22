# Comparing `tmp/pyslth-0.4.7.tar.gz` & `tmp/pyslth-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.4.7.tar", last modified: Tue May 21 10:12:27 2024, max compression
+gzip compressed data, was "pyslth-0.4.8.tar", last modified: Wed May 22 16:45:58 2024, max compression
```

## Comparing `pyslth-0.4.7.tar` & `pyslth-0.4.8.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-21 10:12:27.058977 pyslth-0.4.7/
--rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.4.7/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-21 10:12:27.058755 pyslth-0.4.7/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-21 10:12:27.018871 pyslth-0.4.7/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-21 10:12:26.000000 pyslth-0.4.7/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)     1958 2024-05-21 10:12:26.000000 pyslth-0.4.7/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-21 10:12:26.000000 pyslth-0.4.7/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-21 10:12:26.000000 pyslth-0.4.7/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-21 10:12:26.000000 pyslth-0.4.7/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.4.7/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-21 10:12:27.059038 pyslth-0.4.7/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-21 10:11:09.000000 pyslth-0.4.7/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-21 10:12:27.027652 pyslth-0.4.7/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3779 2024-05-10 13:02:33.000000 pyslth-0.4.7/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     9885 2024-05-21 00:15:25.000000 pyslth-0.4.7/slth/components.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-21 10:12:27.031684 pyslth-0.4.7/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.4.7/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     5031 2024-05-13 19:37:29.000000 pyslth-0.4.7/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    24799 2024-05-21 10:09:07.000000 pyslth-0.4.7/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.4.7/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)     4451 2024-05-16 10:23:26.000000 pyslth-0.4.7/slth/factory.py
--rw-r--r--   0 breno      (501) staff       (20)    26476 2024-05-16 10:18:46.000000 pyslth-0.4.7/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-21 10:12:27.032064 pyslth-0.4.7/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.4.7/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-21 10:12:27.032716 pyslth-0.4.7/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.4.7/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.4.7/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.4.7/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-21 10:12:27.036261 pyslth-0.4.7/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.4.7/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.4.7/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.4.7/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
--rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.4.7/slth/migrations/0004_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.4.7/slth/migrations/0005_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.4.7/slth/migrations/0006_user.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.4.7/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6546 2024-05-11 10:34:23.000000 pyslth-0.4.7/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      565 2024-05-18 08:21:00.000000 pyslth-0.4.7/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 pyslth-0.4.7/slth/oauth.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-05-18 17:29:04.000000 pyslth-0.4.7/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    19965 2024-05-16 13:39:18.000000 pyslth-0.4.7/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.4.7/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-21 10:12:27.036794 pyslth-0.4.7/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.4.7/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.4.7/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    15898 2024-05-13 01:13:17.000000 pyslth-0.4.7/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-21 10:12:27.037416 pyslth-0.4.7/slth/static/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-05-20 11:57:45.000000 pyslth-0.4.7/slth/static/.DS_Store
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-21 10:12:27.039211 pyslth-0.4.7/slth/static/css/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.4.7/slth/static/css/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.4.7/slth/static/css/fontawesome.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-21 10:12:27.043232 pyslth-0.4.7/slth/static/css/fonts/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.4.7/slth/static/css/fonts/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.4.7/slth/static/css/fonts/fa-solid-900.woff2
--rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.4.7/slth/static/css/fonts/rawline-400.woff
--rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.4.7/slth/static/css/fonts/rawline-500i.woff
--rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.4.7/slth/static/css/fonts/rawline-700.woff
--rw-r--r--   0 breno      (501) staff       (20)     1977 2024-05-12 18:54:58.000000 pyslth-0.4.7/slth/static/css/slth.css
--rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.4.7/slth/static/css/solid.min.css
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-05-07 11:57:26.000000 pyslth-0.4.7/slth/static/css/style.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-21 10:12:27.045842 pyslth-0.4.7/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.4.7/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.4.7/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.4.7/slth/static/images/user.png
--rw-r--r--   0 breno      (501) staff       (20)      492 2024-05-07 12:51:28.000000 pyslth-0.4.7/slth/static/images/user.svg
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.4.7/slth/static/index.html
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-21 10:12:27.057767 pyslth-0.4.7/slth/static/js/
--rw-r--r--   0 breno      (501) staff       (20)      946 2024-05-19 17:15:44.000000 pyslth-0.4.7/slth/static/js/default-passive-events.min.js
--rw-r--r--   0 breno      (501) staff       (20)  1112413 2024-05-18 14:48:49.000000 pyslth-0.4.7/slth/static/js/echarts.min.js
--rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-21 10:11:57.000000 pyslth-0.4.7/slth/static/js/index.min.js
--rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.4.7/slth/static/js/ios-splash.min.js
--rw-r--r--   0 breno      (501) staff       (20)   117723 2024-05-08 16:11:56.000000 pyslth-0.4.7/slth/static/js/peerjs.min.js
--rw-r--r--   0 breno      (501) staff       (20)    92865 2024-05-19 22:43:39.000000 pyslth-0.4.7/slth/static/js/peerjs154.min.js
--rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.4.7/slth/static/js/qrcode.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.4.7/slth/static/js/react-trigger-change.js
--rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-21 10:11:57.000000 pyslth-0.4.7/slth/static/js/react.min.js
--rw-r--r--   0 breno      (501) staff       (20)   102016 2024-05-21 10:11:57.000000 pyslth-0.4.7/slth/static/js/slth.min.js
--rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.4.7/slth/static/js/vanilla-masker.js
--rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.4.7/slth/static/js/vanilla-masker.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6361 2024-05-16 13:05:44.000000 pyslth-0.4.7/slth/statistics.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-21 10:12:27.058338 pyslth-0.4.7/slth/templates/
--rw-r--r--   0 breno      (501) staff       (20)     3230 2024-05-19 22:46:51.000000 pyslth-0.4.7/slth/templates/index.html
--rw-r--r--   0 breno      (501) staff       (20)     1456 2024-05-18 10:06:11.000000 pyslth-0.4.7/slth/templates/service-worker.js
--rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.4.7/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.4.7/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1000 2024-05-13 01:26:42.000000 pyslth-0.4.7/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     2572 2024-05-08 14:06:07.000000 pyslth-0.4.7/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.906458 pyslth-0.4.8/
+-rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.4.8/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-22 16:45:58.906188 pyslth-0.4.8/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.805660 pyslth-0.4.8/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-22 16:45:58.000000 pyslth-0.4.8/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)     1958 2024-05-22 16:45:58.000000 pyslth-0.4.8/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-22 16:45:58.000000 pyslth-0.4.8/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-22 16:45:58.000000 pyslth-0.4.8/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-22 16:45:58.000000 pyslth-0.4.8/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.4.8/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-22 16:45:58.906538 pyslth-0.4.8/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-22 16:45:42.000000 pyslth-0.4.8/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.828560 pyslth-0.4.8/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3779 2024-05-10 13:02:33.000000 pyslth-0.4.8/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     9973 2024-05-22 14:21:00.000000 pyslth-0.4.8/slth/components.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.830475 pyslth-0.4.8/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.4.8/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     5031 2024-05-13 19:37:29.000000 pyslth-0.4.8/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    25441 2024-05-22 14:22:43.000000 pyslth-0.4.8/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.4.8/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)     4451 2024-05-16 10:23:26.000000 pyslth-0.4.8/slth/factory.py
+-rw-r--r--   0 breno      (501) staff       (20)    26814 2024-05-22 12:50:05.000000 pyslth-0.4.8/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.830904 pyslth-0.4.8/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.4.8/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.834409 pyslth-0.4.8/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.4.8/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.4.8/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.4.8/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.843896 pyslth-0.4.8/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.4.8/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.4.8/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.4.8/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+-rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.4.8/slth/migrations/0004_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.4.8/slth/migrations/0005_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.4.8/slth/migrations/0006_user.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.4.8/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6546 2024-05-11 10:34:23.000000 pyslth-0.4.8/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      565 2024-05-18 08:21:00.000000 pyslth-0.4.8/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 pyslth-0.4.8/slth/oauth.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-05-18 17:29:04.000000 pyslth-0.4.8/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    19965 2024-05-16 13:39:18.000000 pyslth-0.4.8/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.4.8/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.844860 pyslth-0.4.8/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.4.8/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.4.8/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    15969 2024-05-21 20:16:17.000000 pyslth-0.4.8/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.848045 pyslth-0.4.8/slth/static/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-05-20 11:57:45.000000 pyslth-0.4.8/slth/static/.DS_Store
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.854054 pyslth-0.4.8/slth/static/css/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.4.8/slth/static/css/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.4.8/slth/static/css/fontawesome.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.866796 pyslth-0.4.8/slth/static/css/fonts/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.4.8/slth/static/css/fonts/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.4.8/slth/static/css/fonts/fa-solid-900.woff2
+-rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.4.8/slth/static/css/fonts/rawline-400.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.4.8/slth/static/css/fonts/rawline-500i.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.4.8/slth/static/css/fonts/rawline-700.woff
+-rw-r--r--   0 breno      (501) staff       (20)     1977 2024-05-12 18:54:58.000000 pyslth-0.4.8/slth/static/css/slth.css
+-rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.4.8/slth/static/css/solid.min.css
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-05-07 11:57:26.000000 pyslth-0.4.8/slth/static/css/style.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.874298 pyslth-0.4.8/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.4.8/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.4.8/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.4.8/slth/static/images/user.png
+-rw-r--r--   0 breno      (501) staff       (20)      492 2024-05-07 12:51:28.000000 pyslth-0.4.8/slth/static/images/user.svg
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.4.8/slth/static/index.html
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.902197 pyslth-0.4.8/slth/static/js/
+-rw-r--r--   0 breno      (501) staff       (20)      946 2024-05-19 17:15:44.000000 pyslth-0.4.8/slth/static/js/default-passive-events.min.js
+-rw-r--r--   0 breno      (501) staff       (20)  1112413 2024-05-18 14:48:49.000000 pyslth-0.4.8/slth/static/js/echarts.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-22 16:45:49.000000 pyslth-0.4.8/slth/static/js/index.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.4.8/slth/static/js/ios-splash.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   117723 2024-05-08 16:11:56.000000 pyslth-0.4.8/slth/static/js/peerjs.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    92865 2024-05-19 22:43:39.000000 pyslth-0.4.8/slth/static/js/peerjs154.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.4.8/slth/static/js/qrcode.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.4.8/slth/static/js/react-trigger-change.js
+-rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-22 16:45:49.000000 pyslth-0.4.8/slth/static/js/react.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   102279 2024-05-22 16:45:49.000000 pyslth-0.4.8/slth/static/js/slth.min.js
+-rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.4.8/slth/static/js/vanilla-masker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.4.8/slth/static/js/vanilla-masker.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6361 2024-05-16 13:05:44.000000 pyslth-0.4.8/slth/statistics.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.905684 pyslth-0.4.8/slth/templates/
+-rw-r--r--   0 breno      (501) staff       (20)     3230 2024-05-19 22:46:51.000000 pyslth-0.4.8/slth/templates/index.html
+-rw-r--r--   0 breno      (501) staff       (20)     1456 2024-05-18 10:06:11.000000 pyslth-0.4.8/slth/templates/service-worker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.4.8/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.4.8/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1000 2024-05-13 01:26:42.000000 pyslth-0.4.8/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     2572 2024-05-08 14:06:07.000000 pyslth-0.4.8/slth/views.py
```

### Comparing `pyslth-0.4.7/PKG-INFO` & `pyslth-0.4.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.4.7
+Version: 0.4.8
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.4.7/pyslth.egg-info/PKG-INFO` & `pyslth-0.4.8/pyslth.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.4.7
+Version: 0.4.8
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.4.7/pyslth.egg-info/SOURCES.txt` & `pyslth-0.4.8/pyslth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/setup.py` & `pyslth-0.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.4.7',
+    version='0.4.8',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.4.7/slth/__init__.py` & `pyslth-0.4.8/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/components.py` & `pyslth-0.4.8/slth/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,26 +211,28 @@
     def __init__(self, number, password, name):
         self["type"] = "zoommeet"
         self["number"] = number
         self["password"] = password
         self["name"] = name
 
 class Navbar(dict):
-    def __init__(self, title, subtitle=None, logo=None, user=None):
+    def __init__(self, title, subtitle=None, logo=None, user=None, search=False, roles=None):
         self["type"] = "navbar"
         self["title"] = title
         self["subtitle"] = subtitle
         self["logo"] = logo
         self["user"] = user
         self["usermenu"] = []
         self["adder"] = []
         self["tools"] = []
         self["settings"] = []
         self["actions"] = []
         self["toolbar"] = []
+        self["search"] = search
+        self["roles"] = roles
 
     def add_action(self, entrypoint, name, url, modal=True, icon=None):
         self[entrypoint].append(dict(name=name, url=url, modal=modal, icon=icon))
 
 
 class Menu(dict):
     def __init__(self, items, user=None, image=None):
```

### Comparing `pyslth-0.4.7/slth/db/models.py` & `pyslth-0.4.8/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/endpoints.py` & `pyslth-0.4.8/slth/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,23 +54,25 @@
             name not in ("Endpoint", "ChildEndpoint")
             and "_ChildEndpoint" not in bases_names
         ):
             ENDPOINTS[cls.__name__.lower()] = cls
         if "AdminEndpoint" in bases_names[0:1]:
             model = cls.__orig_bases__[0].__args__[0]
             items = (
-                ("Cadastrar", AddEndpoint[model], "plus"),
-                ("Editar", EditEndpoint[model], "pen"),
-                ("Visualizar", ViewEndpoint[model], "eye"),
-                ("Excluir", DeleteEndpoint[model], "trash"),
+                ("Cadastrar", AddEndpoint[model], "plus", "add"),
+                ("Editar", EditEndpoint[model], "pen", "edit"),
+                ("Visualizar", ViewEndpoint[model], "eye", "view"),
+                ("Excluir", DeleteEndpoint[model], "trash", "delete"),
             )
-            for prefix, base, icon in items:
+            for prefix, base, icon, action in items:
                 endpoint = types.new_class(f"{prefix}{model.__name__}", (base,), {})
+                endpoint.__admin__ = cls
+                endpoint.__action__ = action
                 endpoint.check_permission = lambda self: (
-                    cls().instantiate(self.request, self).check_permission()
+                    getattr(self.__admin__.instantiate(self.request, self), f'check_{self.__action__}_permission')()
                 )
                 endpoint.Meta = type(
                     "Meta",
                     (),
                     dict(
                         icon=icon,
                         modal=prefix != "Visualizar",
@@ -287,14 +289,26 @@
 
     def get(self) -> QuerySet:
         actions = [
             f"{prefix}{self.model.__name__.lower()}"
             for prefix in ("cadastrar", "visualizar", "editar", "excluir")
         ]
         return self.model.objects.all().actions(*actions)
+    
+    def check_add_permission(self):
+        return self.check_permission()
+    
+    def check_view_permission(self):
+        return self.check_permission()
+    
+    def check_edit_permission(self):
+        return self.check_permission()
+    
+    def check_delete_permission(self):
+        return self.check_permission()
 
 
 class ListEndpoint(Generic[T], ModelEndpoint):
     def get(self) -> QuerySet:
         return self.model.objects.contextualize(self.request)
 
 
@@ -624,14 +638,16 @@
         if self.request.user.is_authenticated:
             user = self.request.user.username.split()[0].split("@")[0]
         navbar = Navbar(
             title=APPLICATON["title"],
             subtitle=APPLICATON["subtitle"],
             logo=logo,
             user=user,
+            search=False,
+            roles=' | '.join((str(role) for role in self.objects('slth.role').filter(username=self.request.user.username)))
         )
         for entrypoint in ["actions", "usermenu", "adder", "settings", "tools", "toolbar"]:
             if APPLICATON["dashboard"][entrypoint]:
                 for endpoint in APPLICATON["dashboard"][entrypoint]:
                     cls = ENDPOINTS[endpoint]
                     if cls().instantiate(self.request, self).check_permission():
                         label = cls.get_metadata("verbose_name")
```

### Comparing `pyslth-0.4.7/slth/factory.py` & `pyslth-0.4.8/slth/factory.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/forms.py` & `pyslth-0.4.8/slth/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 DjangoImageField = ImageField
 
 MASKS = dict(
     cpf_cnpj="999.999.999-99|99.999.999/9999-99",
     cpf="999.999.999-99",
     cnpj="99.999.999/9999-99",
     telefone="(99) 99999-9999",
+    cep='99.999-990'
 )
 
 
 class FormController:
 
     def __init__(self, form):
         super().__init__()
@@ -40,14 +41,17 @@
 
     def hide(self, *names):
         self.controls["hide"].extend(names)
 
     def show(self, *names):
         self.controls["show"].extend(names)
 
+    def visible(self, visible, *names):
+        self.show(*names) if visible else self.hide(*names)
+
     def reload(self, *names):
         self.controls["reload"].extend(names)
 
     def set(self, **kwargs):
         for k, v in kwargs.items():
             if isinstance(v, Model):
                 v = dict(id=v.id, value=str(v))
@@ -89,15 +93,16 @@
         method_name = f"get_{fname}_queryset"
         if hasattr(self.form._endpoint, method_name):
             method_attr = getattr(self.form._endpoint, method_name)
         elif hasattr(self.form, "instance") and hasattr(
             self.form.instance, method_name
         ):
             method_attr = getattr(self.form.instance, method_name)
-        return method_attr(qs, self.values()) if method_attr else qs
+        queryset = method_attr(qs, self.values()) if method_attr else qs
+        return queryset.apply_lookups(self.form.request.user)
 
     def values(self):
         data = dict(**self.controls["set"])
         for name in self.form.fields:
             value = self.get(name, self.form.request.GET.get(name))
             if value:
                 data[name] = value
@@ -270,15 +275,19 @@
             extra = {}
             ftype = FIELD_TYPES.get(type(field).__name__, "text")
             if name in self._values:
                 ftype = "hidden"
                 value = self._values[name]
                 value = value.pk if isinstance(value, Model) else value
             else:
-                value = field.initial or self.initial.get(name)
+                value = None
+                if self.instance is None or self.instance.id is None:
+                    value = field.initial
+                else:
+                    value = self.initial.get(name)
                 if callable(value):
                     value = value()
 
                 if isinstance(field, ModelMultipleChoiceField) or isinstance(
                     field, DjangoModelMultipleChoiceField
                 ):
                     value = (
```

### Comparing `pyslth-0.4.7/slth/management/commands/integration_test.py` & `pyslth-0.4.8/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/management/commands/sync.py` & `pyslth-0.4.8/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/migrations/0001_initial.py` & `pyslth-0.4.8/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.4.8/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/migrations/0003_rename_photo_profile_alter_profile_options.py` & `pyslth-0.4.8/slth/migrations/0003_rename_photo_profile_alter_profile_options.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/migrations/0006_user.py` & `pyslth-0.4.8/slth/migrations/0006_user.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/models.py` & `pyslth-0.4.8/slth/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/notifications.py` & `pyslth-0.4.8/slth/notifications.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/oauth.py` & `pyslth-0.4.8/slth/oauth.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/permissions.py` & `pyslth-0.4.8/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/queryset.py` & `pyslth-0.4.8/slth/queryset.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/roles.py` & `pyslth-0.4.8/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/selenium/__init__.py` & `pyslth-0.4.8/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/selenium/browser.py` & `pyslth-0.4.8/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/serializer.py` & `pyslth-0.4.8/slth/serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,14 +318,15 @@
                     if not only or key in only:
                         data = serialize(component)
                     path = self.path + [key]
                     data['url'] = absolute_url(self.request, 'only={}'.format('__'.join(path)))
                     if leaf: raise JsonResponseException(data)
                 elif datatype == 'serializer':
                     serializer = item['serializer']
+                    serializer.request = serializer.serializer.request
                     serializer.lazy = lazy
                     if not only or key in only:
                         serializer.lazy = False
                         serializer.ignore_only = self.ignore_only or leaf
                         data = serializer.to_dict()
                         if leaf: raise JsonResponseException(data)
                 if data:
```

### Comparing `pyslth-0.4.7/slth/static/.DS_Store` & `pyslth-0.4.8/slth/static/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/static/css/.DS_Store` & `pyslth-0.4.8/slth/static/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/static/css/fontawesome.min.css` & `pyslth-0.4.8/slth/static/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/static/css/fonts/.DS_Store` & `pyslth-0.4.8/slth/static/css/fonts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/static/css/fonts/fa-solid-900.woff2` & `pyslth-0.4.8/slth/static/css/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/static/css/fonts/rawline-400.woff` & `pyslth-0.4.8/slth/static/css/fonts/rawline-400.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/static/css/fonts/rawline-500i.woff` & `pyslth-0.4.8/slth/static/css/fonts/rawline-500i.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/static/css/fonts/rawline-700.woff` & `pyslth-0.4.8/slth/static/css/fonts/rawline-700.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/static/css/slth.css` & `pyslth-0.4.8/slth/static/css/slth.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/static/css/solid.min.css` & `pyslth-0.4.8/slth/static/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/static/images/logo.png` & `pyslth-0.4.8/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/static/images/logo.svg` & `pyslth-0.4.8/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/static/images/user.png` & `pyslth-0.4.8/slth/static/images/user.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/static/js/default-passive-events.min.js` & `pyslth-0.4.8/slth/static/js/default-passive-events.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/static/js/echarts.min.js` & `pyslth-0.4.8/slth/static/js/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/static/js/index.min.js` & `pyslth-0.4.8/slth/static/js/index.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/static/js/ios-splash.min.js` & `pyslth-0.4.8/slth/static/js/ios-splash.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/static/js/peerjs.min.js` & `pyslth-0.4.8/slth/static/js/peerjs.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/static/js/peerjs154.min.js` & `pyslth-0.4.8/slth/static/js/peerjs154.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/static/js/qrcode.min.js` & `pyslth-0.4.8/slth/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/static/js/react-trigger-change.js` & `pyslth-0.4.8/slth/static/js/react-trigger-change.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/static/js/react.min.js` & `pyslth-0.4.8/slth/static/js/react.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/static/js/slth.min.js` & `pyslth-0.4.8/slth/static/js/slth.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -141,21 +141,21 @@
         text: e,
         isError: n
     })), setTimeout(function() {
         a.remove()
     }, 3e3)
 }
 
-function oe() {
+function de() {
     document.querySelectorAll(".message").forEach(function(e) {
         e.remove()
     })
 }
 
-function le(e) {
+function J(e) {
     function n() {
         const a = {
             color: j.colors.info,
             backgroundColor: j.background.info,
             padding: 20,
             display: "flex",
             justifyContent: "space-between",
@@ -268,43 +268,43 @@
             return t.jsx("li", {
                 children: i
             }, Math.random())
         })
     }) : typeof e == "object" && JSON.stringify(Object.keys(e)) == JSON.stringify(["id", "text"]) ? e.text : JSON.stringify(e)
 }
 
-function de() {
+function se() {
     document.querySelector(".layer") == null && H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Oe, {}))
 }
 
 function pe(e, n) {
-    oe(), de(), window.reloader = n;
+    de(), se(), window.reloader = n;
     for (var a = document.getElementsByTagName("dialog"), r = 0; r < a.length; r++) a[r].style.display = "none";
     H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(_e, {
         url: A(e)
     }))
 }
 
 function Ae(e) {
-    oe(), de(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Fe, {
+    de(), se(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Fe, {
         url: A(e)
     }))
 }
 
 function Y(e) {
     e != null && showMessage(e);
     for (var n = document.getElementsByTagName("dialog"), a = 0; a < n.length; a++)
         if (a == n.length - 1) {
             var r = n[a];
             r.close(), r.classList.remove("opened"), r.remove(), a == 0 ? (document.querySelector(".layer").style.display = "none", window.reloader && window.reloader()) : n[a - 1].style.display = "block"
         }
 }
 
 function Re(e) {
-    oe(), de(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(ze, {
+    de(), se(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(ze, {
         actions: e
     }))
 }
 
 function Oe(e) {
     const n = {
         backgroundColor: "black",
@@ -509,15 +509,15 @@
             "data-label": C(e.data.name),
             children: o()
         })
     }
     return d()
 }
 
-function K(e) {
+function ee(e) {
     function n(o) {
         var d = o.target.parentNode.querySelector(".dropdown");
         return d == null && (d = o.target.parentNode.parentNode.querySelector(".dropdown")), d == null && (d = o.target.parentNode.parentNode.parentNode.querySelector(".dropdown")), d
     }
 
     function a(o) {
         const d = n(o);
@@ -697,27 +697,27 @@
                 width: 100
             })
         })
     }
     return o()
 }
 
-function se(e) {
+function ae(e) {
     function n() {
         return t.jsx("div", {
             style: {
                 verticalAlign: "center",
                 textAlign: "right",
                 lineHeight: "3rem"
             },
             children: e.data.map(function(a) {
                 return t.jsx(F, {
                     data: a,
                     default: !0,
-                    compact: !0
+                    compact: !(window.innerWidth > 800)
                 }, Math.random())
             })
         })
     }
     return n()
 }
 
@@ -758,15 +758,15 @@
     function a() {
         return t.jsx(ce, {
             data: e.data.data
         })
     }
 
     function r() {
-        return t.jsx(se, {
+        return t.jsx(ae, {
             data: e.data.actions
         })
     }
 
     function i() {
         const o = {
             border: "solid 1px #DDD",
@@ -783,14 +783,15 @@
 
 function Pe(e) {
     _(`
     .cards{
       padding: 10px;
       box-shadow: 0 1px 6px rgba( 0, 0, 0 , 0.16 );
       margin: 10px;
+      max-width: 300px;
     }
     .cards h3{
       margin-top: 5px;
       margin-bottom: 5px;
       height: 3rem;
       overflow-y: hidden;
     }
@@ -810,15 +811,15 @@
     function a() {
         return t.jsx(ce, {
             data: e.data.data
         })
     }
 
     function r() {
-        return t.jsx(se, {
+        return t.jsx(ae, {
             data: e.data.actions
         })
     }
 
     function i() {
         return t.jsxs("div", {
             className: "cards",
@@ -878,15 +879,15 @@
             }), t.jsx("div", {
                 style: s
             })]
         })
     }
 
     function i() {
-        return t.jsx(se, {
+        return t.jsx(ae, {
             data: e.data.actions
         })
     }
 
     function o() {
         const d = {
                 borderBottom: "solid 1px #DDD",
@@ -1179,63 +1180,69 @@
         return e.data.title != "Top" && t.jsx("h2", {
             "data-label": C(e.data.title),
             children: e.data.title
         })
     }
 
     function o() {
+        return t.jsx(ae, {
+            data: e.data.actions
+        })
+    }
+
+    function d() {
         return t.jsx(Je, {
             data: e.data.data,
-            loadContent: s
+            loadContent: u
         })
     }
 
-    function d() {
-        var l = {
+    function c() {
+        var h = {
             ...a
         };
-        l.title = null;
-        const h = {
+        h.title = null;
+        const f = {
             padding: 0
         };
         return t.jsx("div", {
-            style: h,
+            style: f,
             children: t.jsx(x, {
-                data: l
+                data: h
             }, Math.random())
         })
     }
 
-    function c() {
-        const l = {
+    function s() {
+        const h = {
             width: "50%",
             margin: "auto",
             border: "solid 0.5px #DDD",
             marginTop: 30,
             marginBottom: 30
         };
         return t.jsx("div", {
-            style: l
+            style: h
         })
     }
 
-    function s(l) {
-        q("GET", l, function(h) {
-            r(h)
+    function u(h) {
+        q("GET", h, function(f) {
+            r(f)
         })
     }
 
-    function u() {
-        return window[n] = () => s(a.url), e.data.data.length > 0 && t.jsxs("div", {
+    function l() {
+        return window[n] = () => u(a.url), e.data.data.length > 0 && t.jsxs("div", {
             className: "reloadable",
             id: n,
-            children: [i(), o(), d(), c()]
+            children: [i(), o(), d(), c(), s()]
         })
     }
-    return u()
+    return l()
 }
 
 function Ze() {
     document.querySelectorAll(".reloadable").forEach(function(e) {
         window[e.id]()
     })
 }
@@ -1784,26 +1791,26 @@
                                     children: I.text
                                 }, Math.random());
                                 {
                                     const M = {
                                         backgroundColor: s(I),
                                         border: "solid 4px white"
                                     };
-                                    return t.jsx("td", {
+                                    return console.log(I), t.jsx("td", {
                                         align: "center",
                                         style: M,
                                         onMouseDown: h,
                                         onMouseLeave: h,
                                         onMouseUp: h,
                                         "data-day": e.data.matrix[0][w].text,
                                         "data-time": B[0].text,
                                         children: I && I.text && t.jsx(mt, {
                                             text: I.text,
                                             children: t.jsx(S, {
-                                                icon: "stethoscope",
+                                                icon: I.icon || "stethoscope",
                                                 style: {
                                                     color: "white",
                                                     cursor: "help"
                                                 }
                                             })
                                         })
                                     }, Math.random())
@@ -1866,30 +1873,30 @@
     for (let [a, r] of Array.from(n.entries())) {
         const i = e[a];
         i.tagName == "SELECT" && r !== "" || i.tagName == null && r !== "" || i.type == "radio" && r !== "" || i.type == "checkbox" && r !== "" || n.delete(a)
     }
     return new URLSearchParams(n).toString()
 }
 
-function J(e, n) {
+function Q(e, n) {
     const a = e.indexOf("?") < 0 ? "?" : "&",
         r = gt(n);
     return e = e + (r ? a + r : ""), e
 }
 
-function re(e) {
+function oe(e) {
     if (e) {
         const a = [".png", ".jpeg", ".jpeg", ".gif"];
         for (var n = 0; n < a.length; n++)
             if (e.toLowerCase().indexOf(a[n]) > 0) return !0
     }
 }
 
 function V(e, n) {
-    q("GET", J(n, e.closest("form")), Me)
+    q("GET", Q(n, e.closest("form")), Me)
 }
 
 function xt(e) {
     if (e) {
         var n = document.querySelector(".form-fieldset." + e);
         n && (n.style.display = "none");
         var a = document.querySelector(".form-group." + e);
@@ -2005,51 +2012,52 @@
                 children: e.text
             })
         })
     }
     return n()
 }
 
-function ee(e) {
+function te(e) {
     const n = e.data.name + Math.random();
 
     function a() {
         const c = {
             display: "flex",
             justifyContent: "space-between",
             alignItems: "baseline"
         };
         return e.data.action && (e.data.action.icon = null, e.data.action.modal = !0, e.data.action.urlfunc = function() {
-            return J(e.data.action.url, document.getElementById(n).closest("form"))
+            return Q(e.data.action.url, document.getElementById(n).closest("form"))
         }), t.jsxs("div", {
             style: c,
             children: [t.jsxs("label", {
                 className: "bold",
                 children: [e.data.label, " ", e.data.required ? "*" : ""]
             }), e.data.action && t.jsx(F, {
                 data: e.data.action,
                 style: {
-                    padding: 0
+                    padding: 0,
+                    margin: 0
                 }
             })]
         })
     }
 
     function r() {
         return e.data.type == "datetime" && (e.data.type = "datetime-local"), ft.indexOf(e.data.type) >= 0 ? t.jsx(ye, {
             data: e.data
         }) : e.data.type == "choice" && Array.isArray(e.data.choices) ? e.data.pick ? Array.isArray(e.data.value) ? t.jsx(ve, {
             data: e.data
-        }) : t.jsx(ie, {
+        }) : t.jsx(le, {
             data: e.data
         }) : t.jsx(Ct, {
             data: e.data
         }) : e.data.type == "choice" ? e.data.pick ? Array.isArray(e.data.value) ? t.jsx(ve, {
             data: e.data
-        }) : t.jsx(ie, {
+        }) : t.jsx(le, {
             data: e.data
         }) : t.jsx(Ee, {
             data: e.data
         }) : e.data.type == "decimal" ? t.jsx(ye, {
             data: e.data
         }) : e.data.type == "boolean" ? t.jsx(St, {
             data: e.data
@@ -2121,15 +2129,15 @@
     }
 
     function i(d) {
         if (e.data.type == "file" && d.target.files) {
             let s = d.target.files[0];
             var c = new FileReader;
             c.onload = function(u) {
-                if (re(s.name)) {
+                if (oe(s.name)) {
                     const v = "display" + a;
                     var l = document.createElement("img");
                     l.id = d.target.id + "img", l.style.width = "200px", l.style.display = "block", l.style.margin = "auto", l.style.marginTop = "20px", l.onload = function(m) {
                         const b = e.data.width > e.data.height ? e.data.width / l.width : e.data.height / l.height;
                         var y = document.createElement("canvas");
                         const B = y.getContext("2d");
                         y.height = y.width * (l.height / l.width);
@@ -2178,23 +2186,23 @@
                             style: {
                                 fontSize: "2.5rem",
                                 color: j.colors.primary
                             }
                         })
                     }), t.jsxs("div", {
                         style: u,
-                        children: [e.data.value && re(e.data.value) && t.jsx("div", {
+                        children: [e.data.value && oe(e.data.value) && t.jsx("div", {
                             style: {
                                 textAlign: "center"
                             },
                             children: t.jsx("img", {
                                 src: e.data.value,
                                 height: 50
                             })
-                        }), e.data.value && !re(e.data.value) && t.jsx("div", {
+                        }), e.data.value && !oe(e.data.value) && t.jsx("div", {
                             style: {
                                 textAlign: "center"
                             },
                             children: e.data.value
                         }), "Selecione um arquivo clicando no botão ao lado.", t.jsxs("div", {
                             className: "bold",
                             id: "fileinfo" + a,
@@ -2336,26 +2344,26 @@
                 overflowY: "auto",
                 zIndex: 99999
             };
         M.position = "absolute", M.backgroundColor = "white";
         const T = document.getElementById(r);
         if (e.data.icon && (w.paddingLeft = 30), T) {
             let N = null,
-                Q = T,
-                ae = null;
-            for (; !ae && (Q = Q.parentElement) instanceof HTMLElement;) Q.matches("dialog") && (ae = Q);
-            N = ae;
-            const Z = T.getBoundingClientRect();
-            var g = Z.top + Z.height,
-                p = Z.left;
+                Z = T,
+                ie = null;
+            for (; !ie && (Z = Z.parentElement) instanceof HTMLElement;) Z.matches("dialog") && (ie = Z);
+            N = ie;
+            const K = T.getBoundingClientRect();
+            var g = K.top + K.height,
+                p = K.left;
             if (N) {
                 const fe = N.getBoundingClientRect();
                 g = g - fe.top, p = p - fe.left
             } else g += window.scrollY, p += window.scrollX;
-            M.width = Z.width, M.top = g, M.left = p
+            M.width = K.width, M.top = g, M.left = p
         }
         const E = {
                 cursor: "pointer",
                 padding: 10
             },
             L = !i && n.length > 0 && n[0].value || "";
         return t.jsxs(t.Fragment, {
@@ -2416,15 +2424,15 @@
         }
     }
 
     function y(w) {
         clearTimeout(l), l = setTimeout(function() {
             const M = w.target.closest("form"),
                 T = e.data.choices.indexOf("?") < 0 ? "?" : "&";
-            d(!0), q("GET", J(e.data.choices + T + "term=" + w.target.value, M), function(p) {
+            d(!0), q("GET", Q(e.data.choices + T + "term=" + w.target.value, M), function(p) {
                 s(p)
             })
         }, 1e3)
     }
 
     function B(w, M = !1) {
         const T = document.getElementById(a),
@@ -2467,20 +2475,20 @@
     var n = e.data;
     return n.choices = [{
         id: !0,
         value: "Sim"
     }, {
         id: !1,
         value: "Não"
-    }], t.jsx(ie, {
+    }], t.jsx(le, {
         data: n
     })
 }
 
-function ie(e) {
+function le(e) {
     const [n, a] = D.useState(e.data.choices);
     var r = Math.random(),
         i = e.data;
 
     function o(u) {
         return i.value != null ? i.value == u.id ? !0 : i.value.id == u.id : !1
     }
@@ -2493,15 +2501,15 @@
     function c(u) {
         var l = document.getElementById(u);
         i.checked = l.checked
     }
 
     function s() {
         return window["reload-" + i.name + "-field"] = function() {
-            q("GET", J(e.data.pick, document.querySelector(".radio-group." + i.name).closest("form")), function(l) {
+            q("GET", Q(e.data.pick, document.querySelector(".radio-group." + i.name).closest("form")), function(l) {
                 a(l)
             })
         }, n.length > 0 ? t.jsx("div", {
             className: "radio-group " + i.name,
             children: n.map((u, l) => (u.id || u.id === !1) && t.jsxs("div", {
                 style: {
                     paddingTop: 10,
@@ -2524,17 +2532,19 @@
                     }
                 }), t.jsx("label", {
                     htmlFor: i.name + r + l,
                     children: u.value
                 })]
             }, r + l))
         }) : t.jsx("div", {
-            className: "radio-group " + i.name,
-            children: t.jsx("i", {
-                children: "Nenhuma opção disponível para seleção."
+            className: "radio-group empty " + i.name,
+            children: t.jsx(J, {
+                data: {
+                    text: "Nenhuma opção disponível para seleção."
+                }
             })
         })
     }
     return s()
 }
 
 function ve(e) {
@@ -2554,15 +2564,15 @@
 
     function d(s) {
         e.data.onchange && V(s.target, e.data.onchange)
     }
 
     function c() {
         return window["reload-" + i.name + "-field"] = function() {
-            q("GET", J(e.data.pick, document.querySelector(".checkbox-group." + i.name).closest("form")), function(u) {
+            q("GET", Q(e.data.pick, document.querySelector(".checkbox-group." + i.name).closest("form")), function(u) {
                 a(u)
             })
         }, n.length > 0 ? t.jsx("div", {
             className: "checkbox-group " + i.name,
             children: n.map((s, u) => (s.id || s.id === !1) && t.jsxs("div", {
                 style: {
                     paddingTop: 10,
@@ -2580,17 +2590,19 @@
                     "data-label": C(s.value)
                 }), t.jsx("label", {
                     htmlFor: i.name + r + u,
                     children: s.value
                 })]
             }, r + u))
         }) : t.jsx("div", {
-            className: "checkbox-group " + i.name,
-            children: t.jsx("i", {
-                children: "Nenhuma opção disponível para seleção."
+            className: "checkbox-group empty " + i.name,
+            children: t.jsx(J, {
+                data: {
+                    text: "Nenhuma opção disponível para seleção."
+                }
             })
         })
     }
     return c()
 }
 
 function Ct(e) {
@@ -2615,15 +2627,15 @@
     const n = Math.random(),
         a = e.data.value[0],
         r = a.fields ? a.fields[0] : a.fieldsets[0].fields[0][0];
 
     function i() {
         return !e.data.required && t.jsx("div", {
             id: "info-" + n,
-            children: t.jsxs(le, {
+            children: t.jsxs(J, {
                 data: {
                     text: "Esta informação é opcional. Controle seu preenchimento com o botão ao lado."
                 },
                 children: [t.jsx(R, {
                     primary: !0,
                     icon: "pen-clip",
                     onClick: () => o(!0),
@@ -2755,15 +2767,15 @@
         for (var l = [], h = 0; h < n; h++) document.getElementById("form-" + h + "-" + a).style.display == "block" && l.push(h);
         return l
     }
 
     function s() {
         return t.jsx("div", {
             id: "info-" + a,
-            children: t.jsx(le, {
+            children: t.jsx(J, {
                 data: {
                     text: 'Clique no botão com o ícone de "+" para adicionar e com o ícone da "lixeira" para remover.'
                 },
                 children: t.jsx(R, {
                     primary: !0,
                     icon: "add",
                     onClick: () => o(),
@@ -2804,15 +2816,15 @@
     }, []);
 
     function n(r) {
         return r.type == "inline" ? r.max == r.min == 1 ? t.jsx(Mt, {
             data: r
         }, Math.random()) : t.jsx(Et, {
             data: r
-        }, Math.random()) : t.jsx(ee, {
+        }, Math.random()) : t.jsx(te, {
             data: r
         }, Math.random())
     }
 
     function a() {
         return e.data.fields ? t.jsx("div", {
             className: "form-fields",
@@ -3092,22 +3104,19 @@
                                 }) : h.date + h.today
                             }), h.total && t.jsx("div", {
                                 className: "total",
                                 onClick: () => e.onChange(h.date, e.data.month, e.data.year),
                                 children: t.jsx("div", {
                                     className: "number",
                                     style: {
-                                        backgroundColor: j.colors.primary
+                                        backgroundColor: j.colors.primary,
+                                        textDecoration: h.selected ? "underline" : "normal",
+                                        display: "inline-block"
                                     },
-                                    children: t.jsx("span", {
-                                        style: {
-                                            textDecoration: h.selected ? "underline" : "normal"
-                                        },
-                                        children: h.total
-                                    })
+                                    children: h.total
                                 })
                             }), !h.total && t.jsx("div", {
                                 className: "total",
                                 children: " "
                             })]
                         }, Math.random()))
                     }, Math.random()))
@@ -3396,30 +3405,28 @@
     }
 
     function f() {
         return n.data.length > 0 ? (n.render == null && window.innerWidth < 800 && (n.renderer = "rows"), n.renderer ? n.renderer == "cards" ? t.jsx(P, {
             width: 300,
             alignItems: "start",
             children: n.data.map(function(g) {
-                return g.type = n.renderer, t.jsx("div", {
-                    children: t.jsx(x, {
-                        data: g
-                    })
+                return g.type = n.renderer, t.jsx(x, {
+                    data: g
                 }, Math.random())
             })
         }) : t.jsx("div", {
             style: {
                 marginBottom: 15
             },
             children: n.data.map(function(g) {
                 return g.type = n.renderer, t.jsx(x, {
                     data: g
                 }, Math.random())
             })
-        }) : v()) : t.jsx(le, {
+        }) : v()) : t.jsx(J, {
             data: {
                 text: "Nenhum registro encontrado."
             }
         })
     }
 
     function v() {
@@ -3507,33 +3514,33 @@
                 value: n.q
             };
             return t.jsxs("div", {
                 style: g,
                 children: [t.jsxs(P, {
                     width: 250,
                     children: [p && t.jsx("div", {
-                        children: t.jsx(ee, {
+                        children: t.jsx(te, {
                             data: L
                         })
                     }), E && n.filters.map(function(N) {
                         return N.type != "hidden" && t.jsx("div", {
-                            children: t.jsx(ee, {
+                            children: t.jsx(te, {
                                 data: N
                             })
                         }, Math.random())
                     }), t.jsx("div", {
                         children: t.jsx(R, {
                             onClick: I,
                             label: "Filtrar",
                             icon: "filter"
                         })
                     })]
                 }), E && n.filters.map(function(N) {
                     return N.type == "hidden" && t.jsx("div", {
-                        children: t.jsx(ee, {
+                        children: t.jsx(te, {
                             data: N
                         })
                     }, Math.random())
                 })]
             })
         }
     }
@@ -3609,15 +3616,15 @@
                 }), i(), M()]
             })
         })
     }
     return T()
 }
 
-function ne(e) {
+function re(e) {
     var n = Math.random();
 
     function a() {
         var r = document.getElementById(n);
         if (r) {
             var i = echarts.init(r);
             i.setOption(e.option)
@@ -3702,15 +3709,15 @@
                 show: !0,
                 formatter(o) {
                     return o.name + " (" + o.percent.toLocaleString("pt-BR") + "%)"
                 }
             },
             series: a()
         };
-        return t.jsx(ne, {
+        return t.jsx(re, {
             option: i
         })
     }
     return r()
 }
 
 function Bt(e) {
@@ -3800,15 +3807,15 @@
                     return h.value.toLocaleString("pt-BR")
                 }
             },
             xAxis: n ? i : c(),
             yAxis: n ? c() : i,
             series: s()
         };
-        return t.jsx(ne, {
+        return t.jsx(re, {
             option: l
         })
     }
     return u()
 }
 
 function At(e) {
@@ -3901,15 +3908,15 @@
                 show: !0,
                 formatter(i) {
                     return i.name + " (" + i.value.toLocaleString("pt-BR") + ")"
                 }
             },
             series: n()
         };
-        return t.jsx(ne, {
+        return t.jsx(re, {
             option: r
         })
     }
     return a()
 }
 
 function Ht(e) {
@@ -3950,15 +3957,15 @@
                     }
                 },
                 data: [{
                     value: e.value
                 }]
             }]
         };
-        return t.jsx(ne, {
+        return t.jsx(re, {
             option: a
         })
     }
     return n()
 }
 
 function be(e) {
@@ -4214,15 +4221,17 @@
             style: c,
             onClick: n,
             className: "item",
             children: t.jsxs(O, {
                 href: o.url,
                 dataLabel: C(o.label),
                 style: {
-                    textDecoration: "none"
+                    textDecoration: "none",
+                    display: "block",
+                    width: "100%"
                 },
                 children: [d == 0 && t.jsx(S, {
                     icon: o.icon || "dot-circle",
                     style: s
                 }), o.label]
             })
         }, Math.random()) : o.items.length > 0 && t.jsxs("li", {
@@ -4499,15 +4508,15 @@
                     display: "flex",
                     alignItems: "center"
                 },
                 children: [e.data.navbar.adder.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
-                    children: t.jsx(K, {
+                    children: t.jsx(ee, {
                         actions: e.data.navbar.adder,
                         position: {},
                         dataLabel: "plus",
                         children: t.jsx(S, {
                             icon: "plus"
                         })
                     })
@@ -4540,47 +4549,47 @@
                         },
                         children: f.label
                     }, Math.random())
                 }), e.data.navbar.tools.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
-                    children: t.jsx(K, {
+                    children: t.jsx(ee, {
                         actions: e.data.navbar.tools,
                         position: {},
                         dataLabel: "tools",
                         children: t.jsx(S, {
                             icon: "tools"
                         })
                     })
                 }), e.data.navbar.settings.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
-                    children: t.jsx(K, {
+                    children: t.jsx(ee, {
                         actions: e.data.navbar.settings,
                         position: {},
                         dataLabel: "gear",
                         children: t.jsx(S, {
                             icon: "gear"
                         })
                     })
-                }), window.innerWidth > 800 && e.data.navbar.user && t.jsx("div", {
+                }), window.innerWidth > 800 && e.data.navbar.user && e.data.navbar.search && t.jsx("div", {
                     children: t.jsx(Ee, {
                         data: h,
                         style: {
                             padding: 10
                         },
                         onSelect: f => document.location.href = U(f.id)
                     })
                 }), e.data.navbar.user && e.data.navbar.usermenu.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
-                    children: t.jsx(K, {
+                    children: t.jsx(ee, {
                         actions: e.data.navbar.usermenu,
                         position: {},
                         dataLabel: C(e.data.navbar.user),
                         children: t.jsx("img", {
                             src: "/static/images/user.svg",
                             style: {
                                 width: 30,
@@ -4627,14 +4636,15 @@
                     },
                     children: t.jsx(S, {
                         icon: "home",
                         style: h
                     })
                 }), "Área Administrativa"]
             }), t.jsx("div", {
+                title: e.data.navbar.roles,
                 children: e.data.navbar.user
             })]
         })
     }
 
     function c() {
         return t.jsxs("main", {
@@ -4790,15 +4800,15 @@
 
 function Qt(e) {
     _(`
     .container {
         position: relative;
         width: 100%;
         overflow: hidden;
-        padding-top: 100%;
+        padding-top: ${window.innerWidth>800?50:100}%;
       }
       .responsive-iframe {
         position: absolute;
         top: 0;
         left: 0;
         bottom: 0;
         right: 0;
@@ -4835,15 +4845,15 @@
         return t.jsx("div", {
             style: n,
             children: e.data.text
         })
     }
     return a()
 }
-var te, me = {};
+var ne, me = {};
 const Kt = "/api/application/",
     we = localStorage.getItem("application");
 
 function x(e) {
     const n = me[e.data.type];
     return n ? Te.createElement(n, {
         data: e.data
@@ -4851,15 +4861,15 @@
         children: JSON.stringify(e.data)
     })
 }
 x.register = function(e, n) {
     me[n.toLowerCase()] = e
 };
 x.render = function(e) {
-    te = e, document.location.pathname == "/" ? localStorage.getItem("token") ? window.reload("/app/dashboard/") : window.reload("/app/home/") : document.location.pathname == "/app/login/" && (localStorage.getItem("token") || localStorage.getItem("application")) ? (localStorage.removeItem("token"), localStorage.removeItem("application"), document.location.reload()) : window.reload(document.location.href)
+    ne = e, document.location.pathname == "/" ? localStorage.getItem("token") ? window.reload("/app/dashboard/") : window.reload("/app/home/") : document.location.pathname == "/app/login/" && (localStorage.getItem("token") || localStorage.getItem("application")) ? (localStorage.removeItem("token"), localStorage.removeItem("application"), document.location.reload()) : window.reload(document.location.href)
 };
 x.register(ht, "Counter");
 x.register(Tt, "Form");
 x.register(qt, "QuerySet");
 x.register(Ge, "Fieldset");
 x.register(X, "Field");
 x.register($e, "Object");
@@ -4893,35 +4903,38 @@
 x.register(Qt, "ZoomMeet");
 window.addEventListener("popstate", e => {
     window.reload(e.currentTarget.location.href)
 });
 window.reload = function(e) {
     const n = e.split("/app/")[1].split("/")[0];
     me[n] ? q("GET", A(e), function(a) {
-        te.render(t.jsx(x, {
+        ne.render(t.jsx(x, {
             data: {
                 type: n,
                 data: a
             }
         }))
     }) : (e != document.location.href && window.history.pushState({
         url: e
     }, "", e), we ? (window.application = JSON.parse(we), q("GET", A(e), function(a) {
-        window.application.content = a, te.render(t.jsx(x, {
+        window.application.content = a, ne.render(t.jsx(x, {
             data: window.application
         }, Math.random()))
     })) : q("GET", Kt, function(r) {
         window.application = r, localStorage.setItem("application", JSON.stringify(window.application)), q("GET", A(e), function(i) {
-            window.application.content = i, te.render(t.jsx(x, {
+            window.application.content = i, ne.render(t.jsx(x, {
                 data: window.application
             }, Math.random()))
         })
     }))
 };
 window.load = function(e) {
     e.indexOf(window.origin) >= 0 || e.startsWith("/") ? (e != document.location.href && e != document.location.pathname && window.history.pushState({
         url: e
     }, "", e), q("GET", A(e), function(n) {
-        window.loaddata(n)
+        window.loaddata(n), window.scrollTo({
+            top: 0,
+            behavior: "smooth"
+        })
     })) : document.location.href = e
 };
 x.render(H.createRoot(document.getElementById("root")));
```

### Comparing `pyslth-0.4.7/slth/static/js/vanilla-masker.js` & `pyslth-0.4.8/slth/static/js/vanilla-masker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/static/js/vanilla-masker.min.js` & `pyslth-0.4.8/slth/static/js/vanilla-masker.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/statistics.py` & `pyslth-0.4.8/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/templates/index.html` & `pyslth-0.4.8/slth/templates/index.html`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/templates/service-worker.js` & `pyslth-0.4.8/slth/templates/service-worker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/tests.py` & `pyslth-0.4.8/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/urls.py` & `pyslth-0.4.8/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/utils.py` & `pyslth-0.4.8/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.7/slth/views.py` & `pyslth-0.4.8/slth/views.py`

 * *Files identical despite different names*

