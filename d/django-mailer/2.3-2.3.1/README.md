# Comparing `tmp/django-mailer-2.3.tar.gz` & `tmp/django-mailer-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mailer-2.3.tar", last modified: Mon Sep 25 14:36:25 2023, max compression
+gzip compressed data, was "django-mailer-2.3.1.tar", last modified: Fri Dec 29 15:00:14 2023, max compression
```

## Comparing `django-mailer-2.3.tar` & `django-mailer-2.3.1.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-09-25 14:36:25.021690 django-mailer-2.3/
--rw-r--r--   0 luke      (1000) luke      (1000)       56 2014-12-31 11:58:06.000000 django-mailer-2.3/.coveragerc
--rw-r--r--   0 luke      (1000) luke      (1000)      551 2023-09-22 15:49:33.000000 django-mailer-2.3/.pre-commit-config.yaml
--rw-r--r--   0 luke      (1000) luke      (1000)      289 2023-09-22 14:47:19.000000 django-mailer-2.3/AUTHORS
--rw-r--r--   0 luke      (1000) luke      (1000)     5283 2023-09-25 14:36:05.000000 django-mailer-2.3/CHANGES.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     2750 2023-09-22 15:49:33.000000 django-mailer-2.3/CONTRIBUTING.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     1078 2014-12-31 11:28:54.000000 django-mailer-2.3/LICENSE
--rw-r--r--   0 luke      (1000) luke      (1000)      245 2023-09-22 15:49:33.000000 django-mailer-2.3/MANIFEST.in
--rw-rw-rw-   0 luke      (1000) luke      (1000)     1334 2023-09-25 14:36:25.025690 django-mailer-2.3/PKG-INFO
--rw-r--r--   0 luke      (1000) luke      (1000)     4553 2023-09-25 14:35:45.000000 django-mailer-2.3/README.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      655 2023-06-28 18:40:42.000000 django-mailer-2.3/RELEASE.rst
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-09-25 14:36:25.021690 django-mailer-2.3/docs/
--rw-r--r--   0 luke      (1000) luke      (1000)       79 2010-05-24 15:43:21.000000 django-mailer-2.3/docs/index.rst
--rw-r--r--   0 luke      (1000) luke      (1000)    10591 2023-09-25 14:35:45.000000 django-mailer-2.3/docs/usage.rst
--rwxr-xr--   0 luke      (1000) luke      (1000)     1851 2023-09-25 14:35:45.000000 django-mailer-2.3/manage.py
--rw-r--r--   0 luke      (1000) luke      (1000)      302 2023-09-22 15:00:59.000000 django-mailer-2.3/pyproject.toml
--rw-r--r--   0 luke      (1000) luke      (1000)      114 2023-09-22 15:49:33.000000 django-mailer-2.3/pytest.ini
--rwxr-xr--   0 luke      (1000) luke      (1000)      348 2023-09-22 15:00:42.000000 django-mailer-2.3/release.sh
--rw-r--r--   0 luke      (1000) luke      (1000)       26 2023-09-22 15:18:02.000000 django-mailer-2.3/requirements-dev.txt
--rw-r--r--   0 luke      (1000) luke      (1000)       32 2023-09-22 15:49:33.000000 django-mailer-2.3/requirements-test.txt
--rw-r--r--   0 luke      (1000) luke      (1000)     1422 2023-09-25 14:36:25.025690 django-mailer-2.3/setup.cfg
--rwxr-xr--   0 luke      (1000) luke      (1000)       38 2023-09-22 15:00:42.000000 django-mailer-2.3/setup.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-09-25 14:36:25.017690 django-mailer-2.3/src/
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-09-25 14:36:25.021690 django-mailer-2.3/src/django_mailer.egg-info/
--rw-r--r--   0 luke      (1000) luke      (1000)     1334 2023-09-25 14:36:25.000000 django-mailer-2.3/src/django_mailer.egg-info/PKG-INFO
--rw-r-----   0 luke      (1000) luke      (1000)     1419 2023-09-25 14:36:25.000000 django-mailer-2.3/src/django_mailer.egg-info/SOURCES.txt
--rw-r-----   0 luke      (1000) luke      (1000)        1 2023-09-25 14:36:25.000000 django-mailer-2.3/src/django_mailer.egg-info/dependency_links.txt
--rw-r-----   0 luke      (1000) luke      (1000)       26 2023-09-25 14:36:25.000000 django-mailer-2.3/src/django_mailer.egg-info/requires.txt
--rw-r-----   0 luke      (1000) luke      (1000)        7 2023-09-25 14:36:25.000000 django-mailer-2.3/src/django_mailer.egg-info/top_level.txt
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-09-25 14:36:25.021690 django-mailer-2.3/src/mailer/
--rw-r--r--   0 luke      (1000) luke      (1000)     3107 2023-09-25 14:36:05.000000 django-mailer-2.3/src/mailer/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1485 2023-09-22 15:01:19.000000 django-mailer-2.3/src/mailer/admin.py
--rw-r--r--   0 luke      (1000) luke      (1000)      144 2023-09-22 15:01:18.000000 django-mailer-2.3/src/mailer/apps.py
--rw-r--r--   0 luke      (1000) luke      (1000)      485 2023-09-22 15:01:18.000000 django-mailer-2.3/src/mailer/backend.py
--rw-r--r--   0 luke      (1000) luke      (1000)     9734 2023-09-25 14:35:45.000000 django-mailer-2.3/src/mailer/engine.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-09-25 14:36:25.017690 django-mailer-2.3/src/mailer/locale/
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-09-25 14:36:25.017690 django-mailer-2.3/src/mailer/locale/ja/
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-09-25 14:36:25.021690 django-mailer-2.3/src/mailer/locale/ja/LC_MESSAGES/
--rw-r--r--   0 luke      (1000) luke      (1000)     1164 2019-09-23 17:24:14.000000 django-mailer-2.3/src/mailer/locale/ja/LC_MESSAGES/django.po
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-09-25 14:36:25.017690 django-mailer-2.3/src/mailer/locale/ru/
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-09-25 14:36:25.021690 django-mailer-2.3/src/mailer/locale/ru/LC_MESSAGES/
--rw-r--r--   0 luke      (1000) luke      (1000)     1171 2019-09-23 17:24:14.000000 django-mailer-2.3/src/mailer/locale/ru/LC_MESSAGES/django.po
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-09-25 14:36:25.021690 django-mailer-2.3/src/mailer/management/
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2019-09-23 17:24:14.000000 django-mailer-2.3/src/mailer/management/__init__.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-09-25 14:36:25.021690 django-mailer-2.3/src/mailer/management/commands/
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2019-09-23 17:24:14.000000 django-mailer-2.3/src/mailer/management/commands/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)      913 2023-09-22 15:08:37.000000 django-mailer-2.3/src/mailer/management/commands/purge_mail_log.py
--rw-r--r--   0 luke      (1000) luke      (1000)      705 2023-09-22 15:08:37.000000 django-mailer-2.3/src/mailer/management/commands/retry_deferred.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1073 2023-09-25 14:35:45.000000 django-mailer-2.3/src/mailer/management/commands/runmailer.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1208 2023-09-25 14:35:45.000000 django-mailer-2.3/src/mailer/management/commands/runmailer_pg.py
--rw-r--r--   0 luke      (1000) luke      (1000)      956 2023-09-22 15:01:19.000000 django-mailer-2.3/src/mailer/management/commands/send_mail.py
--rw-r--r--   0 luke      (1000) luke      (1000)      710 2023-09-22 15:01:19.000000 django-mailer-2.3/src/mailer/management/helpers.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-09-25 14:36:25.021690 django-mailer-2.3/src/mailer/migrations/
--rw-r--r--   0 luke      (1000) luke      (1000)     2586 2023-09-22 15:01:19.000000 django-mailer-2.3/src/mailer/migrations/0001_initial.py
--rw-r--r--   0 luke      (1000) luke      (1000)      625 2023-09-22 15:01:19.000000 django-mailer-2.3/src/mailer/migrations/0002_auto_20150720_1433.py
--rw-r--r--   0 luke      (1000) luke      (1000)      403 2023-09-22 15:01:19.000000 django-mailer-2.3/src/mailer/migrations/0003_messagelog_message_id.py
--rw-r--r--   0 luke      (1000) luke      (1000)      999 2023-09-22 15:01:19.000000 django-mailer-2.3/src/mailer/migrations/0004_auto_20190920_1512.py
--rw-r--r--   0 luke      (1000) luke      (1000)      874 2023-09-22 15:01:19.000000 django-mailer-2.3/src/mailer/migrations/0005_id_bigautofield.py
--rw-r--r--   0 luke      (1000) luke      (1000)      385 2023-09-22 15:01:19.000000 django-mailer-2.3/src/mailer/migrations/0006_message_retry_count.py
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2019-09-23 17:24:14.000000 django-mailer-2.3/src/mailer/migrations/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     9241 2023-09-22 15:08:37.000000 django-mailer-2.3/src/mailer/models.py
--rw-r--r--   0 luke      (1000) luke      (1000)     4741 2023-09-25 14:35:45.000000 django-mailer-2.3/src/mailer/postgres.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-09-25 14:36:25.021690 django-mailer-2.3/tests/
--rw-r--r--   0 luke      (1000) luke      (1000)      778 2023-09-22 15:01:19.000000 django-mailer-2.3/tests/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)      303 2023-09-22 15:49:33.000000 django-mailer-2.3/tests/settings.py
--rw-r--r--   0 luke      (1000) luke      (1000)    33141 2023-09-22 15:01:20.000000 django-mailer-2.3/tests/test_mailer.py
--rw-r--r--   0 luke      (1000) luke      (1000)      773 2023-09-22 15:49:33.000000 django-mailer-2.3/tox.ini
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-12-29 15:00:14.976361 django-mailer-2.3.1/
+-rw-r--r--   0 luke      (1000) luke      (1000)       56 2014-12-31 11:58:06.000000 django-mailer-2.3.1/.coveragerc
+-rw-r--r--   0 luke      (1000) luke      (1000)      551 2023-09-22 15:49:33.000000 django-mailer-2.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 luke      (1000) luke      (1000)      289 2023-09-22 14:47:19.000000 django-mailer-2.3.1/AUTHORS
+-rw-r--r--   0 luke      (1000) luke      (1000)     5394 2023-12-29 14:58:34.000000 django-mailer-2.3.1/CHANGES.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     2750 2023-09-22 15:49:33.000000 django-mailer-2.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     1078 2014-12-31 11:28:54.000000 django-mailer-2.3.1/LICENSE
+-rw-r--r--   0 luke      (1000) luke      (1000)      245 2023-09-22 15:49:33.000000 django-mailer-2.3.1/MANIFEST.in
+-rw-rw-rw-   0 luke      (1000) luke      (1000)     1336 2023-12-29 15:00:14.976361 django-mailer-2.3.1/PKG-INFO
+-rw-r--r--   0 luke      (1000) luke      (1000)     5088 2023-09-26 13:20:44.000000 django-mailer-2.3.1/README.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      670 2023-12-29 14:59:46.000000 django-mailer-2.3.1/RELEASE.rst
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-12-29 15:00:14.960361 django-mailer-2.3.1/docs/
+-rw-r--r--   0 luke      (1000) luke      (1000)       79 2010-05-24 15:43:21.000000 django-mailer-2.3.1/docs/index.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)    10591 2023-12-28 20:02:13.000000 django-mailer-2.3.1/docs/usage.rst
+-rw-r-----   0 luke      (1000) luke      (1000)    29440 2023-12-28 20:02:15.000000 django-mailer-2.3.1/docs/usage.rst.html
+-rwxr-xr--   0 luke      (1000) luke      (1000)     1851 2023-09-25 14:35:45.000000 django-mailer-2.3.1/manage.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      302 2023-09-22 15:00:59.000000 django-mailer-2.3.1/pyproject.toml
+-rw-r--r--   0 luke      (1000) luke      (1000)      114 2023-09-22 15:49:33.000000 django-mailer-2.3.1/pytest.ini
+-rwxr-xr--   0 luke      (1000) luke      (1000)      348 2023-09-22 15:00:42.000000 django-mailer-2.3.1/release.sh
+-rw-r--r--   0 luke      (1000) luke      (1000)       26 2023-09-22 15:18:02.000000 django-mailer-2.3.1/requirements-dev.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)       32 2023-09-22 15:49:33.000000 django-mailer-2.3.1/requirements-test.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)     1422 2023-12-29 15:00:14.976361 django-mailer-2.3.1/setup.cfg
+-rwxr-xr--   0 luke      (1000) luke      (1000)       38 2023-09-22 15:00:42.000000 django-mailer-2.3.1/setup.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-12-29 15:00:14.956361 django-mailer-2.3.1/src/
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-12-29 15:00:14.964361 django-mailer-2.3.1/src/django_mailer.egg-info/
+-rw-r--r--   0 luke      (1000) luke      (1000)     1336 2023-12-29 15:00:14.000000 django-mailer-2.3.1/src/django_mailer.egg-info/PKG-INFO
+-rw-r-----   0 luke      (1000) luke      (1000)     1439 2023-12-29 15:00:14.000000 django-mailer-2.3.1/src/django_mailer.egg-info/SOURCES.txt
+-rw-r-----   0 luke      (1000) luke      (1000)        1 2023-12-29 15:00:14.000000 django-mailer-2.3.1/src/django_mailer.egg-info/dependency_links.txt
+-rw-r-----   0 luke      (1000) luke      (1000)       26 2023-12-29 15:00:14.000000 django-mailer-2.3.1/src/django_mailer.egg-info/requires.txt
+-rw-r-----   0 luke      (1000) luke      (1000)        7 2023-12-29 15:00:14.000000 django-mailer-2.3.1/src/django_mailer.egg-info/top_level.txt
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-12-29 15:00:14.964361 django-mailer-2.3.1/src/mailer/
+-rw-r--r--   0 luke      (1000) luke      (1000)     3109 2023-12-29 14:59:09.000000 django-mailer-2.3.1/src/mailer/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1485 2023-09-22 15:01:19.000000 django-mailer-2.3.1/src/mailer/admin.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      144 2023-09-22 15:01:18.000000 django-mailer-2.3.1/src/mailer/apps.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      485 2023-09-22 15:01:18.000000 django-mailer-2.3.1/src/mailer/backend.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     9734 2023-09-25 14:35:45.000000 django-mailer-2.3.1/src/mailer/engine.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-12-29 15:00:14.956361 django-mailer-2.3.1/src/mailer/locale/
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-12-29 15:00:14.956361 django-mailer-2.3.1/src/mailer/locale/ja/
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-12-29 15:00:14.968361 django-mailer-2.3.1/src/mailer/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 luke      (1000) luke      (1000)     1164 2019-09-23 17:24:14.000000 django-mailer-2.3.1/src/mailer/locale/ja/LC_MESSAGES/django.po
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-12-29 15:00:14.956361 django-mailer-2.3.1/src/mailer/locale/ru/
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-12-29 15:00:14.968361 django-mailer-2.3.1/src/mailer/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 luke      (1000) luke      (1000)     1171 2019-09-23 17:24:14.000000 django-mailer-2.3.1/src/mailer/locale/ru/LC_MESSAGES/django.po
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-12-29 15:00:14.968361 django-mailer-2.3.1/src/mailer/management/
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2019-09-23 17:24:14.000000 django-mailer-2.3.1/src/mailer/management/__init__.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-12-29 15:00:14.968361 django-mailer-2.3.1/src/mailer/management/commands/
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2019-09-23 17:24:14.000000 django-mailer-2.3.1/src/mailer/management/commands/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      913 2023-09-22 15:08:37.000000 django-mailer-2.3.1/src/mailer/management/commands/purge_mail_log.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      705 2023-09-22 15:08:37.000000 django-mailer-2.3.1/src/mailer/management/commands/retry_deferred.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1073 2023-09-25 14:35:45.000000 django-mailer-2.3.1/src/mailer/management/commands/runmailer.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1208 2023-09-25 14:35:45.000000 django-mailer-2.3.1/src/mailer/management/commands/runmailer_pg.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      956 2023-09-22 15:01:19.000000 django-mailer-2.3.1/src/mailer/management/commands/send_mail.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      710 2023-09-22 15:01:19.000000 django-mailer-2.3.1/src/mailer/management/helpers.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-12-29 15:00:14.972361 django-mailer-2.3.1/src/mailer/migrations/
+-rw-r--r--   0 luke      (1000) luke      (1000)     2586 2023-09-22 15:01:19.000000 django-mailer-2.3.1/src/mailer/migrations/0001_initial.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      625 2023-09-22 15:01:19.000000 django-mailer-2.3.1/src/mailer/migrations/0002_auto_20150720_1433.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      403 2023-09-22 15:01:19.000000 django-mailer-2.3.1/src/mailer/migrations/0003_messagelog_message_id.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      999 2023-09-22 15:01:19.000000 django-mailer-2.3.1/src/mailer/migrations/0004_auto_20190920_1512.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      874 2023-09-22 15:01:19.000000 django-mailer-2.3.1/src/mailer/migrations/0005_id_bigautofield.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      385 2023-09-22 15:01:19.000000 django-mailer-2.3.1/src/mailer/migrations/0006_message_retry_count.py
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2019-09-23 17:24:14.000000 django-mailer-2.3.1/src/mailer/migrations/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     9241 2023-09-22 15:08:37.000000 django-mailer-2.3.1/src/mailer/models.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     5330 2023-12-07 16:48:27.000000 django-mailer-2.3.1/src/mailer/postgres.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-12-29 15:00:14.972361 django-mailer-2.3.1/tests/
+-rw-r--r--   0 luke      (1000) luke      (1000)      778 2023-09-22 15:01:19.000000 django-mailer-2.3.1/tests/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      303 2023-09-22 15:49:33.000000 django-mailer-2.3.1/tests/settings.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    33141 2023-09-22 15:01:20.000000 django-mailer-2.3.1/tests/test_mailer.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      773 2023-09-22 15:49:33.000000 django-mailer-2.3.1/tox.ini
```

### Comparing `django-mailer-2.3/.pre-commit-config.yaml` & `django-mailer-2.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-mailer-2.3/CHANGES.rst` & `django-mailer-2.3.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Change log
 ==========
 
