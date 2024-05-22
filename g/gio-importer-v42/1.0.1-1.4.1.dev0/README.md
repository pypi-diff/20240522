# Comparing `tmp/gio_importer_v42-1.0.1.tar.gz` & `tmp/gio_importer_v42-1.4.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gio_importer_v42-1.0.1.tar", last modified: Tue Jan 30 08:24:26 2024, max compression
+gzip compressed data, was "gio_importer_v42-1.4.1.dev0.tar", last modified: Wed May 22 07:16:00 2024, max compression
```

## Comparing `gio_importer_v42-1.0.1.tar` & `gio_importer_v42-1.4.1.dev0.tar`

### file list

```diff
@@ -1,58 +1,49 @@
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-01-30 08:24:26.317537 gio_importer_v42-1.0.1/
--rw-r--r--   0 chengcheng   (501) staff       (20)     1061 2024-01-26 06:36:14.000000 gio_importer_v42-1.0.1/LICENSE
--rw-r--r--   0 chengcheng   (501) staff       (20)       71 2024-01-26 06:36:14.000000 gio_importer_v42-1.0.1/MANIFEST.in
--rw-r--r--   0 chengcheng   (501) staff       (20)    12105 2024-01-30 08:24:26.317226 gio_importer_v42-1.0.1/PKG-INFO
--rw-r--r--   0 chengcheng   (501) staff       (20)      792 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/README.md
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-01-30 08:24:26.291606 gio_importer_v42-1.0.1/gio_importer_v42.egg-info/
--rw-r--r--   0 chengcheng   (501) staff       (20)    12105 2024-01-30 08:24:26.000000 gio_importer_v42-1.0.1/gio_importer_v42.egg-info/PKG-INFO
--rw-r--r--   0 chengcheng   (501) staff       (20)     1371 2024-01-30 08:24:26.000000 gio_importer_v42-1.0.1/gio_importer_v42.egg-info/SOURCES.txt
--rw-r--r--   0 chengcheng   (501) staff       (20)        1 2024-01-30 08:24:26.000000 gio_importer_v42-1.0.1/gio_importer_v42.egg-info/dependency_links.txt
--rw-r--r--   0 chengcheng   (501) staff       (20)      197 2024-01-30 08:24:26.000000 gio_importer_v42-1.0.1/gio_importer_v42.egg-info/entry_points.txt
--rw-r--r--   0 chengcheng   (501) staff       (20)       84 2024-01-30 08:24:26.000000 gio_importer_v42-1.0.1/gio_importer_v42.egg-info/requires.txt
--rw-r--r--   0 chengcheng   (501) staff       (20)       10 2024-01-30 08:24:26.000000 gio_importer_v42-1.0.1/gio_importer_v42.egg-info/top_level.txt
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-01-30 08:24:26.302799 gio_importer_v42-1.0.1/importers/
--rw-r--r--   0 chengcheng   (501) staff       (20)    11711 2024-01-30 08:23:54.000000 gio_importer_v42-1.0.1/importers/README.md
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/__init__.py
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-01-30 08:24:26.304971 gio_importer_v42-1.0.1/importers/clear_data/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/clear_data/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     2817 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/clear_data/clear_data.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     1649 2024-01-30 08:19:26.000000 gio_importer_v42-1.0.1/importers/clear_user.py
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-01-30 08:24:26.309868 gio_importer_v42-1.0.1/importers/common/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/common/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     5584 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/common/common_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     2425 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/common/config_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     2549 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/common/http_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)      881 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/common/log_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)      731 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/conf.cfg
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-01-30 08:24:26.312738 gio_importer_v42-1.0.1/importers/data_import/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/data_import/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    25273 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/data_import/data_events.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     2865 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/data_import/data_format_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    15889 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/data_import/data_item_variable.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     5129 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/data_import/data_model.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    13122 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/data_import/data_user_variable.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     6663 2024-01-30 08:19:26.000000 gio_importer_v42-1.0.1/importers/data_importer.py
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-01-30 08:24:26.314301 gio_importer_v42-1.0.1/importers/db_import/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/db_import/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     2517 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/db_import/database_import.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    13795 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/db_import/hive_import.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    13483 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/db_import/mysql_import.py
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-01-30 08:24:26.314774 gio_importer_v42-1.0.1/importers/example/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/example/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     5085 2024-01-30 08:19:26.000000 gio_importer_v42-1.0.1/importers/format_importer.py
--rw-r--r--   0 chengcheng   (501) staff       (20)      472 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/log_conf.yaml
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-01-30 08:24:26.316134 gio_importer_v42-1.0.1/importers/meta/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/meta/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    10698 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/meta/check_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     8101 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/meta/data_center.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    20486 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/meta/meta_create.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     3835 2024-01-30 08:20:54.000000 gio_importer_v42-1.0.1/importers/meta_importer.py
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-01-30 08:24:26.316879 gio_importer_v42-1.0.1/importers/saas_export/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/saas_export/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     3303 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/saas_export/saas_meta.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     1179 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/saas_export.py
--rw-r--r--   0 chengcheng   (501) staff       (20)      232 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/setup.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     1372 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/trigger_job.py
--rw-r--r--   0 chengcheng   (501) staff       (20)       95 2024-01-30 08:00:05.000000 gio_importer_v42-1.0.1/importers/zk.py
--rw-r--r--   0 chengcheng   (501) staff       (20)       38 2024-01-30 08:24:26.317599 gio_importer_v42-1.0.1/setup.cfg
--rw-r--r--   0 chengcheng   (501) staff       (20)     1256 2024-01-30 08:19:26.000000 gio_importer_v42-1.0.1/setup.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-05-22 07:16:00.873953 gio_importer_v42-1.4.1.dev0/
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1061 2024-01-26 06:36:14.000000 gio_importer_v42-1.4.1.dev0/LICENSE
+-rw-r--r--   0 chengcheng   (501) staff       (20)    11394 2024-05-22 07:16:00.873174 gio_importer_v42-1.4.1.dev0/PKG-INFO
+-rw-r--r--   0 chengcheng   (501) staff       (20)      792 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/README.md
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-05-22 07:16:00.829513 gio_importer_v42-1.4.1.dev0/gio_importer_v42.egg-info/
+-rw-r--r--   0 chengcheng   (501) staff       (20)    11394 2024-05-22 07:16:00.000000 gio_importer_v42-1.4.1.dev0/gio_importer_v42.egg-info/PKG-INFO
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1154 2024-05-22 07:16:00.000000 gio_importer_v42-1.4.1.dev0/gio_importer_v42.egg-info/SOURCES.txt
+-rw-r--r--   0 chengcheng   (501) staff       (20)        1 2024-05-22 07:16:00.000000 gio_importer_v42-1.4.1.dev0/gio_importer_v42.egg-info/dependency_links.txt
+-rw-r--r--   0 chengcheng   (501) staff       (20)      196 2024-05-22 07:16:00.000000 gio_importer_v42-1.4.1.dev0/gio_importer_v42.egg-info/entry_points.txt
+-rw-r--r--   0 chengcheng   (501) staff       (20)       84 2024-05-22 07:16:00.000000 gio_importer_v42-1.4.1.dev0/gio_importer_v42.egg-info/requires.txt
+-rw-r--r--   0 chengcheng   (501) staff       (20)       10 2024-05-22 07:16:00.000000 gio_importer_v42-1.4.1.dev0/gio_importer_v42.egg-info/top_level.txt
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-05-22 07:16:00.839692 gio_importer_v42-1.4.1.dev0/importers/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/__init__.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-05-22 07:16:00.843130 gio_importer_v42-1.4.1.dev0/importers/clear_data/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/clear_data/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     2817 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/clear_data/clear_data.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1328 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/clear_user.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-05-22 07:16:00.850659 gio_importer_v42-1.4.1.dev0/importers/common/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/common/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     5987 2024-05-22 06:15:45.000000 gio_importer_v42-1.4.1.dev0/importers/common/common_util.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     2425 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/common/config_util.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     2549 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/common/http_util.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)      881 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/common/log_util.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-05-22 07:16:00.863710 gio_importer_v42-1.4.1.dev0/importers/data_import/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/data_import/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    25273 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/data_import/data_events.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     2865 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/data_import/data_format_util.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    15889 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/data_import/data_item_variable.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     5129 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/data_import/data_model.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    13122 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/data_import/data_user_variable.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     5709 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/data_importer.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-05-22 07:16:00.864934 gio_importer_v42-1.4.1.dev0/importers/example/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/example/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     6036 2024-05-22 07:15:19.000000 gio_importer_v42-1.4.1.dev0/importers/format_importer.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-05-22 07:16:00.869826 gio_importer_v42-1.4.1.dev0/importers/meta/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/meta/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    10698 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/meta/check_util.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     8101 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/meta/data_center.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    20486 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/meta/meta_create.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     3521 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/meta_importer.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-05-22 07:16:00.872276 gio_importer_v42-1.4.1.dev0/importers/saas_export/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/saas_export/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     3303 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/saas_export/saas_meta.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1179 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/saas_export.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)      232 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/setup.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1372 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/trigger_job.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)       95 2024-05-16 08:51:02.000000 gio_importer_v42-1.4.1.dev0/importers/zk.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)       38 2024-05-22 07:16:00.874047 gio_importer_v42-1.4.1.dev0/setup.cfg
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1259 2024-05-22 07:08:11.000000 gio_importer_v42-1.4.1.dev0/setup.py
```

### Comparing `gio_importer_v42-1.0.1/LICENSE` & `gio_importer_v42-1.4.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `gio_importer_v42-1.0.1/PKG-INFO` & `gio_importer_v42-1.4.1.dev0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 Metadata-Version: 2.1
 Name: gio_importer_v42
-Version: 1.0.1
+Version: 1.4.1.dev0
 Summary: GrowingIO Importer是GrowingIO CDP平台元数据创建和数据导入工具
-Home-page: UNKNOWN
 Author: gio
 Author-email: dev-growing@startdt.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.8
+Classifier: Development Status :: 3 - Alpha
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pip
+Requires-Dist: numpy
+Requires-Dist: requests
+Requires-Dist: pandas
+Requires-Dist: curlify
+Requires-Dist: PyYAML
+Requires-Dist: psycopg2-binary
+Requires-Dist: pymysql
+Requires-Dist: pyhive
+Requires-Dist: thrift
+Requires-Dist: sasl
 
 # GrowingIO Importer
 
 GrowingIO Importer是GrowingIO CDP平台元数据创建和数据导入工具。
 
 ## 入门
 
 有关GrowingIO Importer请访问[GrowingIO官方文档](https://docs.growingio.com/op/developer-manual/toolbox/ )获取帮助。
 
 ## 环境依赖
 
-| | 4.2 |
-|----|-----|
-|Python| 3.8 |
+| |1.0|
+|----|----|
+|Python|3.6|
 
 ## 安装
 
-pip install gio-importer-v42
-
-## 环境参数
-    import importers
-    print(importers.__path__)
-
-    根据路径信息，进入包目录，修改conf.cfg(导入工具配置信息)
-    需要修改有关FTP，API信息(找负责项目运维提供FTP，API-uri相关信息)
-
+下载工具包GrowingIO Importer,在importer目录下执行脚本sh init.sh完成初始化
 
 ## 元数据导入
 
 目前支持如下：
 
 * 创建事件
 * 创建事件属性
@@ -49,364 +49,278 @@
 * 导出元数据
 * 导入元数据
 
 ### 使用说明
 
 #### 创建事件
 
-    from importers import meta_importer
-
-    params = {
-        'm': 'create_event',
-        'key': '<事件名>',
-        'name': '<事件显示名>',
-        'desc': '<事件描述>'
-    }
-
-    meta_importer.do_meta(params)
+    python3 meta_importer -m create_event \
+    --key <事件名> \
+    [-n <事件显示名>] \
+    [-d <事件描述>] \
 
 |参数|参数说明|
 |----|----|
 |-m|必选参数，项目名。|
-|--key|必选参数，事件名。仅允许大小写英文、数字、以及下划线，并且不能以数字开头，限长30字符|
-|--name|可选参数，事件显示名。默认同事件名，限长30字符|
-|--desc|可选参数，事件描述，默认为空。若描述中有空格则需要加双引号|
+|-k、--key|必选参数，事件名。仅允许大小写英文、数字、以及下划线，并且不能以数字开头，限长30字符|
+|-n、--name|可选参数，事件显示名。默认同事件名，限长30字符|
+|-d、--desc|可选参数，事件描述，默认为空。若描述中有空格则需要加双引号|
 
 #### 创建事件属性
 
-    from importers import meta_importer
-
-    params = {
-        'm': 'create_event_variables',
-        'key': '<事件属性名>',
-        'type': '<事件属性数据类型>',
-        'name': '<事件属性显示名>',
-        'desc': '<事件属性描述>'
-    }
-
-    meta_importer.do_meta(params)
+    python3 meta_importer.py -m create_event_variables \
+                             -k <事件名> \
+                             -t <事件属性数据类型> \
+                             [-n <事件显示名>] \
+                             [-d <事件属性描述>] \
 
 |参数|参数说明|
 |----|----|
 |-m|必选参数，项目名。|
-|--key|必选参数，事件名。仅允许大小写英文、数字、以及下划线，并且不能以数字开头，限长30字符|
-|--type|必选参数，事件属性数据类型。可选值：string/int/double
-|--name|可选参数，事件显示名。默认同事件名，限长30字符|
-|--desc|可选参数，事件描述，默认为空。若描述中有空格则需要加双引号|
+|-k、--key|必选参数，事件名。仅允许大小写英文、数字、以及下划线，并且不能以数字开头，限长30字符|
+|-t、--type|必选参数，事件属性数据类型。可选值：string/int/double
+|-n、--name|可选参数，事件显示名。默认同事件名，限长30字符|
+|-d、--desc|可选参数，事件描述，默认为空。若描述中有空格则需要加双引号|
 
 #### 创建用户属性
 
-    from importers import meta_importer
-
-    params = {
-        'm': 'create_user_variables',
-        'key': '<用户属性名>',
-        'type': '<用户属性数据类型>',
-        'name': '<用户属性显示名>',
-        'desc': '<用户属性描述>'
-    }
-
-    meta_importer.do_meta(params)
+    python3 meta_importer.py -m create_user_variables \
+                             -k <标识符> \
+                             -t <用户属性数据类型> \
+                             [-n <用户显示名>] \
+                             [-d <用户属性描述>] \
 
 |参数|参数说明|
 |----|----|
 |-m|必选参数，项目名。|
-|--key|必选参数，标识符。仅允许大小写英文、数字、以及下划线，并且不能以数字开头，限长30字符|
-|--type|必选参数，可选参数：string/int/date
-|--name|可选参数，用户显示名。默认同标识符，限长30字符|
-|--desc|可选参数，用户属性描述，默认为空。若描述中有空格则需要加双引号|
+|-k、--key|必选参数，标识符。仅允许大小写英文、数字、以及下划线，并且不能以数字开头，限长30字符|
+|-t、--type|必选参数，可选参数：string/int/date
+|-n、--name|可选参数，用户显示名。默认同标识符，限长30字符|
+|-d、--desc|可选参数，用户属性描述，默认为空。若描述中有空格则需要加双引号|
 
 #### 绑定事件与事件属性
 
     python3 meta_importer.py -m bind_event_variables \
                              -k <事件名> \
                              -a <绑定事件属性名> \
 
 |参数|参数说明|
 |----|----|
 |-m|必选参数，项目名。|
-|--key|必选参数，事件名。若事件不存在则创建，否则更新事件|
-|--attr|必选参数，绑定事件属性名。多个属性名使用英文逗号分隔(需加单引号或者在特殊符号前加上\)|
+|-k、--key|必选参数，事件名。若事件不存在则创建，否则更新事件|
+|-a、--attr|必选参数，绑定事件属性名。多个属性名使用英文逗号分隔(需加单引号或者在特殊符号前加上\)|
 
 #### 导出元数据
 
-    from importers import meta_importer
-
-    params = {
-        'm': 'bind_event_variables',
-        'key': '<事件名>',
-        'attr': '<绑定事件属性名集合>'
-    }
-
-    meta_importer.do_meta(params)
+    python3 meta_importer.py -m export_meta \
+                             -f <文件名> \
 
 |参数|参数说明|
 |----|----|
 |-m|必选参数，项目名。|
-|--file|必选参数，导出文件名|
+|-f、--file|必选参数，导出文件名|
 
 #### 导入元数据
 
-    from importers import meta_importer
-
-    params = {
-        'm': 'import_meta',
-        'file': '<文件名>'
-    }
-
-    meta_importer.do_meta(params)
+    python3 meta_importer.py -m import_meta \
+                             -f <文件名> \
 
 |参数|参数说明|
 |----|----|
 |-m|必选参数，项目名。|
-|--file|必选参数，导入文件名|
+|-f、--file|必选参数，导入文件名|
 
 ## 数据导入
 
 目前支持如下：
 
 * 用户属性数据导入
 * 用户行为数据导入
 
 ### 使用说明
 
 #### 用户属性数据导入
 
-    from importers import data_importer
-
-    params = {
-        'm': 'user_variables',
-        'path': '<文件路径>',
-        'datasource_id': '<数据源ID>',
-        'format': '[CSV|TSV|Json]',
-        'separator': ',',
-        'skip_header': 'True',
-        'attributes': 'userId,...'
-    }
-
-    data_importer.do_importer(params)
-
+    python3 data_importer.py -m  user_variables \
+                             -p  文件路径 \
+                             -ds 数据源ID \
+                             -f  [CSV|TSV|Json] \
+                             -d  [True|False] \
+                             -qf " \
+                             -sep , \
+                             -skh \
+                             -attr userId,...
 
 |参数|参数说明|
-|---|----|
+|----|----|
 |-m|必填参数. 用户属性数据导入-user_variables|
-|-path|必填参数. 需要导入的数据所在的路径|
-|-datasource_id|必填参数. 数据源ID|
-|-format|可选参数. 导入数据格式,目前支持JSON,CSV,TSV三种格式.默认值:JSON|
-|-qualifier|可选参数. CSV,TSV格式文本限定符.默认值:"|
-|-separator|可选参数. CSV,TSV格式文本分割符.默认值:,|
-|-skip_header|可选参数. CSV,TSV格式设置则自动跳过首行,此参数不需要设置值.|
-|-attributes|可选参数. CSV,TSV格式导入文件的各列按顺序映射到属性名，逗号分隔.userId必须指定(需加单引号或者在特殊符号前加上\)|
+|-p|必填参数. 需要导入的数据所在的路径|
+|-ds|必填参数. 数据源ID|
+|-f|可选参数. 导入数据格式,目前支持JSON,CSV,TSV三种格式.默认值:JSON|
+|-qf|可选参数. CSV,TSV格式文本限定符.默认值:"|
+|-sep|可选参数. CSV,TSV格式文本分割符.默认值:,|
+|-skh|可选参数. CSV,TSV格式设置则自动跳过首行,此参数不需要设置值.|
+|-attr|可选参数. CSV,TSV格式导入文件的各列按顺序映射到属性名，逗号分隔.userId必须指定(需加单引号或者在特殊符号前加上\)|
 
 #### 用户行为数据导入
 
-    from importers import data_importer
-
-    params = {
-        'm': 'events',
-        'path': '<文件路径>',
-        'datasource_id': '<数据源ID>',
-        'format': '[CSV|TSV|Json]',
-        'separator': ',',
-        'skip_header': 'True',
-        'attributes': 'userId,...,
-        'event_start': '<数据起始日期 YYYY-MM-DD>',
-        'event_end': '<数据结束日期 YYYY-MM-DD>'
-    }
-
-    data_importer.do_importer(params)
-
+    python3 data_importer.py -m  events \
+                             -p  文件路径 \
+                             -ds 数据源ID \
+                             -f  [CSV|TSV|Json] \
+                             -d  [True|False] \
+                             -qf " \
+                             -sep , \
+                             -skh \
+                             -attr userId,... \
+                             -s YYYY-MM-DD \
+                             -e YYYY-MM-DD
 
 |参数|参数说明|
-|-|----|
+|----|----|
 |-m|必填参数. 用户行为数据导入-events|
-|-path|必填参数. 需要导入的数据所在的路径|
-|-datasource_id|必填参数. 数据源ID|
-|-event_start|必选参数. 数据起始时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
-|-event_end|必选参数. 数据结束时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
-|-format|可选参数. 导入数据格式,目前支持JSON,CSV,TSV三种格式.默认值:JSON|
-|-qualifier|可选参数. CSV,TSV格式文本限定符.默认值:"|
-|-separator|可选参数. CSV,TSV格式文本分割符.默认值:,|
-|-skip_header|可选参数. CSV,TSV格式设置则自动跳过首行,此参数不需要设置值.|
-|-attributes|可选参数. CSV,TSV格式导入文件的各列按顺序映射到属性名，逗号分隔.userId,event,timestamp必须指定(需加单引号或者在特殊符号前加上\)|
+|-p|必填参数. 需要导入的数据所在的路径|
+|-ds|必填参数. 数据源ID|
+|-s|必选参数. 数据起始时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
+|-e|必选参数. 数据结束时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
+|-f|可选参数. 导入数据格式,目前支持JSON,CSV,TSV三种格式.默认值:JSON|
+|-qf|可选参数. CSV,TSV格式文本限定符.默认值:"|
+|-sep|可选参数. CSV,TSV格式文本分割符.默认值:,|
+|-skh|可选参数. CSV,TSV格式设置则自动跳过首行,此参数不需要设置值.|
+|-attr|可选参数. CSV,TSV格式导入文件的各列按顺序映射到属性名，逗号分隔.userId,event,timestamp必须指定(需加单引号或者在特殊符号前加上\)|
 
 ## 数据导入之MYSQL
 
 目前支持如下：
 
 * 用户属性数据导入
 * 用户行为数据导入
 
 ### 使用说明
 
 #### 用户属性数据导入
 
-    from importers import format_importer
-
-    params = {
-        'm': 'user_variables',
-        'format': 'mysql',
-        'datasource_id': '<数据源ID>',
-        'host': '<数据库连接地址>',
-        'user': '<数据库连接用户>',
-        'password': '<数据库连接密码>',
-        'port': '<数据库连接端口号>',
-        'sql': '<查询语句>'
-    }
-
-    format_importer.do_importer(params)
+    python3 format_importer.py -m  user_variables \
+                               -ds 数据源ID \
+                               -f  mysql \
+                               -db_host  mysql数据库ip \
+                               -db_user 客户端用户名 \
+                               -db_password 客户端密码 \
+                               -db_port 客户端端口号 \
+                               -sql sql语句 
 
 |参数|参数说明|
 |----|----|
 |-m|必填参数. 用户属性数据导入-user_variables|
-|-datasource_id|必填参数. 数据源ID|
-|-format|必选参数. 导入数据格式,目前支持mysql、hive数据源|
-|-host|必选参数. mysql数据库ip|
-|-user|必选参数. 客户端用户名|
-|-password|必选参数.客户端密码|
-|-port|必选选参数. 客户端端口号|
+|-ds|必填参数. 数据源ID|
+|-f|必选参数. 导入数据格式,目前支持mysql、hive数据源|
+|-db_host|必选参数. mysql数据库ip|
+|-db_user|必选参数. 客户端用户名|
+|-db_password|必选参数.客户端密码|
+|-db_port|必选选参数. 客户端端口号|
 |-sql|必选参数. sql语句|
 
 #### 用户行为数据导入
 
-    from importers import format_importer
-
-    params = {
-        'm': 'events',
-        'format': 'mysql',
-        'datasource_id': '<数据源ID>',
-        'host': '<数据库连接地址>',
-        'user': '<数据库连接用户>',
-        'password': '<数据库连接密码>',
-        'port': '<数据库连接端口号>',
-        'sql': '<查询语句>',
-        'start_time': '<数据起始日期>',
-        'end_time': '<数据结束日期>'
-    }
-
-    format_importer.do_importer(params) 
+    python3 format_importer.py -m  events \
+                               -ds 数据源ID \
+                               -f  mysql \
+                               -db_host  mysql数据库ip \
+                               -db_user 客户端用户名 \
+                               -db_password 客户端密码 \
+                               -db_port 客户端端口号 \
+                               -sql sql语句 \
+                               -s YYYY-MM-DD \
+                               -e YYYY-MM-DD
 
 |参数|参数说明|
 |----|----|
-|-m|必填参数. 用户属性数据导入-user_variables|
-|-datasource_id|必填参数. 数据源ID|
-|-format|必选参数. 导入数据格式,目前支持mysql、hive数据源|
-|-host|必选参数. mysql数据库ip|
-|-user|必选参数. 客户端用户名|
-|-password|必选参数.客户端密码|
-|-port|必选选参数. 客户端端口号|
+|-m|必填参数. 用户行为数据导入-events|
+|-ds|必填参数. 数据源ID|
+|-f|必选参数. 导入数据格式,目前支持mysql数据源|
+|-db_host|必选参数. mysql数据库ip|
+|-db_user|必选参数. 客户端用户名|
+|-db_password|必选参数.客户端密码|
+|-db_port|必选参数. 客户端端口号|
 |-sql|必选参数. sql语句|
-|-start_time|必选参数. 数据起始时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
-|-end_time|必选参数. 数据结束时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
+|-s|必选参数. 数据起始时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
+|-e|必选参数. 数据结束时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
 
 ## 数据导入之HIVE
 
 目前支持如下：
 
 * 用户属性数据导入
 * 用户行为数据导入
 
 ### 使用说明
 
 #### 用户属性数据导入
 
-    from importers import format_importer
-
-    params = {
-        'm': 'user_variables',
-        'format': 'hive',
-        'datasource_id': '<数据源ID>',
-        'host': '<数据库连接地址>',
-        'user': '<数据库连接用户>',
-        'password': '<数据库连接密码>',
-        'port': '<数据库连接端口号>',
-        'sql': '<查询语句>'
-    }
-
-    format_importer.do_importer(params)
+    python3 format_importer.py -m  user_variables \
+                               -ds 数据源ID \
+                               -f  hive \
+                               -db_host  hive数据库ip \
+                               -db_user 客户端用户名 \
+                               -db_port 客户端端口号 \
+                               -sql sql语句 
 
 |参数|参数说明|
 |----|----|
 |-m|必填参数. 用户属性数据导入-user_variables|
-|-datasource_id|必填参数. 数据源ID|
-|-format|必选参数. 导入数据格式,目前支持mysql、hive数据源|
-|-host|必选参数. mysql数据库ip|
-|-user|必选参数. 客户端用户名|
-|-password|必选参数.客户端密码|
-|-port|必选选参数. 客户端端口号|
+|-ds|必填参数. 数据源ID|
+|-f|必选参数. 导入数据格式,目前支持mysql、hive数据源|
+|-db_host|必选参数. hive数据库ip|
+|-db_user|必选参数. 客户端用户名|
+|-db_port|必选选参数. 客户端端口号|
 |-sql|必选参数. sql语句|
 
 #### 用户行为数据导入
 
-    from importers import format_importer
-
-    params = {
-        'm': 'events',
-        'format': 'hive',
-        'datasource_id': '<数据源ID>',
-        'host': '<数据库连接地址>',
-        'user': '<数据库连接用户>',
-        'password': '<数据库连接密码>',
-        'port': '<数据库连接端口号>',
-        'sql': '<查询语句>',
-        'start_time': '<数据起始日期>',
-        'end_time': '<数据结束日期>'
-    }
-
-    format_importer.do_importer(params)
+    python3 format_importer.py -m  events \
+                               -ds 数据源ID \
+                               -f  hive \
+                               -db_host  hive数据库ip \
+                               -db_user 客户端用户名 \
+                               -db_port 客户端端口号 \
+                               -sql sql语句 \
+                               -s YYYY-MM-DD \
+                               -e YYYY-MM-DD
 
 |参数|参数说明|
 |----|----|
-|-m|必填参数. 用户属性数据导入-user_variables|
-|-datasource_id|必填参数. 数据源ID|
-|-format|必选参数. 导入数据格式,目前支持mysql、hive数据源|
-|-host|必选参数. mysql数据库ip|
-|-user|必选参数. 客户端用户名|
-|-password|必选参数.客户端密码|
-|-port|必选选参数. 客户端端口号|
+|-m|必填参数. 用户行为数据导入-events|
+|-ds|必填参数. 数据源ID|
+|-f|必选参数. 导入数据格式,目前支持mysql、hive数据源|
+|-db_host|必选参数. hive数据库ip|
+|-db_user|必选参数. 客户端用户名|
+|-db_port|必选参数. 客户端端口号|
 |-sql|必选参数. sql语句|
-|-start_time|必选参数. 数据起始时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
-|-end_time|必选参数. 数据结束时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
+|-s|必选参数. 数据起始时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
+|-e|必选参数. 数据结束时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
 
 ## 用户删除
 
 目前支持如下：
 
 * 触发用户删除任务
 * 批量添加待删除用户
 
 ### 使用说明
 
 #### 触发用户删除任务
 
-    from importers import clear_user
-
-    params = {
-        'm': 'clear_users',
-        'now': True
-    }
-
-    clear_user.do_user(params)
-
     python3 clear_user.py -m clear_users  -n True 
 
 |参数|参数说明|
-|---|----|
+|----|----|
 |-m|必填参数. 触发用户删除任务-clear_users |
-|-now|必填参数. True - 立即执行离线任务,False - 天任务执行清理任务|
+|-n|必填参数. True - 立即执行离线任务,False - 天任务执行清理任务|
 
 #### 批量添加待删除用户
 
-    from importers import clear_user
-
-    params = {
-        'm': 'clear_users',
-        'users': 'xxx,xxx,xxx'
-    }
-
-    clear_user.do_user(params)
+    python3 clear_user.py -m clear_users_meta -u xxx,xxx,xxx
 
 |参数|参数说明|
 |----|----|
 |-m|必填参数. 批量添加待删除用户-clear_users_meta|
-|-users|必填参数. 添加待删除用户,多个用户以逗号(,)分隔|
-
+|-u|必填参数. 添加待删除用户,多个用户以逗号(,)分隔|
```

