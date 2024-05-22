# Comparing `tmp/python-crontab-3.0.0.tar.gz` & `tmp/python-crontab-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-crontab-3.0.0.tar", last modified: Thu Jul 13 14:53:01 2023, max compression
+gzip compressed data, was "python-crontab-3.1.0.tar", last modified: Wed May 22 06:13:01 2024, max compression
```

## Comparing `python-crontab-3.0.0.tar` & `python-crontab-3.1.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2023-07-13 14:53:01.829805 python-crontab-3.0.0/
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       34 2015-12-28 06:36:10.000000 python-crontab-3.0.0/AUTHORS
--rw-r--r--   0 doctormo  (1000) doctormo  (1000)    14570 2022-12-22 04:33:16.000000 python-crontab-3.0.0/CHANGES.md
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     7651 2015-12-28 06:36:10.000000 python-crontab-3.0.0/COPYING
--rw-r--r--   0 doctormo  (1000) doctormo  (1000)      322 2020-03-23 16:32:58.000000 python-crontab-3.0.0/MANIFEST.in
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)    17141 2023-07-13 14:53:01.829805 python-crontab-3.0.0/PKG-INFO
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)    15879 2023-07-13 14:51:49.000000 python-crontab-3.0.0/README.rst
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3773 2022-12-22 04:41:54.000000 python-crontab-3.0.0/cronlog.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)    51493 2023-07-13 13:57:37.000000 python-crontab-3.0.0/crontab.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     4438 2015-12-28 22:23:00.000000 python-crontab-3.0.0/crontabs.py
-drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2023-07-13 14:53:01.825805 python-crontab-3.0.0/python_crontab.egg-info/
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)    17141 2023-07-13 14:53:01.000000 python-crontab-3.0.0/python_crontab.egg-info/PKG-INFO
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     1118 2023-07-13 14:53:01.000000 python-crontab-3.0.0/python_crontab.egg-info/SOURCES.txt
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)        1 2023-07-13 14:53:01.000000 python-crontab-3.0.0/python_crontab.egg-info/dependency_links.txt
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       78 2023-07-13 14:53:01.000000 python-crontab-3.0.0/python_crontab.egg-info/requires.txt
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       25 2023-07-13 14:53:01.000000 python-crontab-3.0.0/python_crontab.egg-info/top_level.txt
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       38 2023-07-13 14:53:01.829805 python-crontab-3.0.0/setup.cfg
--rwxrwxr-x   0 doctormo  (1000) doctormo  (1000)     2941 2023-07-13 14:52:41.000000 python-crontab-3.0.0/setup.py
-drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2023-07-13 14:53:01.829805 python-crontab-3.0.0/tests/
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)        1 2015-12-29 21:09:18.000000 python-crontab-3.0.0/tests/__init__.py
-drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2023-07-13 14:53:01.829805 python-crontab-3.0.0/tests/data/
-drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2023-07-13 14:53:01.829805 python-crontab-3.0.0/tests/data/anacron/
--rwxr-xr-x   0 doctormo  (1000) doctormo  (1000)        0 2015-12-28 21:48:51.000000 python-crontab-3.0.0/tests/data/anacron/an_command.sh
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)        0 2015-12-28 21:49:06.000000 python-crontab-3.0.0/tests/data/anacron/not_command.txt
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)      108 2015-12-28 06:36:10.000000 python-crontab-3.0.0/tests/data/basic.log
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       49 2015-12-28 18:57:24.000000 python-crontab-3.0.0/tests/data/crontab
-drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2023-07-13 14:53:01.829805 python-crontab-3.0.0/tests/data/crontabs/
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)        0 2015-12-28 21:47:03.000000 python-crontab-3.0.0/tests/data/crontabs/.empty
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       50 2015-12-28 18:17:28.000000 python-crontab-3.0.0/tests/data/crontabs/system_one
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       28 2015-12-28 18:44:58.000000 python-crontab-3.0.0/tests/data/crontabs/system_two
--rwxrwxr-x   0 doctormo  (1000) doctormo  (1000)     1366 2022-12-22 04:30:31.000000 python-crontab-3.0.0/tests/data/crontest
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       50 2015-12-28 06:36:10.000000 python-crontab-3.0.0/tests/data/specials.tab
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       77 2015-12-28 06:36:10.000000 python-crontab-3.0.0/tests/data/specials_enc.tab
-drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2023-07-13 14:53:01.829805 python-crontab-3.0.0/tests/data/spool/
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       23 2015-12-28 06:36:10.000000 python-crontab-3.0.0/tests/data/spool/basic
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       82 2015-12-28 19:06:04.000000 python-crontab-3.0.0/tests/data/spool/hgreen
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       79 2015-12-28 19:03:15.000000 python-crontab-3.0.0/tests/data/spool/jgreen
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       42 2015-12-28 06:36:10.000000 python-crontab-3.0.0/tests/data/spool/user
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     2409 2015-12-28 06:36:10.000000 python-crontab-3.0.0/tests/data/test.log
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)      470 2020-05-15 23:43:15.000000 python-crontab-3.0.0/tests/data/test.tab
--rw-r--r--   0 doctormo  (1000) doctormo  (1000)     4249 2023-07-13 13:44:06.000000 python-crontab-3.0.0/tests/test_compatibility.py
--rw-r--r--   0 doctormo  (1000) doctormo  (1000)     2059 2020-01-27 06:39:48.000000 python-crontab-3.0.0/tests/test_context.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     2906 2015-12-28 06:36:10.000000 python-crontab-3.0.0/tests/test_croniter.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3815 2021-10-19 20:14:53.000000 python-crontab-3.0.0/tests/test_crontabs.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     2041 2016-06-11 20:45:16.000000 python-crontab-3.0.0/tests/test_description.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3600 2016-12-12 16:26:39.000000 python-crontab-3.0.0/tests/test_enums.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     6184 2018-05-08 19:50:48.000000 python-crontab-3.0.0/tests/test_env.py
--rwxr-xr-x   0 doctormo  (1000) doctormo  (1000)     2078 2020-01-27 07:25:15.000000 python-crontab-3.0.0/tests/test_equality.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3402 2022-12-22 04:40:59.000000 python-crontab-3.0.0/tests/test_every.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     7052 2022-12-31 19:51:32.000000 python-crontab-3.0.0/tests/test_frequency.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)    13878 2022-12-22 04:47:17.000000 python-crontab-3.0.0/tests/test_interaction.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     5603 2015-12-31 05:53:07.000000 python-crontab-3.0.0/tests/test_log.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     4721 2022-12-22 04:39:45.000000 python-crontab-3.0.0/tests/test_range.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     5103 2022-12-22 04:39:23.000000 python-crontab-3.0.0/tests/test_removal.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3378 2022-12-31 19:59:46.000000 python-crontab-3.0.0/tests/test_scheduler.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     4123 2019-01-03 16:19:25.000000 python-crontab-3.0.0/tests/test_system_cron.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     9251 2023-07-13 14:00:42.000000 python-crontab-3.0.0/tests/test_usage.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3651 2022-12-22 04:38:56.000000 python-crontab-3.0.0/tests/test_utf8.py
--rw-r--r--   0 doctormo  (1000) doctormo  (1000)     2831 2018-05-25 14:54:01.000000 python-crontab-3.0.0/tests/utils.py
+drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2024-05-22 06:13:01.749803 python-crontab-3.1.0/
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       34 2015-12-28 06:36:10.000000 python-crontab-3.1.0/AUTHORS
+-rw-r--r--   0 doctormo  (1000) doctormo  (1000)    14570 2022-12-22 04:33:16.000000 python-crontab-3.1.0/CHANGES.md
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     7651 2015-12-28 06:36:10.000000 python-crontab-3.1.0/COPYING
+-rw-r--r--   0 doctormo  (1000) doctormo  (1000)      322 2020-03-23 16:32:58.000000 python-crontab-3.1.0/MANIFEST.in
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)    17143 2024-05-22 06:13:01.749803 python-crontab-3.1.0/PKG-INFO
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)    15879 2023-07-13 14:51:49.000000 python-crontab-3.1.0/README.rst
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3773 2022-12-22 04:41:54.000000 python-crontab-3.1.0/cronlog.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)    51719 2024-05-22 06:02:45.000000 python-crontab-3.1.0/crontab.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     4570 2024-05-22 05:37:50.000000 python-crontab-3.1.0/crontabs.py
+drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2024-05-22 06:13:01.749803 python-crontab-3.1.0/python_crontab.egg-info/
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)    17143 2024-05-22 06:13:01.000000 python-crontab-3.1.0/python_crontab.egg-info/PKG-INFO
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     1118 2024-05-22 06:13:01.000000 python-crontab-3.1.0/python_crontab.egg-info/SOURCES.txt
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)        1 2024-05-22 06:13:01.000000 python-crontab-3.1.0/python_crontab.egg-info/dependency_links.txt
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       78 2024-05-22 06:13:01.000000 python-crontab-3.1.0/python_crontab.egg-info/requires.txt
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       25 2024-05-22 06:13:01.000000 python-crontab-3.1.0/python_crontab.egg-info/top_level.txt
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       38 2024-05-22 06:13:01.749803 python-crontab-3.1.0/setup.cfg
+-rwxrwxr-x   0 doctormo  (1000) doctormo  (1000)     2941 2023-07-13 14:52:41.000000 python-crontab-3.1.0/setup.py
+drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2024-05-22 06:13:01.749803 python-crontab-3.1.0/tests/
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)        1 2015-12-29 21:09:18.000000 python-crontab-3.1.0/tests/__init__.py
+drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2024-05-22 06:13:01.749803 python-crontab-3.1.0/tests/data/
+drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2024-05-22 06:13:01.749803 python-crontab-3.1.0/tests/data/anacron/
+-rwxr-xr-x   0 doctormo  (1000) doctormo  (1000)        0 2015-12-28 21:48:51.000000 python-crontab-3.1.0/tests/data/anacron/an_command.sh
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)        0 2015-12-28 21:49:06.000000 python-crontab-3.1.0/tests/data/anacron/not_command.txt
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)      108 2015-12-28 06:36:10.000000 python-crontab-3.1.0/tests/data/basic.log
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       49 2015-12-28 18:57:24.000000 python-crontab-3.1.0/tests/data/crontab
+drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2024-05-22 06:13:01.749803 python-crontab-3.1.0/tests/data/crontabs/
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)        0 2015-12-28 21:47:03.000000 python-crontab-3.1.0/tests/data/crontabs/.empty
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       50 2015-12-28 18:17:28.000000 python-crontab-3.1.0/tests/data/crontabs/system_one
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       28 2015-12-28 18:44:58.000000 python-crontab-3.1.0/tests/data/crontabs/system_two
+-rwxrwxr-x   0 doctormo  (1000) doctormo  (1000)     1366 2022-12-22 04:30:31.000000 python-crontab-3.1.0/tests/data/crontest
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       50 2015-12-28 06:36:10.000000 python-crontab-3.1.0/tests/data/specials.tab
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       77 2015-12-28 06:36:10.000000 python-crontab-3.1.0/tests/data/specials_enc.tab
+drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2024-05-22 06:13:01.749803 python-crontab-3.1.0/tests/data/spool/
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       23 2015-12-28 06:36:10.000000 python-crontab-3.1.0/tests/data/spool/basic
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       82 2015-12-28 19:06:04.000000 python-crontab-3.1.0/tests/data/spool/hgreen
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       79 2015-12-28 19:03:15.000000 python-crontab-3.1.0/tests/data/spool/jgreen
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       42 2015-12-28 06:36:10.000000 python-crontab-3.1.0/tests/data/spool/user
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     2409 2015-12-28 06:36:10.000000 python-crontab-3.1.0/tests/data/test.log
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)      471 2024-05-22 06:02:22.000000 python-crontab-3.1.0/tests/data/test.tab
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     4267 2023-10-21 19:16:57.000000 python-crontab-3.1.0/tests/test_compatibility.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     2076 2023-10-21 19:16:57.000000 python-crontab-3.1.0/tests/test_context.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     2923 2023-10-21 19:16:57.000000 python-crontab-3.1.0/tests/test_croniter.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3831 2023-10-21 19:16:57.000000 python-crontab-3.1.0/tests/test_crontabs.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     2058 2023-10-21 19:16:57.000000 python-crontab-3.1.0/tests/test_description.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3617 2023-10-21 19:16:57.000000 python-crontab-3.1.0/tests/test_enums.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     6201 2024-05-22 06:09:44.000000 python-crontab-3.1.0/tests/test_env.py
+-rwxrwxr-x   0 doctormo  (1000) doctormo  (1000)     2094 2023-10-21 19:16:57.000000 python-crontab-3.1.0/tests/test_equality.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3419 2023-10-21 19:16:57.000000 python-crontab-3.1.0/tests/test_every.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     7349 2024-05-22 05:29:48.000000 python-crontab-3.1.0/tests/test_frequency.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)    13894 2023-10-21 19:16:57.000000 python-crontab-3.1.0/tests/test_interaction.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     5620 2023-10-21 19:16:57.000000 python-crontab-3.1.0/tests/test_log.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     4738 2023-10-21 19:16:57.000000 python-crontab-3.1.0/tests/test_range.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     5120 2023-10-21 19:16:57.000000 python-crontab-3.1.0/tests/test_removal.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3394 2024-05-22 05:32:35.000000 python-crontab-3.1.0/tests/test_scheduler.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     4140 2023-10-21 19:16:57.000000 python-crontab-3.1.0/tests/test_system_cron.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     9267 2023-10-21 19:16:57.000000 python-crontab-3.1.0/tests/test_usage.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3668 2023-10-21 19:16:57.000000 python-crontab-3.1.0/tests/test_utf8.py
+-rw-r--r--   0 doctormo  (1000) doctormo  (1000)     2831 2018-05-25 14:54:01.000000 python-crontab-3.1.0/tests/utils.py
```

### Comparing `python-crontab-3.0.0/CHANGES.md` & `python-crontab-3.1.0/CHANGES.md`

 * *Files identical despite different names*

### Comparing `python-crontab-3.0.0/COPYING` & `python-crontab-3.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `python-crontab-3.0.0/PKG-INFO` & `python-crontab-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-crontab
-Version: 3.0.0
+Version: 3.1.0
 Summary: Python Crontab API
 Home-page: https://gitlab.com/doctormo/python-crontab/
 Author: Martin Owens
 Author-email: doctormo@gmail.com
 License: LGPLv3
 Platform: linux
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,16 +23,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides: crontab
 Provides: crontabs
 Provides: cronlog
 Description-Content-Type: text/x-rst
-Provides-Extra: cron-schedule
 Provides-Extra: cron-description
+Provides-Extra: cron-schedule
 License-File: COPYING
 License-File: AUTHORS
 
 Python Crontab
 --------------
 
 .. image:: https://gitlab.com/doctormo/python-crontab/raw/master/branding.svg
@@ -513,7 +513,9 @@
  - Customise the location of the crontab command by setting the global CRON_COMMAND
    or the per-object cron_command attribute.
  - Support for vixie cron with username addition with user flag
  - Support for SunOS, AIX & HP with compatibility 'SystemV' mode.
  - Python 3 (3.7, 3.8, 3.10) tested, python 2.6, 2.7 removed from support.
  - Windows support works for non-system crontabs only.
    ( see mem_cron and file_cron examples above for usage )
+
+
```

