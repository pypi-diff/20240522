# Comparing `tmp/liveramp_automation-1.4.3.tar.gz` & `tmp/liveramp_automation-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation-1.4.3.tar", last modified: Fri May 17 02:32:53 2024, max compression
+gzip compressed data, was "liveramp_automation-1.4.4.tar", last modified: Wed May 22 05:54:13 2024, max compression
```

## Comparing `liveramp_automation-1.4.3.tar` & `liveramp_automation-1.4.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-17 02:32:53.495974 liveramp_automation-1.4.3/
--rw-r--r--   0 jasqia     (503) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-1.4.3/LICENSE
--rw-r--r--   0 jasqia     (503) staff       (20)     2986 2024-05-17 02:32:53.495665 liveramp_automation-1.4.3/PKG-INFO
--rwxrwxrwx   0 jasqia     (503) staff       (20)     1744 2024-03-18 02:41:18.000000 liveramp_automation-1.4.3/README.md
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-17 02:32:53.483094 liveramp_automation-1.4.3/liveramp_automation/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-09-13 07:36:00.000000 liveramp_automation-1.4.3/liveramp_automation/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)      479 2024-05-17 02:32:51.000000 liveramp_automation-1.4.3/liveramp_automation/__version__.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-17 02:32:53.486480 liveramp_automation-1.4.3/liveramp_automation/helpers/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.4.3/liveramp_automation/helpers/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)    10820 2024-05-17 02:15:01.000000 liveramp_automation-1.4.3/liveramp_automation/helpers/bigquery.py
--rw-r--r--   0 jasqia     (503) staff       (20)     8134 2024-04-16 03:01:46.000000 liveramp_automation-1.4.3/liveramp_automation/helpers/bucket.py
--rw-r--r--   0 jasqia     (503) staff       (20)     7898 2024-03-28 09:52:13.000000 liveramp_automation-1.4.3/liveramp_automation/helpers/file.py
--rw-r--r--   0 jasqia     (503) staff       (20)     7369 2024-04-17 09:01:03.000000 liveramp_automation-1.4.3/liveramp_automation/helpers/fixture.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6184 2024-04-17 08:58:00.000000 liveramp_automation-1.4.3/liveramp_automation/helpers/login.py
--rw-r--r--   0 jasqia     (503) staff       (20)    10686 2024-04-17 08:09:25.000000 liveramp_automation-1.4.3/liveramp_automation/helpers/notification.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-17 02:32:53.490101 liveramp_automation-1.4.3/liveramp_automation/utils/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.4.3/liveramp_automation/utils/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1934 2024-04-01 03:10:38.000000 liveramp_automation-1.4.3/liveramp_automation/utils/allure.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6445 2024-03-01 06:50:54.000000 liveramp_automation-1.4.3/liveramp_automation/utils/log.py
--rw-r--r--   0 jasqia     (503) staff       (20)     5025 2024-04-17 09:04:21.000000 liveramp_automation-1.4.3/liveramp_automation/utils/pagerduty.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1728 2023-08-16 02:33:25.000000 liveramp_automation-1.4.3/liveramp_automation/utils/parsers.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4025 2023-09-13 03:08:07.000000 liveramp_automation-1.4.3/liveramp_automation/utils/playwright.py
--rw-r--r--   0 jasqia     (503) staff       (20)    10164 2023-12-01 07:13:44.000000 liveramp_automation-1.4.3/liveramp_automation/utils/request.py
--rw-r--r--   0 jasqia     (503) staff       (20)    49909 2023-12-11 09:06:44.000000 liveramp_automation-1.4.3/liveramp_automation/utils/selenium.py
--rw-r--r--   0 jasqia     (503) staff       (20)    10500 2024-03-05 09:08:06.000000 liveramp_automation-1.4.3/liveramp_automation/utils/slack.py
--rw-r--r--   0 jasqia     (503) staff       (20)      795 2024-04-23 06:11:59.000000 liveramp_automation-1.4.3/liveramp_automation/utils/steps.py
--rw-r--r--   0 jasqia     (503) staff       (20)     8423 2024-04-23 05:42:40.000000 liveramp_automation-1.4.3/liveramp_automation/utils/testrail.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1660 2023-12-11 09:11:45.000000 liveramp_automation-1.4.3/liveramp_automation/utils/time.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-17 02:32:53.495143 liveramp_automation-1.4.3/liveramp_automation.egg-info/
--rw-r--r--   0 jasqia     (503) staff       (20)     2986 2024-05-17 02:32:53.000000 liveramp_automation-1.4.3/liveramp_automation.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (503) staff       (20)     1608 2024-05-17 02:32:53.000000 liveramp_automation-1.4.3/liveramp_automation.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (503) staff       (20)        1 2024-05-17 02:32:53.000000 liveramp_automation-1.4.3/liveramp_automation.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (503) staff       (20)      460 2024-05-17 02:32:53.000000 liveramp_automation-1.4.3/liveramp_automation.egg-info/requires.txt
--rw-r--r--   0 jasqia     (503) staff       (20)       26 2024-05-17 02:32:53.000000 liveramp_automation-1.4.3/liveramp_automation.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (503) staff       (20)       38 2024-05-17 02:32:53.496033 liveramp_automation-1.4.3/setup.cfg
--rw-r--r--   0 jasqia     (503) staff       (20)     1502 2024-05-17 02:32:43.000000 liveramp_automation-1.4.3/setup.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-17 02:32:53.490334 liveramp_automation-1.4.3/tests/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.4.3/tests/__init__.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-17 02:32:53.492072 liveramp_automation-1.4.3/tests/test_helpers/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-1.4.3/tests/test_helpers/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4384 2024-05-14 09:08:10.000000 liveramp_automation-1.4.3/tests/test_helpers/test_bigquery.py
--rw-r--r--   0 jasqia     (503) staff       (20)     2347 2024-05-14 05:26:06.000000 liveramp_automation-1.4.3/tests/test_helpers/test_bucket.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4132 2024-04-01 03:42:11.000000 liveramp_automation-1.4.3/tests/test_helpers/test_file.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1247 2024-03-14 08:05:22.000000 liveramp_automation-1.4.3/tests/test_helpers/test_fixtures.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1676 2024-03-14 09:32:27.000000 liveramp_automation-1.4.3/tests/test_helpers/test_login.py
--rw-r--r--   0 jasqia     (503) staff       (20)     3508 2024-03-05 09:08:06.000000 liveramp_automation-1.4.3/tests/test_helpers/test_notification.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-17 02:32:53.494665 liveramp_automation-1.4.3/tests/test_utils/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.4.3/tests/test_utils/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1832 2024-03-28 09:52:13.000000 liveramp_automation-1.4.3/tests/test_utils/test_log.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4783 2024-03-28 09:52:13.000000 liveramp_automation-1.4.3/tests/test_utils/test_pagerduty.py
--rw-r--r--   0 jasqia     (503) staff       (20)     3324 2024-05-10 03:07:09.000000 liveramp_automation-1.4.3/tests/test_utils/test_parsers.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1014 2024-03-14 08:40:57.000000 liveramp_automation-1.4.3/tests/test_utils/test_playwright.py
--rw-r--r--   0 jasqia     (503) staff       (20)    13489 2024-04-01 03:10:38.000000 liveramp_automation-1.4.3/tests/test_utils/test_request.py
--rw-r--r--   0 jasqia     (503) staff       (20)    39767 2024-03-28 09:52:13.000000 liveramp_automation-1.4.3/tests/test_utils/test_selenium.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6615 2024-03-28 09:52:13.000000 liveramp_automation-1.4.3/tests/test_utils/test_slack.py
--rw-r--r--   0 jasqia     (503) staff       (20)     5406 2024-05-10 03:16:07.000000 liveramp_automation-1.4.3/tests/test_utils/test_testrail.py
--rw-r--r--   0 jasqia     (503) staff       (20)      742 2024-03-14 08:51:35.000000 liveramp_automation-1.4.3/tests/test_utils/test_version.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-22 05:54:13.594927 liveramp_automation-1.4.4/
+-rw-r--r--   0 jasqia     (503) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-1.4.4/LICENSE
+-rw-r--r--   0 jasqia     (503) staff       (20)     2986 2024-05-22 05:54:13.594583 liveramp_automation-1.4.4/PKG-INFO
+-rwxrwxrwx   0 jasqia     (503) staff       (20)     1744 2024-03-18 02:41:18.000000 liveramp_automation-1.4.4/README.md
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-22 05:54:13.576980 liveramp_automation-1.4.4/liveramp_automation/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-09-13 07:36:00.000000 liveramp_automation-1.4.4/liveramp_automation/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)      479 2024-05-22 05:53:51.000000 liveramp_automation-1.4.4/liveramp_automation/__version__.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-22 05:54:13.581108 liveramp_automation-1.4.4/liveramp_automation/helpers/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.4.4/liveramp_automation/helpers/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10820 2024-05-17 02:15:01.000000 liveramp_automation-1.4.4/liveramp_automation/helpers/bigquery.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     8134 2024-04-16 03:01:46.000000 liveramp_automation-1.4.4/liveramp_automation/helpers/bucket.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     7898 2024-03-28 09:52:13.000000 liveramp_automation-1.4.4/liveramp_automation/helpers/file.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     7369 2024-04-17 09:01:03.000000 liveramp_automation-1.4.4/liveramp_automation/helpers/fixture.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6184 2024-04-17 08:58:00.000000 liveramp_automation-1.4.4/liveramp_automation/helpers/login.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10686 2024-04-17 08:09:25.000000 liveramp_automation-1.4.4/liveramp_automation/helpers/notification.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-22 05:54:13.586100 liveramp_automation-1.4.4/liveramp_automation/utils/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.4.4/liveramp_automation/utils/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1934 2024-04-01 03:10:38.000000 liveramp_automation-1.4.4/liveramp_automation/utils/allure.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6445 2024-03-01 06:50:54.000000 liveramp_automation-1.4.4/liveramp_automation/utils/log.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     5025 2024-04-17 09:04:21.000000 liveramp_automation-1.4.4/liveramp_automation/utils/pagerduty.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1728 2023-08-16 02:33:25.000000 liveramp_automation-1.4.4/liveramp_automation/utils/parsers.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4025 2023-09-13 03:08:07.000000 liveramp_automation-1.4.4/liveramp_automation/utils/playwright.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    11696 2024-05-22 05:53:51.000000 liveramp_automation-1.4.4/liveramp_automation/utils/request.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    49909 2023-12-11 09:06:44.000000 liveramp_automation-1.4.4/liveramp_automation/utils/selenium.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10500 2024-03-05 09:08:06.000000 liveramp_automation-1.4.4/liveramp_automation/utils/slack.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     5578 2024-05-22 05:53:51.000000 liveramp_automation-1.4.4/liveramp_automation/utils/steps.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     8423 2024-04-23 05:42:40.000000 liveramp_automation-1.4.4/liveramp_automation/utils/testrail.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1660 2023-12-11 09:11:45.000000 liveramp_automation-1.4.4/liveramp_automation/utils/time.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-22 05:54:13.593997 liveramp_automation-1.4.4/liveramp_automation.egg-info/
+-rw-r--r--   0 jasqia     (503) staff       (20)     2986 2024-05-22 05:54:13.000000 liveramp_automation-1.4.4/liveramp_automation.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (503) staff       (20)     1608 2024-05-22 05:54:13.000000 liveramp_automation-1.4.4/liveramp_automation.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)        1 2024-05-22 05:54:13.000000 liveramp_automation-1.4.4/liveramp_automation.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)      460 2024-05-22 05:54:13.000000 liveramp_automation-1.4.4/liveramp_automation.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)       26 2024-05-22 05:54:13.000000 liveramp_automation-1.4.4/liveramp_automation.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)       38 2024-05-22 05:54:13.594980 liveramp_automation-1.4.4/setup.cfg
+-rw-r--r--   0 jasqia     (503) staff       (20)     1502 2024-05-17 02:32:43.000000 liveramp_automation-1.4.4/setup.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-22 05:54:13.586555 liveramp_automation-1.4.4/tests/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.4.4/tests/__init__.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-22 05:54:13.589086 liveramp_automation-1.4.4/tests/test_helpers/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-1.4.4/tests/test_helpers/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4384 2024-05-14 09:08:10.000000 liveramp_automation-1.4.4/tests/test_helpers/test_bigquery.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     2347 2024-05-14 05:26:06.000000 liveramp_automation-1.4.4/tests/test_helpers/test_bucket.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4132 2024-04-01 03:42:11.000000 liveramp_automation-1.4.4/tests/test_helpers/test_file.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1247 2024-03-14 08:05:22.000000 liveramp_automation-1.4.4/tests/test_helpers/test_fixtures.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1676 2024-03-14 09:32:27.000000 liveramp_automation-1.4.4/tests/test_helpers/test_login.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     3508 2024-03-05 09:08:06.000000 liveramp_automation-1.4.4/tests/test_helpers/test_notification.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-22 05:54:13.593231 liveramp_automation-1.4.4/tests/test_utils/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.4.4/tests/test_utils/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1832 2024-03-28 09:52:13.000000 liveramp_automation-1.4.4/tests/test_utils/test_log.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4783 2024-03-28 09:52:13.000000 liveramp_automation-1.4.4/tests/test_utils/test_pagerduty.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     3324 2024-05-10 03:07:09.000000 liveramp_automation-1.4.4/tests/test_utils/test_parsers.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1014 2024-03-14 08:40:57.000000 liveramp_automation-1.4.4/tests/test_utils/test_playwright.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    13489 2024-04-01 03:10:38.000000 liveramp_automation-1.4.4/tests/test_utils/test_request.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    39767 2024-03-28 09:52:13.000000 liveramp_automation-1.4.4/tests/test_utils/test_selenium.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6615 2024-03-28 09:52:13.000000 liveramp_automation-1.4.4/tests/test_utils/test_slack.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     5406 2024-05-10 03:16:07.000000 liveramp_automation-1.4.4/tests/test_utils/test_testrail.py
+-rw-r--r--   0 jasqia     (503) staff       (20)      742 2024-03-14 08:51:35.000000 liveramp_automation-1.4.4/tests/test_utils/test_version.py
```

### Comparing `liveramp_automation-1.4.3/LICENSE` & `liveramp_automation-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/PKG-INFO` & `liveramp_automation-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp_automation
-Version: 1.4.3
+Version: 1.4.4
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: allure-pytest-bdd
```

### Comparing `liveramp_automation-1.4.3/README.md` & `liveramp_automation-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/liveramp_automation/helpers/bigquery.py` & `liveramp_automation-1.4.4/liveramp_automation/helpers/bigquery.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/liveramp_automation/helpers/bucket.py` & `liveramp_automation-1.4.4/liveramp_automation/helpers/bucket.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/liveramp_automation/helpers/file.py` & `liveramp_automation-1.4.4/liveramp_automation/helpers/file.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/liveramp_automation/helpers/fixture.py` & `liveramp_automation-1.4.4/liveramp_automation/helpers/fixture.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/liveramp_automation/helpers/login.py` & `liveramp_automation-1.4.4/liveramp_automation/helpers/login.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/liveramp_automation/helpers/notification.py` & `liveramp_automation-1.4.4/liveramp_automation/helpers/notification.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/liveramp_automation/utils/allure.py` & `liveramp_automation-1.4.4/liveramp_automation/utils/allure.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/liveramp_automation/utils/log.py` & `liveramp_automation-1.4.4/liveramp_automation/utils/log.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/liveramp_automation/utils/pagerduty.py` & `liveramp_automation-1.4.4/liveramp_automation/utils/pagerduty.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/liveramp_automation/utils/parsers.py` & `liveramp_automation-1.4.4/liveramp_automation/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/liveramp_automation/utils/playwright.py` & `liveramp_automation-1.4.4/liveramp_automation/utils/playwright.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/liveramp_automation/utils/request.py` & `liveramp_automation-1.4.4/liveramp_automation/utils/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,7 +233,42 @@
     except requests.exceptions.Timeout as error:
         Logger.info("Request timed out {}".format(error))
         allure_attach_text("Request Timed Out:", str(error))
     except requests.exceptions.RequestException as error:
         Logger.info("An error occurred {}".format(error))
         allure_attach_text("An Error Occurred", str(error))
     return response