### Comparing `gio_importer_v42-1.0.1/README.md` & `gio_importer_v42-1.4.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `gio_importer_v42-1.0.1/gio_importer_v42.egg-info/PKG-INFO` & `gio_importer_v42-1.4.1.dev0/gio_importer_v42.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 Metadata-Version: 2.1
 Name: gio-importer-v42
-Version: 1.0.1
+Version: 1.4.1.dev0
 Summary: GrowingIO Importer是GrowingIO CDP平台元数据创建和数据导入工具
-Home-page: UNKNOWN
 Author: gio
 Author-email: dev-growing@startdt.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.8
+Classifier: Development Status :: 3 - Alpha
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pip
+Requires-Dist: numpy
+Requires-Dist: requests
+Requires-Dist: pandas
+Requires-Dist: curlify
+Requires-Dist: PyYAML
+Requires-Dist: psycopg2-binary
+Requires-Dist: pymysql
+Requires-Dist: pyhive
+Requires-Dist: thrift
+Requires-Dist: sasl
 
 # GrowingIO Importer
 
 GrowingIO Importer是GrowingIO CDP平台元数据创建和数据导入工具。
 
 ## 入门
 
 有关GrowingIO Importer请访问[GrowingIO官方文档](https://docs.growingio.com/op/developer-manual/toolbox/ )获取帮助。
 
 ## 环境依赖
 
-| | 4.2 |
-|----|-----|
-|Python| 3.8 |
+| |1.0|
+|----|----|
+|Python|3.6|
 
 ## 安装
 
-pip install gio-importer-v42
-
-## 环境参数
-    import importers
-    print(importers.__path__)
-
-    根据路径信息，进入包目录，修改conf.cfg(导入工具配置信息)
-    需要修改有关FTP，API信息(找负责项目运维提供FTP，API-uri相关信息)
-
+下载工具包GrowingIO Importer,在importer目录下执行脚本sh init.sh完成初始化
 
 ## 元数据导入
 
 目前支持如下：
 
 * 创建事件
 * 创建事件属性
@@ -49,364 +49,278 @@
 * 导出元数据
 * 导入元数据
 
 ### 使用说明
 
 #### 创建事件
 
-    from importers import meta_importer
-
-    params = {
-        'm': 'create_event',
-        'key': '<事件名>',
-        'name': '<事件显示名>',
-        'desc': '<事件描述>'
-    }
-
-    meta_importer.do_meta(params)
+    python3 meta_importer -m create_event \
+    --key <事件名> \
+    [-n <事件显示名>] \
+    [-d <事件描述>] \
 
 |参数|参数说明|
 |----|----|
 |-m|必选参数，项目名。|
-|--key|必选参数，事件名。仅允许大小写英文、数字、以及下划线，并且不能以数字开头，限长30字符|
-|--name|可选参数，事件显示名。默认同事件名，限长30字符|
-|--desc|可选参数，事件描述，默认为空。若描述中有空格则需要加双引号|
+|-k、--key|必选参数，事件名。仅允许大小写英文、数字、以及下划线，并且不能以数字开头，限长30字符|
+|-n、--name|可选参数，事件显示名。默认同事件名，限长30字符|
+|-d、--desc|可选参数，事件描述，默认为空。若描述中有空格则需要加双引号|
 
 #### 创建事件属性
 
-    from importers import meta_importer
-
-    params = {
-        'm': 'create_event_variables',
-        'key': '<事件属性名>',
-        'type': '<事件属性数据类型>',
-        'name': '<事件属性显示名>',
-        'desc': '<事件属性描述>'
-    }
-
-    meta_importer.do_meta(params)
+    python3 meta_importer.py -m create_event_variables \
+                             -k <事件名> \
+                             -t <事件属性数据类型> \
+                             [-n <事件显示名>] \
+                             [-d <事件属性描述>] \
 
 |参数|参数说明|
 |----|----|
 |-m|必选参数，项目名。|
-|--key|必选参数，事件名。仅允许大小写英文、数字、以及下划线，并且不能以数字开头，限长30字符|
-|--type|必选参数，事件属性数据类型。可选值：string/int/double
-|--name|可选参数，事件显示名。默认同事件名，限长30字符|
-|--desc|可选参数，事件描述，默认为空。若描述中有空格则需要加双引号|
+|-k、--key|必选参数，事件名。仅允许大小写英文、数字、以及下划线，并且不能以数字开头，限长30字符|
+|-t、--type|必选参数，事件属性数据类型。可选值：string/int/double
+|-n、--name|可选参数，事件显示名。默认同事件名，限长30字符|
+|-d、--desc|可选参数，事件描述，默认为空。若描述中有空格则需要加双引号|
 
 #### 创建用户属性
 
-    from importers import meta_importer
-
-    params = {
-        'm': 'create_user_variables',
-        'key': '<用户属性名>',
-        'type': '<用户属性数据类型>',
-        'name': '<用户属性显示名>',
-        'desc': '<用户属性描述>'
-    }
-
-    meta_importer.do_meta(params)
+    python3 meta_importer.py -m create_user_variables \
+                             -k <标识符> \
+                             -t <用户属性数据类型> \
+                             [-n <用户显示名>] \
+                             [-d <用户属性描述>] \
 
 |参数|参数说明|
 |----|----|
 |-m|必选参数，项目名。|
-|--key|必选参数，标识符。仅允许大小写英文、数字、以及下划线，并且不能以数字开头，限长30字符|
-|--type|必选参数，可选参数：string/int/date
-|--name|可选参数，用户显示名。默认同标识符，限长30字符|
-|--desc|可选参数，用户属性描述，默认为空。若描述中有空格则需要加双引号|
+|-k、--key|必选参数，标识符。仅允许大小写英文、数字、以及下划线，并且不能以数字开头，限长30字符|
+|-t、--type|必选参数，可选参数：string/int/date
+|-n、--name|可选参数，用户显示名。默认同标识符，限长30字符|
+|-d、--desc|可选参数，用户属性描述，默认为空。若描述中有空格则需要加双引号|
 
 #### 绑定事件与事件属性
 
     python3 meta_importer.py -m bind_event_variables \
                              -k <事件名> \
                              -a <绑定事件属性名> \
 
 |参数|参数说明|
 |----|----|
 |-m|必选参数，项目名。|
-|--key|必选参数，事件名。若事件不存在则创建，否则更新事件|
-|--attr|必选参数，绑定事件属性名。多个属性名使用英文逗号分隔(需加单引号或者在特殊符号前加上\)|
+|-k、--key|必选参数，事件名。若事件不存在则创建，否则更新事件|
+|-a、--attr|必选参数，绑定事件属性名。多个属性名使用英文逗号分隔(需加单引号或者在特殊符号前加上\)|
 
 #### 导出元数据
 
-    from importers import meta_importer
-
-    params = {
-        'm': 'bind_event_variables',
-        'key': '<事件名>',
-        'attr': '<绑定事件属性名集合>'
-    }
-
-    meta_importer.do_meta(params)
+    python3 meta_importer.py -m export_meta \
+                             -f <文件名> \
 
 |参数|参数说明|
 |----|----|
 |-m|必选参数，项目名。|
-|--file|必选参数，导出文件名|
+|-f、--file|必选参数，导出文件名|
 
 #### 导入元数据
 
-    from importers import meta_importer
-
-    params = {
-        'm': 'import_meta',
-        'file': '<文件名>'
-    }
-
-    meta_importer.do_meta(params)
+    python3 meta_importer.py -m import_meta \
+                             -f <文件名> \
 
 |参数|参数说明|
 |----|----|
 |-m|必选参数，项目名。|
-|--file|必选参数，导入文件名|
+|-f、--file|必选参数，导入文件名|
 
 ## 数据导入
 
 目前支持如下：
 
 * 用户属性数据导入
 * 用户行为数据导入
 
 ### 使用说明
 
 #### 用户属性数据导入
 
-    from importers import data_importer
-
-    params = {
-        'm': 'user_variables',
-        'path': '<文件路径>',
-        'datasource_id': '<数据源ID>',
-        'format': '[CSV|TSV|Json]',
-        'separator': ',',
-        'skip_header': 'True',
-        'attributes': 'userId,...'
-    }
-
-    data_importer.do_importer(params)
-
+    python3 data_importer.py -m  user_variables \
+                             -p  文件路径 \
+                             -ds 数据源ID \
+                             -f  [CSV|TSV|Json] \
+                             -d  [True|False] \
+                             -qf " \
+                             -sep , \
+                             -skh \
+                             -attr userId,...
 
 |参数|参数说明|
-|---|----|
+|----|----|
 |-m|必填参数. 用户属性数据导入-user_variables|
-|-path|必填参数. 需要导入的数据所在的路径|
-|-datasource_id|必填参数. 数据源ID|
-|-format|可选参数. 导入数据格式,目前支持JSON,CSV,TSV三种格式.默认值:JSON|
-|-qualifier|可选参数. CSV,TSV格式文本限定符.默认值:"|
-|-separator|可选参数. CSV,TSV格式文本分割符.默认值:,|
-|-skip_header|可选参数. CSV,TSV格式设置则自动跳过首行,此参数不需要设置值.|
-|-attributes|可选参数. CSV,TSV格式导入文件的各列按顺序映射到属性名，逗号分隔.userId必须指定(需加单引号或者在特殊符号前加上\)|
+|-p|必填参数. 需要导入的数据所在的路径|
+|-ds|必填参数. 数据源ID|
+|-f|可选参数. 导入数据格式,目前支持JSON,CSV,TSV三种格式.默认值:JSON|
+|-qf|可选参数. CSV,TSV格式文本限定符.默认值:"|
+|-sep|可选参数. CSV,TSV格式文本分割符.默认值:,|
+|-skh|可选参数. CSV,TSV格式设置则自动跳过首行,此参数不需要设置值.|
+|-attr|可选参数. CSV,TSV格式导入文件的各列按顺序映射到属性名，逗号分隔.userId必须指定(需加单引号或者在特殊符号前加上\)|
 
 #### 用户行为数据导入
 
-    from importers import data_importer
-
-    params = {
-        'm': 'events',
-        'path': '<文件路径>',
-        'datasource_id': '<数据源ID>',
-        'format': '[CSV|TSV|Json]',
-        'separator': ',',
-        'skip_header': 'True',
-        'attributes': 'userId,...,
-        'event_start': '<数据起始日期 YYYY-MM-DD>',
-        'event_end': '<数据结束日期 YYYY-MM-DD>'
-    }
-
-    data_importer.do_importer(params)
-
+    python3 data_importer.py -m  events \
+                             -p  文件路径 \
+                             -ds 数据源ID \
+                             -f  [CSV|TSV|Json] \
+                             -d  [True|False] \
+                             -qf " \
+                             -sep , \
+                             -skh \
+                             -attr userId,... \
+                             -s YYYY-MM-DD \
+                             -e YYYY-MM-DD
 
 |参数|参数说明|
-|-|----|
+|----|----|
 |-m|必填参数. 用户行为数据导入-events|
-|-path|必填参数. 需要导入的数据所在的路径|
-|-datasource_id|必填参数. 数据源ID|
-|-event_start|必选参数. 数据起始时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
-|-event_end|必选参数. 数据结束时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
-|-format|可选参数. 导入数据格式,目前支持JSON,CSV,TSV三种格式.默认值:JSON|
-|-qualifier|可选参数. CSV,TSV格式文本限定符.默认值:"|
-|-separator|可选参数. CSV,TSV格式文本分割符.默认值:,|
-|-skip_header|可选参数. CSV,TSV格式设置则自动跳过首行,此参数不需要设置值.|
-|-attributes|可选参数. CSV,TSV格式导入文件的各列按顺序映射到属性名，逗号分隔.userId,event,timestamp必须指定(需加单引号或者在特殊符号前加上\)|
+|-p|必填参数. 需要导入的数据所在的路径|
+|-ds|必填参数. 数据源ID|
+|-s|必选参数. 数据起始时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
+|-e|必选参数. 数据结束时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
+|-f|可选参数. 导入数据格式,目前支持JSON,CSV,TSV三种格式.默认值:JSON|
+|-qf|可选参数. CSV,TSV格式文本限定符.默认值:"|
+|-sep|可选参数. CSV,TSV格式文本分割符.默认值:,|
+|-skh|可选参数. CSV,TSV格式设置则自动跳过首行,此参数不需要设置值.|
+|-attr|可选参数. CSV,TSV格式导入文件的各列按顺序映射到属性名，逗号分隔.userId,event,timestamp必须指定(需加单引号或者在特殊符号前加上\)|
 
 ## 数据导入之MYSQL
 
 目前支持如下：
 
 * 用户属性数据导入
 * 用户行为数据导入
 
 ### 使用说明
 
 #### 用户属性数据导入
 
-    from importers import format_importer
-
-    params = {
-        'm': 'user_variables',
-        'format': 'mysql',
-        'datasource_id': '<数据源ID>',
-        'host': '<数据库连接地址>',
-        'user': '<数据库连接用户>',
-        'password': '<数据库连接密码>',
-        'port': '<数据库连接端口号>',
-        'sql': '<查询语句>'
-    }
-
-    format_importer.do_importer(params)
+    python3 format_importer.py -m  user_variables \
+                               -ds 数据源ID \
+                               -f  mysql \
+                               -db_host  mysql数据库ip \
+                               -db_user 客户端用户名 \
+                               -db_password 客户端密码 \
+                               -db_port 客户端端口号 \
+                               -sql sql语句 
 
 |参数|参数说明|
 |----|----|
 |-m|必填参数. 用户属性数据导入-user_variables|
-|-datasource_id|必填参数. 数据源ID|
-|-format|必选参数. 导入数据格式,目前支持mysql、hive数据源|
-|-host|必选参数. mysql数据库ip|
-|-user|必选参数. 客户端用户名|
-|-password|必选参数.客户端密码|
-|-port|必选选参数. 客户端端口号|
+|-ds|必填参数. 数据源ID|
+|-f|必选参数. 导入数据格式,目前支持mysql、hive数据源|
+|-db_host|必选参数. mysql数据库ip|
+|-db_user|必选参数. 客户端用户名|
+|-db_password|必选参数.客户端密码|
+|-db_port|必选选参数. 客户端端口号|
 |-sql|必选参数. sql语句|
 
 #### 用户行为数据导入
 
-    from importers import format_importer
-
-    params = {
-        'm': 'events',
-        'format': 'mysql',
-        'datasource_id': '<数据源ID>',
-        'host': '<数据库连接地址>',
-        'user': '<数据库连接用户>',
-        'password': '<数据库连接密码>',
-        'port': '<数据库连接端口号>',
-        'sql': '<查询语句>',
-        'start_time': '<数据起始日期>',
-        'end_time': '<数据结束日期>'
-    }
-
-    format_importer.do_importer(params) 
+    python3 format_importer.py -m  events \
+                               -ds 数据源ID \
+                               -f  mysql \
+                               -db_host  mysql数据库ip \
+                               -db_user 客户端用户名 \
+                               -db_password 客户端密码 \
+                               -db_port 客户端端口号 \
+                               -sql sql语句 \
+                               -s YYYY-MM-DD \
+                               -e YYYY-MM-DD
 
 |参数|参数说明|
 |----|----|
-|-m|必填参数. 用户属性数据导入-user_variables|
-|-datasource_id|必填参数. 数据源ID|
-|-format|必选参数. 导入数据格式,目前支持mysql、hive数据源|
-|-host|必选参数. mysql数据库ip|
-|-user|必选参数. 客户端用户名|
-|-password|必选参数.客户端密码|
-|-port|必选选参数. 客户端端口号|
+|-m|必填参数. 用户行为数据导入-events|
+|-ds|必填参数. 数据源ID|
+|-f|必选参数. 导入数据格式,目前支持mysql数据源|
+|-db_host|必选参数. mysql数据库ip|
+|-db_user|必选参数. 客户端用户名|
+|-db_password|必选参数.客户端密码|
+|-db_port|必选参数. 客户端端口号|
 |-sql|必选参数. sql语句|
-|-start_time|必选参数. 数据起始时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
-|-end_time|必选参数. 数据结束时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
+|-s|必选参数. 数据起始时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
+|-e|必选参数. 数据结束时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
 
 ## 数据导入之HIVE
 
 目前支持如下：
 
 * 用户属性数据导入
 * 用户行为数据导入
 
 ### 使用说明
 
 #### 用户属性数据导入
 
-    from importers import format_importer
-
-    params = {
-        'm': 'user_variables',
-        'format': 'hive',
-        'datasource_id': '<数据源ID>',
-        'host': '<数据库连接地址>',
-        'user': '<数据库连接用户>',
-        'password': '<数据库连接密码>',
-        'port': '<数据库连接端口号>',
-        'sql': '<查询语句>'
-    }
-
-    format_importer.do_importer(params)
+    python3 format_importer.py -m  user_variables \
+                               -ds 数据源ID \
+                               -f  hive \
+                               -db_host  hive数据库ip \
+                               -db_user 客户端用户名 \
+                               -db_port 客户端端口号 \
+                               -sql sql语句 
 
 |参数|参数说明|
 |----|----|
 |-m|必填参数. 用户属性数据导入-user_variables|
-|-datasource_id|必填参数. 数据源ID|
-|-format|必选参数. 导入数据格式,目前支持mysql、hive数据源|
-|-host|必选参数. mysql数据库ip|
-|-user|必选参数. 客户端用户名|
-|-password|必选参数.客户端密码|
-|-port|必选选参数. 客户端端口号|
+|-ds|必填参数. 数据源ID|
+|-f|必选参数. 导入数据格式,目前支持mysql、hive数据源|
+|-db_host|必选参数. hive数据库ip|
+|-db_user|必选参数. 客户端用户名|
+|-db_port|必选选参数. 客户端端口号|
 |-sql|必选参数. sql语句|
 
 #### 用户行为数据导入
 
-    from importers import format_importer
-
-    params = {
-        'm': 'events',
-        'format': 'hive',
-        'datasource_id': '<数据源ID>',
-        'host': '<数据库连接地址>',
-        'user': '<数据库连接用户>',
-        'password': '<数据库连接密码>',
-        'port': '<数据库连接端口号>',
-        'sql': '<查询语句>',
-        'start_time': '<数据起始日期>',
-        'end_time': '<数据结束日期>'
-    }
-
-    format_importer.do_importer(params)
+    python3 format_importer.py -m  events \
+                               -ds 数据源ID \
+                               -f  hive \
+                               -db_host  hive数据库ip \
+                               -db_user 客户端用户名 \
+                               -db_port 客户端端口号 \
+                               -sql sql语句 \
+                               -s YYYY-MM-DD \
+                               -e YYYY-MM-DD
 
 |参数|参数说明|
 |----|----|
-|-m|必填参数. 用户属性数据导入-user_variables|
-|-datasource_id|必填参数. 数据源ID|
-|-format|必选参数. 导入数据格式,目前支持mysql、hive数据源|
-|-host|必选参数. mysql数据库ip|
-|-user|必选参数. 客户端用户名|
-|-password|必选参数.客户端密码|
-|-port|必选选参数. 客户端端口号|
+|-m|必填参数. 用户行为数据导入-events|
+|-ds|必填参数. 数据源ID|
+|-f|必选参数. 导入数据格式,目前支持mysql、hive数据源|
+|-db_host|必选参数. hive数据库ip|
+|-db_user|必选参数. 客户端用户名|
+|-db_port|必选参数. 客户端端口号|
 |-sql|必选参数. sql语句|
-|-start_time|必选参数. 数据起始时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
-|-end_time|必选参数. 数据结束时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
+|-s|必选参数. 数据起始时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
+|-e|必选参数. 数据结束时间,导入用户行为数据时指定.格式:YYYY-MM-DD|
 
 ## 用户删除
 
 目前支持如下：
 
 * 触发用户删除任务
 * 批量添加待删除用户
 
 ### 使用说明
 
 #### 触发用户删除任务
 
-    from importers import clear_user
-
-    params = {
-        'm': 'clear_users',
-        'now': True
-    }
-
-    clear_user.do_user(params)
-
     python3 clear_user.py -m clear_users  -n True 
 
 |参数|参数说明|
-|---|----|
+|----|----|
 |-m|必填参数. 触发用户删除任务-clear_users |
-|-now|必填参数. True - 立即执行离线任务,False - 天任务执行清理任务|
+|-n|必填参数. True - 立即执行离线任务,False - 天任务执行清理任务|
 
 #### 批量添加待删除用户
 
-    from importers import clear_user
-
-    params = {
-        'm': 'clear_users',
-        'users': 'xxx,xxx,xxx'
-    }
-
-    clear_user.do_user(params)
+    python3 clear_user.py -m clear_users_meta -u xxx,xxx,xxx
 
 |参数|参数说明|
 |----|----|
 |-m|必填参数. 批量添加待删除用户-clear_users_meta|
-|-users|必填参数. 添加待删除用户,多个用户以逗号(,)分隔|
-
+|-u|必填参数. 添加待删除用户,多个用户以逗号(,)分隔|
```

### Comparing `gio_importer_v42-1.0.1/gio_importer_v42.egg-info/SOURCES.txt` & `gio_importer_v42-1.4.1.dev0/gio_importer_v42.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 LICENSE
-MANIFEST.in
 README.md
 setup.py
 gio_importer_v42.egg-info/PKG-INFO
 gio_importer_v42.egg-info/SOURCES.txt
 gio_importer_v42.egg-info/dependency_links.txt
 gio_importer_v42.egg-info/entry_points.txt
 gio_importer_v42.egg-info/requires.txt
 gio_importer_v42.egg-info/top_level.txt
-importers/README.md
 importers/__init__.py
 importers/clear_user.py
-importers/conf.cfg
 importers/data_importer.py
 importers/format_importer.py
-importers/log_conf.yaml
 importers/meta_importer.py
 importers/saas_export.py
 importers/setup.py
 importers/trigger_job.py
 importers/zk.py
 importers/clear_data/__init__.py
 importers/clear_data/clear_data.py
@@ -29,18 +25,14 @@
 importers/common/log_util.py
 importers/data_import/__init__.py
 importers/data_import/data_events.py
 importers/data_import/data_format_util.py
 importers/data_import/data_item_variable.py
 importers/data_import/data_model.py
 importers/data_import/data_user_variable.py
-importers/db_import/__init__.py
-importers/db_import/database_import.py
-importers/db_import/hive_import.py
-importers/db_import/mysql_import.py
 importers/example/__init__.py
 importers/meta/__init__.py
 importers/meta/check_util.py
 importers/meta/data_center.py
 importers/meta/meta_create.py
 importers/saas_export/__init__.py
 importers/saas_export/saas_meta.py
```

### Comparing `gio_importer_v42-1.0.1/importers/clear_data/clear_data.py` & `gio_importer_v42-1.4.1.dev0/importers/clear_data/clear_data.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v42-1.0.1/importers/common/common_util.py` & `gio_importer_v42-1.4.1.dev0/importers/common/common_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import os
 import shutil
 from pyhive import hive
 import pymysql
 import pytz
 import datetime
 import time
+from krbcontext import krbcontext
 
 from importers.common.config_util import BaseConfig
 
 
 def split_str(s, sep, qualifier):
     """
     分割复杂字符串
@@ -119,42 +120,49 @@
     delimiter = time_str[4:5]
     if delimiters.__contains__(delimiter):
         format = format[:2] + delimiter + format[3:5] + delimiter + format[6:]
 
     return format
 
 
-def mysql_connect(user, password, host, port):
+def mysql_connect(user, password, host, port, database):
     """
      获取mysql连接
     :param user: mysql用户名
     :param password: mysql密码
     :param host: mysql Host
     :param port: mysql 端口号
+    :param database: mysql 数据库
     :return:
     """
     return pymysql.connect(
         host=host,
         port=port,
         user=user,
         charset='utf8',
         passwd=password,
-        db='information_schema'
+        db=database
     )
 
 
-def hive_connect(host, port, user):
+def hive_connect(host, port, user, password, auth, database, principal, keytab):
     """
      获取hive连接
     :param host: hive Host
     :param port: hive 端口号
     :param user: hive用户名
+    :param password: hive密码
+    :param auth: hive认证方式
+    :param database: 数据库
+    :param principal: Kerberos 主体名称
+    :param keytab: Kerberos凭证
     :return:
     """
-    return hive.Connection(host=host, port=port, username=user, database='default')
+    with krbcontext(using_keytab=True, principal=principal, keytab_file=keytab):
+        return hive.Connection(host=host, port=port, username=user, password=password, auth=auth, database=database)
 
 
 def getVariables(dataCenter):
     """
      获取变量标识符列表
     :param dataCenter: getdataCenterEventVariables、getdataCenterUserVariables
     :return:标识符列表
```

### Comparing `gio_importer_v42-1.0.1/importers/common/config_util.py` & `gio_importer_v42-1.4.1.dev0/importers/common/config_util.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v42-1.0.1/importers/common/http_util.py` & `gio_importer_v42-1.4.1.dev0/importers/common/http_util.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v42-1.0.1/importers/common/log_util.py` & `gio_importer_v42-1.4.1.dev0/importers/common/log_util.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v42-1.0.1/importers/data_import/data_events.py` & `gio_importer_v42-1.4.1.dev0/importers/data_import/data_events.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v42-1.0.1/importers/data_import/data_format_util.py` & `gio_importer_v42-1.4.1.dev0/importers/data_import/data_format_util.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v42-1.0.1/importers/data_import/data_item_variable.py` & `gio_importer_v42-1.4.1.dev0/importers/data_import/data_item_variable.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v42-1.0.1/importers/data_import/data_model.py` & `gio_importer_v42-1.4.1.dev0/importers/data_import/data_model.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v42-1.0.1/importers/data_import/data_user_variable.py` & `gio_importer_v42-1.4.1.dev0/importers/data_import/data_user_variable.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v42-1.0.1/importers/data_importer.py` & `gio_importer_v42-1.4.1.dev0/importers/data_importer.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,44 +16,43 @@
 from importers.data_import.data_events import events_import
 from importers.data_import.data_user_variable import user_variables_import
 from importers.common.common_util import get_all_file
 from importers.common.log_util import logger
 from importers.meta.data_center import getTunnels
 from importers.data_import.data_item_variable import item_variables_import
 
-
 def parse_args():
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument('-m',
-                        help='必填参数. 用户属性数据导入:user_variables，用户行为数据导入:events，主体数据导入:item_variables.',
+                        help='必填参数. 用户属性数据导入:user_variables，用户行为数据导入:events，维度表数据导入:item_variables.',
                         required=True,
                         default='',
                         type=str)
     parser.add_argument('-p', '--path',
                         help='必填参数. 需要导入的数据所在的路径',
                         required=True,
                         default='',
                         type=str)
     parser.add_argument('-ds', '--datasource_id',
                         help='必填参数. 数据源ID.',
-                        required=True,
+                        required=False,
                         default='',
                         type=str)
     parser.add_argument('-f', '--format',
                         help='可选参数. 导入数据格式,目前支持JSON,CSV,TSV三种格式.',
                         default='JSON',
                         type=str)
     parser.add_argument('-item_key',
                         help='必填参数. item_key',
                         required=False,  # 根据-m参数判断是否必填
                         default='',
                         type=str)
     # 暂时取消
     parser.add_argument('-d', '--debug',
-                        help='可选参数. True-导入数据全量校验,false-不校验数据是否平台定义立即创建导入任务进入导入队列.',
+                        help='可选参数. True-导入数据全量校验但不导,false-立即创建导入任务进入导入队列.',
                         default=True)
     parser.add_argument('-s', '--event_start',
                         help='可选参数. 数据起始时间,导入用户行为数据时指定',
                         default='',
                         type=str)
     parser.add_argument('-e', '--event_end',
                         help='可选参数. 数据结束时间,导入用户行为数据时指定',
@@ -82,92 +81,62 @@
                         help='可选参数. True-导入数据成功后清理掉FTP上数据,False-导入数据成功后不清理掉FTP上数据.',
                         default=False)
     parser.add_argument('-v', '--version', action='version', version='Gio_DataImporter_1.0')
     args = parser.parse_args()
     return args.__dict__
 
 
-def execute_importer(args):
+def main():
+    # Step one: 解析命令行参数
+    args = parse_args()
+    logger.debug(f"解析命令行参数: {args}")
+    # Step one: 校验基础参数,并预处理参数
     # 1. 校验导入文件
     p = args.get('path')
     ps = []
     if os.path.exists(p):
         ps.extend(get_all_file(p))
     else:
         logger.error("需要导入的数据文件不存在")
-        exit(-1)
+        return
     args['path'] = ps
     # 2. 校验Debug参数
     # 暂时取下
     d = str(args.get('debug')).upper()
     if 'TRUE'.__eq__(d):
         d = True
     elif 'FALSE'.__eq__(d):
         d = False
     else:
         logger.error("[-d/--debug]参数值不对")
-        exit(-1)
+        return
     args['debug'] = d
     # 3. 校验数据格式
     f = str(args.get('format')).upper()
     if 'JSON'.__eq__(f) is False and 'CSV'.__eq__(f) is False and 'TSV'.__eq__(f) is False:
         logger.error("目前支持JSON,CSV,TSV三种格式")
-        exit(-1)
+        return
     args['format'] = f
     # 4. 校验数据源
     m = args.get('m')
-    tunnels = getTunnels()
-    if args.get('datasource_id') not in tunnels:
-        logger.error("数据源不存在")
-        exit(-1)
-    args['datasource_id'] = [args.get('datasource_id'), tunnels[args.get('datasource_id')]]
+    if 'user_variables'.__eq__(m) or 'events'.__eq__(m):
+        tunnels = getTunnels()
+        if args.get('datasource_id') not in tunnels:
+            logger.error("数据源不存在")
+            return
+        args['datasource_id'] = [args.get('datasource_id'), tunnels[args.get('datasource_id')]]
     # Step three:  按导入模块处理
     if 'user_variables'.__eq__(m):
         user_variables_import(args)
     elif 'events'.__eq__(m):
         events_import(args)
     elif 'item_variables'.__eq__(m):
         item_variables_import(args)
     else:
-        logger.warn("目前只支持用户行为数据、用户属性数据导入和主体导入")
-        exit(-1)
-
-
-def do_importer(params):
-    logger.info("Data Importer Start")
-    # 设置默认参数值
-    default_params = {
-        'm': '',
-        'path': '',
-        'datasource_id': '',
-        'format': 'JSON',  # 默认为 'JSON'
-        'item_key': '',  # 默认为空字符串
-        'debug': True,  # 默认为 True
-        'event_start': '',  # 默认为空字符串
-        'event_end': '',  # 默认为空字符串
-        'qualifier': '"',  # 默认为双引号
-        'separator': '',  # 默认为空字符串
-        'skip_header': False,  # 默认为 False
-        'attributes': '',  # 默认为空字符串
-        'jobName': '',  # 默认为空字符串
-        'clear': False,  # 默认为 False
-    }
-
-    # 如果 params 中有相同的键，则 params 的值会覆盖 default_params 中的默认值
-    combined_params = {**default_params, **params}
-
-    execute_importer(combined_params)
-    logger.info("Data Importer Finish")
-
-
-def main():
-    # Step one: 解析命令行参数
-    args = parse_args()
-    logger.debug(f"解析命令行参数: {args}")
-    # Step one: 校验基础参数,并预处理参数
-    execute_importer(args)
+        logger.warn("目前只支持用户行为数据、用户属性数据导入和维度表导入")
+        return
 
 
 if __name__ == '__main__':
     logger.info("Data Importer Start")
     main()
     logger.info("Data Importer Finish")
```

### Comparing `gio_importer_v42-1.0.1/importers/format_importer.py` & `gio_importer_v42-1.4.1.dev0/importers/format_importer.py`

 * *Files 14% similar despite different names*

```diff
@@ -64,14 +64,34 @@
                         metavar="")
     parser.add_argument('-j', '--jobName',
                         help='指定导入任务名称',
                         metavar="")
     parser.add_argument('-c', '--clear',
                         help='可选参数. True-导入数据成功后清理掉FTP上数据,False-导入数据成功后不清理掉FTP上数据.',
                         default=False)