### Comparing `python-crontab-3.0.0/README.rst` & `python-crontab-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-crontab-3.0.0/cronlog.py` & `python-crontab-3.1.0/cronlog.py`

 * *Files identical despite different names*

### Comparing `python-crontab-3.0.0/crontab.py` & `python-crontab-3.1.0/crontab.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
 from calendar import monthrange
 from time import sleep
 from datetime import time, date, datetime, timedelta
 from collections import OrderedDict
 
 __pkgname__ = 'python-crontab'
-__version__ = '3.0.0'
+__version__ = '3.1.0'
 
 ITEMREX = re.compile(r'^\s*([^@#\s]+)\s+([^@#\s]+)\s+([^@#\s]+)\s+([^@#\s]+)'
                      r'\s+([^@#\s]+)\s+([^\n]*?)(\s+#\s*([^\n]*)|$)')
 SPECREX = re.compile(r'^\s*@(\w+)\s([^#\n]*)(\s+#\s*([^\n]*)|$)')
 DEVNULL = ">/dev/null 2>&1"
 
 WEEK_ENUM = ['sun', 'mon', 'tue', 'wed', 'thu', 'fri', 'sat', 'sun']
@@ -667,15 +667,15 @@
         self.pre_comment = pre_comment
 
     def parse(self, line):
         """Parse a cron line string and save the info as the objects."""
         line = _str(line)
         if not line or line[0] == '#':
             self.enabled = False
