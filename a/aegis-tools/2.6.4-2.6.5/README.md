# Comparing `tmp/aegis-tools-2.6.4.tar.gz` & `tmp/aegis-tools-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aegis-tools-2.6.4.tar", last modified: Wed May 15 02:29:26 2024, max compression
+gzip compressed data, was "aegis-tools-2.6.5.tar", last modified: Wed May 22 01:29:20 2024, max compression
```

## Comparing `aegis-tools-2.6.4.tar` & `aegis-tools-2.6.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-15 02:29:26.555724 aegis-tools-2.6.4/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/LICENSE
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/MANIFEST.in
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-05-15 02:29:26.555724 aegis-tools-2.6.4/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/README.md
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-15 02:29:26.539724 aegis-tools-2.6.4/aegis/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/aegis/__init__.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    20802 2024-04-30 00:13:47.000000 aegis-tools-2.6.4/aegis/aegis_.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    19087 2024-04-30 00:19:28.000000 aegis-tools-2.6.4/aegis/build.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2831 2024-02-09 21:33:25.000000 aegis-tools-2.6.4/aegis/config.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    26399 2024-05-15 02:29:17.000000 aegis-tools-2.6.4/aegis/database.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    27302 2024-04-22 18:29:41.000000 aegis-tools-2.6.4/aegis/hydra.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     7559 2023-05-24 02:47:45.000000 aegis-tools-2.6.4/aegis/mailer.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    46365 2024-05-15 02:29:17.000000 aegis-tools-2.6.4/aegis/model.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-15 02:29:26.547724 aegis-tools-2.6.4/aegis/sql/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.6.4/aegis/sql/auditing-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4611 2024-01-31 22:04:42.000000 aegis-tools-2.6.4/aegis/sql/auditing-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/aegis/sql/build-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.6.4/aegis/sql/build-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/aegis/sql/cache_system.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.6.4/aegis/sql/email_system-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-05-22 20:40:27.000000 aegis-tools-2.6.4/aegis/sql/google_signin.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/aegis/sql/hydra-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/aegis/sql/hydra-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/aegis/sql/member_auth.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/aegis/sql/monitor-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/aegis/sql/reports.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    37012 2024-04-18 02:54:56.000000 aegis-tools-2.6.4/aegis/stdlib.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-15 02:29:26.551725 aegis-tools-2.6.4/aegis/templates/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3071 2023-09-30 03:49:20.000000 aegis-tools-2.6.4/aegis/templates/build.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.6.4/aegis/templates/build_confirm.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.6.4/aegis/templates/build_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.6.4/aegis/templates/build_view.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/aegis/templates/error_message.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3377 2023-08-14 03:31:20.000000 aegis-tools-2.6.4/aegis/templates/frame.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2238 2023-09-30 03:49:39.000000 aegis-tools-2.6.4/aegis/templates/hydra.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.6.4/aegis/templates/hydra_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1857 2023-09-30 03:52:25.000000 aegis-tools-2.6.4/aegis/templates/hydra_queue.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.6.4/aegis/templates/index.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.6.4/aegis/templates/report.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.6.4/aegis/templates/report_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.6.4/aegis/templates/reports.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.6.4/aegis/templates/w3.css
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/aegis/threadpool.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    78528 2024-04-30 00:13:28.000000 aegis-tools-2.6.4/aegis/webapp.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-15 02:29:26.555724 aegis-tools-2.6.4/aegis_tools.egg-info/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-05-15 02:29:26.000000 aegis-tools-2.6.4/aegis_tools.egg-info/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2024-05-15 02:29:26.000000 aegis-tools-2.6.4/aegis_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2024-05-15 02:29:26.000000 aegis-tools-2.6.4/aegis_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2024-05-15 02:29:26.000000 aegis-tools-2.6.4/aegis_tools.egg-info/entry_points.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2024-05-15 02:29:26.000000 aegis-tools-2.6.4/aegis_tools.egg-info/requires.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2024-05-15 02:29:26.000000 aegis-tools-2.6.4/aegis_tools.egg-info/top_level.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2024-05-15 02:29:26.555724 aegis-tools-2.6.4/setup.cfg
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1716 2023-09-26 15:24:50.000000 aegis-tools-2.6.4/setup.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-22 01:29:20.623621 aegis-tools-2.6.5/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.6.5/LICENSE
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.6.5/MANIFEST.in
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-05-22 01:29:20.619621 aegis-tools-2.6.5/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.6.5/README.md
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-22 01:29:20.611621 aegis-tools-2.6.5/aegis/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.6.5/aegis/__init__.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    20802 2024-04-30 00:13:47.000000 aegis-tools-2.6.5/aegis/aegis_.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    19087 2024-04-30 00:19:28.000000 aegis-tools-2.6.5/aegis/build.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2831 2024-02-09 21:33:25.000000 aegis-tools-2.6.5/aegis/config.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    26500 2024-05-22 01:29:04.000000 aegis-tools-2.6.5/aegis/database.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    27302 2024-04-22 18:29:41.000000 aegis-tools-2.6.5/aegis/hydra.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     7559 2023-05-24 02:47:45.000000 aegis-tools-2.6.5/aegis/mailer.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    46365 2024-05-15 02:29:17.000000 aegis-tools-2.6.5/aegis/model.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-22 01:29:20.615620 aegis-tools-2.6.5/aegis/sql/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.6.5/aegis/sql/auditing-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4611 2024-01-31 22:04:42.000000 aegis-tools-2.6.5/aegis/sql/auditing-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.6.5/aegis/sql/build-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.6.5/aegis/sql/build-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.6.5/aegis/sql/cache_system.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.6.5/aegis/sql/email_system-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-05-22 20:40:27.000000 aegis-tools-2.6.5/aegis/sql/google_signin.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.6.5/aegis/sql/hydra-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.6.5/aegis/sql/hydra-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.6.5/aegis/sql/member_auth.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.6.5/aegis/sql/monitor-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.6.5/aegis/sql/reports.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    37012 2024-04-18 02:54:56.000000 aegis-tools-2.6.5/aegis/stdlib.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-22 01:29:20.619621 aegis-tools-2.6.5/aegis/templates/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3071 2023-09-30 03:49:20.000000 aegis-tools-2.6.5/aegis/templates/build.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.6.5/aegis/templates/build_confirm.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.6.5/aegis/templates/build_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.6.5/aegis/templates/build_view.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.6.5/aegis/templates/error_message.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3377 2023-08-14 03:31:20.000000 aegis-tools-2.6.5/aegis/templates/frame.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2238 2023-09-30 03:49:39.000000 aegis-tools-2.6.5/aegis/templates/hydra.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.6.5/aegis/templates/hydra_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1857 2023-09-30 03:52:25.000000 aegis-tools-2.6.5/aegis/templates/hydra_queue.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.6.5/aegis/templates/index.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.6.5/aegis/templates/report.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.6.5/aegis/templates/report_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.6.5/aegis/templates/reports.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.6.5/aegis/templates/w3.css
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.6.5/aegis/threadpool.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    78528 2024-04-30 00:13:28.000000 aegis-tools-2.6.5/aegis/webapp.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-22 01:29:20.619621 aegis-tools-2.6.5/aegis_tools.egg-info/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-05-22 01:29:20.000000 aegis-tools-2.6.5/aegis_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2024-05-22 01:29:20.000000 aegis-tools-2.6.5/aegis_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2024-05-22 01:29:20.000000 aegis-tools-2.6.5/aegis_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2024-05-22 01:29:20.000000 aegis-tools-2.6.5/aegis_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2024-05-22 01:29:20.000000 aegis-tools-2.6.5/aegis_tools.egg-info/requires.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2024-05-22 01:29:20.000000 aegis-tools-2.6.5/aegis_tools.egg-info/top_level.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2024-05-22 01:29:20.623621 aegis-tools-2.6.5/setup.cfg
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1716 2023-09-26 15:24:50.000000 aegis-tools-2.6.5/setup.py
```

### Comparing `aegis-tools-2.6.4/LICENSE` & `aegis-tools-2.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/PKG-INFO` & `aegis-tools-2.6.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.6.4
+Version: 2.6.5
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.6.4/README.md` & `aegis-tools-2.6.5/README.md`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/aegis_.py` & `aegis-tools-2.6.5/aegis/aegis_.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/build.py` & `aegis-tools-2.6.5/aegis/build.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/config.py` & `aegis-tools-2.6.5/aegis/config.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/database.py` & `aegis-tools-2.6.5/aegis/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -501,14 +501,15 @@
                 # 1213: 'Deadlock found when trying to get lock; try restarting transaction'
                 retry_errors = (1205, 1213)
                 if hasattr(ex, 'args') and ex.args[0] in retry_errors:
                     logging.warning("Deadlock found or Lock wait timeout exceeded. Restarting transaction")
                     max_tries += 1
                     continue
                 logging.error("OperationalError with MySQL on %s. Close connection and raise.", self.hostname)
+                logging.error("Query Was: %s", query)
                 logging.exception(ex)
                 self.close()
                 raise
 
 
 # To support inserting something literally, like NOW(), into mini-ORM below
 class Literal(str):
@@ -626,20 +627,22 @@
         return dbconn.execute(sql, *args)
 
     @classmethod
     def update_columns(cls, columns, where, dbconn=None):
         dbconn = dbconn if dbconn else db()
         if not columns:
             logging.debug('Nothing to update. Skipping query')
-            return
+            return 0
         db_table = cls._table_name()
         # Filter out anything that's not in optional, pre-specified list of data columns
         data_columns = hasattr(cls, 'data_columns') and cls.data_columns
         if data_columns:
             columns = dict( [ (key,val) for key, val in columns.items() if key in data_columns] )
+        if not columns:
+            return 0
         # SET clause
         keys, values, args = cls.kva_split(columns)
         set_clause = ', '.join(['%s=%s' % (key, value) for key, value in zip(keys, values)])
         # WHERE clause
         keys, values, args2 = cls.kva_split(where)
         args += args2
         where_clause = ' AND '.join(['%s=%s' % (key, value) for key, value in zip(keys, values)])
```

