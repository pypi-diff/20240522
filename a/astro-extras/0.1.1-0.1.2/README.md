# Comparing `tmp/astro_extras-0.1.1.tar.gz` & `tmp/astro_extras-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_extras-0.1.1.tar", last modified: Wed May 22 07:53:51 2024, max compression
+gzip compressed data, was "astro_extras-0.1.2.tar", last modified: Wed May 22 09:07:13 2024, max compression
```

## Comparing `astro_extras-0.1.1.tar` & `astro_extras-0.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 07:53:51.084584 astro_extras-0.1.1/
--rw-rw-r--   0 kol       (1000) kol       (1000)     1074 2023-11-17 10:43:31.000000 astro_extras-0.1.1/LICENSE
--rw-rw-r--   0 kol       (1000) kol       (1000)       24 2023-10-26 14:10:20.000000 astro_extras-0.1.1/MANIFEST.in
--rw-r--r--   0 kol       (1000) kol       (1000)     7920 2024-05-22 07:53:51.084584 astro_extras-0.1.1/PKG-INFO
--rw-rw-r--   0 kol       (1000) kol       (1000)     7444 2023-11-20 09:59:52.000000 astro_extras-0.1.1/README.md
--rw-rw-r--   0 kol       (1000) kol       (1000)      352 2023-10-26 14:10:20.000000 astro_extras-0.1.1/pyproject.toml
--rw-rw-r--   0 kol       (1000) kol       (1000)      288 2024-05-22 07:52:04.000000 astro_extras-0.1.1/requirements.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)       38 2024-05-22 07:53:51.088584 astro_extras-0.1.1/setup.cfg
--rw-rw-r--   0 kol       (1000) kol       (1000)     1193 2024-05-22 07:52:04.000000 astro_extras-0.1.1/setup.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 07:53:51.044584 astro_extras-0.1.1/src/
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 07:53:51.056584 astro_extras-0.1.1/src/astro_extras/
--rw-rw-r--   0 kol       (1000) kol       (1000)     1206 2024-05-22 07:52:04.000000 astro_extras-0.1.1/src/astro_extras/__init__.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 07:53:51.080584 astro_extras-0.1.1/src/astro_extras/hooks/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.1/src/astro_extras/hooks/__init__.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 07:53:51.080584 astro_extras-0.1.1/src/astro_extras/operators/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.1/src/astro_extras/operators/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     3861 2024-04-06 11:05:12.000000 astro_extras-0.1.1/src/astro_extras/operators/direct.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    18221 2024-05-22 07:52:04.000000 astro_extras-0.1.1/src/astro_extras/operators/session.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    52923 2024-05-22 07:52:50.000000 astro_extras-0.1.1/src/astro_extras/operators/table.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 07:53:51.080584 astro_extras-0.1.1/src/astro_extras/sensors/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2024-04-02 07:09:42.000000 astro_extras-0.1.1/src/astro_extras/sensors/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)      659 2024-04-23 14:51:38.000000 astro_extras-0.1.1/src/astro_extras/sensors/auto.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5536 2024-04-06 11:03:48.000000 astro_extras-0.1.1/src/astro_extras/sensors/file.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 07:53:51.084584 astro_extras-0.1.1/src/astro_extras/templates/
--rw-rw-r--   0 kol       (1000) kol       (1000)      121 2024-05-22 07:52:04.000000 astro_extras-0.1.1/src/astro_extras/templates/session_close.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)      269 2024-05-22 07:52:04.000000 astro_extras-0.1.1/src/astro_extras/templates/session_open.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)      489 2024-05-22 07:52:04.000000 astro_extras-0.1.1/src/astro_extras/templates/table_actuals_select.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)      138 2024-05-22 07:52:04.000000 astro_extras-0.1.1/src/astro_extras/templates/table_timed_update.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)       81 2024-05-22 07:52:04.000000 astro_extras-0.1.1/src/astro_extras/templates/table_transfer_nosess.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)      187 2024-05-22 07:52:04.000000 astro_extras-0.1.1/src/astro_extras/templates/table_transfer_sess.sql
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 07:53:51.084584 astro_extras-0.1.1/src/astro_extras/utils/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.1/src/astro_extras/utils/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    10671 2024-05-02 14:17:47.000000 astro_extras-0.1.1/src/astro_extras/utils/data_compare.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     1675 2024-03-11 13:15:59.000000 astro_extras-0.1.1/src/astro_extras/utils/datetime_local.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     3707 2024-05-22 07:52:04.000000 astro_extras-0.1.1/src/astro_extras/utils/postgres_sql.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5818 2024-05-22 07:52:04.000000 astro_extras-0.1.1/src/astro_extras/utils/template.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     4032 2024-05-22 07:52:50.000000 astro_extras-0.1.1/src/astro_extras/utils/utils.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 07:53:51.084584 astro_extras-0.1.1/src/astro_extras.egg-info/
--rw-r--r--   0 kol       (1000) kol       (1000)     7920 2024-05-22 07:53:50.000000 astro_extras-0.1.1/src/astro_extras.egg-info/PKG-INFO
--rw-rw-r--   0 kol       (1000) kol       (1000)     1188 2024-05-22 07:53:51.000000 astro_extras-0.1.1/src/astro_extras.egg-info/SOURCES.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)        1 2024-05-22 07:53:50.000000 astro_extras-0.1.1/src/astro_extras.egg-info/dependency_links.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)      139 2024-05-22 07:53:51.000000 astro_extras-0.1.1/src/astro_extras.egg-info/requires.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)       13 2024-05-22 07:53:51.000000 astro_extras-0.1.1/src/astro_extras.egg-info/top_level.txt
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 07:53:51.084584 astro_extras-0.1.1/tests/
--rw-rw-r--   0 kol       (1000) kol       (1000)     4172 2023-11-17 09:41:29.000000 astro_extras-0.1.1/tests/test_session.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    28649 2024-05-22 07:52:04.000000 astro_extras-0.1.1/tests/test_table.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     1295 2023-11-17 09:42:18.000000 astro_extras-0.1.1/tests/test_templates.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5772 2024-05-02 14:33:06.000000 astro_extras-0.1.1/tests/test_utils.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 09:07:13.922525 astro_extras-0.1.2/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1074 2023-11-17 10:43:31.000000 astro_extras-0.1.2/LICENSE
+-rw-rw-r--   0 kol       (1000) kol       (1000)       24 2023-10-26 14:10:20.000000 astro_extras-0.1.2/MANIFEST.in
+-rw-r--r--   0 kol       (1000) kol       (1000)     7920 2024-05-22 09:07:13.922525 astro_extras-0.1.2/PKG-INFO
+-rw-rw-r--   0 kol       (1000) kol       (1000)     7444 2023-11-20 09:59:52.000000 astro_extras-0.1.2/README.md
+-rw-rw-r--   0 kol       (1000) kol       (1000)      352 2023-10-26 14:10:20.000000 astro_extras-0.1.2/pyproject.toml
+-rw-rw-r--   0 kol       (1000) kol       (1000)      288 2024-05-22 07:52:04.000000 astro_extras-0.1.2/requirements.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)       38 2024-05-22 09:07:13.922525 astro_extras-0.1.2/setup.cfg
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1193 2024-05-22 08:53:58.000000 astro_extras-0.1.2/setup.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 09:07:13.918525 astro_extras-0.1.2/src/
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 09:07:13.918525 astro_extras-0.1.2/src/astro_extras/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1206 2024-05-22 08:53:06.000000 astro_extras-0.1.2/src/astro_extras/__init__.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 09:07:13.918525 astro_extras-0.1.2/src/astro_extras/hooks/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.2/src/astro_extras/hooks/__init__.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 09:07:13.918525 astro_extras-0.1.2/src/astro_extras/operators/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.2/src/astro_extras/operators/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     3861 2024-04-06 11:05:12.000000 astro_extras-0.1.2/src/astro_extras/operators/direct.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    18221 2024-05-22 07:52:04.000000 astro_extras-0.1.2/src/astro_extras/operators/session.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    53135 2024-05-22 09:05:03.000000 astro_extras-0.1.2/src/astro_extras/operators/table.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 09:07:13.918525 astro_extras-0.1.2/src/astro_extras/sensors/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2024-04-02 07:09:42.000000 astro_extras-0.1.2/src/astro_extras/sensors/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)      659 2024-04-23 14:51:38.000000 astro_extras-0.1.2/src/astro_extras/sensors/auto.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5536 2024-04-06 11:03:48.000000 astro_extras-0.1.2/src/astro_extras/sensors/file.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 09:07:13.918525 astro_extras-0.1.2/src/astro_extras/templates/
+-rw-rw-r--   0 kol       (1000) kol       (1000)      121 2024-05-22 07:52:04.000000 astro_extras-0.1.2/src/astro_extras/templates/session_close.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      269 2024-05-22 07:52:04.000000 astro_extras-0.1.2/src/astro_extras/templates/session_open.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      545 2024-05-22 09:04:48.000000 astro_extras-0.1.2/src/astro_extras/templates/table_actuals_select.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      138 2024-05-22 07:52:04.000000 astro_extras-0.1.2/src/astro_extras/templates/table_timed_update.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)       81 2024-05-22 07:52:04.000000 astro_extras-0.1.2/src/astro_extras/templates/table_transfer_nosess.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      187 2024-05-22 07:52:04.000000 astro_extras-0.1.2/src/astro_extras/templates/table_transfer_sess.sql
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 09:07:13.918525 astro_extras-0.1.2/src/astro_extras/utils/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.2/src/astro_extras/utils/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    10671 2024-05-02 14:17:47.000000 astro_extras-0.1.2/src/astro_extras/utils/data_compare.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1675 2024-03-11 13:15:59.000000 astro_extras-0.1.2/src/astro_extras/utils/datetime_local.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     3707 2024-05-22 07:52:04.000000 astro_extras-0.1.2/src/astro_extras/utils/postgres_sql.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5818 2024-05-22 07:52:04.000000 astro_extras-0.1.2/src/astro_extras/utils/template.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     4032 2024-05-22 07:52:50.000000 astro_extras-0.1.2/src/astro_extras/utils/utils.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 09:07:13.922525 astro_extras-0.1.2/src/astro_extras.egg-info/
+-rw-r--r--   0 kol       (1000) kol       (1000)     7920 2024-05-22 09:07:13.000000 astro_extras-0.1.2/src/astro_extras.egg-info/PKG-INFO
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1188 2024-05-22 09:07:13.000000 astro_extras-0.1.2/src/astro_extras.egg-info/SOURCES.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)        1 2024-05-22 09:07:13.000000 astro_extras-0.1.2/src/astro_extras.egg-info/dependency_links.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)      139 2024-05-22 09:07:13.000000 astro_extras-0.1.2/src/astro_extras.egg-info/requires.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)       13 2024-05-22 09:07:13.000000 astro_extras-0.1.2/src/astro_extras.egg-info/top_level.txt
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 09:07:13.922525 astro_extras-0.1.2/tests/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     4172 2023-11-17 09:41:29.000000 astro_extras-0.1.2/tests/test_session.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    28649 2024-05-22 07:52:04.000000 astro_extras-0.1.2/tests/test_table.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1295 2023-11-17 09:42:18.000000 astro_extras-0.1.2/tests/test_templates.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5772 2024-05-02 14:33:06.000000 astro_extras-0.1.2/tests/test_utils.py
```

### Comparing `astro_extras-0.1.1/LICENSE` & `astro_extras-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.1/PKG-INFO` & `astro_extras-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_extras
-Version: 0.1.1
+Version: 0.1.2
 Summary: Additional Astro SDK operators
 Home-page: https://github.com/skolchin/astro-extras
 Author: Kol
 Author-email: skolchin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Apache Airflow
