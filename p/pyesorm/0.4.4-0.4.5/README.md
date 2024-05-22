# Comparing `tmp/pyesorm-0.4.4.tar.gz` & `tmp/pyesorm-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyesorm-0.4.4.tar", last modified: Sat May 18 15:26:29 2024, max compression
+gzip compressed data, was "pyesorm-0.4.5.tar", last modified: Wed May 22 09:06:23 2024, max compression
```

## Comparing `pyesorm-0.4.4.tar` & `pyesorm-0.4.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-18 15:26:29.526158 pyesorm-0.4.4/
--rw-r--r--   0 wallner    (501) staff       (20)    16725 2023-10-30 16:10:12.000000 pyesorm-0.4.4/LICENSE
--rw-r--r--   0 wallner    (501) staff       (20)    23956 2024-05-18 15:26:29.525956 pyesorm-0.4.4/PKG-INFO
--rw-r--r--   0 wallner    (501) staff       (20)    22319 2024-05-07 06:59:22.000000 pyesorm-0.4.4/README.md
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-18 15:26:29.516506 pyesorm-0.4.4/docs/
--rw-r--r--   0 wallner    (501) staff       (20)        0 2024-01-17 15:06:14.000000 pyesorm-0.4.4/docs/__init__.py
--rw-r--r--   0 wallner    (501) staff       (20)     1484 2024-01-17 15:18:18.000000 pyesorm-0.4.4/docs/changelog.py
--rw-r--r--   0 wallner    (501) staff       (20)     1462 2024-01-17 15:10:11.000000 pyesorm-0.4.4/docs/conf.py
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-18 15:26:29.520966 pyesorm-0.4.4/esorm/
--rw-r--r--   0 wallner    (501) staff       (20)      762 2024-05-18 14:17:08.000000 pyesorm-0.4.4/esorm/__init__.py
--rw-r--r--   0 wallner    (501) staff       (20)     3132 2024-01-22 17:32:29.000000 pyesorm-0.4.4/esorm/aggs.py
--rw-r--r--   0 wallner    (501) staff       (20)     4447 2024-05-07 05:08:54.000000 pyesorm-0.4.4/esorm/bulk.py
--rw-r--r--   0 wallner    (501) staff       (20)     1267 2024-05-07 05:07:07.000000 pyesorm-0.4.4/esorm/error.py
--rw-r--r--   0 wallner    (501) staff       (20)     2144 2024-05-18 14:16:43.000000 pyesorm-0.4.4/esorm/esorm.py
--rw-r--r--   0 wallner    (501) staff       (20)     3500 2024-01-24 09:39:22.000000 pyesorm-0.4.4/esorm/fastapi.py
--rw-r--r--   0 wallner    (501) staff       (20)    11640 2023-10-31 19:12:30.000000 pyesorm-0.4.4/esorm/fields.py
--rw-r--r--   0 wallner    (501) staff       (20)       52 2023-10-30 16:10:12.000000 pyesorm-0.4.4/esorm/logger.py
--rw-r--r--   0 wallner    (501) staff       (20)    42498 2024-05-18 14:17:26.000000 pyesorm-0.4.4/esorm/model.py
--rw-r--r--   0 wallner    (501) staff       (20)     9605 2024-01-18 19:16:18.000000 pyesorm-0.4.4/esorm/query.py
--rw-r--r--   0 wallner    (501) staff       (20)     1315 2024-01-18 19:06:35.000000 pyesorm-0.4.4/esorm/response.py
--rw-r--r--   0 wallner    (501) staff       (20)      996 2024-01-23 07:15:23.000000 pyesorm-0.4.4/esorm/utils.py
--rw-r--r--   0 wallner    (501) staff       (20)     5538 2023-10-30 16:10:12.000000 pyesorm-0.4.4/esorm/watcher.py
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-18 15:26:29.524105 pyesorm-0.4.4/pyesorm.egg-info/
--rw-r--r--   0 wallner    (501) staff       (20)    23956 2024-05-18 15:26:29.000000 pyesorm-0.4.4/pyesorm.egg-info/PKG-INFO
--rw-r--r--   0 wallner    (501) staff       (20)      514 2024-05-18 15:26:29.000000 pyesorm-0.4.4/pyesorm.egg-info/SOURCES.txt
--rw-r--r--   0 wallner    (501) staff       (20)        1 2024-05-18 15:26:29.000000 pyesorm-0.4.4/pyesorm.egg-info/dependency_links.txt
--rw-r--r--   0 wallner    (501) staff       (20)      272 2024-05-18 15:26:29.000000 pyesorm-0.4.4/pyesorm.egg-info/requires.txt
--rw-r--r--   0 wallner    (501) staff       (20)       17 2024-05-18 15:26:29.000000 pyesorm-0.4.4/pyesorm.egg-info/top_level.txt
--rw-r--r--   0 wallner    (501) staff       (20)       87 2023-10-31 20:33:56.000000 pyesorm-0.4.4/pyproject.toml
--rw-r--r--   0 wallner    (501) staff       (20)     1306 2024-05-18 15:26:29.526701 pyesorm-0.4.4/setup.cfg
--rw-r--r--   0 wallner    (501) staff       (20)       37 2023-10-30 16:10:12.000000 pyesorm-0.4.4/setup.py
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-18 15:26:29.523617 pyesorm-0.4.4/tests/
--rw-r--r--   0 wallner    (501) staff       (20)        0 2023-10-30 16:10:12.000000 pyesorm-0.4.4/tests/__init__.py
--rw-r--r--   0 wallner    (501) staff       (20)     7993 2024-05-18 15:08:50.000000 pyesorm-0.4.4/tests/conftest.py
--rw-r--r--   0 wallner    (501) staff       (20)    32738 2024-05-18 15:12:48.000000 pyesorm-0.4.4/tests/test_esorm.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-22 09:06:23.030310 pyesorm-0.4.5/
+-rw-r--r--   0 wallner    (501) staff       (20)    16725 2023-10-30 16:10:12.000000 pyesorm-0.4.5/LICENSE
+-rw-r--r--   0 wallner    (501) staff       (20)    23992 2024-05-22 09:06:23.029401 pyesorm-0.4.5/PKG-INFO
+-rw-r--r--   0 wallner    (501) staff       (20)    22355 2024-05-22 09:02:45.000000 pyesorm-0.4.5/README.md
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-22 09:06:23.011434 pyesorm-0.4.5/docs/
+-rw-r--r--   0 wallner    (501) staff       (20)        0 2024-01-17 15:06:14.000000 pyesorm-0.4.5/docs/__init__.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1484 2024-01-17 15:18:18.000000 pyesorm-0.4.5/docs/changelog.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1462 2024-01-17 15:10:11.000000 pyesorm-0.4.5/docs/conf.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-22 09:06:23.022216 pyesorm-0.4.5/esorm/
+-rw-r--r--   0 wallner    (501) staff       (20)      762 2024-05-18 14:17:08.000000 pyesorm-0.4.5/esorm/__init__.py
+-rw-r--r--   0 wallner    (501) staff       (20)     3132 2024-01-22 17:32:29.000000 pyesorm-0.4.5/esorm/aggs.py
+-rw-r--r--   0 wallner    (501) staff       (20)     4447 2024-05-07 05:08:54.000000 pyesorm-0.4.5/esorm/bulk.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1267 2024-05-07 05:07:07.000000 pyesorm-0.4.5/esorm/error.py
+-rw-r--r--   0 wallner    (501) staff       (20)     2144 2024-05-18 14:16:43.000000 pyesorm-0.4.5/esorm/esorm.py
+-rw-r--r--   0 wallner    (501) staff       (20)     3500 2024-01-24 09:39:22.000000 pyesorm-0.4.5/esorm/fastapi.py
+-rw-r--r--   0 wallner    (501) staff       (20)    11640 2023-10-31 19:12:30.000000 pyesorm-0.4.5/esorm/fields.py
+-rw-r--r--   0 wallner    (501) staff       (20)       52 2023-10-30 16:10:12.000000 pyesorm-0.4.5/esorm/logger.py
+-rw-r--r--   0 wallner    (501) staff       (20)    42594 2024-05-22 09:00:37.000000 pyesorm-0.4.5/esorm/model.py
+-rw-r--r--   0 wallner    (501) staff       (20)     9605 2024-01-18 19:16:18.000000 pyesorm-0.4.5/esorm/query.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1315 2024-01-18 19:06:35.000000 pyesorm-0.4.5/esorm/response.py
+-rw-r--r--   0 wallner    (501) staff       (20)      996 2024-01-23 07:15:23.000000 pyesorm-0.4.5/esorm/utils.py
+-rw-r--r--   0 wallner    (501) staff       (20)     5538 2023-10-30 16:10:12.000000 pyesorm-0.4.5/esorm/watcher.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-22 09:06:23.027265 pyesorm-0.4.5/pyesorm.egg-info/
+-rw-r--r--   0 wallner    (501) staff       (20)    23992 2024-05-22 09:06:22.000000 pyesorm-0.4.5/pyesorm.egg-info/PKG-INFO
+-rw-r--r--   0 wallner    (501) staff       (20)      514 2024-05-22 09:06:22.000000 pyesorm-0.4.5/pyesorm.egg-info/SOURCES.txt
+-rw-r--r--   0 wallner    (501) staff       (20)        1 2024-05-22 09:06:22.000000 pyesorm-0.4.5/pyesorm.egg-info/dependency_links.txt
+-rw-r--r--   0 wallner    (501) staff       (20)      272 2024-05-22 09:06:22.000000 pyesorm-0.4.5/pyesorm.egg-info/requires.txt
+-rw-r--r--   0 wallner    (501) staff       (20)       17 2024-05-22 09:06:22.000000 pyesorm-0.4.5/pyesorm.egg-info/top_level.txt
+-rw-r--r--   0 wallner    (501) staff       (20)       87 2023-10-31 20:33:56.000000 pyesorm-0.4.5/pyproject.toml
+-rw-r--r--   0 wallner    (501) staff       (20)     1306 2024-05-22 09:06:23.030948 pyesorm-0.4.5/setup.cfg
+-rw-r--r--   0 wallner    (501) staff       (20)       37 2023-10-30 16:10:12.000000 pyesorm-0.4.5/setup.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-05-22 09:06:23.025998 pyesorm-0.4.5/tests/
+-rw-r--r--   0 wallner    (501) staff       (20)        0 2023-10-30 16:10:12.000000 pyesorm-0.4.5/tests/__init__.py
+-rw-r--r--   0 wallner    (501) staff       (20)     8066 2024-05-22 08:55:19.000000 pyesorm-0.4.5/tests/conftest.py
+-rw-r--r--   0 wallner    (501) staff       (20)    32851 2024-05-22 08:53:40.000000 pyesorm-0.4.5/tests/test_esorm.py
```

### Comparing `pyesorm-0.4.4/LICENSE` & `pyesorm-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.4/PKG-INFO` & `pyesorm-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyesorm
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python ElasticSearch ORM based on Pydantic
 Home-page: https://github.com/wallneradam/esorm
 Author: Adam Wallner
 Author-email: Adam.wallner@gmail.com
 License: MPL-2.0
 Project-URL: Bug Tracker, https://github.com/wallneradam/esorm/issues
 Project-URL: Documentation, https://esorm.readthedocs.io/en/latest/