+    parser.add_argument('-at', '--auth',
+                        help='可选参数. hive认证方式',
+                        type=str,
+                        default="NONE",
+                        metavar="")
+    parser.add_argument('-db', '--database',
+                        help='可选参数. 指定数据库',
+                        type=str,
+                        default='',
+                        metavar="")
+    parser.add_argument('-pc', '--principal',
+                        help='可选参数. Kerberos 主体名称',
+                        type=str,
+                        default="",
+                        metavar="")
+    parser.add_argument('-kt', '--keytab',
+                        help='可选参数. Kerberos凭证',
+                        type=str,
+                        default='',
+                        metavar="")
     args = parser.parse_args()
     return args.__dict__
 
 
 def execute_importer(args):
     tunnels = getTunnels()
     m = args.get('m')
@@ -104,14 +124,18 @@
         'port': None,  # 必填参数, 没有默认值
         'sql': None,  # 必选参数, 没有默认值
         'batch': 100000,  # 默认为 100000
         'start_time': None,  # 用户行为数据必选参数, 没有默认值
         'end_time': None,  # 用户行为数据必选参数, 没有默认值
         'jobName': None,  # 可选参数, 没有默认值
         'clear': False,  # 默认为 False
+        'auth': "NONE",
+        'database': '',
+        'principal': '',
+        'keytab': ''
     }
 
     combined_params = {**default_params, **params}
     # 如果 params 中有相同的键，则 params 的值会覆盖 default_params 中的默认值
     execute_importer(combined_params)
     logger.info("Data Importer Finish")