### Comparing `aegis-tools-2.6.4/aegis/hydra.py` & `aegis-tools-2.6.5/aegis/hydra.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/mailer.py` & `aegis-tools-2.6.5/aegis/mailer.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/model.py` & `aegis-tools-2.6.5/aegis/model.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/sql/auditing-mysql.sql` & `aegis-tools-2.6.5/aegis/sql/auditing-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/sql/auditing-pgsql.sql` & `aegis-tools-2.6.5/aegis/sql/auditing-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/sql/build-mysql.sql` & `aegis-tools-2.6.5/aegis/sql/build-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/sql/build-pgsql.sql` & `aegis-tools-2.6.5/aegis/sql/build-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/sql/email_system-pgsql.sql` & `aegis-tools-2.6.5/aegis/sql/email_system-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/sql/google_signin.sql` & `aegis-tools-2.6.5/aegis/sql/google_signin.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/sql/hydra-mysql.sql` & `aegis-tools-2.6.5/aegis/sql/hydra-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/sql/hydra-pgsql.sql` & `aegis-tools-2.6.5/aegis/sql/hydra-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/sql/member_auth.sql` & `aegis-tools-2.6.5/aegis/sql/member_auth.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/sql/monitor-mysql.sql` & `aegis-tools-2.6.5/aegis/sql/monitor-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/sql/reports.sql` & `aegis-tools-2.6.5/aegis/sql/reports.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/stdlib.py` & `aegis-tools-2.6.5/aegis/stdlib.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/templates/build.html` & `aegis-tools-2.6.5/aegis/templates/build.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/templates/build_confirm.html` & `aegis-tools-2.6.5/aegis/templates/build_confirm.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/templates/build_form.html` & `aegis-tools-2.6.5/aegis/templates/build_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/templates/build_view.html` & `aegis-tools-2.6.5/aegis/templates/build_view.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/templates/frame.html` & `aegis-tools-2.6.5/aegis/templates/frame.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/templates/hydra.html` & `aegis-tools-2.6.5/aegis/templates/hydra.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/templates/hydra_form.html` & `aegis-tools-2.6.5/aegis/templates/hydra_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/templates/hydra_queue.html` & `aegis-tools-2.6.5/aegis/templates/hydra_queue.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/templates/report.html` & `aegis-tools-2.6.5/aegis/templates/report.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/templates/report_form.html` & `aegis-tools-2.6.5/aegis/templates/report_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/templates/reports.html` & `aegis-tools-2.6.5/aegis/templates/reports.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/templates/w3.css` & `aegis-tools-2.6.5/aegis/templates/w3.css`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/threadpool.py` & `aegis-tools-2.6.5/aegis/threadpool.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis/webapp.py` & `aegis-tools-2.6.5/aegis/webapp.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/aegis_tools.egg-info/PKG-INFO` & `aegis-tools-2.6.5/aegis_tools.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.6.4
+Version: 2.6.5
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.6.4/aegis_tools.egg-info/SOURCES.txt` & `aegis-tools-2.6.5/aegis_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.4/setup.py` & `aegis-tools-2.6.5/setup.py`

 * *Files identical despite different names*

