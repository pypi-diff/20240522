# Comparing `tmp/orbitkit-0.6.8.tar.gz` & `tmp/orbitkit-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/orbitkit-0.6.8.tar", last modified: Tue May 14 05:12:33 2024, max compression
+gzip compressed data, was "dist/orbitkit-0.6.9.tar", last modified: Tue May 14 05:52:50 2024, max compression
```

## Comparing `orbitkit-0.6.8.tar` & `orbitkit-0.6.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:12:33.000000 orbitkit-0.6.8/
--rw-r--r--   0 crown      (501) staff       (20)     1073 2020-10-28 02:45:18.000000 orbitkit-0.6.8/LICENSE
--rw-r--r--   0 crown      (501) staff       (20)      118 2022-01-24 08:00:21.000000 orbitkit-0.6.8/MANIFEST.in
--rw-r--r--   0 crown      (501) staff       (20)     3137 2024-05-14 05:12:33.000000 orbitkit-0.6.8/PKG-INFO
--rw-r--r--   0 crown      (501) staff       (20)     1684 2023-05-25 06:23:46.000000 orbitkit-0.6.8/README.md
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:12:32.000000 orbitkit-0.6.8/orbitkit/
--rw-r--r--   0 crown      (501) staff       (20)        6 2024-05-14 05:12:12.000000 orbitkit-0.6.8/orbitkit/VERSION
--rw-r--r--   0 crown      (501) staff       (20)      292 2023-05-25 06:23:46.000000 orbitkit-0.6.8/orbitkit/__init__.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:12:32.000000 orbitkit-0.6.8/orbitkit/id_srv/
--rw-r--r--   0 crown      (501) staff       (20)       22 2021-12-26 09:49:52.000000 orbitkit-0.6.8/orbitkit/id_srv/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     3598 2023-12-06 02:14:34.000000 orbitkit-0.6.8/orbitkit/id_srv/id_gen.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:12:33.000000 orbitkit-0.6.8/orbitkit/lark_send/
--rw-r--r--   0 crown      (501) staff       (20)       20 2022-01-05 07:16:58.000000 orbitkit-0.6.8/orbitkit/lark_send/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     6886 2023-09-11 08:05:37.000000 orbitkit-0.6.8/orbitkit/lark_send/lark.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:12:33.000000 orbitkit-0.6.8/orbitkit/pdf_embedding/
--rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.6.8/orbitkit/pdf_embedding/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)    10265 2024-01-31 06:10:24.000000 orbitkit-0.6.8/orbitkit/pdf_embedding/pdf_txt_embedding.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:12:33.000000 orbitkit-0.6.8/orbitkit/pdf_extractor/
--rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.6.8/orbitkit/pdf_extractor/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)      898 2023-08-07 08:25:29.000000 orbitkit-0.6.8/orbitkit/pdf_extractor/exceptions.py
--rw-r--r--   0 crown      (501) staff       (20)      621 2023-05-10 06:21:50.000000 orbitkit-0.6.8/orbitkit/pdf_extractor/pdf_block_extractor_base.py
--rw-r--r--   0 crown      (501) staff       (20)     6340 2024-01-31 05:10:37.000000 orbitkit-0.6.8/orbitkit/pdf_extractor/pdf_block_extractor_v1.py
--rw-r--r--   0 crown      (501) staff       (20)    13790 2024-01-31 05:10:37.000000 orbitkit-0.6.8/orbitkit/pdf_extractor/pdf_block_extractor_v2.py
--rw-r--r--   0 crown      (501) staff       (20)    12635 2024-01-31 06:10:24.000000 orbitkit-0.6.8/orbitkit/pdf_extractor/pdf_extractor_azure.py
--rw-r--r--   0 crown      (501) staff       (20)    10724 2024-01-31 06:28:50.000000 orbitkit-0.6.8/orbitkit/pdf_extractor/pdf_extractor_orbit.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:12:33.000000 orbitkit-0.6.8/orbitkit/pdf_extractor_simple/
--rw-r--r--   0 crown      (501) staff       (20)     1233 2024-05-14 03:51:14.000000 orbitkit-0.6.8/orbitkit/pdf_extractor_simple/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)      785 2024-04-23 09:31:55.000000 orbitkit-0.6.8/orbitkit/pdf_extractor_simple/base.py
--rw-r--r--   0 crown      (501) staff       (20)     4593 2024-05-11 05:36:15.000000 orbitkit-0.6.8/orbitkit/pdf_extractor_simple/cloud_provider.py
--rw-r--r--   0 crown      (501) staff       (20)     4078 2024-05-11 07:46:00.000000 orbitkit-0.6.8/orbitkit/pdf_extractor_simple/core.py
--rw-r--r--   0 crown      (501) staff       (20)       59 2024-04-23 05:22:52.000000 orbitkit-0.6.8/orbitkit/pdf_extractor_simple/exceptions.py
--rw-r--r--   0 crown      (501) staff       (20)     8078 2024-05-10 08:28:59.000000 orbitkit-0.6.8/orbitkit/pdf_extractor_simple/extractors.py
--rw-r--r--   0 crown      (501) staff       (20)     1002 2024-05-14 04:33:27.000000 orbitkit-0.6.8/orbitkit/pdf_extractor_simple/utils.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:12:33.000000 orbitkit-0.6.8/orbitkit/util/
--rw-r--r--   0 crown      (501) staff       (20)      997 2024-04-25 01:40:35.000000 orbitkit-0.6.8/orbitkit/util/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     2137 2024-04-25 01:41:05.000000 orbitkit-0.6.8/orbitkit/util/common.py
--rw-r--r--   0 crown      (501) staff       (20)      365 2024-04-25 01:29:34.000000 orbitkit-0.6.8/orbitkit/util/util_aliyun.py
--rw-r--r--   0 crown      (501) staff       (20)     1000 2024-05-11 08:50:16.000000 orbitkit-0.6.8/orbitkit/util/util_aliyun_oss_simple.py
--rw-r--r--   0 crown      (501) staff       (20)     2122 2024-01-31 06:27:51.000000 orbitkit-0.6.8/orbitkit/util/util_aws.py
--rw-r--r--   0 crown      (501) staff       (20)     5837 2024-02-21 06:49:24.000000 orbitkit-0.6.8/orbitkit/util/util_aws_s3_wrapper.py
--rw-r--r--   0 crown      (501) staff       (20)     4698 2024-05-14 05:11:29.000000 orbitkit-0.6.8/orbitkit/util/util_date.py
--rw-r--r--   0 crown      (501) staff       (20)      189 2024-01-24 10:42:04.000000 orbitkit-0.6.8/orbitkit/util/util_html.py
--rw-r--r--   0 crown      (501) staff       (20)      751 2023-11-13 08:39:24.000000 orbitkit-0.6.8/orbitkit/util/util_md5.py
--rw-r--r--   0 crown      (501) staff       (20)     2023 2024-04-25 01:40:35.000000 orbitkit-0.6.8/orbitkit/util/util_selenium.py
--rw-r--r--   0 crown      (501) staff       (20)      336 2023-11-13 08:30:33.000000 orbitkit-0.6.8/orbitkit/util/util_simple_timer.py
--rw-r--r--   0 crown      (501) staff       (20)      723 2024-04-25 01:43:47.000000 orbitkit-0.6.8/orbitkit/util/util_str.py
--rw-r--r--   0 crown      (501) staff       (20)    22822 2024-04-29 03:18:06.000000 orbitkit-0.6.8/orbitkit/util/util_type_mapping.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:12:32.000000 orbitkit-0.6.8/orbitkit.egg-info/
--rw-r--r--   0 crown      (501) staff       (20)     3137 2024-05-14 05:12:32.000000 orbitkit-0.6.8/orbitkit.egg-info/PKG-INFO
--rw-r--r--   0 crown      (501) staff       (20)     1452 2024-05-14 05:12:32.000000 orbitkit-0.6.8/orbitkit.egg-info/SOURCES.txt
--rw-r--r--   0 crown      (501) staff       (20)        1 2024-05-14 05:12:32.000000 orbitkit-0.6.8/orbitkit.egg-info/dependency_links.txt
--rw-r--r--   0 crown      (501) staff       (20)        1 2024-05-14 05:12:32.000000 orbitkit-0.6.8/orbitkit.egg-info/not-zip-safe
--rw-r--r--   0 crown      (501) staff       (20)       74 2024-05-14 05:12:32.000000 orbitkit-0.6.8/orbitkit.egg-info/requires.txt
--rw-r--r--   0 crown      (501) staff       (20)        9 2024-05-14 05:12:32.000000 orbitkit-0.6.8/orbitkit.egg-info/top_level.txt
--rw-r--r--   0 crown      (501) staff       (20)       38 2024-05-14 05:12:33.000000 orbitkit-0.6.8/setup.cfg
--rw-r--r--   0 crown      (501) staff       (20)     1530 2024-01-24 09:21:31.000000 orbitkit-0.6.8/setup.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:52:50.000000 orbitkit-0.6.9/
+-rw-r--r--   0 crown      (501) staff       (20)     1073 2020-10-28 02:45:18.000000 orbitkit-0.6.9/LICENSE
+-rw-r--r--   0 crown      (501) staff       (20)      118 2022-01-24 08:00:21.000000 orbitkit-0.6.9/MANIFEST.in
+-rw-r--r--   0 crown      (501) staff       (20)     3137 2024-05-14 05:52:50.000000 orbitkit-0.6.9/PKG-INFO
+-rw-r--r--   0 crown      (501) staff       (20)     1684 2023-05-25 06:23:46.000000 orbitkit-0.6.9/README.md
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:52:50.000000 orbitkit-0.6.9/orbitkit/
+-rw-r--r--   0 crown      (501) staff       (20)        6 2024-05-14 05:52:12.000000 orbitkit-0.6.9/orbitkit/VERSION
+-rw-r--r--   0 crown      (501) staff       (20)      292 2023-05-25 06:23:46.000000 orbitkit-0.6.9/orbitkit/__init__.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:52:50.000000 orbitkit-0.6.9/orbitkit/id_srv/
+-rw-r--r--   0 crown      (501) staff       (20)       22 2021-12-26 09:49:52.000000 orbitkit-0.6.9/orbitkit/id_srv/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     3598 2023-12-06 02:14:34.000000 orbitkit-0.6.9/orbitkit/id_srv/id_gen.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:52:50.000000 orbitkit-0.6.9/orbitkit/lark_send/
+-rw-r--r--   0 crown      (501) staff       (20)       20 2022-01-05 07:16:58.000000 orbitkit-0.6.9/orbitkit/lark_send/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     6886 2023-09-11 08:05:37.000000 orbitkit-0.6.9/orbitkit/lark_send/lark.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:52:50.000000 orbitkit-0.6.9/orbitkit/pdf_embedding/
+-rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.6.9/orbitkit/pdf_embedding/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)    10265 2024-01-31 06:10:24.000000 orbitkit-0.6.9/orbitkit/pdf_embedding/pdf_txt_embedding.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:52:50.000000 orbitkit-0.6.9/orbitkit/pdf_extractor/
+-rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.6.9/orbitkit/pdf_extractor/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)      898 2023-08-07 08:25:29.000000 orbitkit-0.6.9/orbitkit/pdf_extractor/exceptions.py
+-rw-r--r--   0 crown      (501) staff       (20)      621 2023-05-10 06:21:50.000000 orbitkit-0.6.9/orbitkit/pdf_extractor/pdf_block_extractor_base.py
+-rw-r--r--   0 crown      (501) staff       (20)     6340 2024-01-31 05:10:37.000000 orbitkit-0.6.9/orbitkit/pdf_extractor/pdf_block_extractor_v1.py
+-rw-r--r--   0 crown      (501) staff       (20)    13790 2024-01-31 05:10:37.000000 orbitkit-0.6.9/orbitkit/pdf_extractor/pdf_block_extractor_v2.py
+-rw-r--r--   0 crown      (501) staff       (20)    12635 2024-01-31 06:10:24.000000 orbitkit-0.6.9/orbitkit/pdf_extractor/pdf_extractor_azure.py
+-rw-r--r--   0 crown      (501) staff       (20)    10724 2024-01-31 06:28:50.000000 orbitkit-0.6.9/orbitkit/pdf_extractor/pdf_extractor_orbit.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:52:50.000000 orbitkit-0.6.9/orbitkit/pdf_extractor_simple/
+-rw-r--r--   0 crown      (501) staff       (20)     1233 2024-05-14 03:51:14.000000 orbitkit-0.6.9/orbitkit/pdf_extractor_simple/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)      785 2024-04-23 09:31:55.000000 orbitkit-0.6.9/orbitkit/pdf_extractor_simple/base.py
+-rw-r--r--   0 crown      (501) staff       (20)     4593 2024-05-11 05:36:15.000000 orbitkit-0.6.9/orbitkit/pdf_extractor_simple/cloud_provider.py
+-rw-r--r--   0 crown      (501) staff       (20)     4078 2024-05-11 07:46:00.000000 orbitkit-0.6.9/orbitkit/pdf_extractor_simple/core.py
+-rw-r--r--   0 crown      (501) staff       (20)       59 2024-04-23 05:22:52.000000 orbitkit-0.6.9/orbitkit/pdf_extractor_simple/exceptions.py
+-rw-r--r--   0 crown      (501) staff       (20)     8162 2024-05-14 05:52:12.000000 orbitkit-0.6.9/orbitkit/pdf_extractor_simple/extractors.py
+-rw-r--r--   0 crown      (501) staff       (20)     1002 2024-05-14 04:33:27.000000 orbitkit-0.6.9/orbitkit/pdf_extractor_simple/utils.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:52:50.000000 orbitkit-0.6.9/orbitkit/util/
+-rw-r--r--   0 crown      (501) staff       (20)      997 2024-04-25 01:40:35.000000 orbitkit-0.6.9/orbitkit/util/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     2137 2024-04-25 01:41:05.000000 orbitkit-0.6.9/orbitkit/util/common.py
+-rw-r--r--   0 crown      (501) staff       (20)      365 2024-04-25 01:29:34.000000 orbitkit-0.6.9/orbitkit/util/util_aliyun.py
+-rw-r--r--   0 crown      (501) staff       (20)     1000 2024-05-11 08:50:16.000000 orbitkit-0.6.9/orbitkit/util/util_aliyun_oss_simple.py
+-rw-r--r--   0 crown      (501) staff       (20)     2122 2024-01-31 06:27:51.000000 orbitkit-0.6.9/orbitkit/util/util_aws.py
+-rw-r--r--   0 crown      (501) staff       (20)     5837 2024-02-21 06:49:24.000000 orbitkit-0.6.9/orbitkit/util/util_aws_s3_wrapper.py
+-rw-r--r--   0 crown      (501) staff       (20)     4698 2024-05-14 05:11:29.000000 orbitkit-0.6.9/orbitkit/util/util_date.py
+-rw-r--r--   0 crown      (501) staff       (20)      189 2024-01-24 10:42:04.000000 orbitkit-0.6.9/orbitkit/util/util_html.py
+-rw-r--r--   0 crown      (501) staff       (20)      751 2023-11-13 08:39:24.000000 orbitkit-0.6.9/orbitkit/util/util_md5.py
+-rw-r--r--   0 crown      (501) staff       (20)     2023 2024-04-25 01:40:35.000000 orbitkit-0.6.9/orbitkit/util/util_selenium.py
+-rw-r--r--   0 crown      (501) staff       (20)      336 2023-11-13 08:30:33.000000 orbitkit-0.6.9/orbitkit/util/util_simple_timer.py
+-rw-r--r--   0 crown      (501) staff       (20)      723 2024-04-25 01:43:47.000000 orbitkit-0.6.9/orbitkit/util/util_str.py
+-rw-r--r--   0 crown      (501) staff       (20)    22822 2024-04-29 03:18:06.000000 orbitkit-0.6.9/orbitkit/util/util_type_mapping.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-14 05:52:50.000000 orbitkit-0.6.9/orbitkit.egg-info/
+-rw-r--r--   0 crown      (501) staff       (20)     3137 2024-05-14 05:52:50.000000 orbitkit-0.6.9/orbitkit.egg-info/PKG-INFO
+-rw-r--r--   0 crown      (501) staff       (20)     1452 2024-05-14 05:52:50.000000 orbitkit-0.6.9/orbitkit.egg-info/SOURCES.txt
+-rw-r--r--   0 crown      (501) staff       (20)        1 2024-05-14 05:52:50.000000 orbitkit-0.6.9/orbitkit.egg-info/dependency_links.txt
+-rw-r--r--   0 crown      (501) staff       (20)        1 2024-05-14 05:52:50.000000 orbitkit-0.6.9/orbitkit.egg-info/not-zip-safe
+-rw-r--r--   0 crown      (501) staff       (20)       74 2024-05-14 05:52:50.000000 orbitkit-0.6.9/orbitkit.egg-info/requires.txt
+-rw-r--r--   0 crown      (501) staff       (20)        9 2024-05-14 05:52:50.000000 orbitkit-0.6.9/orbitkit.egg-info/top_level.txt
+-rw-r--r--   0 crown      (501) staff       (20)       38 2024-05-14 05:52:50.000000 orbitkit-0.6.9/setup.cfg
+-rw-r--r--   0 crown      (501) staff       (20)     1530 2024-01-24 09:21:31.000000 orbitkit-0.6.9/setup.py
```

### Comparing `orbitkit-0.6.8/LICENSE` & `orbitkit-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/PKG-INFO` & `orbitkit-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbitkit
-Version: 0.6.8
+Version: 0.6.9
 Summary: This project is only for Orbit Tech internal use.
 Home-page: https://github.com/clown-0726/orbitkit
 Author: Lilu Cao
 Author-email: lilu.cao@qq.com
 Maintainer: Lilu Cao
 Maintainer-email: lilu.cao@qq.com
 License: MIT License