+
+
+def request_any(method, url, headers, data=None, json=None, **kwargs):
+    """Sends an any type request.
+
+    :param url: URL for the request.
+    :param headers: Headers for the request.
+    :param data: Data for the request body.
+    :param json: JSON for the request body.
+    :param kwargs: Additional arguments for the request.
+    :return: Response object.
+    """
+    Logger.info("Sending an any type request to {}".format(url))
+    allure_attach_text("Sending an any type request to:", url)
+    response = None
+    if data:
+        Logger.info("Request data: {}".format(data))
+        allure_attach_text("Request Data:", data)
+    if json:
+        Logger.info("Request JSON: {}".format(json))
+        allure_attach_json("Request JSON:", json)
+    try:
+        response = requests.request(method, url=url, data=data, json=json, headers=headers, **kwargs)
+        Logger.info("Response content: {}".format(response.text))
+        allure_attach_text("Response content:", response.text)
+    except requests.exceptions.HTTPError as error:
+        Logger.info("HTTP error occurred {}".format(error))
+        allure_attach_text("HTTP Error Exception:", str(error))
+    except requests.exceptions.Timeout as error:
+        Logger.info("Request timed out {}".format(error))
+        allure_attach_text("Request Timed Out:", str(error))
+    except requests.exceptions.RequestException as error:
+        Logger.info("An error occurred {}".format(error))
+        allure_attach_text("An Error Occurred", str(error))
+    return response
```

### Comparing `liveramp_automation-1.4.3/liveramp_automation/utils/selenium.py` & `liveramp_automation-1.4.4/liveramp_automation/utils/selenium.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/liveramp_automation/utils/slack.py` & `liveramp_automation-1.4.4/liveramp_automation/utils/slack.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/liveramp_automation/utils/testrail.py` & `liveramp_automation-1.4.4/liveramp_automation/utils/testrail.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/liveramp_automation/utils/time.py` & `liveramp_automation-1.4.4/liveramp_automation/utils/time.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/liveramp_automation.egg-info/PKG-INFO` & `liveramp_automation-1.4.4/liveramp_automation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp-automation
-Version: 1.4.3
+Version: 1.4.4
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: allure-pytest-bdd
```

### Comparing `liveramp_automation-1.4.3/liveramp_automation.egg-info/SOURCES.txt` & `liveramp_automation-1.4.4/liveramp_automation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/setup.py` & `liveramp_automation-1.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/tests/test_helpers/test_bigquery.py` & `liveramp_automation-1.4.4/tests/test_helpers/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/tests/test_helpers/test_bucket.py` & `liveramp_automation-1.4.4/tests/test_helpers/test_bucket.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/tests/test_helpers/test_file.py` & `liveramp_automation-1.4.4/tests/test_helpers/test_file.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/tests/test_helpers/test_fixtures.py` & `liveramp_automation-1.4.4/tests/test_helpers/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/tests/test_helpers/test_login.py` & `liveramp_automation-1.4.4/tests/test_helpers/test_login.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/tests/test_helpers/test_notification.py` & `liveramp_automation-1.4.4/tests/test_helpers/test_notification.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/tests/test_utils/test_log.py` & `liveramp_automation-1.4.4/tests/test_utils/test_log.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/tests/test_utils/test_pagerduty.py` & `liveramp_automation-1.4.4/tests/test_utils/test_pagerduty.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/tests/test_utils/test_parsers.py` & `liveramp_automation-1.4.4/tests/test_utils/test_parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/tests/test_utils/test_playwright.py` & `liveramp_automation-1.4.4/tests/test_utils/test_playwright.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/tests/test_utils/test_request.py` & `liveramp_automation-1.4.4/tests/test_utils/test_request.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/tests/test_utils/test_selenium.py` & `liveramp_automation-1.4.4/tests/test_utils/test_selenium.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/tests/test_utils/test_slack.py` & `liveramp_automation-1.4.4/tests/test_utils/test_slack.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/tests/test_utils/test_testrail.py` & `liveramp_automation-1.4.4/tests/test_utils/test_testrail.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.3/tests/test_utils/test_version.py` & `liveramp_automation-1.4.4/tests/test_utils/test_version.py`

 * *Files identical despite different names*

