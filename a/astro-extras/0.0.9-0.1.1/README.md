# Comparing `tmp/astro_extras-0.0.9.tar.gz` & `tmp/astro_extras-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_extras-0.0.9.tar", last modified: Mon Apr 15 17:00:57 2024, max compression
+gzip compressed data, was "astro_extras-0.1.1.tar", last modified: Wed May 22 07:53:51 2024, max compression
```

## Comparing `astro_extras-0.0.9.tar` & `astro_extras-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,48 @@
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-15 17:00:57.045239 astro_extras-0.0.9/
--rw-rw-r--   0 kol       (1000) kol       (1000)     1074 2023-11-17 10:43:31.000000 astro_extras-0.0.9/LICENSE
--rw-rw-r--   0 kol       (1000) kol       (1000)       24 2023-10-26 14:10:20.000000 astro_extras-0.0.9/MANIFEST.in
--rw-r--r--   0 kol       (1000) kol       (1000)     7878 2024-04-15 17:00:57.045239 astro_extras-0.0.9/PKG-INFO
--rw-rw-r--   0 kol       (1000) kol       (1000)     7444 2023-11-20 09:59:52.000000 astro_extras-0.0.9/README.md
--rw-rw-r--   0 kol       (1000) kol       (1000)      352 2023-10-26 14:10:20.000000 astro_extras-0.0.9/pyproject.toml
--rw-rw-r--   0 kol       (1000) kol       (1000)      260 2024-03-11 13:15:33.000000 astro_extras-0.0.9/requirements.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)       38 2024-04-15 17:00:57.045239 astro_extras-0.0.9/setup.cfg
--rw-rw-r--   0 kol       (1000) kol       (1000)     1114 2024-04-15 17:00:54.000000 astro_extras-0.0.9/setup.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-15 17:00:57.005240 astro_extras-0.0.9/src/
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-15 17:00:57.013239 astro_extras-0.0.9/src/astro_extras/
--rw-rw-r--   0 kol       (1000) kol       (1000)      963 2024-04-15 16:59:07.000000 astro_extras-0.0.9/src/astro_extras/__init__.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-15 17:00:57.029239 astro_extras-0.0.9/src/astro_extras/hooks/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.9/src/astro_extras/hooks/__init__.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-15 17:00:57.033239 astro_extras-0.0.9/src/astro_extras/operators/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.9/src/astro_extras/operators/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     3861 2024-04-06 11:05:12.000000 astro_extras-0.0.9/src/astro_extras/operators/direct.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    18308 2024-04-15 16:59:36.000000 astro_extras-0.0.9/src/astro_extras/operators/session.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    24781 2024-04-15 15:17:52.000000 astro_extras-0.0.9/src/astro_extras/operators/table.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-15 17:00:57.037239 astro_extras-0.0.9/src/astro_extras/sensors/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2024-04-02 07:09:42.000000 astro_extras-0.0.9/src/astro_extras/sensors/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5536 2024-04-06 11:03:48.000000 astro_extras-0.0.9/src/astro_extras/sensors/file.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-15 17:00:57.037239 astro_extras-0.0.9/src/astro_extras/utils/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.9/src/astro_extras/utils/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    10650 2024-04-06 10:39:43.000000 astro_extras-0.0.9/src/astro_extras/utils/data_compare.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     1675 2024-03-11 13:15:59.000000 astro_extras-0.0.9/src/astro_extras/utils/datetime_local.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5378 2024-03-11 14:28:15.000000 astro_extras-0.0.9/src/astro_extras/utils/template.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     2199 2024-04-15 14:31:16.000000 astro_extras-0.0.9/src/astro_extras/utils/utils.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-15 17:00:57.045239 astro_extras-0.0.9/src/astro_extras.egg-info/
--rw-r--r--   0 kol       (1000) kol       (1000)     7878 2024-04-15 17:00:56.000000 astro_extras-0.0.9/src/astro_extras.egg-info/PKG-INFO
--rw-rw-r--   0 kol       (1000) kol       (1000)      821 2024-04-15 17:00:57.000000 astro_extras-0.0.9/src/astro_extras.egg-info/SOURCES.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)        1 2024-04-15 17:00:56.000000 astro_extras-0.0.9/src/astro_extras.egg-info/dependency_links.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)      112 2024-04-15 17:00:56.000000 astro_extras-0.0.9/src/astro_extras.egg-info/requires.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)       13 2024-04-15 17:00:56.000000 astro_extras-0.0.9/src/astro_extras.egg-info/top_level.txt
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-15 17:00:57.045239 astro_extras-0.0.9/tests/
--rw-rw-r--   0 kol       (1000) kol       (1000)     4172 2023-11-17 09:41:29.000000 astro_extras-0.0.9/tests/test_session.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     6158 2023-11-17 10:36:18.000000 astro_extras-0.0.9/tests/test_table.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     1295 2023-11-17 09:42:18.000000 astro_extras-0.0.9/tests/test_templates.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5772 2024-03-11 14:20:58.000000 astro_extras-0.0.9/tests/test_utils.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 07:53:51.084584 astro_extras-0.1.1/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1074 2023-11-17 10:43:31.000000 astro_extras-0.1.1/LICENSE
+-rw-rw-r--   0 kol       (1000) kol       (1000)       24 2023-10-26 14:10:20.000000 astro_extras-0.1.1/MANIFEST.in
+-rw-r--r--   0 kol       (1000) kol       (1000)     7920 2024-05-22 07:53:51.084584 astro_extras-0.1.1/PKG-INFO
+-rw-rw-r--   0 kol       (1000) kol       (1000)     7444 2023-11-20 09:59:52.000000 astro_extras-0.1.1/README.md
+-rw-rw-r--   0 kol       (1000) kol       (1000)      352 2023-10-26 14:10:20.000000 astro_extras-0.1.1/pyproject.toml
+-rw-rw-r--   0 kol       (1000) kol       (1000)      288 2024-05-22 07:52:04.000000 astro_extras-0.1.1/requirements.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)       38 2024-05-22 07:53:51.088584 astro_extras-0.1.1/setup.cfg
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1193 2024-05-22 07:52:04.000000 astro_extras-0.1.1/setup.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 07:53:51.044584 astro_extras-0.1.1/src/
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 07:53:51.056584 astro_extras-0.1.1/src/astro_extras/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1206 2024-05-22 07:52:04.000000 astro_extras-0.1.1/src/astro_extras/__init__.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 07:53:51.080584 astro_extras-0.1.1/src/astro_extras/hooks/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.1/src/astro_extras/hooks/__init__.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 07:53:51.080584 astro_extras-0.1.1/src/astro_extras/operators/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.1/src/astro_extras/operators/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     3861 2024-04-06 11:05:12.000000 astro_extras-0.1.1/src/astro_extras/operators/direct.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    18221 2024-05-22 07:52:04.000000 astro_extras-0.1.1/src/astro_extras/operators/session.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    52923 2024-05-22 07:52:50.000000 astro_extras-0.1.1/src/astro_extras/operators/table.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 07:53:51.080584 astro_extras-0.1.1/src/astro_extras/sensors/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2024-04-02 07:09:42.000000 astro_extras-0.1.1/src/astro_extras/sensors/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)      659 2024-04-23 14:51:38.000000 astro_extras-0.1.1/src/astro_extras/sensors/auto.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5536 2024-04-06 11:03:48.000000 astro_extras-0.1.1/src/astro_extras/sensors/file.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 07:53:51.084584 astro_extras-0.1.1/src/astro_extras/templates/
+-rw-rw-r--   0 kol       (1000) kol       (1000)      121 2024-05-22 07:52:04.000000 astro_extras-0.1.1/src/astro_extras/templates/session_close.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      269 2024-05-22 07:52:04.000000 astro_extras-0.1.1/src/astro_extras/templates/session_open.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      489 2024-05-22 07:52:04.000000 astro_extras-0.1.1/src/astro_extras/templates/table_actuals_select.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      138 2024-05-22 07:52:04.000000 astro_extras-0.1.1/src/astro_extras/templates/table_timed_update.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)       81 2024-05-22 07:52:04.000000 astro_extras-0.1.1/src/astro_extras/templates/table_transfer_nosess.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      187 2024-05-22 07:52:04.000000 astro_extras-0.1.1/src/astro_extras/templates/table_transfer_sess.sql
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 07:53:51.084584 astro_extras-0.1.1/src/astro_extras/utils/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.1/src/astro_extras/utils/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    10671 2024-05-02 14:17:47.000000 astro_extras-0.1.1/src/astro_extras/utils/data_compare.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1675 2024-03-11 13:15:59.000000 astro_extras-0.1.1/src/astro_extras/utils/datetime_local.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     3707 2024-05-22 07:52:04.000000 astro_extras-0.1.1/src/astro_extras/utils/postgres_sql.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5818 2024-05-22 07:52:04.000000 astro_extras-0.1.1/src/astro_extras/utils/template.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     4032 2024-05-22 07:52:50.000000 astro_extras-0.1.1/src/astro_extras/utils/utils.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 07:53:51.084584 astro_extras-0.1.1/src/astro_extras.egg-info/
+-rw-r--r--   0 kol       (1000) kol       (1000)     7920 2024-05-22 07:53:50.000000 astro_extras-0.1.1/src/astro_extras.egg-info/PKG-INFO
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1188 2024-05-22 07:53:51.000000 astro_extras-0.1.1/src/astro_extras.egg-info/SOURCES.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)        1 2024-05-22 07:53:50.000000 astro_extras-0.1.1/src/astro_extras.egg-info/dependency_links.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)      139 2024-05-22 07:53:51.000000 astro_extras-0.1.1/src/astro_extras.egg-info/requires.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)       13 2024-05-22 07:53:51.000000 astro_extras-0.1.1/src/astro_extras.egg-info/top_level.txt
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-22 07:53:51.084584 astro_extras-0.1.1/tests/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     4172 2023-11-17 09:41:29.000000 astro_extras-0.1.1/tests/test_session.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    28649 2024-05-22 07:52:04.000000 astro_extras-0.1.1/tests/test_table.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1295 2023-11-17 09:42:18.000000 astro_extras-0.1.1/tests/test_templates.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5772 2024-05-02 14:33:06.000000 astro_extras-0.1.1/tests/test_utils.py
```

### Comparing `astro_extras-0.0.9/LICENSE` & `astro_extras-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.9/PKG-INFO` & `astro_extras-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: astro_extras
-Version: 0.0.9
+Version: 0.1.1
 Summary: Additional Astro SDK operators
 Home-page: https://github.com/skolchin/astro-extras
 Author: Kol
 Author-email: skolchin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: apache-airflow[pandas,postgres]>=2.7.0
 Requires-Dist: astro-sdk-python[postgres]>=1.6.0