-            line = line[1:].strip()
+            line = line.strip().lstrip('#').strip()
         # We parse all lines so we can detect disabled entries.
         self._set_parse(ITEMREX.findall(line), line)
         self._set_parse(SPECREX.findall(line), line)
 
     def _set_parse(self, result, line=""):
         """Set all the parsed variables into the item"""
         if not result:
@@ -1251,14 +1251,15 @@
         return str(self) == str(value)
 
     def __str__(self):
         return self.render()
 
     def every(self, n_value, also=False):
         """Set the every X units value"""
+        n_value = self.test_value(n_value)
         if not also:
             self.clear()
         self.parts += self.get_range(int(n_value))
         return self.parts[-1]
 
     def on(self, *n_value, **opts):
         """Set the time values to the specified placements."""
@@ -1318,23 +1319,26 @@
             val = self.min
         try:
             out = get_cronvalue(val, self.enum)
         except ValueError as err:
             raise ValueError(f"Unrecognised {self.name}: '{val}'") from err
         except KeyError as err:
             raise KeyError(f"No enumeration for {self.name}: '{val}'") from err
+        return self.test_value(out, sunday=sunday)
 
-        if self.max == 6 and int(out) == 7:
+    def test_value(self, value, sunday=None):
+        """Test the value is within range for this slice"""
+        if self.max == 6 and int(value) == 7:
             if sunday is not None:
                 return sunday
             raise SundayError("Detected Sunday as 7 instead of 0!")
 