```

### Comparing `astro_extras-0.1.1/README.md` & `astro_extras-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.1/setup.py` & `astro_extras-0.1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.readlines()
 
 setuptools.setup(
     name="astro_extras",
-    version="0.1.1",
+    version="0.1.2",
     author="Kol",
     author_email="skolchin@gmail.com",
     description="Additional Astro SDK operators",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/skolchin/astro-extras",
     classifiers=[
```

### Comparing `astro_extras-0.1.1/src/astro_extras/__init__.py` & `astro_extras-0.1.2/src/astro_extras/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Astro SDK Extras project
 # (c) kol, 2023-2024
 
-__version__ = '0.1.1'
+__version__ = '0.1.2'
 
 from .operators.session import (
     open_session, 
     close_session,
     ETLSession,
     get_current_session,
     get_session_period,
```

### Comparing `astro_extras-0.1.1/src/astro_extras/operators/direct.py` & `astro_extras-0.1.2/src/astro_extras/operators/direct.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.1/src/astro_extras/operators/session.py` & `astro_extras-0.1.2/src/astro_extras/operators/session.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.1/src/astro_extras/operators/table.py` & `astro_extras-0.1.2/src/astro_extras/operators/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from sqlalchemy.engine.base import Connection as SqlaConnection
 
 from airflow.models.dag import DagContext
 from airflow.utils.context import Context
 from airflow.models.xcom_arg import XComArg
 from airflow.utils.task_group import TaskGroup
 from airflow.exceptions import AirflowFailException
-from airflow.providers.common.sql.hooks.sql import DbApiHook
 from airflow.operators.generic_transfer import GenericTransfer
 
 from astro import sql as aql
 from astro.databases import create_database
 from astro.sql.table import BaseTable, Table
 from astro.databases.base import BaseDatabase
 from astro.airflow.datasets import kwargs_with_datasets
@@ -27,14 +26,17 @@
 from ..utils.utils import ensure_table, schedule_ops, is_same_database_uri, adjust_table_name_case
 from ..utils.template import get_template, get_template_file, get_predefined_template
 from ..utils.data_compare import compare_datasets, compare_timed_dict
 from ..utils.postgres_sql import postgres_merge_tables
 
 from typing import Iterable, Type
 
+TOSQL_CHUNK_SIZE: int = 100000
+""" Chunk size for `pd.to_sql()` calls. Set to value lesser than `DEFAULT_CHUNK_SIZE` in Astro SDK to avoid memory overload """
+
 class TableTransfer(GenericTransfer):
     """
     Table transfer operator to be used within `transfer_table` function.
     Implements 'bulk' data transfer without any extra conditioning.
     """
 
     template_fields = ("sql", "preoperator", "source_table", "destination_table")
@@ -194,15 +196,19 @@
         if data is None or data.empty:
             self.log.info('No data to transfer')
         else:
             # save to target table
             # TODO: cast integer NaNs to proper types
             self._row_count = len(data)
             self.log.info(f'{self._row_count} records to be transferred')
-            self.dest_db.load_pandas_dataframe_to_table(data, self.destination, if_exists='append')
+            self.dest_db.load_pandas_dataframe_to_table(
+                data, 
+                self.destination, 
+                if_exists='append',
+                chunksize=TOSQL_CHUNK_SIZE)
 
     def get_openlineage_facets_on_complete(self, task_instance):  # skipcq: PYL-W0613
         """
         Collect the input, output, job and run facets for DataframeOperator
         """
         from airflow.providers.openlineage.extractors.base import OperatorLineage
         from openlineage.client.run import Dataset
@@ -352,14 +358,15 @@
             self.log.info(f'Saving {data.shape[0]} {category} records to {self.destination_table}')
             data.to_sql(
                 self.destination.name,
                 con=conn,
                 schema=self.destination.metadata.schema if self.destination.metadata else None,
                 if_exists='append',
                 method='multi',
+                chunksize=TOSQL_CHUNK_SIZE,
                 index=False,
             )
             self._row_count += len(data)
 
     def execute(self, context: Context):
         """ Execute operator """
 
@@ -446,19 +453,18 @@
                 if dest_cols[0].primary_key:
                     id_cols.append(dest_cols[0].name)
 
         # Check there are any ID columns on target
         if not id_cols:
             raise AirflowFailException(f'Could not detect primary key on {self.destination_table}')
 
-        # Wrap data selection query into `select distinct on` in order to avoid having multiple IDs error
-        # Also, replace `t.*` with exact columns list and proper session_id
-        id_cols_str = ",".join(id_cols)
-        all_cols_str = f'{self.session.session_id} as session_id, ' + ",".join([col for col in col_map if col != 'session_id'])
-        sql = f'select distinct on ({id_cols_str}) {all_cols_str} from ({self.sql}) q order by {id_cols_str}, q.session_id desc'
+        # Replace `t.id` with ids and `t.*` with selection columns list and proper session_id
+        id_cols_str = ", ".join(id_cols)
+        all_cols_str = f'{self.session.session_id} as session_id, ' + ", ".join([col for col in col_map if col != 'session_id'])
+        sql = self.sql.replace('t.id', id_cols_str).replace('t.*', all_cols_str)
         self.log.info(f'Source extraction SQL:\n{sql}')
 
         # Check whether the hooks point to the same database
         same_db = is_same_database_uri(self.source_db.hook.get_uri(), self.dest_db.hook.get_uri())
 
         # Update/merge
         with self.source_db.connection as src_conn, self.dest_db.connection as dest_conn, dest_conn.begin():
@@ -505,14 +511,15 @@
                     # Save data to temporary table
                     data.to_sql(
                         temp_table.name,
                         con=dest_conn,
                         schema=temp_table.metadata.schema if temp_table.metadata else None,
                         if_exists='append',
                         method='multi',
+                        chunksize=TOSQL_CHUNK_SIZE,
                         index=False,
                     )
 
                     # If `replace_data` is set, purge target table
                     if self.replace_data:
                         dest_conn.execute(text(f'delete from {self.destination_table}'))
 
@@ -570,14 +577,15 @@
             if df_opening is not None and not df_opening.empty:
                 df_opening.to_sql(
                     self.destination.name,
                     con=dest_conn,
                     schema=self.destination.metadata.schema if self.destination.metadata else None,
                     if_exists='append',
                     method='multi',
+                    chunksize=TOSQL_CHUNK_SIZE,
                     index=False,
                 )
 
 
 class CompareTableOperator(ChangedTableTransfer):
     """
     Table comparsion operator to be used within `compare_table` function.
```

### Comparing `astro_extras-0.1.1/src/astro_extras/sensors/auto.py` & `astro_extras-0.1.2/src/astro_extras/sensors/auto.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.1/src/astro_extras/sensors/file.py` & `astro_extras-0.1.2/src/astro_extras/sensors/file.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.1/src/astro_extras/utils/data_compare.py` & `astro_extras-0.1.2/src/astro_extras/utils/data_compare.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.1/src/astro_extras/utils/datetime_local.py` & `astro_extras-0.1.2/src/astro_extras/utils/datetime_local.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.1/src/astro_extras/utils/postgres_sql.py` & `astro_extras-0.1.2/src/astro_extras/utils/postgres_sql.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.1/src/astro_extras/utils/template.py` & `astro_extras-0.1.2/src/astro_extras/utils/template.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.1/src/astro_extras/utils/utils.py` & `astro_extras-0.1.2/src/astro_extras/utils/utils.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.1/src/astro_extras.egg-info/PKG-INFO` & `astro_extras-0.1.2/src/astro_extras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_extras
-Version: 0.1.1
+Version: 0.1.2
 Summary: Additional Astro SDK operators
 Home-page: https://github.com/skolchin/astro-extras
 Author: Kol
 Author-email: skolchin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Apache Airflow
```

### Comparing `astro_extras-0.1.1/src/astro_extras.egg-info/SOURCES.txt` & `astro_extras-0.1.2/src/astro_extras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.1/tests/test_session.py` & `astro_extras-0.1.2/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.1/tests/test_table.py` & `astro_extras-0.1.2/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.1/tests/test_templates.py` & `astro_extras-0.1.2/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.1/tests/test_utils.py` & `astro_extras-0.1.2/tests/test_utils.py`

 * *Files identical despite different names*