+Requires-Dist: openlineage-python>=1.14.0
 Requires-Dist: openpyxl>=3.0.0
 Requires-Dist: python-dateutil>=2.8.0
 
 # Astro SDK extras project
 
 We've been using [Apache Airflow](https://airflow.apache.org/docs/apache-airflow/stable/)
 as ETL tool for quite some time. Recently I came across
```

### Comparing `astro_extras-0.0.9/README.md` & `astro_extras-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.9/setup.py` & `astro_extras-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,26 +8,28 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.readlines()
 
 setuptools.setup(
     name="astro_extras",
-    version="0.0.9",
+    version="0.1.1",
     author="Kol",
     author_email="skolchin@gmail.com",
     description="Additional Astro SDK operators",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/skolchin/astro-extras",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "Framework :: Apache Airflow",
         "Framework :: Apache Airflow :: Provider",
     ],
     package_dir={"": "src"},
     packages=['astro_extras', 'astro_extras.hooks', 'astro_extras.operators', 'astro_extras.sensors', 'astro_extras.utils'],
+    package_data = {"": ["templates/*.sql"]},
+    include_package_data=True,
     python_requires=">=3.10",
     install_requires=requirements,
     setup_requires=['setuptools', 'wheel'],
 )
```

### Comparing `astro_extras-0.0.9/src/astro_extras/__init__.py` & `astro_extras-0.1.1/src/astro_extras/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Astro SDK Extras project
 # (c) kol, 2023-2024
 