```

### Comparing `gio_importer_v42-1.0.1/importers/meta/check_util.py` & `gio_importer_v42-1.4.1.dev0/importers/meta/check_util.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v42-1.0.1/importers/meta/data_center.py` & `gio_importer_v42-1.4.1.dev0/importers/meta/data_center.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v42-1.0.1/importers/meta/meta_create.py` & `gio_importer_v42-1.4.1.dev0/importers/meta/meta_create.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v42-1.0.1/importers/meta_importer.py` & `gio_importer_v42-1.4.1.dev0/importers/meta_importer.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,39 +4,38 @@
 # Copyright (c) 2020 growingio.com, Inc.  All Rights Reserved
 import argparse
 import os
 import pathlib
 import sys
 import logging
 
-from importers.common.log_util import logger
-
 sys.path.append(str(pathlib.Path(os.path.abspath(__file__)).parent.parent))
 from importers.meta.meta_create import *
 
 
 def parse_args():
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument('-m',
                         help='必填参数. 创建事件-create_event,创建事件属性-create_event_variables,创建用户属性-create_user_variables,'
-                             '创建主体字段-create_item_variables,绑定事件与事件属性-bind_event_variables,导入元数据-export_meta，导出元数据-import_meta',
+                             '创建维度字段-create_item_variables,绑定事件与事件属性-bind_event_variables,导入元数据-export_meta，导出元数据-import_meta',
                         required=True, metavar="")