+2.3.1 - 2023-12-29
+------------------
+
+* Fixed rare crasher in runmailer_pg when notifications list is empty.
+
 2.3 - 2023-09-25
 ----------------
 
 * Dropped Python 3.7 support.
 * Added ``runmailer_pg`` - advanced sending method for sending emails without delay
   immediate, PostgreSQL only.
```

### Comparing `django-mailer-2.3/CONTRIBUTING.rst` & `django-mailer-2.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-mailer-2.3/LICENSE` & `django-mailer-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mailer-2.3/PKG-INFO` & `django-mailer-2.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mailer
-Version: 2.3
+Version: 2.3.1
 Summary: A reusable Django app for queuing the sending of email
 Home-page: http://github.com/pinax/django-mailer/
 Author: Pinax Team
 Author-email: developers@pinaxproject.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-mailer-2.3/README.rst` & `django-mailer-2.3.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -21,38 +21,47 @@
 -------------
 
 ``django-mailer`` is a reusable Django app for queuing the sending of email. It
 works by storing email in the database for later sending. This has a number of
 advantages:
 
 - **robustness** - if your email provider goes down or has a temporary error,
-  the email won’t be lost.
+  the email won’t be lost. In addition, since the ``send_mail()`` call always
+  succeeds (unless your database is out of action), then the HTTP request that
+  triggered the email to be sent won’t crash, and any ongoing transaction won’t
+  be rolled back.
 
 - **correctness** - when an outgoing email is created as part of a transaction,
   since it is stored in the database it will participate in transactions. This
   means it won’t be sent until the transaction is committed, and won’t be sent
   at all if the transaction is rolled back.
 
 
 In addition, if you want to ensure that mails are sent very quickly, and without
 heaving polling, django-mailer comes with a PostgreSQL specific ``runmailer_pg``