-__version__ = '0.0.9'
+__version__ = '0.1.1'
 
 from .operators.session import (
     open_session, 
     close_session,
     ETLSession,
     get_current_session,
     get_session_period,
@@ -13,25 +13,35 @@
 )
 from .operators.table import (
     load_table,
     save_table,
     declare_tables,
     transfer_table, 
     transfer_tables,
+    transfer_changed_table,
+    transfer_changed_tables,
+    transfer_ods_table,
+    transfer_ods_tables,
+    transfer_actuals_table,
+    transfer_actuals_tables,
+    compare_table,
+    compare_tables,
     update_timed_table, 
     update_timed_tables,
-    compare_tables,
 )
 from .operators.direct import (
     run_sql_template,
     run_sql_templates,
 )
 from .sensors.file import (
     FileChangedSensor
 )
+from .sensors.auto import (
+    AutoOnlyTaskSensor
+)
 from .utils.template import (
     get_template_file,
     get_template,
 )
 from .utils.utils import (
     split_table_name,
     ensure_table,
@@ -43,8 +53,7 @@
     datetime_to_local,
     datetime_to_utc,
     datetime_to_tz,
     datetime_to_naive,
     days_ago,
     months_ago
 )
-
```

### Comparing `astro_extras-0.0.9/src/astro_extras/operators/direct.py` & `astro_extras-0.1.1/src/astro_extras/operators/direct.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.9/src/astro_extras/operators/session.py` & `astro_extras-0.1.1/src/astro_extras/operators/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 # (c) kol, 2023
 
 """ ETL session management routines """
 
 import re
 from datetime import datetime, timedelta
 from dateutil.parser import isoparse