@@ -160,14 +160,15 @@
 | `str`               | `text`    |
 | `int`               | `long`    |
 | `float`             | `double`  |
 | `bool`              | `boolean` |
 | `datetime.datetime` | `date`    |
 | `datetime.date`     | `date`    |
 | `datetime.time`     | `date`    |
+| `typing.Literal`    | `keyword` |
 
 <a id="esorm-field-types"></a>
 #### ESORM field types
 
 You can specify ElasticSearch special fields using `esorm.fields` module.
 
 ```python
```

### Comparing `pyesorm-0.4.4/README.md` & `pyesorm-0.4.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,15 @@
 | `str`               | `text`    |
 | `int`               | `long`    |
 | `float`             | `double`  |
 | `bool`              | `boolean` |
 | `datetime.datetime` | `date`    |
 | `datetime.date`     | `date`    |
 | `datetime.time`     | `date`    |
+| `typing.Literal`    | `keyword` |
 
 <a id="esorm-field-types"></a>
 #### ESORM field types
 
 You can specify ElasticSearch special fields using `esorm.fields` module.
 
 ```python
```

### Comparing `pyesorm-0.4.4/docs/changelog.py` & `pyesorm-0.4.5/docs/changelog.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.4/docs/conf.py` & `pyesorm-0.4.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.4/esorm/__init__.py` & `pyesorm-0.4.5/esorm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.4/esorm/aggs.py` & `pyesorm-0.4.5/esorm/aggs.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.4/esorm/bulk.py` & `pyesorm-0.4.5/esorm/bulk.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.4/esorm/error.py` & `pyesorm-0.4.5/esorm/error.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.4/esorm/esorm.py` & `pyesorm-0.4.5/esorm/esorm.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.4/esorm/fastapi.py` & `pyesorm-0.4.5/esorm/fastapi.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.4/esorm/fields.py` & `pyesorm-0.4.5/esorm/fields.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.4/esorm/model.py` & `pyesorm-0.4.5/esorm/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1098,14 +1098,18 @@
             args = get_args(pydantic_type)
             create_mapping(args[0], properties)
             return {
                 'type': 'nested',
                 'properties': properties
             }
 
