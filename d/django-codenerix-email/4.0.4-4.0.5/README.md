# Comparing `tmp/django-codenerix-email-4.0.4.tar.gz` & `tmp/django-codenerix-email-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-codenerix-email-4.0.4.tar", last modified: Mon Apr  8 11:05:01 2024, max compression
+gzip compressed data, was "django-codenerix-email-4.0.5.tar", last modified: Wed May 22 12:44:54 2024, max compression
```

## Comparing `django-codenerix-email-4.0.4.tar` & `django-codenerix-email-4.0.5.tar`

### file list

```diff
@@ -1,84 +1,89 @@
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-08 11:05:01.052900 django-codenerix-email-4.0.4/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    11339 2024-03-27 07:06:52.000000 django-codenerix-email-4.0.4/LICENSE
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      247 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/MANIFEST.in
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     2543 2024-04-08 11:05:01.052900 django-codenerix-email-4.0.4/PKG-INFO
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1344 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/README.rst
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-08 11:05:01.040900 django-codenerix-email-4.0.4/codenerix_email/
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)      148 2024-04-08 11:05:00.000000 django-codenerix-email-4.0.4/codenerix_email/__init__.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1208 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/admin.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      149 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/apps.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3157 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/forms.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-08 11:05:01.040900 django-codenerix-email-4.0.4/codenerix_email/management/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/management/__init__.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-08 11:05:01.044900 django-codenerix-email-4.0.4/codenerix_email/management/__pycache__/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      179 2023-10-27 11:25:38.000000 django-codenerix-email-4.0.4/codenerix_email/management/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      195 2024-02-26 06:56:17.000000 django-codenerix-email-4.0.4/codenerix_email/management/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      160 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/management/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      168 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/management/__pycache__/__init__.cpython-39.pyc
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-08 11:05:01.044900 django-codenerix-email-4.0.4/codenerix_email/management/commands/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/management/commands/__init__.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     5603 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/management/commands/send_emails.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1645 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/management/commands/test_email.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-08 11:05:01.044900 django-codenerix-email-4.0.4/codenerix_email/migrations/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3511 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/0001_initial.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2369 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/0002_auto_20170502_1043.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      656 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/0003_auto_20170921_1206.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      486 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/0004_auto_20171108_1628.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      495 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/0005_emailmessage_retries.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      489 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/0006_emailmessage_error.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      602 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/0007_emailmessage_next_retry.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      731 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/0008_auto_20171201_0928.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__init__.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-08 11:05:01.052900 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2005 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3682 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0001_initial.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2373 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0001_initial.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2020 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1500 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2664 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1692 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1515 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      694 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      967 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      782 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      709 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      676 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      939 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      713 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      691 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      691 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      954 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      728 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      706 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      675 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      938 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      712 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      690 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      802 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1111 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      854 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      817 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      779 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1178 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      839 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      794 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      151 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      195 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      147 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      168 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    12659 2024-04-08 11:00:35.000000 django-codenerix-email-4.0.4/codenerix_email/models.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-08 11:05:01.040900 django-codenerix-email-4.0.4/codenerix_email/static/
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-08 11:05:01.040900 django-codenerix-email-4.0.4/codenerix_email/static/codenerix_email/
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-08 11:05:01.052900 django-codenerix-email-4.0.4/codenerix_email/static/codenerix_email/partials/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      994 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/codenerix_email/static/codenerix_email/partials/emailmessages_rows.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2595 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.4/codenerix_email/urls.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3804 2024-02-07 09:54:44.000000 django-codenerix-email-4.0.4/codenerix_email/views.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-08 11:05:01.052900 django-codenerix-email-4.0.4/django_codenerix_email.egg-info/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2543 2024-04-08 11:05:00.000000 django-codenerix-email-4.0.4/django_codenerix_email.egg-info/PKG-INFO
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     4221 2024-04-08 11:05:00.000000 django-codenerix-email-4.0.4/django_codenerix_email.egg-info/SOURCES.txt
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2024-04-08 11:05:00.000000 django-codenerix-email-4.0.4/django_codenerix_email.egg-info/dependency_links.txt
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.4/django_codenerix_email.egg-info/not-zip-safe
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       53 2024-04-08 11:05:00.000000 django-codenerix-email-4.0.4/django_codenerix_email.egg-info/requires.txt
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       16 2024-04-08 11:05:00.000000 django-codenerix-email-4.0.4/django_codenerix_email.egg-info/top_level.txt
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)       38 2024-04-08 11:05:01.052900 django-codenerix-email-4.0.4/setup.cfg
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1707 2024-04-08 11:04:22.000000 django-codenerix-email-4.0.4/setup.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 12:44:54.978218 django-codenerix-email-4.0.5/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    11339 2024-03-27 07:06:52.000000 django-codenerix-email-4.0.5/LICENSE
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      247 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/MANIFEST.in
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     2543 2024-05-22 12:44:54.974218 django-codenerix-email-4.0.5/PKG-INFO
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1344 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/README.rst
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 12:44:54.966218 django-codenerix-email-4.0.5/codenerix_email/
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)      148 2024-05-22 12:44:54.000000 django-codenerix-email-4.0.5/codenerix_email/__init__.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1208 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/admin.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      149 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/apps.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3706 2024-05-22 12:29:39.000000 django-codenerix-email-4.0.5/codenerix_email/forms.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 12:44:54.966218 django-codenerix-email-4.0.5/codenerix_email/management/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/management/__init__.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 12:44:54.970219 django-codenerix-email-4.0.5/codenerix_email/management/__pycache__/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      179 2023-10-27 11:25:38.000000 django-codenerix-email-4.0.5/codenerix_email/management/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      195 2024-02-26 06:56:17.000000 django-codenerix-email-4.0.5/codenerix_email/management/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      160 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/management/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      168 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/management/__pycache__/__init__.cpython-39.pyc
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 12:44:54.970219 django-codenerix-email-4.0.5/codenerix_email/management/commands/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/management/commands/__init__.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     6290 2024-04-09 05:53:51.000000 django-codenerix-email-4.0.5/codenerix_email/management/commands/send_emails.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1655 2024-04-09 05:53:42.000000 django-codenerix-email-4.0.5/codenerix_email/management/commands/test_email.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 12:44:54.970219 django-codenerix-email-4.0.5/codenerix_email/migrations/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3511 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/0001_initial.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2369 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/0002_auto_20170502_1043.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      656 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/0003_auto_20170921_1206.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      486 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/0004_auto_20171108_1628.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      495 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/0005_emailmessage_retries.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      489 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/0006_emailmessage_error.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      602 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/0007_emailmessage_next_retry.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      731 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/0008_auto_20171201_0928.py
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     1219 2024-05-22 11:42:23.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/0009_emailmessage_opened_emailmessage_uuid.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__init__.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 12:44:54.974218 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2005 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3682 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2373 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0001_initial.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2020 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1500 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2664 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1692 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1515 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      694 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      967 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      782 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      709 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      676 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      939 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      713 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      691 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      691 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      954 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      728 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      706 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      675 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      938 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      712 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      690 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      802 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1111 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      854 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      817 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      779 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1178 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      839 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      794 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-39.pyc
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)      733 2024-05-21 07:57:54.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0009_delete_emailtemplatetexten.cpython-311.pyc
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     1860 2024-05-22 11:44:13.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0009_emailmessage_opened_emailmessage_uuid.cpython-311.pyc
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     3104 2024-05-22 11:40:40.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0010_emailmessage_opened_emailmessage_uuid_and_more.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      151 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      195 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      147 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      168 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    13201 2024-05-22 12:41:41.000000 django-codenerix-email-4.0.5/codenerix_email/models.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 12:44:54.966218 django-codenerix-email-4.0.5/codenerix_email/static/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 12:44:54.966218 django-codenerix-email-4.0.5/codenerix_email/static/codenerix_email/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 12:44:54.974218 django-codenerix-email-4.0.5/codenerix_email/static/codenerix_email/partials/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1060 2024-05-22 11:47:17.000000 django-codenerix-email-4.0.5/codenerix_email/static/codenerix_email/partials/emailmessages_rows.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2595 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/urls.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      873 2024-05-22 12:21:01.000000 django-codenerix-email-4.0.5/codenerix_email/urls_frontend.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     4820 2024-05-22 12:38:27.000000 django-codenerix-email-4.0.5/codenerix_email/views.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 12:44:54.974218 django-codenerix-email-4.0.5/django_codenerix_email.egg-info/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2543 2024-05-22 12:44:54.000000 django-codenerix-email-4.0.5/django_codenerix_email.egg-info/PKG-INFO
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     4619 2024-05-22 12:44:54.000000 django-codenerix-email-4.0.5/django_codenerix_email.egg-info/SOURCES.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2024-05-22 12:44:54.000000 django-codenerix-email-4.0.5/django_codenerix_email.egg-info/dependency_links.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/django_codenerix_email.egg-info/not-zip-safe
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       53 2024-05-22 12:44:54.000000 django-codenerix-email-4.0.5/django_codenerix_email.egg-info/requires.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       16 2024-05-22 12:44:54.000000 django-codenerix-email-4.0.5/django_codenerix_email.egg-info/top_level.txt
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)       38 2024-05-22 12:44:54.978218 django-codenerix-email-4.0.5/setup.cfg
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1707 2024-04-08 11:04:22.000000 django-codenerix-email-4.0.5/setup.py
```

### Comparing `django-codenerix-email-4.0.4/LICENSE` & `django-codenerix-email-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/PKG-INFO` & `django-codenerix-email-4.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-codenerix-email
-Version: 4.0.4
+Version: 4.0.5
 Summary: Codenerix Email is a module that enables CODENERIX to set send emails in a general manner.
 Home-page: https://github.com/codenerix/django-codenerix-email
 Author: Juan Miguel Taboada Godoy <juanmi@juanmitaboada.com>, Juan Soler Ruiz <soleronline@gmail.com>
 License: Apache License Version 2.0
 Keywords: django,codenerix,management,erp,crm,send email
 Platform: OS Independent
 Classifier: Environment :: Web Environment