-
+from sqlalchemy import text
 from airflow.models import DAG, BaseOperator
 from airflow.models.xcom_arg import XComArg
 from airflow.models.dag import DagContext
 from airflow.operators.python import get_current_context
 from airflow.utils.context import Context
 from airflow.utils.state import TaskInstanceState
 from airflow.utils.trigger_rule import TriggerRule
+from airflow.providers.common.sql.hooks.sql import DbApiHook
 from airflow.exceptions import AirflowException, AirflowFailException
 from airflow.settings import TIMEZONE
-
 from attr import define, field
 from astro import sql as aql
-from astro.sql.operators.raw_sql import RawSQLOperator
-from typing import Optional, Union, Any, Tuple, cast
+from typing import Any, Tuple, cast
 
 from ..utils.datetime_local import datetime_to_tz
+from ..utils.template import get_predefined_template
 
 @define(slots=False)
 class ETLSession:
     """ Session data object. Holds all ETL session attributes, can be pushed to XCom.
     Implements context manager protocol (see examples). 
     
     See `open_session` function for more information.
@@ -99,57 +99,54 @@
         return self._actual_sesssion
 
     def __exit__(self, type, value, traceback):
         dag = cast(DAG, DagContext.get_current_dag())
         if len(dag.tasks) > 1:
             t1, t2 = dag.tasks[0], dag.tasks[1]
             if t1.task_id == 'open-session' and 'open-session' not in t2.upstream_task_ids:
-                if not t2.task_group:
-                    # stand-alone operator
+                if t2.task_group is None or t2.task_group.is_root:
                     t2.set_upstream(t1)
                 else:
                     t2.task_group.set_upstream(t1)
 
         close_session(self._actual_sesssion).set_downstream(aql.cleanup())
 
 class OpenSessionOperator(BaseOperator):
     """ Session opening operator. Normally is used within `open_session` function """
+    ui_color = "#82eef0"
 
     def __init__(self,
                  *,
-                 source_conn_id: Optional[str] = 'default',
-                 destination_conn_id: Optional[str] = 'default',
-                 session_conn_id: Optional[str] = None,
+                 source_conn_id: str = 'default',
+                 destination_conn_id: str = 'default',
+                 session_conn_id: str = None,
                  **kwargs):
 
         task_id = kwargs.pop('task_id', 'open-session')
         super().__init__(task_id=task_id, **kwargs)
 
         self.source_conn_id = source_conn_id
         self.destination_conn_id = destination_conn_id
         self.session_conn_id = session_conn_id if session_conn_id else destination_conn_id
         self.session: ETLSession = None
 
     def _new_session(self, period_start: str, period_end: str, context: Context) -> int:
-        # TODO: use database-neutral statement with SQLA
-        sql = f"""insert into public.sessions(source, target, period, started, status, run_id) 
-            values('{self.source_conn_id}','{self.destination_conn_id}','{{ {period_start}, {period_end} }}', 
-            '{datetime.now()}','running','{context['run_id']}') returning session_id"""
-
-        op = RawSQLOperator(
-            task_id=self.task_id,
-            python_callable=lambda : sql,
-            conn_id=self.session_conn_id,
-            handler=lambda result: result.fetchone(),
-            response_size=1)
-        
-        return op.execute(context)[0]
+        template = get_predefined_template('session_open.sql')
+        sql = template.render(
+            source_conn_id=self.source_conn_id,
+            destination_conn_id=self.destination_conn_id,
+            period_str=f'{{ "{period_start}", "{period_end}" }}',
+            started=datetime.now().isoformat(),
+            run_id=context['run_id'],
+        )
+        hook: DbApiHook = DbApiHook.get_hook(self.session_conn_id)
+        result = hook.get_first(sql)
+        return result[0]
 
     def execute(self, context: Context):
-
         period_start, period_end = get_session_period(context)
         session_id = self._new_session(period_start, period_end, context)
         self.log.info(f'New session {session_id} for period [{period_start},{period_end}] started')
 
         session = ETLSession(
             source_conn_id=self.source_conn_id,
             destination_conn_id=self.destination_conn_id, 
@@ -159,18 +156,19 @@
             period_end=period_end)
         
         context['ti'].xcom_push(key='session', value=session)
         return session
 
 class CloseSessionOperator(BaseOperator):
     """ Session closing operator. Normally is used within `close_session` function """
+    ui_color = "#78f0f0"
 
     def __init__(self,
                  *,
-                 session: Union[ETLSession, XComArg, None] = None,
+                 session: ETLSession | XComArg | None = None,
                  **kwargs):
 
         task_id = kwargs.pop('task_id', 'close-session')
         trigger_rule = kwargs.pop('trigger_rule', TriggerRule.ALL_DONE)
         super().__init__(task_id=task_id, trigger_rule=trigger_rule, **kwargs)
         self.session = session
 
@@ -178,32 +176,32 @@
         self.session = ensure_session(self.session)
 
         dag_run = context['dag_run']
         failed_tasks = [ti for ti in dag_run.get_task_instances(state=TaskInstanceState.FAILED)]
         status = 'error' if failed_tasks else 'success'
 
         # TBD: use of database-neutral statement
-        sql = f"update public.sessions set finished=current_timestamp, status='{status}' " \
-                   f"where session_id={self.session.session_id}"
-        op = RawSQLOperator(
-            task_id=self.task_id,
-            python_callable=lambda : sql,
-            conn_id=self.session.session_conn_id,
-            response_size=1)
-        op.execute(context)
+        template = get_predefined_template('session_close.sql')
+        sql = template.render(
+            session_id=self.session.session_id,
+            status=status,
+            finished=datetime.now().isoformat()
+        )
+        hook: DbApiHook = DbApiHook.get_hook(self.session.session_conn_id)
+        hook.run(sql)
         self.log.info(f'Session {self.session.session_id} closed with status {status}')
 
         if status == 'error':
             raise AirflowException('Setting drives to idle')
 
 def open_session(
         source_conn_id: str, 
         destination_conn_id: str, 
-        session_conn_id: Optional[str] = None, 
-        dag: Optional[DAG] = None,
+        session_conn_id: str | None = None, 
+        dag: DAG | None = None,
         **kwargs) -> XComArg:
     """ Opens a new ETL session.
 
     ETL session is a logical group of data transfers united by single identifier (`session_id`).
     Sessions store information about data transfer source, target, data loading period
     and completion state thus providing all necessary information about the data flow.
 