```

### Comparing `orbitkit-0.6.8/README.md` & `orbitkit-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/id_srv/id_gen.py` & `orbitkit-0.6.9/orbitkit/id_srv/id_gen.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/lark_send/lark.py` & `orbitkit-0.6.9/orbitkit/lark_send/lark.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/pdf_embedding/pdf_txt_embedding.py` & `orbitkit-0.6.9/orbitkit/pdf_embedding/pdf_txt_embedding.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/pdf_extractor/exceptions.py` & `orbitkit-0.6.9/orbitkit/pdf_extractor/exceptions.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/pdf_extractor/pdf_block_extractor_base.py` & `orbitkit-0.6.9/orbitkit/pdf_extractor/pdf_block_extractor_base.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/pdf_extractor/pdf_block_extractor_v1.py` & `orbitkit-0.6.9/orbitkit/pdf_extractor/pdf_block_extractor_v1.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/pdf_extractor/pdf_block_extractor_v2.py` & `orbitkit-0.6.9/orbitkit/pdf_extractor/pdf_block_extractor_v2.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/pdf_extractor/pdf_extractor_azure.py` & `orbitkit-0.6.9/orbitkit/pdf_extractor/pdf_extractor_azure.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/pdf_extractor/pdf_extractor_orbit.py` & `orbitkit-0.6.9/orbitkit/pdf_extractor/pdf_extractor_orbit.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/pdf_extractor_simple/__init__.py` & `orbitkit-0.6.9/orbitkit/pdf_extractor_simple/__init__.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/pdf_extractor_simple/base.py` & `orbitkit-0.6.9/orbitkit/pdf_extractor_simple/base.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/pdf_extractor_simple/cloud_provider.py` & `orbitkit-0.6.9/orbitkit/pdf_extractor_simple/cloud_provider.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/pdf_extractor_simple/core.py` & `orbitkit-0.6.9/orbitkit/pdf_extractor_simple/core.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/pdf_extractor_simple/extractors.py` & `orbitkit-0.6.9/orbitkit/pdf_extractor_simple/extractors.py`

 * *Files 9% similar despite different names*

```diff
@@ -99,32 +99,33 @@
 
     def extract(self, local_path_pdf: str):
         self.local_path_pdf_txt = local_path_pdf + ".txt"
         try:
             with open(local_path_pdf, 'rb') as pdf_file, open(self.local_path_pdf_txt, "w+", encoding="utf-8") as pdf_file_txt:
                 pdf_reader = pypdf.PdfReader(pdf_file)
                 for index, page_obj in enumerate(pdf_reader.pages, start=1):