+        # String literals
+        if origin is Literal:
+            return {'type': 'keyword'}
+
         # Not supported origin type
         if origin:
             raise ValueError(f'Unknown ES field type: {pydantic_type}')
 
         # Nested class
         if issubclass(pydantic_type, BaseModel):
             # If it is a model but has an es_type, use it (e.g. geo_point)
```

### Comparing `pyesorm-0.4.4/esorm/query.py` & `pyesorm-0.4.5/esorm/query.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.4/esorm/response.py` & `pyesorm-0.4.5/esorm/response.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.4/esorm/utils.py` & `pyesorm-0.4.5/esorm/utils.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.4/esorm/watcher.py` & `pyesorm-0.4.5/esorm/watcher.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.4/pyesorm.egg-info/PKG-INFO` & `pyesorm-0.4.5/pyesorm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyesorm
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python ElasticSearch ORM based on Pydantic
 Home-page: https://github.com/wallneradam/esorm
 Author: Adam Wallner
 Author-email: Adam.wallner@gmail.com
 License: MPL-2.0
 Project-URL: Bug Tracker, https://github.com/wallneradam/esorm/issues
 Project-URL: Documentation, https://esorm.readthedocs.io/en/latest/
@@ -160,14 +160,15 @@
 | `str`               | `text`    |
 | `int`               | `long`    |
 | `float`             | `double`  |
 | `bool`              | `boolean` |
 | `datetime.datetime` | `date`    |
 | `datetime.date`     | `date`    |
 | `datetime.time`     | `date`    |