@@ -297,17 +295,17 @@
         dag=dag,
         source_conn_id=source_conn_id,
         destination_conn_id=destination_conn_id,
         session_conn_id=session_conn_id,
         **kwargs))
 
 def close_session(
-        session: Union[ETLSession, XComArg], 
-        upstream: Optional[Any] = None,
-        dag: Optional[DAG] = None,
+        session: ETLSession | XComArg, 
+        upstream: Any | None = None,
+        dag: DAG | None = None,
         **kwargs) -> XComArg:
     """ Closes the ETL session.
 
     Updates `public.sessions` table for currently running session
     saving completion time and state. If all tasks in a DAG run were successfull,
     session's state will be set to `success`, otherwise - to `error`. Note that 
     session closing task will also fail in later case in order to be
@@ -339,50 +337,52 @@
         if upstream.task_group and not upstream.task_group.is_root:
             upstream = upstream.task_group
 
     op = CloseSessionOperator(dag=dag, session=session, **kwargs)
     op.set_upstream(upstream)
     return XComArg(op)
 
-def get_current_session(context: Optional[Context] = None) -> ETLSession:
+def get_current_session(context: Context | None = None) -> ETLSession:
     """ Retrieves current session from XCom.
     
     Args:
         context:    DAG execution context (optional)
 
     Returns:
         Current ETL session as `ETLSession` class instance
     """
     context = context or get_current_context()
     return context['ti'].xcom_pull(key='session')
 
-def ensure_session(session: Optional[Union[ETLSession, XComArg]], 
-                   context: Optional[Context] = None) -> ETLSession:
+def ensure_session(session: ETLSession | XComArg | None, 
+                   context: Context | None = None) -> ETLSession:
     """ Returns current session. If a placeholder object returned by `open_session` is passed in,
     retrieves actual session from XCom. 
     
     Args:
         session: Either the `ETLSession` instance or a placeholder returned by `open_session` call
         context:    DAG execution context (optional)
 
     Returns:
         Current ETL session as `ETLSession` class instance
     """
-    if session is None:
-        return None
-    if isinstance(session, ETLSession):
-        return session
-    if isinstance(session, XComArg):
-        return get_current_session(context)
-    raise TypeError(f'Either ETLSession or XComArg expected, {session.__class__.__name__} found')
+    match session:
+        case None:
+            return None
+        case ETLSession():
+            return session
+        case XComArg():
+            return get_current_session(context)
+        case _:
+            raise TypeError(f'Either ETLSession or XComArg expected, {session.__class__.__name__} found')
 
 _TS_REGX = r'\d{4}-([0]\d|1[0-2])-([0-2]\d|3[01])(T\d{2}:\d{2}:\d{2})?'
 _FULL_REGX = r'\[\d{4}-([0]\d|1[0-2])-([0-2]\d|3[01])(T\d{2}:\d{2}:\d{2})?,\s*\d{4}-([0]\d|1[0-2])-([0-2]\d|3[01])(T\d{2}:\d{2}:\d{2})?]'
 
-def get_session_period(context: Optional[Context] = None) -> Tuple[str, str]:
+def get_session_period(context: Context | None = None) -> Tuple[str, str]:
     """ Calculates ETL session loading period.
     
     This function is used when a new session is created. It recognizes a "period"
     DAG run parameter, which must be provided as two valid dates or datetimes defining
     lower and upper bound of loading period. If a date-only upper bound is used,
     it will be increased to hold entire day (see examples).
     