-        if int(out) < self.min or int(out) > self.max:
-            raise ValueError(f"'{val}', not in {self.min}-{self.max} for {self.name}")
-        return out
+        if int(value) < self.min or int(value) > self.max:
+            raise ValueError(f"'{value}', not in {self.min}-{self.max} for {self.name}")
+        return value
 
 
 def get_cronvalue(value, enums):
     """Returns a value as int (pass-through) or a special enum value"""
     if isinstance(value, int):
         return value
     if str(value).isdigit():
```

### Comparing `python-crontab-3.0.0/crontabs.py` & `python-crontab-3.1.0/crontabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,22 @@
 #
 """
 The crontabs manager will list all available crontabs on the system.
 """
 
 import os
 import sys
-import pwd
 import itertools
 
 from os import stat, access, X_OK
-from pwd import getpwuid
-from crontab import CronTab
+from crontab import CronTab, WINOS
+
+getpwuid = None
+if not WINOS:
+    from pwd import getpwuid
 
 class UserSpool(list):
     """Generates all user crontabs, yields both owned and abandoned tabs"""
     def __init__(self, loc, tabs=None):
         for username in self.listdir(loc):
             tab = self.generate(loc, username)
             if tab:
@@ -43,14 +45,16 @@
         try:
             return os.listdir(loc)
         except OSError:
             return []
 
     def get_owner(self, path):
         """Returns user file at path"""
+        if not getpwuid:
+            raise OSError("This functionality is not available on Windows")
         try:
             return getpwuid(stat(path).st_uid).pw_name
         except KeyError:
             return
 
     def generate(self, loc, username):
         path = os.path.join(loc, username)
```

### Comparing `python-crontab-3.0.0/python_crontab.egg-info/PKG-INFO` & `python-crontab-3.1.0/python_crontab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-crontab
-Version: 3.0.0
+Version: 3.1.0
 Summary: Python Crontab API
 Home-page: https://gitlab.com/doctormo/python-crontab/
 Author: Martin Owens
 Author-email: doctormo@gmail.com
 License: LGPLv3
 Platform: linux
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,16 +23,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides: crontab
 Provides: crontabs
 Provides: cronlog
 Description-Content-Type: text/x-rst
-Provides-Extra: cron-schedule
 Provides-Extra: cron-description
+Provides-Extra: cron-schedule
 License-File: COPYING
 License-File: AUTHORS
 
 Python Crontab
 --------------
 
 .. image:: https://gitlab.com/doctormo/python-crontab/raw/master/branding.svg