-command. This uses PostgresSQLs NOTIFY/LISTEN feature to be able to send emails
-as soon as they are added to the queue.
+command. This uses PostgreSQL’s `NOTIFY
+<https://www.postgresql.org/docs/16/sql-notify.html>`_/`LISTEN
+<https://www.postgresql.org/docs/16/sql-listen.html>`_ feature to be able to
+send emails as soon as they are added to the queue.
 
 
 Limitations
 -----------
 
 File attachments are also temporarily stored in the database, which means if you
 are sending files larger than several hundred KB in size, you are likely to run
 into database limitations on how large your query can be. If this happens,
 you'll either need to fall back to using Django's default mail backend, or
 increase your database limits (a procedure that depends on which database you
 are using).
 
+With django-mailer, you can’t know in a Django view function whether the email
+has actually been sent or not - the ``send_mail`` function just stores mail on
+the queue to be sent later.
+
 django-mailer was developed as part of the `Pinax ecosystem
 <http://pinaxproject.com>`_ but is just a Django app and can be used
 independently of other Pinax apps.
 
 
 Requirements
 ------------
```

### Comparing `django-mailer-2.3/RELEASE.rst` & `django-mailer-2.3.1/RELEASE.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Release process
 ---------------
 
 * Check that the master branching is passing all tests:
   https://github.com/pinax/django-mailer/actions/workflows/build.yml
 