```

### Comparing `django-codenerix-email-4.0.4/README.rst` & `django-codenerix-email-4.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/admin.py` & `django-codenerix-email-4.0.5/codenerix_email/admin.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/management/commands/send_emails.py` & `django-codenerix-email-4.0.5/codenerix_email/management/commands/send_emails.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,98 +20,130 @@
 
 import time
 
 from django.core.management.base import BaseCommand
 from django.conf import settings
 from django.utils import timezone
 
-from codenerix.lib.debugger import Debugger
+from codenerix_lib.debugger import Debugger
 from codenerix_email.models import EmailMessage
 
 
 class Command(BaseCommand, Debugger):
 
     # Show this when the user types help
     help = "Try to send all emails in the queue"
 
     def add_arguments(self, parser):
 
         # Named (optional) arguments
-        parser.add_argument('-d',
-                            action='store_true',
-                            dest='d',
-                            default=False,
-                            help='Keep the command working forever as a daemon')
+        parser.add_argument(
+            "-d",
+            action="store_true",
+            dest="d",
+            default=False,
+            help="Keep the command working forever as a daemon",
+        )
 
         # Named (optional) arguments
-        parser.add_argument('--daemon',
-                            action='store_true',
-                            dest='daemon',
-                            default=False,
-                            help='Keep the command working forever as a daemon')
+        parser.add_argument(
+            "--daemon",
+            action="store_true",
+            dest="daemon",
+            default=False,
+            help="Keep the command working forever as a daemon",
+        )
 
         # Named (optional) arguments