-    parser.add_argument('-ik', '--item_key', help='创建主体时必填参数:指定主体标识符', default="", metavar="")
+    parser.add_argument('-ik', '--item_key', help='创建维度表时必填参数:指定维度表标识符', default="", metavar="")
     parser.add_argument('-k', '--key', help='必填参数. 需要创建事件名', default="", metavar="")
-    parser.add_argument('-t', '--type', help='创建事件/用户属性必填参数. 数据类型-(string,int,double)', default="",
-                        metavar="")
+    parser.add_argument('-t', '--type', help='创建事件/用户属性必填参数. 数据类型-(string,int,double)', default="", metavar="")
     parser.add_argument('-a', '--attr', help='绑定事件与属性必填参数，多个属性名使用英文逗号分隔', metavar="")
     parser.add_argument('-n', '--name', help='可选参数. 事件显示名', default="", metavar="")
     parser.add_argument('-d', '--desc', help='可选参数. 事件描述', default="", metavar="")
     parser.add_argument('-f', '--file', help='导入/导出元数据必填参数. 文件名', metavar="")
     args = parser.parse_args()
     return args.__dict__
 
 
-def execute_importer(args):
+def main():
+    args = parse_args()
+    # print(args)
     m = args.get("m")
     token = get_token()
     if 'create_event'.__eq__(m):
         key = args.get('key')
         check_key(key)
         create_info = create_event(token, key, args.get('name'), args.get('desc'))
         print("创建事件成功", create_info)