-* In CHANGES.rst, change the 'Unreleased' heading to the new version, and commit.
+* In CHANGES.rst, change the 'Unreleased' heading to the new version.
 
-* Change the version in mailer/__init__.py, removing ``.dev1`` if necessary, and commit.
+* Change the version in mailer/__init__.py, removing ``.dev1`` if necessary, and commit with “Version bump …”
 
 * Release::
 
     $ ./release.sh
 
 * Tag the release e.g.::
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-mailer-2.3/docs/usage.rst` & `django-mailer-2.3.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `django-mailer-2.3/manage.py` & `django-mailer-2.3.1/manage.py`

 * *Files identical despite different names*

### Comparing `django-mailer-2.3/setup.cfg` & `django-mailer-2.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-mailer-2.3/src/django_mailer.egg-info/PKG-INFO` & `django-mailer-2.3.1/src/django_mailer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mailer
-Version: 2.3
+Version: 2.3.1
 Summary: A reusable Django app for queuing the sending of email
 Home-page: http://github.com/pinax/django-mailer/
 Author: Pinax Team
 Author-email: developers@pinaxproject.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-mailer-2.3/src/django_mailer.egg-info/SOURCES.txt` & `django-mailer-2.3.1/src/django_mailer.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 requirements-dev.txt
 requirements-test.txt
 setup.cfg
 setup.py
 tox.ini
 docs/index.rst
 docs/usage.rst