-        parser.add_argument('-c',
-                            action='store_true',
-                            dest='c',
-                            default=False,
-                            help='Clear the sending status to all the Queue')
+        parser.add_argument(
+            "-c",
+            action="store_true",
+            dest="c",
+            default=False,
+            help="Clear the sending status to all the Queue",
+        )
 
         # Named (optional) arguments
-        parser.add_argument('--clear',
-                            action='store_true',
-                            dest='clear',
-                            default=False,
-                            help='Clear the sending status to all the Queue')
+        parser.add_argument(
+            "--clear",
+            action="store_true",
+            dest="clear",
+            default=False,
+            help="Clear the sending status to all the Queue",
+        )
 
     def handle(self, *args, **options):
 
         # Autoconfigure Debugger
         self.set_name("CODENERIX-EMAIL")
         self.set_debug()
 
         # Get user configuration
-        daemon = bool(options['daemon'] or options['d'])
-        clear = bool(options['clear'] or options['c'])
-        BUCKET_SIZE = getattr(settings, 'CLIENT_EMAIL_BUCKETS', 10)
+        daemon = bool(options["daemon"] or options["d"])
+        clear = bool(options["clear"] or options["c"])
+        BUCKET_SIZE = getattr(settings, "CLIENT_EMAIL_BUCKETS", 10)
         if daemon:
-            self.debug("Starting command in DAEMON mode with a queue of {} emails".format(BUCKET_SIZE), color='cyan')
+            self.debug(
+                "Starting command in DAEMON mode with a queue of {} emails".format(
+                    BUCKET_SIZE
+                ),
+                color="cyan",
+            )
         else:
-            self.debug("Starting a queue of {} emails".format(BUCKET_SIZE), color='blue')
+            self.debug(
+                "Starting a queue of {} emails".format(BUCKET_SIZE),
+                color="blue",
+            )
 
         # In if requested set sending status for all the list to False
         if clear:
             EmailMessage.objects.filter(sending=True).update(sending=False)
 
         # Get a bunch of emails in the queue
         connection = None
 
         # If daemon mode is requested
         first = True
         while first or daemon:
 
             # Get a bucket of emails
-            emails = EmailMessage.objects.filter(sent=False, sending=False, error=False, next_retry__lte=timezone.now()).order_by('priority', 'next_retry')[0:BUCKET_SIZE+1]
+            emails = EmailMessage.objects.filter(
+                sent=False,
+                sending=False,
+                error=False,
+                next_retry__lte=timezone.now(),
+            ).order_by("priority", "next_retry")[0 : BUCKET_SIZE + 1]
 
             # Check if there are emails to process
             if emails:
 
                 # Convert to list
                 list_emails = [x.pk for x in emails]
 
                 # Set sending status for all the list
-                EmailMessage.objects.filter(pk__in=list_emails).update(sending=True)
+                EmailMessage.objects.filter(pk__in=list_emails).update(
+                    sending=True
+                )
 
                 # For each email
                 for email in emails:
-                    self.debug("Sending to {}".format(email.eto), color='white', tail=False)
+                    self.debug(
+                        "Sending to {}".format(email.eto),
+                        color="white",
+                        tail=False,
+                    )
 
                     # Check if we have connection
                     if not connection:
-                        self.debug(" - Connecting", color='yellow', head=False, tail=False)
+                        self.debug(
+                            " - Connecting",
+                            color="yellow",
+                            head=False,
+                            tail=False,
+                        )
                         connection = email.connect()
 
                     # Send the email
                     try:
                         email.send(connection, debug=False)
                     except Exception as e:
                         email.sending = False
@@ -119,31 +151,45 @@
                         if email.log:
                             email.log += error
                         else:
                             email.log = error
                         email.save()
                         self.error(error)
                     if email.sent:
-                        self.debug(" -> SENT", color='green', head=False)
+                        self.debug(" -> SENT", color="green", head=False)
                     else:
-                        self.debug(" -> ERROR", color='red', head=False, tail=False)
-                        self.debug(" ({} retries left)".format(getattr(settings, 'CLIENT_EMAIL_RETRIES', 10) - email.retries), color='cyan', head=False)
+                        self.debug(
+                            " -> ERROR", color="red", head=False, tail=False
+                        )
+                        self.debug(
+                            " ({} retries left)".format(
+                                getattr(settings, "CLIENT_EMAIL_RETRIES", 10)
+                                - email.retries
+                            ),
+                            color="cyan",
+                            head=False,
+                        )
 
                 # Delete all that have been sent
-                if not getattr(settings, 'CLIENT_EMAIL_HISTORY', True):
-                    EmailMessage.objects.filter(pk__in=list_emails, sent=True).delete()
+                if not getattr(settings, "CLIENT_EMAIL_HISTORY", True):
+                    EmailMessage.objects.filter(
+                        pk__in=list_emails, sent=True
+                    ).delete()
 
             elif daemon:
 
                 # Sleep for a while
                 try:
                     time.sleep(10)
                 except KeyboardInterrupt:
-                    self.debug("Exited by user request!", color='green')
+                    self.debug("Exited by user request!", color="green")
                     break
 
             else:
                 # No emails to send
-                self.debug("No emails to be sent at this moment in the queue!", color='green')
+                self.debug(
+                    "No emails to be sent at this moment in the queue!",
+                    color="green",
+                )
 
             # This was the first time
             first = False
```

### Comparing `django-codenerix-email-4.0.4/codenerix_email/management/commands/test_email.py` & `django-codenerix-email-4.0.5/codenerix_email/management/commands/test_email.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,39 +18,41 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from django.core.management.base import BaseCommand
 from django.conf import settings
 