@@ -513,7 +513,9 @@
  - Customise the location of the crontab command by setting the global CRON_COMMAND
    or the per-object cron_command attribute.
  - Support for vixie cron with username addition with user flag
  - Support for SunOS, AIX & HP with compatibility 'SystemV' mode.
  - Python 3 (3.7, 3.8, 3.10) tested, python 2.6, 2.7 removed from support.
  - Windows support works for non-system crontabs only.
    ( see mem_cron and file_cron examples above for usage )
+
+
```

### Comparing `python-crontab-3.0.0/python_crontab.egg-info/SOURCES.txt` & `python-crontab-3.1.0/python_crontab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-crontab-3.0.0/setup.py` & `python-crontab-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-crontab-3.0.0/tests/data/crontest` & `python-crontab-3.1.0/tests/data/crontest`

 * *Files identical despite different names*

### Comparing `python-crontab-3.0.0/tests/data/test.log` & `python-crontab-3.1.0/tests/data/test.log`

 * *Files identical despite different names*

### Comparing `python-crontab-3.0.0/tests/test_compatibility.py` & `python-crontab-3.1.0/tests/test_compatibility.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,14 @@
 """
 
 import os
 import sys
 
 import unittest
 import crontab
-try:
-    from test import test_support
-except ImportError:
-    from test import support as test_support
 
 TEST_DIR = os.path.dirname(__file__)
 
 INITAL_TAB = """
 # First Comment
 0,30 * * * * firstcommand
 """
@@ -105,15 +101,15 @@
         self.assertEqual(cron[0].comment, '{job_name}')
         self.assertEqual(cron[0].command, '{command}')
         self.assertEqual(str(cron[0]), '#Ansible: {job_name}\n* * * * * {command}')
 
     def test_06_escaped_chars(self):
         """Do escaped chars parse correctly when read in"""
         cron = crontab.CronTab(tab="""
-* * * * * cmd arg_with_\#_character # comment
+* * * * * cmd arg_with_\\#_character # comment
 """)
         self.assertEqual(cron[0].command, 'cmd arg_with_\\#_character')
         self.assertEqual(cron[0].comment, 'comment')
 
     def test_07_non_posix_shell(self):
         """Shell in windows environments is split correctly"""
         from crontab import Process
@@ -122,10 +118,15 @@
         self.assertEqual(pipe.wait(), 0, 'Windows shell command not found!')
         (out, err) = pipe.communicate()
         self.assertEqual(out, b'Double Glazing Installed:SLASHED\n')
         self.assertEqual(err, b'')
 
 
 if __name__ == '__main__':
+    try:
+        from test import test_support
+    except ImportError:
+        from test import support as test_support
+
     test_support.run_unittest(
        CompatTestCase,
     )
```

### Comparing `python-crontab-3.0.0/tests/test_context.py` & `python-crontab-3.1.0/tests/test_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,18 +22,14 @@
 import os
 import sys
 
 sys.path.insert(0, '../')
 
 import unittest
 from crontab import CronTab
-try:
-    from test import test_support
-except ImportError:
-    from test import support as test_support
 
 INITAL_TAB = """
 * * * JAN     SAT          enums
 * * * MAR-APR *            ranges
 * * * *       MON,FRI,WED  multiples
 * * * *       *            com1 # Comment One
 * * * *       *            com2 # Comment One
@@ -60,10 +56,15 @@
             self.assertEqual(str(line), results[line_no])
         with CronTab(tab=INITAL_TAB) as crontab_context:
             self.crontab_context = crontab_context
         for line_no, line in enumerate(self.crontab_context.intab.split('\n')):
             self.assertEqual(str(line), results[line_no])
 
 if __name__ == '__main__':
+    try:
+        from test import test_support
+    except ImportError:
+        from test import support as test_support
+
     test_support.run_unittest(
        ContextTestCase,
     )
```

### Comparing `python-crontab-3.0.0/tests/test_croniter.py` & `python-crontab-3.1.0/tests/test_croniter.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,18 +23,14 @@
 import sys
 from datetime import datetime
 
 sys.path.insert(0, '../')
 
 import unittest
 import crontab
-try:
-    from test import test_support
-except ImportError:
-    from test import support as test_support
 
 INITAL_TAB = """
 # Basic Comment
 20 * * * * execute # comment
 """
 
 class CroniterTestCase(unittest.TestCase):
@@ -80,10 +76,15 @@
     def test_04_current(self):
         """Get Current Item"""
         ct = self.job.schedule(datetime(2001, 10, 11, 1, 12, 10))
         self.assertEqual(ct.get_current(), datetime(2001, 10, 11, 1, 12, 10))
         self.assertEqual(ct.get_current(), datetime(2001, 10, 11, 1, 12, 10))
 
 if __name__ == '__main__':
+    try:
+        from test import test_support
+    except ImportError:
+        from test import support as test_support
+
     test_support.run_unittest(
        CroniterTestCase,
     )
```

### Comparing `python-crontab-3.0.0/tests/test_crontabs.py` & `python-crontab-3.1.0/tests/test_crontabs.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,19 +22,14 @@
 import os
 import sys
 
 import unittest
 import crontab
 import crontabs
 
-try:
-    from test import test_support
-except ImportError:
-    from test import support as test_support
-
 TEST_DIR = os.path.dirname(__file__)
 
 class fake_getpwuid(object):
     def __init__(self, st):
         self.pw_name = st
         if st == 'error':
             raise KeyError("Expected Error")