+docs/usage.rst.html
 src/django_mailer.egg-info/PKG-INFO
 src/django_mailer.egg-info/SOURCES.txt
 src/django_mailer.egg-info/dependency_links.txt
 src/django_mailer.egg-info/requires.txt
 src/django_mailer.egg-info/top_level.txt
 src/mailer/__init__.py
 src/mailer/admin.py
```

### Comparing `django-mailer-2.3/src/mailer/__init__.py` & `django-mailer-2.3.1/src/mailer/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import warnings
 
-__version__ = "2.3"
+__version__ = "2.3.1"
 
 
 def get_priority(priority):
     from mailer.models import PRIORITY_MAPPING, PRIORITY_MEDIUM
 
     if priority is None:
         priority = PRIORITY_MEDIUM
```

### Comparing `django-mailer-2.3/src/mailer/admin.py` & `django-mailer-2.3.1/src/mailer/admin.py`

 * *Files identical despite different names*

### Comparing `django-mailer-2.3/src/mailer/engine.py` & `django-mailer-2.3.1/src/mailer/engine.py`

 * *Files identical despite different names*

### Comparing `django-mailer-2.3/src/mailer/locale/ja/LC_MESSAGES/django.po` & `django-mailer-2.3.1/src/mailer/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-mailer-2.3/src/mailer/locale/ru/LC_MESSAGES/django.po` & `django-mailer-2.3.1/src/mailer/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-mailer-2.3/src/mailer/management/commands/purge_mail_log.py` & `django-mailer-2.3.1/src/mailer/management/commands/purge_mail_log.py`

 * *Files identical despite different names*

### Comparing `django-mailer-2.3/src/mailer/management/commands/retry_deferred.py` & `django-mailer-2.3.1/src/mailer/management/commands/retry_deferred.py`

 * *Files identical despite different names*

### Comparing `django-mailer-2.3/src/mailer/management/commands/runmailer.py` & `django-mailer-2.3.1/src/mailer/management/commands/runmailer.py`

 * *Files identical despite different names*

### Comparing `django-mailer-2.3/src/mailer/management/commands/runmailer_pg.py` & `django-mailer-2.3.1/src/mailer/management/commands/runmailer_pg.py`

 * *Files identical despite different names*

### Comparing `django-mailer-2.3/src/mailer/management/commands/send_mail.py` & `django-mailer-2.3.1/src/mailer/management/commands/send_mail.py`

 * *Files identical despite different names*

### Comparing `django-mailer-2.3/src/mailer/management/helpers.py` & `django-mailer-2.3.1/src/mailer/management/helpers.py`

 * *Files identical despite different names*

### Comparing `django-mailer-2.3/src/mailer/migrations/0001_initial.py` & `django-mailer-2.3.1/src/mailer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mailer-2.3/src/mailer/migrations/0002_auto_20150720_1433.py` & `django-mailer-2.3.1/src/mailer/migrations/0002_auto_20150720_1433.py`

 * *Files identical despite different names*

### Comparing `django-mailer-2.3/src/mailer/migrations/0004_auto_20190920_1512.py` & `django-mailer-2.3.1/src/mailer/migrations/0004_auto_20190920_1512.py`

 * *Files identical despite different names*

### Comparing `django-mailer-2.3/src/mailer/migrations/0005_id_bigautofield.py` & `django-mailer-2.3.1/src/mailer/migrations/0005_id_bigautofield.py`

 * *Files identical despite different names*

### Comparing `django-mailer-2.3/src/mailer/models.py` & `django-mailer-2.3.1/src/mailer/models.py`

 * *Files identical despite different names*

### Comparing `django-mailer-2.3/src/mailer/postgres.py` & `django-mailer-2.3.1/src/mailer/postgres.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 CHANNEL = "django_mailer_new_message"
 
 
 def postgres_send_loop():
     """
-    Loop indefinitely, checking queue using NOTIFY/LISTEN and running send_mail(),
+    Loop indefinitely, checking queue using NOTIFY/LISTEN and running send_all(),
     and additional running every MAILER_EMPTY_QUEUE_SLEEP seconds.
     """
     # See https://www.psycopg.org/docs/advanced.html#asynchronous-notifications
 
     # Get a connection, for a few lower level operations.
     dj_conn = connections[Message.objects.db]
     if dj_conn.connection is None:
@@ -56,41 +56,51 @@
     SELECT_TIMEOUT = 5
     while True:
         if select.select([conn], [], [], SELECT_TIMEOUT) == ([], [], []):
             # timeout
             pass
         else:
             conn.poll()
-            last = conn.notifies.pop()
+            try:
+                last = conn.notifies.pop()
+            except IndexError:
+                # Not entirely sure how this happens, but it could only happen
+                # if `notifies` is empty, because there are no more notifications
+                # to process.
+                continue
+
             # We don't care about payload or how many NOTIFY there were,
-            # we'll just run once.
-            dropped = conn.notifies
-            if dropped:
-                logger.debug("Dropping notifications %r", dropped)
+            # we'll just run once, so drop the rest:
+            to_drop = conn.notifies
+            if to_drop:
+                # This happens if several messages were inserted in the same
+                # transaction - we get multiple items on `conn.notifies` after a
+                # single `conn.poll()`
+                logger.debug("Dropping notifications %r", to_drop)
             conn.notifies.clear()
 
             if notify_q.empty():
                 logger.debug("Putting %r on queue", last)
                 notify_q.put(last)
             else:
                 # notify_q is not empty.
 
                 # Our worker thread always processes all Messages. If it still
                 # has an item on the queue, it will process all remaining
                 # messages next time it runs, so there is no point adding
                 # another item to the non-empty queue - this will just cause
                 # `send_all()` to run pointlessly.
 
