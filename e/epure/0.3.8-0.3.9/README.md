# Comparing `tmp/epure-0.3.8.tar.gz` & `tmp/epure-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epure-0.3.8.tar", max compression
+gzip compressed data, was "epure-0.3.9.tar", max compression
```

## Comparing `epure-0.3.8.tar` & `epure-0.3.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0      554 2023-12-18 11:12:41.221860 epure-0.3.8/epure/__init__.py
--rw-r--r--   0        0        0       41 2023-11-07 16:52:30.754332 epure-0.3.8/epure/dbs.py
--rw-r--r--   0        0        0    14962 2024-02-29 22:59:37.602196 epure-0.3.8/epure/epure.py
--rw-r--r--   0        0        0     1142 2023-12-12 17:41:18.741223 epure-0.3.8/epure/errors.py
--rw-r--r--   0        0        0       90 2023-11-07 16:52:30.754332 epure-0.3.8/epure/files.py
--rw-r--r--   0        0        0       71 2023-11-07 16:52:30.754332 epure-0.3.8/epure/generics.py
--rw-r--r--   0        0        0        0 2023-11-07 16:52:30.754332 epure-0.3.8/epure/helpers/__init__.py
--rw-r--r--   0        0        0       90 2023-11-07 16:52:30.754332 epure-0.3.8/epure/helpers/dict_helper.py
--rw-r--r--   0        0        0     1402 2023-11-07 16:52:30.754332 epure-0.3.8/epure/helpers/string_helper.py
--rw-r--r--   0        0        0     1302 2023-12-19 11:29:21.861685 epure-0.3.8/epure/helpers/type_helper.py
--rw-r--r--   0        0        0     1298 2023-12-12 17:41:18.742225 epure-0.3.8/epure/named.py
--rw-r--r--   0        0        0        0 2023-11-07 16:52:30.754332 epure-0.3.8/epure/parser/__init__.py
--rw-r--r--   0        0        0     4582 2023-12-18 10:04:36.568326 epure-0.3.8/epure/parser/bin_operation.py
--rw-r--r--   0        0        0     4942 2023-11-07 16:52:30.754332 epure-0.3.8/epure/parser/binary.py
--rw-r--r--   0        0        0        0 2023-11-11 15:26:22.818810 epure-0.3.8/epure/parser/inspect_parser/__init__.py
--rw-r--r--   0        0        0     1549 2023-12-18 10:04:36.568326 epure-0.3.8/epure/parser/inspect_parser/column_proxy.py
--rw-r--r--   0        0        0     1271 2023-12-29 18:55:19.428651 epure-0.3.8/epure/parser/inspect_parser/domain.py
--rw-r--r--   0        0        0    12645 2024-02-15 23:38:36.785029 epure-0.3.8/epure/parser/inspect_parser/inspect_parser.py
--rw-r--r--   0        0        0     2413 2024-02-24 17:42:43.690896 epure-0.3.8/epure/parser/inspect_parser/model.py
--rw-r--r--   0        0        0     4032 2023-12-26 15:00:03.958463 epure-0.3.8/epure/parser/inspect_parser/term.py
--rw-r--r--   0        0        0     7055 2023-12-29 18:54:53.974968 epure-0.3.8/epure/parser/leaf.py
--rw-r--r--   0        0        0       62 2023-12-18 10:04:36.568326 epure-0.3.8/epure/parser/proxy_base_cls.py
--rw-r--r--   0        0        0     8138 2023-11-07 16:52:30.754332 epure-0.3.8/epure/parser/term.py
--rw-r--r--   0        0        0     3398 2023-11-07 16:52:30.754332 epure-0.3.8/epure/parser/term_debugger.py
--rw-r--r--   0        0        0     7982 2023-12-18 11:13:12.148800 epure-0.3.8/epure/parser/term_parser.py
--rw-r--r--   0        0        0       44 2023-11-07 16:52:30.754332 epure-0.3.8/epure/resource/__init__.py
--rw-r--r--   0        0        0     1565 2023-12-25 12:46:51.802123 epure-0.3.8/epure/resource/data_promise.py
--rw-r--r--   0        0        0        0 2023-11-07 16:52:30.769952 epure-0.3.8/epure/resource/db/__init__.py
--rw-r--r--   0        0        0     3366 2024-01-29 19:05:24.499649 epure-0.3.8/epure/resource/db/constraint.py
--rw-r--r--   0        0        0     4353 2023-12-06 17:19:44.089088 epure-0.3.8/epure/resource/db/db.py
--rw-r--r--   0        0        0      863 2023-11-07 16:52:30.769952 epure-0.3.8/epure/resource/db/db_entity.py
--rw-r--r--   0        0        0     2896 2023-12-07 18:05:04.199047 epure-0.3.8/epure/resource/db/db_entity_resource.py
--rw-r--r--   0        0        0     2289 2023-11-07 16:52:30.769952 epure-0.3.8/epure/resource/db/pseudo_table.py
--rw-r--r--   0        0        0     5658 2023-11-07 16:52:30.769952 epure-0.3.8/epure/resource/db/query_old.py
--rw-r--r--   0        0        0     2786 2023-11-07 16:52:30.769952 epure-0.3.8/epure/resource/db/select_query.py
--rw-r--r--   0        0        0    20714 2024-02-08 16:20:15.560350 epure-0.3.8/epure/resource/db/table.py
--rw-r--r--   0        0        0     1236 2024-01-13 18:25:19.982737 epure-0.3.8/epure/resource/db/table_column.py
--rw-r--r--   0        0        0    11139 2024-01-19 21:10:28.490653 epure-0.3.8/epure/resource/db/table_header.py
--rw-r--r--   0        0        0     6968 2024-01-19 20:08:40.993526 epure-0.3.8/epure/resource/db/table_storage.py
--rw-r--r--   0        0        0     4300 2023-11-07 16:52:30.769952 epure-0.3.8/epure/resource/db/term.py
--rw-r--r--   0        0        0        0 2023-11-07 16:52:30.769952 epure-0.3.8/epure/resource/edata/__init__.py
--rw-r--r--   0        0        0     2891 2024-01-26 11:40:13.227841 epure-0.3.8/epure/resource/edata/ecollection_metacls.py
--rw-r--r--   0        0        0    12674 2024-01-25 19:49:48.422131 epure-0.3.8/epure/resource/edata/edata.py
--rw-r--r--   0        0        0    16745 2024-01-26 15:28:21.932658 epure-0.3.8/epure/resource/edata/elist.py
--rw-r--r--   0        0        0     2787 2023-12-18 11:22:17.211302 epure-0.3.8/epure/resource/edata/proto.py
--rw-r--r--   0        0        0        0 2023-11-07 16:52:30.769952 epure-0.3.8/epure/resource/file/__init__.py
--rw-r--r--   0        0        0      250 2023-11-07 16:52:30.769952 epure-0.3.8/epure/resource/file/file_storage.py
--rw-r--r--   0        0        0     1220 2023-11-07 16:52:30.769952 epure-0.3.8/epure/resource/file/ini_file.py
--rw-r--r--   0        0        0     2108 2023-11-07 16:52:30.769952 epure-0.3.8/epure/resource/file/ini_section.py
--rw-r--r--   0        0        0      440 2023-11-07 16:52:30.769952 epure-0.3.8/epure/resource/file/json_file.py
--rw-r--r--   0        0        0        0 2023-11-07 16:52:30.769952 epure-0.3.8/epure/resource/gres/__init__.py
--rw-r--r--   0        0        0    11802 2023-12-29 18:52:22.976702 epure-0.3.8/epure/resource/gres/gres_db.py
--rw-r--r--   0        0        0      131 2023-11-07 16:52:30.769952 epure-0.3.8/epure/resource/gres/gres_entity.py
--rw-r--r--   0        0        0     3682 2023-11-07 16:52:30.769952 epure-0.3.8/epure/resource/gres/gres_header.py
--rw-r--r--   0        0        0     5906 2024-02-08 15:22:59.329812 epure-0.3.8/epure/resource/gres/gres_table.py
--rw-r--r--   0        0        0     1553 2023-12-18 11:26:57.236954 epure-0.3.8/epure/resource/gres/jsonb_table.py
--rw-r--r--   0        0        0     2051 2024-02-25 13:04:00.707894 epure-0.3.8/epure/resource/join_resource/join_resource.py
--rw-r--r--   0        0        0       53 2023-11-07 16:52:30.769952 epure-0.3.8/epure/resource/lite_db/lite_db.py
--rw-r--r--   0        0        0       65 2023-11-07 16:52:30.769952 epure-0.3.8/epure/resource/lite_db/lite_table.py
--rw-r--r--   0        0        0     1932 2024-02-08 16:05:08.020421 epure-0.3.8/epure/resource/resource.py
--rw-r--r--   0        0        0     3075 2024-01-17 17:55:55.067265 epure-0.3.8/epure/resource/savable.py
--rw-r--r--   0        0        0      943 2024-04-22 23:19:19.024171 epure-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     2116 2024-04-22 23:17:09.913303 epure-0.3.8/README.md
--rw-r--r--   0        0        0     2806 1970-01-01 00:00:00.000000 epure-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      554 2023-12-18 11:12:41.221860 epure-0.3.9/epure/__init__.py
+-rw-r--r--   0        0        0       41 2023-11-07 16:52:30.754332 epure-0.3.9/epure/dbs.py
+-rw-r--r--   0        0        0    14962 2024-02-29 22:59:37.602196 epure-0.3.9/epure/epure.py
+-rw-r--r--   0        0        0     1142 2023-12-12 17:41:18.741223 epure-0.3.9/epure/errors.py
+-rw-r--r--   0        0        0       90 2023-11-07 16:52:30.754332 epure-0.3.9/epure/files.py
+-rw-r--r--   0        0        0       71 2023-11-07 16:52:30.754332 epure-0.3.9/epure/generics.py
+-rw-r--r--   0        0        0        0 2023-11-07 16:52:30.754332 epure-0.3.9/epure/helpers/__init__.py
+-rw-r--r--   0        0        0       90 2023-11-07 16:52:30.754332 epure-0.3.9/epure/helpers/dict_helper.py
+-rw-r--r--   0        0        0     1402 2023-11-07 16:52:30.754332 epure-0.3.9/epure/helpers/string_helper.py
+-rw-r--r--   0        0        0     1302 2023-12-19 11:29:21.861685 epure-0.3.9/epure/helpers/type_helper.py
+-rw-r--r--   0        0        0     1298 2023-12-12 17:41:18.742225 epure-0.3.9/epure/named.py
+-rw-r--r--   0        0        0        0 2023-11-07 16:52:30.754332 epure-0.3.9/epure/parser/__init__.py
+-rw-r--r--   0        0        0     4582 2023-12-18 10:04:36.568326 epure-0.3.9/epure/parser/bin_operation.py
+-rw-r--r--   0        0        0     4942 2023-11-07 16:52:30.754332 epure-0.3.9/epure/parser/binary.py
+-rw-r--r--   0        0        0        0 2023-11-11 15:26:22.818810 epure-0.3.9/epure/parser/inspect_parser/__init__.py
+-rw-r--r--   0        0        0     1549 2023-12-18 10:04:36.568326 epure-0.3.9/epure/parser/inspect_parser/column_proxy.py
+-rw-r--r--   0        0        0     1271 2023-12-29 18:55:19.428651 epure-0.3.9/epure/parser/inspect_parser/domain.py
+-rw-r--r--   0        0        0    12645 2024-02-15 23:38:36.785029 epure-0.3.9/epure/parser/inspect_parser/inspect_parser.py
+-rw-r--r--   0        0        0     2413 2024-02-24 17:42:43.690896 epure-0.3.9/epure/parser/inspect_parser/model.py
+-rw-r--r--   0        0        0     4032 2023-12-26 15:00:03.958463 epure-0.3.9/epure/parser/inspect_parser/term.py
+-rw-r--r--   0        0        0     7055 2023-12-29 18:54:53.974968 epure-0.3.9/epure/parser/leaf.py
+-rw-r--r--   0        0        0       62 2023-12-18 10:04:36.568326 epure-0.3.9/epure/parser/proxy_base_cls.py
+-rw-r--r--   0        0        0     8138 2023-11-07 16:52:30.754332 epure-0.3.9/epure/parser/term.py
+-rw-r--r--   0        0        0     3398 2023-11-07 16:52:30.754332 epure-0.3.9/epure/parser/term_debugger.py
+-rw-r--r--   0        0        0     7982 2023-12-18 11:13:12.148800 epure-0.3.9/epure/parser/term_parser.py
+-rw-r--r--   0        0        0       44 2023-11-07 16:52:30.754332 epure-0.3.9/epure/resource/__init__.py
+-rw-r--r--   0        0        0     1565 2023-12-25 12:46:51.802123 epure-0.3.9/epure/resource/data_promise.py
+-rw-r--r--   0        0        0        0 2023-11-07 16:52:30.769952 epure-0.3.9/epure/resource/db/__init__.py
+-rw-r--r--   0        0        0     3366 2024-01-29 19:05:24.499649 epure-0.3.9/epure/resource/db/constraint.py
+-rw-r--r--   0        0        0     4353 2023-12-06 17:19:44.089088 epure-0.3.9/epure/resource/db/db.py
+-rw-r--r--   0        0        0      863 2023-11-07 16:52:30.769952 epure-0.3.9/epure/resource/db/db_entity.py
+-rw-r--r--   0        0        0     2896 2023-12-07 18:05:04.199047 epure-0.3.9/epure/resource/db/db_entity_resource.py
+-rw-r--r--   0        0        0     2289 2023-11-07 16:52:30.769952 epure-0.3.9/epure/resource/db/pseudo_table.py
+-rw-r--r--   0        0        0     5658 2023-11-07 16:52:30.769952 epure-0.3.9/epure/resource/db/query_old.py
+-rw-r--r--   0        0        0     2786 2023-11-07 16:52:30.769952 epure-0.3.9/epure/resource/db/select_query.py
+-rw-r--r--   0        0        0    20714 2024-02-08 16:20:15.560350 epure-0.3.9/epure/resource/db/table.py
+-rw-r--r--   0        0        0     1236 2024-01-13 18:25:19.982737 epure-0.3.9/epure/resource/db/table_column.py
+-rw-r--r--   0        0        0    11139 2024-01-19 21:10:28.490653 epure-0.3.9/epure/resource/db/table_header.py
+-rw-r--r--   0        0        0     6968 2024-01-19 20:08:40.993526 epure-0.3.9/epure/resource/db/table_storage.py
+-rw-r--r--   0        0        0     4300 2023-11-07 16:52:30.769952 epure-0.3.9/epure/resource/db/term.py
+-rw-r--r--   0        0        0        0 2023-11-07 16:52:30.769952 epure-0.3.9/epure/resource/edata/__init__.py
+-rw-r--r--   0        0        0     2891 2024-01-26 11:40:13.227841 epure-0.3.9/epure/resource/edata/ecollection_metacls.py
+-rw-r--r--   0        0        0    12666 2024-05-16 15:59:18.290258 epure-0.3.9/epure/resource/edata/edata.py
+-rw-r--r--   0        0        0    16745 2024-01-26 15:28:21.932658 epure-0.3.9/epure/resource/edata/elist.py
+-rw-r--r--   0        0        0     2787 2023-12-18 11:22:17.211302 epure-0.3.9/epure/resource/edata/proto.py
+-rw-r--r--   0        0        0        0 2023-11-07 16:52:30.769952 epure-0.3.9/epure/resource/file/__init__.py
+-rw-r--r--   0        0        0      250 2023-11-07 16:52:30.769952 epure-0.3.9/epure/resource/file/file_storage.py
+-rw-r--r--   0        0        0     1220 2023-11-07 16:52:30.769952 epure-0.3.9/epure/resource/file/ini_file.py
+-rw-r--r--   0        0        0     2108 2023-11-07 16:52:30.769952 epure-0.3.9/epure/resource/file/ini_section.py
+-rw-r--r--   0        0        0      440 2023-11-07 16:52:30.769952 epure-0.3.9/epure/resource/file/json_file.py
+-rw-r--r--   0        0        0        0 2023-11-07 16:52:30.769952 epure-0.3.9/epure/resource/gres/__init__.py
+-rw-r--r--   0        0        0    11802 2023-12-29 18:52:22.976702 epure-0.3.9/epure/resource/gres/gres_db.py
+-rw-r--r--   0        0        0      131 2023-11-07 16:52:30.769952 epure-0.3.9/epure/resource/gres/gres_entity.py
+-rw-r--r--   0        0        0     3682 2023-11-07 16:52:30.769952 epure-0.3.9/epure/resource/gres/gres_header.py
+-rw-r--r--   0        0        0     5906 2024-02-08 15:22:59.329812 epure-0.3.9/epure/resource/gres/gres_table.py
+-rw-r--r--   0        0        0     1553 2023-12-18 11:26:57.236954 epure-0.3.9/epure/resource/gres/jsonb_table.py
+-rw-r--r--   0        0        0     2051 2024-02-25 13:04:00.707894 epure-0.3.9/epure/resource/join_resource/join_resource.py
+-rw-r--r--   0        0        0       53 2023-11-07 16:52:30.769952 epure-0.3.9/epure/resource/lite_db/lite_db.py
+-rw-r--r--   0        0        0       65 2023-11-07 16:52:30.769952 epure-0.3.9/epure/resource/lite_db/lite_table.py
+-rw-r--r--   0        0        0     1932 2024-02-08 16:05:08.020421 epure-0.3.9/epure/resource/resource.py
+-rw-r--r--   0        0        0     3075 2024-01-17 17:55:55.067265 epure-0.3.9/epure/resource/savable.py
+-rw-r--r--   0        0        0      943 2024-05-16 16:02:23.076047 epure-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     2116 2024-04-22 23:17:09.913303 epure-0.3.9/README.md
+-rw-r--r--   0        0        0     2806 1970-01-01 00:00:00.000000 epure-0.3.9/PKG-INFO
```

### Comparing `epure-0.3.8/epure/__init__.py` & `epure-0.3.9/epure/__init__.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/epure.py` & `epure-0.3.9/epure/epure.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/errors.py` & `epure-0.3.9/epure/errors.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/helpers/string_helper.py` & `epure-0.3.9/epure/helpers/string_helper.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/helpers/type_helper.py` & `epure-0.3.9/epure/helpers/type_helper.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/named.py` & `epure-0.3.9/epure/named.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/parser/bin_operation.py` & `epure-0.3.9/epure/parser/bin_operation.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/parser/binary.py` & `epure-0.3.9/epure/parser/binary.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/parser/inspect_parser/column_proxy.py` & `epure-0.3.9/epure/parser/inspect_parser/column_proxy.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/parser/inspect_parser/domain.py` & `epure-0.3.9/epure/parser/inspect_parser/domain.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/parser/inspect_parser/inspect_parser.py` & `epure-0.3.9/epure/parser/inspect_parser/inspect_parser.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/parser/inspect_parser/model.py` & `epure-0.3.9/epure/parser/inspect_parser/model.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/parser/inspect_parser/term.py` & `epure-0.3.9/epure/parser/inspect_parser/term.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/parser/leaf.py` & `epure-0.3.9/epure/parser/leaf.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/parser/term.py` & `epure-0.3.9/epure/parser/term.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/parser/term_debugger.py` & `epure-0.3.9/epure/parser/term_debugger.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/parser/term_parser.py` & `epure-0.3.9/epure/parser/term_parser.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/data_promise.py` & `epure-0.3.9/epure/resource/data_promise.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/db/constraint.py` & `epure-0.3.9/epure/resource/db/constraint.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/db/db.py` & `epure-0.3.9/epure/resource/db/db.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/db/db_entity.py` & `epure-0.3.9/epure/resource/db/db_entity.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/db/db_entity_resource.py` & `epure-0.3.9/epure/resource/db/db_entity_resource.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/db/pseudo_table.py` & `epure-0.3.9/epure/resource/db/pseudo_table.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/db/query_old.py` & `epure-0.3.9/epure/resource/db/query_old.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/db/select_query.py` & `epure-0.3.9/epure/resource/db/select_query.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/db/table.py` & `epure-0.3.9/epure/resource/db/table.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/db/table_column.py` & `epure-0.3.9/epure/resource/db/table_column.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/db/table_header.py` & `epure-0.3.9/epure/resource/db/table_header.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/db/table_storage.py` & `epure-0.3.9/epure/resource/db/table_storage.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/db/term.py` & `epure-0.3.9/epure/resource/db/term.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/edata/ecollection_metacls.py` & `epure-0.3.9/epure/resource/edata/ecollection_metacls.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/edata/edata.py` & `epure-0.3.9/epure/resource/edata/edata.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
 class TableData(EData):
     db:Resource
     data_id: UUID
     resource:Savable
 
     def __init__(self, data_id:object=None, resource:Resource=None, **kwargs) -> None:
-        if data_id != None and isinstance(data_id, str):
+        if data_id != None and is_uuid(data_id):
             data_id = UUID(data_id)
 
         if not isinstance(data_id, UUID):
             data_id = None
 
         super().__init__(data_id, resource)
```

### Comparing `epure-0.3.8/epure/resource/edata/elist.py` & `epure-0.3.9/epure/resource/edata/elist.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/edata/proto.py` & `epure-0.3.9/epure/resource/edata/proto.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/file/ini_file.py` & `epure-0.3.9/epure/resource/file/ini_file.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/file/ini_section.py` & `epure-0.3.9/epure/resource/file/ini_section.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/gres/gres_db.py` & `epure-0.3.9/epure/resource/gres/gres_db.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/gres/gres_header.py` & `epure-0.3.9/epure/resource/gres/gres_header.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/gres/gres_table.py` & `epure-0.3.9/epure/resource/gres/gres_table.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/gres/jsonb_table.py` & `epure-0.3.9/epure/resource/gres/jsonb_table.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/join_resource/join_resource.py` & `epure-0.3.9/epure/resource/join_resource/join_resource.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/resource.py` & `epure-0.3.9/epure/resource/resource.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/epure/resource/savable.py` & `epure-0.3.9/epure/resource/savable.py`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/pyproject.toml` & `epure-0.3.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "epure"
-version = "0.3.8"
+version = "0.3.9"
 description = "purest architecture"
 authors = ["Nikita Umarov <nagvalhm@yandex.ru>", "Pavel Pichugin"]
 license = "MIT"
 readme = "README.md"
 packages = [
     # { include = "pypi_stub" },
     { include = "epure" }
```

### Comparing `epure-0.3.8/README.md` & `epure-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `epure-0.3.8/PKG-INFO` & `epure-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epure
-Version: 0.3.8
+Version: 0.3.9
 Summary: purest architecture
 License: MIT
 Author: Nikita Umarov
 Author-email: nagvalhm@yandex.ru
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: epure Version: 0.3.8 Summary: purest architecture
+Metadata-Version: 2.1 Name: epure Version: 0.3.9 Summary: purest architecture
 License: MIT Author: Nikita Umarov Author-email: nagvalhm@yandex.ru Requires-
 Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: inflection (>=0.5.1,<0.6.0) Requires-Dist: jsonpickle
 (>=2.2.0,<3.0.0) Requires-Dist: psycopg2 (==2.9.3) Project-URL: Documentation,
 https://github.com/nagvalhm/epure/blob/main/README.md Project-URL: Homepage,
```