@@ -50,15 +49,15 @@
         check_key(key)
         create_info = create_user_variables(token, key, args.get('type'), args.get('name'), args.get('desc'))
         print("创建用户属性成功", create_info)
     elif 'create_item'.__eq__(m):
         item_key = args.get('item_key')
         check_key(item_key)
         create_info = create_item(token, item_key, args.get('name'), args.get('desc'))
-        print("创建主体成功", create_info)
+        print("创建维度表成功", create_info)
     elif 'create_item_variables'.__eq__(m):
         item_key = args.get('item_key')
         check_key(item_key)
         import_item_variables(token, item_key, args.get('file'))
     elif 'bind_event_variables'.__eq__(m):
         key = args.get('key')
         check_key(key)
@@ -69,22 +68,9 @@
     elif 'import_meta'.__eq__(m):
         import_meta(token, args.get('file'))
     else:
         logging.error("请确认填写项目名！")
         exit(-1)
 
 
-def do_meta(params):
-    logger.info("Meta Data Task Start")
-    execute_importer(params)
-    logger.info("Meta Data Task Finish")
-
-
-def main():
-    args = parse_args()
-    execute_importer(args)
-
-
 if __name__ == '__main__':
-    logger.info("Meta Data Task Start")
     main()
-    logger.info("Meta Data Task Finish")
```

### Comparing `gio_importer_v42-1.0.1/importers/saas_export/saas_meta.py` & `gio_importer_v42-1.4.1.dev0/importers/saas_export/saas_meta.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v42-1.0.1/importers/saas_export.py` & `gio_importer_v42-1.4.1.dev0/importers/saas_export.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v42-1.0.1/importers/trigger_job.py` & `gio_importer_v42-1.4.1.dev0/importers/trigger_job.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v42-1.0.1/setup.py` & `gio_importer_v42-1.4.1.dev0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,28 +16,28 @@
     'pyhive',
     'thrift',
     'sasl'
 ]
 
 setup(
     name='gio_importer_v42',
-    version='1.0.01',
+    version='1.4.01.dev',
     description='GrowingIO Importer是GrowingIO CDP平台元数据创建和数据导入工具',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='gio',
     author_email='dev-growing@startdt.com',
     packages=find_packages(include=["importers*"]),
     include_package_data=True,
     install_requires=install_requires,
     classifiers=[
-        # 'Development Status :: 3 - Alpha',  # 发布开发版分类器
-        'Development Status :: 5 - Production/Stable',  # 发布稳定版分类器
+        'Development Status :: 3 - Alpha',  # 发布开发版分类器
+        #'Development Status :: 5 - Production/Stable',  # 发布稳定版分类器
     ],
-    python_requires='>=3.8',
+    python_requires='>=3.7',
     entry_points={
         'console_scripts': [
             'clear_user=importers.clear_user:main',
             'data_importer=importers.data_importer:main',
             'format_importer=importers.format_importer:main',
             'meta_importer=importers.meta_importer:main',
         ],
```