@@ -104,9 +99,14 @@
         self.assertNotInTabs('anacron_cmd')
         jobs = self.assertInTabs('an_command.sh', 'root')
         self.assertEqual(str(jobs[0].slices), AnacronSourceTab.slices)
         self.assertNotInTabs('not_command.txt')
         
 
 if __name__ == '__main__':
+    try:
+        from test import test_support
+    except ImportError:
+        from test import support as test_support
+
     test_support.run_unittest(CronTabsTestCase)
```

### Comparing `python-crontab-3.0.0/tests/test_description.py` & `python-crontab-3.1.0/tests/test_description.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,18 +20,14 @@
 """
 
 import sys
 sys.path.insert(0, '../')
 
 import unittest
 import crontab
-try:
-    from test import test_support
-except ImportError:
-    from test import support as test_support
 
 INITAL_TAB = """
 # Basic Comment
 20 10-20 */2 * * execute # At 20 minutes past the hour, between 10:00 AM and 08:59 PM, every 2 days
 """
 
 class DescriptorTestCase(unittest.TestCase):
@@ -58,9 +54,14 @@
         sys.path = old
 
     def test_01_description(self):
         """Get Job Description"""
         self.assertEqual(self.job.description(), self.job.comment)
 
 if __name__ == '__main__':
+    try:
+        from test import test_support
+    except ImportError:
+        from test import support as test_support
+
     test_support.run_unittest(DescriptorTestCase)
```

### Comparing `python-crontab-3.0.0/tests/test_enums.py` & `python-crontab-3.1.0/tests/test_enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,14 @@
 import os
 import sys
 
 sys.path.insert(0, '../')
 
 import unittest
 from crontab import CronTab
-try:
-    from test import test_support
-except ImportError:
-    from test import support as test_support
 
 INITAL_TAB = """
 * * * JAN     SAT          enums
 * * * MAR-APR *            ranges
 * * * *       MON,FRI,WED  multiples
 * * * *       *            com1 # Comment One
 * * * *       *            com2 # Comment One
@@ -112,10 +108,15 @@
         """Comment Set"""
         jobs = list(self.crontab.find_comment('Comment One'))
         self.assertEqual(len(jobs), 2)
         for job in jobs:
             self.assertEqual(job.comment, 'Comment One')
 
 if __name__ == '__main__':
+    try:
+        from test import test_support
+    except ImportError:
+        from test import support as test_support
+
     test_support.run_unittest(
        EnumTestCase,
     )
```

### Comparing `python-crontab-3.0.0/tests/test_env.py` & `python-crontab-3.1.0/tests/test_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,18 +25,14 @@
 
 from .test_usage import TEST_DIR
 
 import unittest
 from collections import OrderedDict
 
 from crontab import CronTab
-try:
-    from test import test_support
-except ImportError:
-    from test import support as test_support
 
 INITIAL_TAB = """PERSONAL_VAR=bar
 
 CRON_VAR=fork
 34 12 * * * eat_soup
 
 CRON_VAR=spoon
@@ -213,8 +209,13 @@
 # B
 # C
 */10 * * * * /home/pi/job.py # any job
 """)
         os.unlink(filename)
 
 if __name__ == '__main__':
+    try:
+        from test import test_support
+    except ImportError:
+        from test import support as test_support
+
     test_support.run_unittest(EnvTestCase)
```

### Comparing `python-crontab-3.0.0/tests/test_equality.py` & `python-crontab-3.1.0/tests/test_equality.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,19 +19,14 @@
 """
 Test equality between CronItems
 """
 
 import unittest
 from crontab import CronTab
 