-from codenerix.lib.debugger import Debugger
+from codenerix_lib.debugger import Debugger
 from codenerix_email.models import EmailMessage
 from codenerix_email import __version__
 
 
 class Command(BaseCommand, Debugger):
 
     # Show this when the user types help
     help = "Test"
-    
+
     def handle(self, *args, **options):
-        
+
         # Autoconfigure Debugger
         self.set_name("CODENERIX-EMAIL")
         self.set_debug()
 
-        message = '''Hello,
+        message = """Hello,
 
 this email has been sent using Django Codenerix Email.
 
 Best regards, Codenerix Team
 
 --
-Django Codenerix Email v{}'''.format(__version__)
+Django Codenerix Email v{}""".format(
+            __version__
+        )
 
         for name, email in settings.ADMINS:
             email_message = EmailMessage()
             email_message.efrom = settings.DEFAULT_FROM_EMAIL
             email_message.eto = email
-            email_message.subject = '[Codenerix Email] Test'
+            email_message.subject = "[Codenerix Email] Test"
             email_message.body = message
             email_message.send(legacy=False, silent=False)
```

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/0001_initial.py` & `django-codenerix-email-4.0.5/codenerix_email/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/0002_auto_20170502_1043.py` & `django-codenerix-email-4.0.5/codenerix_email/migrations/0002_auto_20170502_1043.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/0003_auto_20170921_1206.py` & `django-codenerix-email-4.0.5/codenerix_email/migrations/0003_auto_20170921_1206.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/0007_emailmessage_next_retry.py` & `django-codenerix-email-4.0.5/codenerix_email/migrations/0007_emailmessage_next_retry.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/0008_auto_20171201_0928.py` & `django-codenerix-email-4.0.5/codenerix_email/migrations/0008_auto_20171201_0928.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0001_initial.cpython-311.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0001_initial.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0001_initial.cpython-35.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0001_initial.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0001_initial.cpython-39.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-310.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-311.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-35.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-39.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-310.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-311.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-35.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-39.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-310.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-311.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-35.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-39.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-310.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-311.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-35.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-39.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-310.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-311.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-35.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-39.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-310.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-311.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-35.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-39.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-310.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-311.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-35.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-39.pyc` & `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/models.py` & `django-codenerix-email-4.0.5/codenerix_email/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,29 +17,41 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import re
 import ssl
 import smtplib
+from uuid import uuid4
 
 from django.utils import timezone
 from django.utils.translation import gettext_lazy as _
 from django.db import models
 from django.template import Context, Template
 from django.core.exceptions import ValidationError
 from django.conf import settings
 
-from codenerix.models import CodenerixModel
+from codenerix.models import CodenerixModel  # type: ignore
 from codenerix_lib.debugger import Debugger
-from codenerix.lib.genmail import EmailMessage as EM, get_connection
-from codenerix.fields import WysiwygAngularField
+from codenerix.lib.genmail import (  # type: ignore # noqa: N817
+    EmailMessage as EM,
+    get_connection,
+)
+from codenerix.fields import WysiwygAngularField  # type: ignore
 
 
 class EmailMessage(CodenerixModel, Debugger):
+    uuid = models.UUIDField(
+        _("UUID"),
+        unique=True,
+        default=uuid4,
+        editable=False,
+        null=False,
+        blank=False,
+    )
     efrom = models.EmailField(_("From"), blank=False, null=False)
     eto = models.EmailField(_("To"), blank=False, null=False)
     subject = models.CharField(
         _("Subject"), max_length=256, blank=False, null=False
     )
     body = models.TextField(_("Body"), blank=False, null=False)
     priority = models.PositiveIntegerField(
@@ -55,33 +67,42 @@
         _("Error"), blank=False, null=False, default=False
     )
     retries = models.PositiveIntegerField(
         _("Retries"), blank=False, null=False, default=0
     )
     next_retry = models.DateTimeField(_("Next retry"), auto_now_add=True)
     log = models.TextField(_("Log"), blank=True, null=True)
+    opened = models.DateTimeField(
+        _("Opened"), null=True, blank=True, default=None
+    )
 
     def __fields__(self, info):
         fields = []
         fields.append(("sending", None, 100))
         fields.append(("error", None, 100))
         fields.append(("sent", _("Send"), 100))
         fields.append(("priority", _("Priority"), 100))
+        fields.append(("uuid", _("UUID"), 100))
         fields.append(("created", _("Created"), 100))
+        fields.append(("opened", _("Opened"), 100))
         fields.append(("efrom", _("From"), 100))
         fields.append(("eto", _("To"), 100))
         fields.append(("subject", _("Subject"), 100))
         fields.append(("retries", _("Retries"), 100))
         fields.append(("next_retry", _("Next retry"), 100))
         fields.append(("pk", _("ID"), 100))
         return fields
 
     def __unicode__(self):
         return "{} ({})".format(self.eto, self.pk)
 
+    def set_opened(self):
+        self.opened = timezone.now()
+        self.save()
+
     def connect(self, legacy=False):
         """
         This class will return a connection instance, you can disconnect it with connection.close()
         """
 
         if not legacy:
             host = settings.CLIENT_EMAIL_HOST
```

### Comparing `django-codenerix-email-4.0.4/codenerix_email/static/codenerix_email/partials/emailmessages_rows.html` & `django-codenerix-email-4.0.5/codenerix_email/static/codenerix_email/partials/emailmessages_rows.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 <td>
     <span class='fa fa-refresh fa-spin fa-fw text-info' ng-if='!row.error && row.sending' alt='{{data.meta.gentranslate.sending}}...' title='{{data.meta.gentranslate.sending}}...'></span>
     <span class='fa fa-envelope-o text-success' ng-if='!row.error && !row.sending && row.sent' alt='{{data.meta.gentranslate.sent}}' title='{{data.meta.gentranslate.sent}}'></span>
     <span class='fa fa-envelope-open-o' ng-if='!row.error && !row.sending && !row.sent' alt='{{data.meta.gentranslate.waiting}}' title='{{data.meta.gentranslate.waiting}}'></span>
     <span ng-if='row.error' alt='{{data.meta.gentranslate.notsent}}' title='{{data.meta.gentranslate.notsent}}' codenerix-html-compile="false|codenerix"></span>
 </td>
 <td>{{row.priority|codenerix}}</td>
+<td>{{row.uuid|codenerix}}</td>
 <td>{{row.created|codenerix}}</td>
+<td>{{row.opened|codenerix}}</td>
 <td>{{row.efrom|codenerix}}</td>
 <td>{{row.eto|codenerix}}</td>
 <td>{{row.subject|codenerix}}</td>
 <td>{{row.retries|codenerix}}</td>
 <td>{{row.next_retry|codenerix}}</td>
 <td>{{row.pk|codenerix}}</td>
```

### Comparing `django-codenerix-email-4.0.4/codenerix_email/urls.py` & `django-codenerix-email-4.0.5/codenerix_email/urls.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.4/codenerix_email/views.py` & `django-codenerix-email-4.0.5/codenerix_email/views.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,22 +14,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Optional, Tuple, List, Dict, Any
+import base64
 
+from typing import Optional, Tuple, List, Dict
+from django.http import HttpResponse
+from django.views.generic import View
+
+from django.shortcuts import get_object_or_404
 from django.utils.translation import gettext as _
 from django.conf import settings
-from django.http import HttpRequest
+from django.http import HttpRequest, Http404
 
-from codenerix.multiforms import MultiForm
-from codenerix.views import (
+from codenerix.multiforms import MultiForm  # type: ignore
+from codenerix.views import (  # type: ignore
     GenList,
     GenCreate,
     GenCreateModal,
     GenUpdate,
     GenUpdateModal,
     GenDelete,
     GenDetail,
@@ -67,14 +72,46 @@
                 field,
                 None,
             )
         )
 
 
 # ############################################
+# EmailFollow
+class EmailFollow(View):
+    def get(self, request, *args, **kwargs):
+
+        # Get uuid from email
+        uid = kwargs.get("uuid_ext", None)
+
+        if uid:
+
+            # Get email message or return 404
+            email_message = get_object_or_404(EmailMessage, uuid=uid)
+
+            # Set email message as opened
+            if not email_message.opened:
+                email_message.set_opened()
+            email_message.set_opened()
+
+            # Return an image of 1x1 pixel
+            return HttpResponse(
+                base64.b64decode(
+                    "R0lGODlhAQABAIAAAP///wAAACH5BAEAAAAALAAAAAABAAEAAAICRAEAOw=="
+                ),
+                content_type="image/gif",
+            )
+
+        else:
+
+            # Return 404
+            raise Http404
+
+
+# ############################################
 # EmailTemplate
 class EmailTemplateList(GenList):
     model = EmailTemplate
     extra_context = {
         "menu": ["EmailTemplate", "people"],
         "bread": [_("EmailTemplate"), _("People")],
     }
```

### Comparing `django-codenerix-email-4.0.4/django_codenerix_email.egg-info/PKG-INFO` & `django-codenerix-email-4.0.5/django_codenerix_email.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-codenerix-email
-Version: 4.0.4
+Version: 4.0.5
 Summary: Codenerix Email is a module that enables CODENERIX to set send emails in a general manner.
 Home-page: https://github.com/codenerix/django-codenerix-email
 Author: Juan Miguel Taboada Godoy <juanmi@juanmitaboada.com>, Juan Soler Ruiz <soleronline@gmail.com>
 License: Apache License Version 2.0
 Keywords: django,codenerix,management,erp,crm,send email
 Platform: OS Independent
 Classifier: Environment :: Web Environment
```

### Comparing `django-codenerix-email-4.0.4/django_codenerix_email.egg-info/SOURCES.txt` & `django-codenerix-email-4.0.5/django_codenerix_email.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 codenerix_email/__init__.py
 codenerix_email/admin.py
 codenerix_email/apps.py
 codenerix_email/forms.py
 codenerix_email/models.py
 codenerix_email/urls.py
+codenerix_email/urls_frontend.py
 codenerix_email/views.py
 codenerix_email/management/__init__.py
 codenerix_email/management/__pycache__/__init__.cpython-310.pyc
 codenerix_email/management/__pycache__/__init__.cpython-311.pyc
 codenerix_email/management/__pycache__/__init__.cpython-35.pyc
 codenerix_email/management/__pycache__/__init__.cpython-39.pyc
 codenerix_email/management/commands/__init__.py
@@ -21,14 +22,15 @@
 codenerix_email/migrations/0002_auto_20170502_1043.py
 codenerix_email/migrations/0003_auto_20170921_1206.py
 codenerix_email/migrations/0004_auto_20171108_1628.py
 codenerix_email/migrations/0005_emailmessage_retries.py
 codenerix_email/migrations/0006_emailmessage_error.py
 codenerix_email/migrations/0007_emailmessage_next_retry.py
 codenerix_email/migrations/0008_auto_20171201_0928.py
+codenerix_email/migrations/0009_emailmessage_opened_emailmessage_uuid.py
 codenerix_email/migrations/__init__.py
 codenerix_email/migrations/__pycache__/0001_initial.cpython-310.pyc
 codenerix_email/migrations/__pycache__/0001_initial.cpython-311.pyc
 codenerix_email/migrations/__pycache__/0001_initial.cpython-35.pyc
 codenerix_email/migrations/__pycache__/0001_initial.cpython-39.pyc
 codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-310.pyc
 codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-311.pyc
@@ -54,14 +56,17 @@
 codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-311.pyc
 codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-35.pyc
 codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-39.pyc
 codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-310.pyc
 codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-311.pyc
 codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-35.pyc
 codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-39.pyc
+codenerix_email/migrations/__pycache__/0009_delete_emailtemplatetexten.cpython-311.pyc
+codenerix_email/migrations/__pycache__/0009_emailmessage_opened_emailmessage_uuid.cpython-311.pyc
+codenerix_email/migrations/__pycache__/0010_emailmessage_opened_emailmessage_uuid_and_more.cpython-311.pyc
 codenerix_email/migrations/__pycache__/__init__.cpython-310.pyc
 codenerix_email/migrations/__pycache__/__init__.cpython-311.pyc
 codenerix_email/migrations/__pycache__/__init__.cpython-35.pyc
 codenerix_email/migrations/__pycache__/__init__.cpython-39.pyc
 codenerix_email/static/codenerix_email/partials/emailmessages_rows.html
 django_codenerix_email.egg-info/PKG-INFO
 django_codenerix_email.egg-info/SOURCES.txt
```

### Comparing `django-codenerix-email-4.0.4/setup.py` & `django-codenerix-email-4.0.5/setup.py`

 * *Files identical despite different names*