+                    logger.warning(f"page: {str(index)} is processing...")
                     logger.debug(f"page: {str(index)} --------------------------------------------------------------------------------------")
                     full_text = page_obj.extract_text().strip()
 
                     if len(full_text) < 10:
-                        logger.debug("1) low to 10 char length...")
+                        logger.warning("1) low to 10 char length...")
                         full_text_ocr = self._extract_by_ocr(index, local_path_pdf)
                         if len(full_text_ocr) < 10:
-                            logger.debug("1.1) OCR failed with char length >>>>>>>>>>>>>>>")
+                            logger.warning("1.1) OCR failed with char length >>>>>>>>>>>>>>>")
                             logger.debug(full_text_ocr + "\n<<<<<<<<<<<<<<<<<<<<<<<<<")
                             self.judge_length_wrong += 1
                         else:
-                            logger.debug("1.2) OCR extract success >>>>>>>>>>>>>>>")
+                            logger.warning("1.2) OCR extract success >>>>>>>>>>>>>>>")
                             logger.debug(full_text_ocr + "\n<<<<<<<<<<<<<<<<<<<<<<<<<")
                             # OCR 提取的文本 > 10，不需要判断乱码问题
                             pdf_file_txt.write(json.dumps({"page_no": str(index), "text": full_text_ocr}, ensure_ascii=False))
                             pdf_file_txt.write('\n')
                     else:
-                        logger.debug("2) good larger than 10 char length...")
+                        logger.debug("2) Good, larger than 10 char length...")
                         if is_no_mess_code(full_text):
                             logger.debug("2.1) No mess code >>>>>>>>>>>>>>>>>>>>>>>>>")
                             logger.debug(full_text + "\n<<<<<<<<<<<<<<<<<<<<<<<<<<<<")
                             # >10 没有乱码，则直接写入
                             try:
                                 pdf_file_txt.write(
                                     json.dumps({"page_no": str(index), "text": full_text}, ensure_ascii=False))
@@ -132,15 +133,15 @@
                             except UnicodeEncodeError as e:
                                 full_text = full_text.encode('utf-8', 'replace').decode('utf-8').strip()
                                 pdf_file_txt.write(
                                     json.dumps({"page_no": str(index), "text": full_text}, ensure_ascii=False))
                                 pdf_file_txt.write('\n')
                                 logger.warning(f"{str(index)} -->  {e}")
                         else:
-                            logger.debug("2.2) with mess code so go OCR >>>>>>>>>>>>>>>>")
+                            logger.warning("2.2) with mess code so go OCR >>>>>>>>>>>>>>>>")
                             logger.debug(full_text + "\n<<<<<<<<<<<<<<<<<<<<<<<<<<<<")
                             full_text_ocr = self._extract_by_ocr(index, local_path_pdf)
                             logger.debug(">>>>>>>>>>>>>>>>\n" + full_text_ocr + "\n<<<<<<<<<<<<<<<<<<<<<<<<<<<<")
                             if len(full_text_ocr) < 10:
                                 logger.debug("2.2.1) err")
                                 self.judge_length_wrong += 1
                             else:
```

### Comparing `orbitkit-0.6.8/orbitkit/pdf_extractor_simple/utils.py` & `orbitkit-0.6.9/orbitkit/pdf_extractor_simple/utils.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/util/__init__.py` & `orbitkit-0.6.9/orbitkit/util/__init__.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/util/common.py` & `orbitkit-0.6.9/orbitkit/util/common.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/util/util_aliyun_oss_simple.py` & `orbitkit-0.6.9/orbitkit/util/util_aliyun_oss_simple.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/util/util_aws.py` & `orbitkit-0.6.9/orbitkit/util/util_aws.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/util/util_aws_s3_wrapper.py` & `orbitkit-0.6.9/orbitkit/util/util_aws_s3_wrapper.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/util/util_date.py` & `orbitkit-0.6.9/orbitkit/util/util_date.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/util/util_md5.py` & `orbitkit-0.6.9/orbitkit/util/util_md5.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/util/util_selenium.py` & `orbitkit-0.6.9/orbitkit/util/util_selenium.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/util/util_str.py` & `orbitkit-0.6.9/orbitkit/util/util_str.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit/util/util_type_mapping.py` & `orbitkit-0.6.9/orbitkit/util/util_type_mapping.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/orbitkit.egg-info/PKG-INFO` & `orbitkit-0.6.9/orbitkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbitkit
-Version: 0.6.8
+Version: 0.6.9
 Summary: This project is only for Orbit Tech internal use.
 Home-page: https://github.com/clown-0726/orbitkit
 Author: Lilu Cao
 Author-email: lilu.cao@qq.com
 Maintainer: Lilu Cao
 Maintainer-email: lilu.cao@qq.com
 License: MIT License
```

### Comparing `orbitkit-0.6.8/orbitkit.egg-info/SOURCES.txt` & `orbitkit-0.6.9/orbitkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.8/setup.py` & `orbitkit-0.6.9/setup.py`

 * *Files identical despite different names*