-try:
-    from test import test_support
-except ImportError:
-    from test import support as test_support
-
 CRONTAB1 = """
     3 * * * * command1 # CommentID C
     2 * * * * command2 # CommentID AAB
     1 * * * * command3 # CommentID B3
 """
 
 CRONTAB2 = """
@@ -60,8 +55,13 @@
         self.assertEqual(set(self.crontab2) - set(self.crontab1), {self.crontab2[3]})
 
     def test_hash(self):
         """Test object hashing"""
         self.assertEqual(self.crontab1[0].__hash__(), hash((self.crontab1[0])))
 
 if __name__ == '__main__':
+    try:
+        from test import test_support
+    except ImportError:
+        from test import support as test_support
+
     test_support.run_unittest(EqualityTestCase)
```

### Comparing `python-crontab-3.0.0/tests/test_every.py` & `python-crontab-3.1.0/tests/test_every.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,14 @@
 import os
 import sys
 
 sys.path.insert(0, '../')
 
 import unittest
 from crontab import CronTab
-try:
-    from test import test_support
-except ImportError:
-    from test import support as test_support
 
 TEST_DIR = os.path.dirname(__file__)
 
 class EveryTestCase(unittest.TestCase):
     """Test basic functionality of crontab."""
     def setUp(self):
         self.crontab = CronTab(tabfile=os.path.join(TEST_DIR, 'data', 'test.tab'))
@@ -97,10 +93,15 @@
         job.every().hour()
         self.assertEqual(job.slices.render(), '@hourly')
         job = self.crontab.new(command='firstly')
         job.hours.every(2)
         self.assertEqual(job.slices.render(), '* */2 * * *')
 
 if __name__ == '__main__':
+    try:
+        from test import test_support
+    except ImportError:
+        from test import support as test_support
+
     test_support.run_unittest(
        EveryTestCase,
     )
```

### Comparing `python-crontab-3.0.0/tests/test_frequency.py` & `python-crontab-3.1.0/tests/test_frequency.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,23 +17,21 @@
 #
 """
 Test frequency calculations
 """
 
 import os
 import sys
+from calendar import isleap
+from datetime import date
 
 sys.path.insert(0, '../')
 
 import unittest
 from crontab import CronTab
-try:
-    from test import test_support
-except ImportError:
-    from test import support as test_support
 
 START_TAB = """
 """
 
 class FrequencyTestCase(unittest.TestCase):
     """Test basic functionality of crontab."""
     def setUp(self):
@@ -173,23 +171,33 @@
 
     def test_19_frequency_at_month(self):
         """Frequency per month at moment"""
         job = self.crontab.new(command='at_month')
         job.setall("2,4 9 7,14 10,11 *")
         self.assertEqual(job.frequency_at_month(2021, 10), 4)
         self.assertEqual(job.frequency_at_month(2021, 12), 0)
-        self.assertEqual(job.frequency_at_month(), 0)
+        self.assertIn(job.frequency_at_month(), [0, 4])
         self.assertRaises(ValueError, job.frequency_at_month, 2021)
 
     def test_20_frequency_at_year(self):
         """Frequency at leap year day"""
         job = self.crontab.new(command='at_year')
         job.setall("0 * 3,29 2 *")
         self.assertEqual(job.frequency_at_year(2021), 24)
         self.assertEqual(job.frequency_at_year(2024), 48)
-        self.assertEqual(job.frequency_at_year(), 24)
+        self.assertEqual(job.frequency_at_year(), [24, 48][isleap(date.today().year)])
+
+    def test_21_bad_frequency(self):
+        """Frequency must be within range"""
+        job = self.crontab.new(command='at_year')
+        self.assertRaises(ValueError, job.hour.every, 72)
 
 
 if __name__ == '__main__':
+    try:
+        from test import test_support
+    except ImportError:
+        from test import support as test_support
+
     test_support.run_unittest(
        FrequencyTestCase,
     )
```

### Comparing `python-crontab-3.0.0/tests/test_interaction.py` & `python-crontab-3.1.0/tests/test_interaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,19 +22,14 @@
 import re
 import os
 import unittest
 
 from crontab import CronTab, CronSlices, CronSlice
 from .utils import LoggingMixin
 
-try:
-    from test import test_support
-except ImportError:
-    from test import support as test_support
-
 TEST_DIR = os.path.dirname(__file__)
 
 COMMANDS = [
     'firstcommand',
     'range',
     'byweek',
     'disabled',
@@ -388,8 +383,13 @@
         self.assertEqual(str(cron), '\n*/30 * * * * firstcommand\n')
 
         with self.assertRaises(AttributeError):
             cron.crons = ['A']
 
 
 if __name__ == '__main__':
+    try:
+        from test import test_support
+    except ImportError:
+        from test import support as test_support
+
     test_support.run_unittest(InteractionTestCase)
```

### Comparing `python-crontab-3.0.0/tests/test_log.py` & `python-crontab-3.1.0/tests/test_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,14 @@
 import os
 import sys
 from datetime import datetime, date
 
 import unittest
 from crontab import CronTab
 from cronlog import CronLog, LogReader
-try:
-    from test import test_support
-except ImportError:
-    from test import support as test_support
 
 TEST_DIR = os.path.dirname(__file__)
 
 INITAL_TAB = """
 * * * * * userscript &> /dev/null
 * * * * * rootscript &> /dev/null
 * * * * * shadowscript &> /dev/null
@@ -152,10 +148,15 @@
         """Cron Log Error"""
         self.crontab.log.pipe = False
         with self.assertRaises(IOError):
             list(self.crontab.log.readlines())
 
 
 if __name__ == '__main__':
+    try:
+        from test import test_support
+    except ImportError:
+        from test import support as test_support
+
     test_support.run_unittest(
        BasicTestCase,
     )
```

### Comparing `python-crontab-3.0.0/tests/test_range.py` & `python-crontab-3.1.0/tests/test_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,14 @@
 # License along with this library.
 #
 """
 Test crontab ranges.
 """
 import unittest
 from crontab import CronTab, CronSlice
-try:
-    from test import test_support
-except ImportError:
-    from test import support as test_support
 
 from .utils import LoggingMixin
 
 class RangeTestCase(LoggingMixin, unittest.TestCase):
     """Test basic functionality of crontab."""
     log_name = 'crontab'
 
@@ -126,8 +122,13 @@
     def test_06_backwards(self):
         """Test backwards ranges for error"""
         tab = CronTab(tab="* * * * 3-1 command")
         self.assertEqual(str(tab), "# DISABLED LINE\n# * * * * 3-1 command\n")
         self.assertLog("error", "Bad range '3-1'")
 
 if __name__ == '__main__':
+    try:
+        from test import test_support
+    except ImportError:
+        from test import support as test_support
+
     test_support.run_unittest(RangeTestCase)
```

### Comparing `python-crontab-3.0.0/tests/test_removal.py` & `python-crontab-3.1.0/tests/test_removal.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,18 +22,14 @@
 import os
 import sys
 
 sys.path.insert(0, '../')
 
 import unittest
 from crontab import CronTab