-                # This is quite important for efficiency - if we have a
-                # transaction that inserts 100 items into the Message table,
-                # once it commits the NOTIFY gets sent 100 times. Each one is
-                # received individually by the `.poll()` call above. The first
-                # `send_all()` command will deal with them all - we don't want
-                # `send_all()` to thrash away doing nothing another 99 times
-                # afterwards.
+                # This could be important for efficiency: if 100 records are
+                # inserted into the Message table at the same time, this process
+                # will get NOTIFY sent 100 times (unless they were all part of
+                # the same transaction). The first `send_all()` command will
+                # deal with them all (or a large fraction of them, depending on
+                # timing). We don't want `send_all()` to thrash away doing
+                # nothing another 99 times afterwards.
                 logger.debug("Discarding item %r as work queue is not empty", last)
 
     # Clean up:
     worker_thread.join()
     if beat_thread is not None:
         beat_thread.join()
 
@@ -132,15 +142,15 @@
         send_all()
         logger.debug("Finished %r", item)
         notify_q.task_done()
 
 
 @dataclass
 class Scheduled:
-    now: datetime
+    now: datetime  # this is used for debugging only, we just need some object on the queue
 
 
 def beat():
     while True:
         if notify_q.empty():
             scheduled = Scheduled(now=datetime.now())
             logger.debug("Putting scheduled item %r on queue", scheduled)
```

### Comparing `django-mailer-2.3/tests/__init__.py` & `django-mailer-2.3.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-mailer-2.3/tests/test_mailer.py` & `django-mailer-2.3.1/tests/test_mailer.py`

 * *Files identical despite different names*

### Comparing `django-mailer-2.3/tox.ini` & `django-mailer-2.3.1/tox.ini`

 * *Files identical despite different names*