@@ -412,19 +412,19 @@
         ```
 
     """
     context = context or get_current_context()
 
     if (period_str := context['dag_run'].conf.get('period')):
         if not re.match(_FULL_REGX, period_str):
-            raise AirflowFailException('Period must be specified as "period": "[<date_from>,<date_to>]"')
+            raise AirflowFailException('Period must be specified as {"period": "[<from>,<to>]"}, got %s instead', period_str)
         
         period = [isoparse(x.group(0)) for x in re.finditer(_TS_REGX, period_str)]
         if len(period) < 2:
-            raise AirflowFailException('Invalid period: two valid dates in YYYY-MM-DD format must be specified')
+            raise AirflowFailException('Invalid period: two valid dates in ISO format must be specified, got %s instead', period_str)
 
         # If no time part is provided in the upper period bound,
         # consider this to be date-only and add 1 day to align to days'end
         # For example, specifying period = ["2023-05-01", "2023-05-01"] will be converted
         # to ["2023-05-01 00:00:00", "2023-05-02 00:00:00"]
         if period[1].hour == 0 and period[1].minute == 0 and period[1].second == 0:
             period[1] += timedelta(days=1)
```

### Comparing `astro_extras-0.0.9/src/astro_extras/sensors/file.py` & `astro_extras-0.1.1/src/astro_extras/sensors/file.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.9/src/astro_extras/utils/data_compare.py` & `astro_extras-0.1.1/src/astro_extras/utils/data_compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,18 +52,18 @@
         if df_a.dtypes[col] == 'datetime64[ns]' and df_b.dtypes[col] != 'datetime64[ns]':
             raise AirflowFailException(f'Incompatible timestamp column {col} type: ' \
                                    f'{df_a.dtypes[col]} on source, {df_b.dtypes[col]} on target')
 
 def compare_datasets(
     df_src: pd.DataFrame, 
     df_trg: pd.DataFrame, 
-    id_cols: Iterable = None, 
-    exclude_cols: Iterable = None, 
+    id_cols: Iterable | None = None, 
+    exclude_cols: Iterable | None = None, 
     stop_on_first_diff: bool = True,
-    logger: logging.Logger = None) -> Union[bool, Tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame]]:
+    logger: logging.Logger | None = None) -> Union[bool, Tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame]]:
 
     """ Compare two dataframes by columns, their types and values.
 
     Args:
         df_src: Source dataframe
 
         df_trg: Target dataframe
```

### Comparing `astro_extras-0.0.9/src/astro_extras/utils/datetime_local.py` & `astro_extras-0.1.1/src/astro_extras/utils/datetime_local.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.9/src/astro_extras/utils/template.py` & `astro_extras-0.1.1/src/astro_extras/utils/template.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # Astro SDK Extras project
 # (c) kol, 2023
 
 """ Template utility functions """
 
 import os
+import jinja2
+import importlib.resources
 from airflow.models import DAG
 from airflow.models.dag import DagContext
 from airflow.configuration import conf
 from airflow.exceptions import AirflowFailException
 
-from typing import Optional, Union
-
 def get_template_file(
         template: str, 
-        ext: Optional[str] = '.sql', 
-        dag: Optional[DAG] = None,
-        fail_if_not_found: Optional[bool] = False) -> Optional[str]:
+        ext: str = '.sql', 
+        dag: DAG | None = None,
+        fail_if_not_found: bool = False) -> str | None:
     
     """ Returns reference to DAG-specific template file, if one exists.
     
     This function looks up for a template file in `./templates/<dag_id>` folder
     under directory set as DAGS_HOME in Airflow config (usually `./dags`).
 
     Templates are used for SQL operations, html reporting and so on.
     They consists of some plain-text content mixed with Jinja macros inside `{{...}}` brackets,
     which will be substituted ('rendered`) with some variables either by Airflow runtime or manually.
 
     Args:
         template:   Template name (e.g. table name or reporting object) without any extension
         ext:        Template file extension, `.sql` by default
-        dag:        Optional DAG context
+        dag:        Optional DAG context. If not provided, current DAG context will be used
         fail_if_not_found: If `True`, `AirflowFailException` will be raised if template does not exist
             (default is `False`)
 
     Returns:
         Name of template file relative to Airflow's `DAG_HOME` folder or `None` if no file was found
         and `fail_if_not_found = False`
 
@@ -64,27 +64,27 @@
         return rel_file_name
     if fail_if_not_found:
         raise AirflowFailException(f'Template file {full_file_name} was not found')
     return None
 
 def get_template(
         template: str, 
-        ext: Optional[str] = '.sql', 
-        dag: Optional[DAG] = None,
-        fail_if_not_found: Optional[bool] = False,
-        read_mode: Optional[str] = 'rt') -> Optional[Union[str, bytes]]:
+        ext: str = '.sql', 
+        dag: DAG | None = None,
+        fail_if_not_found: bool = False,
+        read_mode: str = 'rt') -> str | bytes | None:
     
     """ Returns template content. See `get_template_file` for details on templates.
 
     Args:
-        template:  Template name (e.g. table name or reporting object) without any extension
-        ext:    Template file extension, `.sql` by default
-        dag:    Optional DAG context
+        template:   Template name (e.g. table name or reporting object) without any extension
+        ext:        Template file extension, `.sql` by default
+        dag:        Optional DAG context. If not provided, current DAG context will be used
         fail_if_not_found: If `True`, `AirflowFailException` will be raised if template does not exist
-        read_mode:   Read mode (`rt` for text, `rb` for binary, other will fail)
+        read_mode:  Read mode (either `rt` for text or `rb` for binary)
 
     Returns:
         Template file content or `None` if no file was found and `fail_if_not_found = False`.
 
     Examples:
         Load template from `./dags/templates/test_dag/mail.html`, manually render it
         with Airflow DAG context and send it as a mail:
@@ -117,7 +117,14 @@
     assert read_mode in ('rt', 'rb'), f'Read_mode must be either `rt` or `rb`'
     template_file = get_template_file(template, ext, dag, fail_if_not_found)
     if not template_file:
         return None
     full_file_name = os.path.join(conf.get('core','dags_folder'), template_file)
     with open(full_file_name, read_mode) as fp:
         return fp.read()
+
+def get_predefined_template(name: str) -> jinja2.Template:
+    """ Retrieves a template from package resources. Mostly for internal use. """
+    template_file = f'templates/{name}'
+    template_res = importlib.resources.files('astro_extras').joinpath(template_file)
+    with importlib.resources.as_file(template_res) as template_file:
+        return jinja2.Template(template_file.read_text())
```

### Comparing `astro_extras-0.0.9/src/astro_extras.egg-info/PKG-INFO` & `astro_extras-0.1.1/src/astro_extras.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: astro_extras
-Version: 0.0.9
+Version: 0.1.1
 Summary: Additional Astro SDK operators
 Home-page: https://github.com/skolchin/astro-extras
 Author: Kol
 Author-email: skolchin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: apache-airflow[pandas,postgres]>=2.7.0
 Requires-Dist: astro-sdk-python[postgres]>=1.6.0
+Requires-Dist: openlineage-python>=1.14.0
 Requires-Dist: openpyxl>=3.0.0
 Requires-Dist: python-dateutil>=2.8.0
 
 # Astro SDK extras project
 
 We've been using [Apache Airflow](https://airflow.apache.org/docs/apache-airflow/stable/)
 as ETL tool for quite some time. Recently I came across
```

### Comparing `astro_extras-0.0.9/src/astro_extras.egg-info/SOURCES.txt` & `astro_extras-0.1.1/src/astro_extras.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -12,17 +12,25 @@
 src/astro_extras.egg-info/top_level.txt
 src/astro_extras/hooks/__init__.py
 src/astro_extras/operators/__init__.py
 src/astro_extras/operators/direct.py
 src/astro_extras/operators/session.py
 src/astro_extras/operators/table.py
 src/astro_extras/sensors/__init__.py
+src/astro_extras/sensors/auto.py
 src/astro_extras/sensors/file.py
+src/astro_extras/templates/session_close.sql
+src/astro_extras/templates/session_open.sql
+src/astro_extras/templates/table_actuals_select.sql
+src/astro_extras/templates/table_timed_update.sql
+src/astro_extras/templates/table_transfer_nosess.sql
+src/astro_extras/templates/table_transfer_sess.sql
 src/astro_extras/utils/__init__.py
 src/astro_extras/utils/data_compare.py
 src/astro_extras/utils/datetime_local.py
+src/astro_extras/utils/postgres_sql.py
 src/astro_extras/utils/template.py
 src/astro_extras/utils/utils.py
 tests/test_session.py
 tests/test_table.py
 tests/test_templates.py
 tests/test_utils.py
```

### Comparing `astro_extras-0.0.9/tests/test_session.py` & `astro_extras-0.1.1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.9/tests/test_templates.py` & `astro_extras-0.1.1/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.9/tests/test_utils.py` & `astro_extras-0.1.1/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,19 +112,19 @@
     op2 = next((task for task in dag_tasks if task['task_id'] == 'op2'), None)
     op3 = next((task for task in dag_tasks if task['task_id'] == 'op3'), None)
     op4 = next((task for task in dag_tasks if task['task_id'] == 'op4'), None)
     
     # Check that all tasks were found
     assert op1 is not None and op2 is not None and op3 is not None and op4 is not None
     # Check that task op2 depends on task op1 (determined by downstream_task_ids)
-    assert 'op2' in op1['downstream_task_ids']
+    assert 'op3' in op1['downstream_task_ids']
     # Check that task op4 depends on task op3
-    assert 'op4' in op3['downstream_task_ids']
+    assert 'op4' in op2['downstream_task_ids']
     # Check that task op2 has no downstream tasks (i.e., it is the last task in the DAG)
-    assert not op2['downstream_task_ids']
+    assert not op3['downstream_task_ids']
     # Check that task op4 has no downstream tasks (i.e., it is the last task in the DAG)
     assert not op4['downstream_task_ids']
     
 def test_datetime():
     if localnow is None:
         return pytest.skip('Astro-extras was not installed')
```