+| `typing.Literal`    | `keyword` |
 
 <a id="esorm-field-types"></a>
 #### ESORM field types
 
 You can specify ElasticSearch special fields using `esorm.fields` module.
 
 ```python
```

### Comparing `pyesorm-0.4.4/pyesorm.egg-info/SOURCES.txt` & `pyesorm-0.4.5/pyesorm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyesorm-0.4.4/setup.cfg` & `pyesorm-0.4.5/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyesorm
-version = 0.4.4
+version = 0.4.5
 author = Adam Wallner
 author_email = Adam.wallner@gmail.com
 description = Python ElasticSearch ORM based on Pydantic
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = ElasticSearch, ORM, Pydantic
 license = MPL-2.0
```

### Comparing `pyesorm-0.4.4/tests/conftest.py` & `pyesorm-0.4.5/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,24 +87,26 @@
 
 # noinspection PyUnresolvedReferences
 @pytest.fixture(scope="class")
 def model_python(esorm):
     """
     Model to test python types
     """
+    from typing import Literal
     from datetime import datetime, date, time
 
     class PythonFieldModel(esorm.ESModel):
         f_str: str
         f_int: int
         f_float: float
         f_bool: bool
         f_datetime: datetime
         f_date: date
         f_time: time
+        f_literal: Literal['a', 'b', 'c']
 
     return PythonFieldModel
 
 
 # noinspection PyUnresolvedReferences
 @pytest.fixture(scope="class")
 def model_es(esorm):
```

### Comparing `pyesorm-0.4.4/tests/test_esorm.py` & `pyesorm-0.4.5/tests/test_esorm.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,15 @@
         assert mappings[model_python.ESConfig.index]['mappings']['properties']['f_str']['type'] == 'keyword'
         assert mappings[model_python.ESConfig.index]['mappings']['properties']['f_int']['type'] == 'long'
         assert mappings[model_python.ESConfig.index]['mappings']['properties']['f_float']['type'] == 'double'
         assert mappings[model_python.ESConfig.index]['mappings']['properties']['f_bool']['type'] == 'boolean'
         assert mappings[model_python.ESConfig.index]['mappings']['properties']['f_datetime']['type'] == 'date'
         assert mappings[model_python.ESConfig.index]['mappings']['properties']['f_date']['type'] == 'date'
         assert mappings[model_python.ESConfig.index]['mappings']['properties']['f_time']['type'] == 'date'
+        assert mappings[model_python.ESConfig.index]['mappings']['properties']['f_literal']['type'] == 'keyword'
         # Check if mappings are correct for ES fields
         mappings = await es.indices.get_mapping(index=model_es.ESConfig.index)
         assert mappings[model_es.ESConfig.index]['mappings']['properties']['f_keyword']['type'] == 'keyword'
         assert mappings[model_es.ESConfig.index]['mappings']['properties']['f_text']['type'] == 'text'
         assert mappings[model_es.ESConfig.index]['mappings']['properties']['f_binary']['type'] == 'binary'
         assert mappings[model_es.ESConfig.index]['mappings']['properties']['f_byte']['type'] == 'byte'
         assert mappings[model_es.ESConfig.index]['mappings']['properties']['f_short']['type'] == 'short'
```