-try:
-    from test import test_support
-except ImportError:
-    from test import support as test_support
 
 START_TAB = """
 3 * * * * command1 # CommentID C
 2 * * * * command2 # CommentID AAB
 1 * * * * command3 # CommentID B3
 """
 
@@ -142,10 +138,15 @@
     def tearDown(self):
         for filename in self.filenames:
             if os.path.isfile(filename):
                 os.unlink(filename)
 
 
 if __name__ == '__main__':
+    try:
+        from test import test_support
+    except ImportError:
+        from test import support as test_support
+
     test_support.run_unittest(
        RemovalTestCase,
     )
```

### Comparing `python-crontab-3.0.0/tests/test_scheduler.py` & `python-crontab-3.1.0/tests/test_scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,14 @@
     from StringIO import StringIO
 except ImportError:
     from io import StringIO
 
 logger = logging.getLogger()
 logger.level = logging.WARNING
 
-try:
-    from test import test_support
-except ImportError:
-    from test import support as test_support
-
 TEST_DIR = os.path.dirname(__file__)
 COMMAND = os.path.join(TEST_DIR, 'data', 'crontest ')
 
 class SchedulerTestCase(unittest.TestCase):
     """Test scheduling functions of CronTab."""
     def setUp(self):
         self.tab = crontab.CronTab()
@@ -97,17 +92,22 @@
 
     def test_03_schedule(self):
         """Simple Schedule"""
         self.assertSchedule("* * * * *", 5, 4)
 
     def test_04_schedule_ten(self):
         """Every Ten Minutes"""
-        self.assertSchedule("*/10 * * * *", 12, 1)
+        self.assertSchedule("*/10 * * * *", 10, 1)
 
     def test_05_env_passed(self):
         """Environment is passed in"""
         self.tab.env['CR_VAR'] = 'BABARIAN'
         ret = self.tab.new(command=COMMAND+' -ev').run()
         self.assertEqual(ret, 'BABARIAN')
 
 if __name__ == '__main__':
+    try:
+        from test import test_support
+    except ImportError:
+        from test import support as test_support
+
     test_support.run_unittest(SchedulerTestCase)
```

### Comparing `python-crontab-3.0.0/tests/test_system_cron.py` & `python-crontab-3.1.0/tests/test_system_cron.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,14 @@
 import os
 import sys
 
 sys.path.insert(0, '../')
 
 import unittest
 from crontab import CronTab
-try:
-    from test import test_support
-except ImportError:
-    from test import support as test_support
 
 TEST_FILE = os.path.join(os.path.dirname(__file__), 'data', 'crontab')
 INITIAL_TAB = """
 */30 * * * * palin one_cross_each
 */30 * * * * matias\ttab_user_error
 """
 
@@ -115,8 +111,13 @@
 
     def test_10_system_file(self):
         """Load system crontab from a file"""
         crontab = CronTab(user=False, tabfile=TEST_FILE)
         self.assertEqual(repr(crontab), "<System CronTab '%s'>" % TEST_FILE)
 
 if __name__ == '__main__':
+    try:
+        from test import test_support
+    except ImportError:
+        from test import support as test_support
+
     test_support.run_unittest(SystemCronTestCase)
```

### Comparing `python-crontab-3.0.0/tests/test_usage.py` & `python-crontab-3.1.0/tests/test_usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,19 +24,14 @@
 import sys
 
 import unittest
 import crontab
 
 from datetime import date, time, datetime, timedelta
 
-try:
-    from test import test_support
-except ImportError:
-    from test import support as test_support
-
 crontab.LOG.setLevel(crontab.logging.ERROR)
 TEST_DIR = os.path.dirname(__file__)
 
 class DummyStdout(object):
     def write(self, text):
         pass
 
@@ -254,10 +249,15 @@
     def tearDown(self):
         for filename in self.filenames:
             if os.path.exists(filename):
                 os.unlink(filename)
 
 
 if __name__ == '__main__':
+    try:
+        from test import test_support
+    except ImportError:
+        from test import support as test_support
+
     test_support.run_unittest(
        UseTestCase,
     )
```

### Comparing `python-crontab-3.0.0/tests/test_utf8.py` & `python-crontab-3.1.0/tests/test_utf8.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,14 @@
 
 import os
 import sys
 
 import locale
 import unittest
 from crontab import CronTab
-try:
-    from test import test_support
-except ImportError:
-    from test import support as test_support
 
 TEST_DIR = os.path.dirname(__file__)
 
 content = """
 */4 * * * * ůțƒ_command # ůțƒ_comment
 """
 filename = os.path.join(TEST_DIR, 'data', 'output-ůțƒ-8.tab')
@@ -104,10 +100,15 @@
             os.unlink(filename + '.in')
 
         cron.write(filename + '.out')
         if os.path.isfile(filename + '.out'):
             os.unlink(filename + '.out')
 
 if __name__ == '__main__':
+    try:
+        from test import test_support
+    except ImportError:
+        from test import support as test_support
+
     test_support.run_unittest(
        Utf8TestCase,
     )
```

### Comparing `python-crontab-3.0.0/tests/utils.py` & `python-crontab-3.1.0/tests/utils.py`

 * *Files identical despite different names*

