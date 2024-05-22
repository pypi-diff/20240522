# Comparing `tmp/rizaio-0.1.0a6.tar.gz` & `tmp/rizaio-0.1.0a7.tar.gz`

## Comparing `rizaio-0.1.0a6.tar` & `rizaio-0.1.0a7.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/__init__.py
--rw-r--r--   0        0        0    64250 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_base_client.py
--rw-r--r--   0        0        0    14864 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_constants.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_files.py
--rw-r--r--   0        0        0    26079 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_qs.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_resource.py
--rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_response.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_streaming.py
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_types.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_utils/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_utils/_typing.py
--rw-r--r--   0        0        0    11451 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/lib/.keep
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/resources/__init__.py
--rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/resources/v1.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/types/__init__.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/types/v1_execute_params.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/riza/types/v1_execute_response.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/__init__.py
--rw-r--r--   0        0        0    64250 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_base_client.py
--rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_constants.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_files.py
--rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_qs.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_resource.py
--rw-r--r--   0        0        0    28371 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_response.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_streaming.py
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_types.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_utils/__init__.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/lib/.keep
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/resources/__init__.py
--rw-r--r--   0        0        0     6609 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/resources/command.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/types/__init__.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/types/command_exec_params.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/src/rizaio/types/command_exec_response.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/.gitignore
--rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/LICENSE
--rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/pyproject.toml
--rw-r--r--   0        0        0    12118 2020-02-02 00:00:00.000000 rizaio-0.1.0a6/PKG-INFO
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/__init__.py
+-rw-r--r--   0        0        0    64250 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/_base_client.py
+-rw-r--r--   0        0        0    14864 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/_constants.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/_files.py
+-rw-r--r--   0        0        0    26079 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/_qs.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/_resource.py
+-rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/_response.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/_streaming.py
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/_types.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/_utils/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/_utils/_typing.py
+-rw-r--r--   0        0        0    11451 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/lib/.keep
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/resources/__init__.py
+-rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/resources/v1.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/types/__init__.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/types/v1_execute_params.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/riza/types/v1_execute_response.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/__init__.py
+-rw-r--r--   0        0        0    64412 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/_base_client.py
+-rw-r--r--   0        0        0    14908 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/_constants.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/_qs.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/_resource.py
+-rw-r--r--   0        0        0    28371 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/_response.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/_streaming.py
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/_types.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/_utils/__init__.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/lib/.keep
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/resources/__init__.py
+-rw-r--r--   0        0        0     7184 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/resources/command.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/types/__init__.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/types/command_exec_params.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/src/rizaio/types/command_exec_response.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/.gitignore
+-rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/LICENSE
+-rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/pyproject.toml
+-rw-r--r--   0        0        0    12116 2020-02-02 00:00:00.000000 rizaio-0.1.0a7/PKG-INFO
```

### Comparing `rizaio-0.1.0a6/src/riza/__init__.py` & `rizaio-0.1.0a7/src/riza/__init__.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/riza/_base_client.py` & `rizaio-0.1.0a7/src/riza/_base_client.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/riza/_client.py` & `rizaio-0.1.0a7/src/riza/_client.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/riza/_compat.py` & `rizaio-0.1.0a7/src/riza/_compat.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/riza/_exceptions.py` & `rizaio-0.1.0a7/src/riza/_exceptions.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/riza/_files.py` & `rizaio-0.1.0a7/src/riza/_files.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/riza/_models.py` & `rizaio-0.1.0a7/src/riza/_models.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/riza/_qs.py` & `rizaio-0.1.0a7/src/riza/_qs.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/riza/_resource.py` & `rizaio-0.1.0a7/src/riza/_resource.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/riza/_response.py` & `rizaio-0.1.0a7/src/riza/_response.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/riza/_streaming.py` & `rizaio-0.1.0a7/src/riza/_streaming.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/riza/_types.py` & `rizaio-0.1.0a7/src/riza/_types.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/riza/_utils/__init__.py` & `rizaio-0.1.0a7/src/riza/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/riza/_utils/_logs.py` & `rizaio-0.1.0a7/src/riza/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/riza/_utils/_proxy.py` & `rizaio-0.1.0a7/src/riza/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/riza/_utils/_sync.py` & `rizaio-0.1.0a7/src/riza/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/riza/_utils/_transform.py` & `rizaio-0.1.0a7/src/riza/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/riza/_utils/_typing.py` & `rizaio-0.1.0a7/src/riza/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/riza/_utils/_utils.py` & `rizaio-0.1.0a7/src/riza/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/riza/resources/v1.py` & `rizaio-0.1.0a7/src/riza/resources/v1.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/rizaio/__init__.py` & `rizaio-0.1.0a7/src/rizaio/__init__.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/rizaio/_base_client.py` & `rizaio-0.1.0a7/src/rizaio/_base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -941,14 +941,16 @@
         request = self._build_request(options)
         self._prepare_request(request)
 
         kwargs: HttpxSendArgs = {}
         if self.custom_auth is not None:
             kwargs["auth"] = self.custom_auth
 
+        log.debug("Sending HTTP Request: %s %s", request.method, request.url)
+
         try:
             response = self._client.send(
                 request,
                 stream=stream or self._should_stream_response_body(request=request),
                 **kwargs,
             )
         except httpx.TimeoutException as err:
@@ -979,15 +981,20 @@
                     response_headers=None,
                 )
 
             log.debug("Raising connection error")
             raise APIConnectionError(request=request) from err
 
         log.debug(
-            'HTTP Request: %s %s "%i %s"', request.method, request.url, response.status_code, response.reason_phrase
+            'HTTP Response: %s %s "%i %s" %s',
+            request.method,
+            request.url,
+            response.status_code,
+            response.reason_phrase,
+            response.headers,
         )
 
         try:
             response.raise_for_status()
         except httpx.HTTPStatusError as err:  # thrown on 4xx and 5xx status code
             log.debug("Encountered httpx.HTTPStatusError", exc_info=True)
```

### Comparing `rizaio-0.1.0a6/src/rizaio/_client.py` & `rizaio-0.1.0a7/src/rizaio/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     "AsyncRiza",
     "Client",
     "AsyncClient",
 ]
 
 
 class Riza(SyncAPIClient):
-    command: resources.Command
+    command: resources.CommandResource
     with_raw_response: RizaWithRawResponse
     with_streaming_response: RizaWithStreamedResponse
 
     # client options
     api_key: str
 
     def __init__(
@@ -100,15 +100,15 @@
             timeout=timeout,
             http_client=http_client,
             custom_headers=default_headers,
             custom_query=default_query,
             _strict_response_validation=_strict_response_validation,
         )
 
-        self.command = resources.Command(self)
+        self.command = resources.CommandResource(self)
         self.with_raw_response = RizaWithRawResponse(self)
         self.with_streaming_response = RizaWithStreamedResponse(self)
 
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
@@ -210,15 +210,15 @@
 
         if response.status_code >= 500:
             return _exceptions.InternalServerError(err_msg, response=response, body=body)
         return APIStatusError(err_msg, response=response, body=body)
 
 
 class AsyncRiza(AsyncAPIClient):
-    command: resources.AsyncCommand
+    command: resources.AsyncCommandResource
     with_raw_response: AsyncRizaWithRawResponse
     with_streaming_response: AsyncRizaWithStreamedResponse
 
     # client options
     api_key: str
 
     def __init__(
@@ -268,15 +268,15 @@
             timeout=timeout,
             http_client=http_client,
             custom_headers=default_headers,
             custom_query=default_query,
             _strict_response_validation=_strict_response_validation,
         )
 
-        self.command = resources.AsyncCommand(self)
+        self.command = resources.AsyncCommandResource(self)
         self.with_raw_response = AsyncRizaWithRawResponse(self)
         self.with_streaming_response = AsyncRizaWithStreamedResponse(self)
 
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
@@ -379,28 +379,28 @@
         if response.status_code >= 500:
             return _exceptions.InternalServerError(err_msg, response=response, body=body)
         return APIStatusError(err_msg, response=response, body=body)
 
 
 class RizaWithRawResponse:
     def __init__(self, client: Riza) -> None:
-        self.command = resources.CommandWithRawResponse(client.command)
+        self.command = resources.CommandResourceWithRawResponse(client.command)
 
 
 class AsyncRizaWithRawResponse:
     def __init__(self, client: AsyncRiza) -> None:
-        self.command = resources.AsyncCommandWithRawResponse(client.command)
+        self.command = resources.AsyncCommandResourceWithRawResponse(client.command)
 
 
 class RizaWithStreamedResponse:
     def __init__(self, client: Riza) -> None:
-        self.command = resources.CommandWithStreamingResponse(client.command)
+        self.command = resources.CommandResourceWithStreamingResponse(client.command)
 
 
 class AsyncRizaWithStreamedResponse:
     def __init__(self, client: AsyncRiza) -> None:
-        self.command = resources.AsyncCommandWithStreamingResponse(client.command)
+        self.command = resources.AsyncCommandResourceWithStreamingResponse(client.command)
 
 
 Client = Riza
 
 AsyncClient = AsyncRiza
```

### Comparing `rizaio-0.1.0a6/src/rizaio/_compat.py` & `rizaio-0.1.0a7/src/rizaio/_compat.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/rizaio/_exceptions.py` & `rizaio-0.1.0a7/src/rizaio/_exceptions.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/rizaio/_files.py` & `rizaio-0.1.0a7/src/rizaio/_files.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/rizaio/_models.py` & `rizaio-0.1.0a7/src/rizaio/_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     get_model_config,
     get_model_fields,
     field_get_default,
 )
 from ._constants import RAW_RESPONSE_HEADER
 
 if TYPE_CHECKING:
-    from pydantic_core.core_schema import ModelField, ModelFieldsSchema
+    from pydantic_core.core_schema import ModelField, LiteralSchema, ModelFieldsSchema
 
 __all__ = ["BaseModel", "GenericModel"]
 
 _T = TypeVar("_T")
 
 
 @runtime_checkable
@@ -247,15 +247,17 @@
             include: IncEx = None,
             exclude: IncEx = None,
             by_alias: bool = False,
             exclude_unset: bool = False,
             exclude_defaults: bool = False,
             exclude_none: bool = False,
             round_trip: bool = False,
-            warnings: bool = True,
+            warnings: bool | Literal["none", "warn", "error"] = True,
+            context: dict[str, Any] | None = None,
+            serialize_as_any: bool = False,
         ) -> dict[str, Any]:
             """Usage docs: https://docs.pydantic.dev/2.4/concepts/serialization/#modelmodel_dump
 
             Generate a dictionary representation of the model, optionally specifying which fields to include or exclude.
 
             Args:
                 mode: The mode in which `to_python` should run.
@@ -275,14 +277,18 @@
             """
             if mode != "python":
                 raise ValueError("mode is only supported in Pydantic v2")
             if round_trip != False:
                 raise ValueError("round_trip is only supported in Pydantic v2")
             if warnings != True:
                 raise ValueError("warnings is only supported in Pydantic v2")
+            if context is not None:
+                raise ValueError("context is only supported in Pydantic v2")
+            if serialize_as_any != False:
+                raise ValueError("serialize_as_any is only supported in Pydantic v2")
             return super().dict(  # pyright: ignore[reportDeprecated]
                 include=include,
                 exclude=exclude,
                 by_alias=by_alias,
                 exclude_unset=exclude_unset,
                 exclude_defaults=exclude_defaults,
                 exclude_none=exclude_none,
@@ -296,15 +302,17 @@
             include: IncEx = None,
             exclude: IncEx = None,
             by_alias: bool = False,
             exclude_unset: bool = False,
             exclude_defaults: bool = False,
             exclude_none: bool = False,
             round_trip: bool = False,
-            warnings: bool = True,
+            warnings: bool | Literal["none", "warn", "error"] = True,
+            context: dict[str, Any] | None = None,
+            serialize_as_any: bool = False,
         ) -> str:
             """Usage docs: https://docs.pydantic.dev/2.4/concepts/serialization/#modelmodel_dump_json
 
             Generates a JSON representation of the model using Pydantic's `to_json` method.
 
             Args:
                 indent: Indentation to use in the JSON output. If None is passed, the output will be compact.
@@ -320,14 +328,18 @@
             Returns:
                 A JSON string representation of the model.
             """
             if round_trip != False:
                 raise ValueError("round_trip is only supported in Pydantic v2")
             if warnings != True:
                 raise ValueError("warnings is only supported in Pydantic v2")
+            if context is not None:
+                raise ValueError("context is only supported in Pydantic v2")
+            if serialize_as_any != False:
+                raise ValueError("serialize_as_any is only supported in Pydantic v2")
             return super().json(  # type: ignore[reportDeprecated]
                 indent=indent,
                 include=include,
                 exclude=exclude,
                 by_alias=by_alias,
                 exclude_unset=exclude_unset,
                 exclude_defaults=exclude_defaults,
@@ -546,15 +558,15 @@
 
                 # Note: if one variant defines an alias then they all should
                 discriminator_alias = field.get("serialization_alias")
 
                 field_schema = field["schema"]
 
                 if field_schema["type"] == "literal":
-                    for entry in field_schema["expected"]:
+                    for entry in cast("LiteralSchema", field_schema)["expected"]:
                         if isinstance(entry, str):
                             mapping[entry] = variant
             else:
                 field_info = cast("dict[str, FieldInfo]", variant.__fields__).get(discriminator_field_name)  # pyright: ignore[reportDeprecated, reportUnnecessaryCast]
                 if not field_info:
                     continue
```

### Comparing `rizaio-0.1.0a6/src/rizaio/_qs.py` & `rizaio-0.1.0a7/src/rizaio/_qs.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/rizaio/_resource.py` & `rizaio-0.1.0a7/src/rizaio/_resource.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/rizaio/_response.py` & `rizaio-0.1.0a7/src/rizaio/_response.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/rizaio/_streaming.py` & `rizaio-0.1.0a7/src/rizaio/_streaming.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/rizaio/_types.py` & `rizaio-0.1.0a7/src/rizaio/_types.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/rizaio/_utils/__init__.py` & `rizaio-0.1.0a7/src/rizaio/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/rizaio/_utils/_logs.py` & `rizaio-0.1.0a7/src/rizaio/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/rizaio/_utils/_proxy.py` & `rizaio-0.1.0a7/src/rizaio/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/rizaio/_utils/_sync.py` & `rizaio-0.1.0a7/src/rizaio/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/rizaio/_utils/_transform.py` & `rizaio-0.1.0a7/src/rizaio/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/rizaio/_utils/_typing.py` & `rizaio-0.1.0a7/src/rizaio/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/rizaio/_utils/_utils.py` & `rizaio-0.1.0a7/src/rizaio/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/src/rizaio/resources/command.py` & `rizaio-0.1.0a7/src/rizaio/resources/command.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 from typing import Dict, List
 from typing_extensions import Literal
 
 import httpx
 
-from ..types import CommandExecResponse, command_exec_params
+from ..types import command_exec_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import (
     maybe_transform,
     async_maybe_transform,
 )
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
@@ -20,32 +20,34 @@
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
 from .._base_client import (
     make_request_options,
 )
+from ..types.command_exec_response import CommandExecResponse
 
-__all__ = ["Command", "AsyncCommand"]
+__all__ = ["CommandResource", "AsyncCommandResource"]
 
 
-class Command(SyncAPIResource):
+class CommandResource(SyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> CommandWithRawResponse:
-        return CommandWithRawResponse(self)
+    def with_raw_response(self) -> CommandResourceWithRawResponse:
+        return CommandResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> CommandWithStreamingResponse:
-        return CommandWithStreamingResponse(self)
+    def with_streaming_response(self) -> CommandResourceWithStreamingResponse:
+        return CommandResourceWithStreamingResponse(self)
 
     def exec(
         self,
         *,
         code: str,
         language: Literal["PYTHON", "JAVASCRIPT", "TYPESCRIPT", "RUBY", "PHP"],
+        allow_http_hosts: List[str] | NotGiven = NOT_GIVEN,
         args: List[str] | NotGiven = NOT_GIVEN,
         env: Dict[str, str] | NotGiven = NOT_GIVEN,
         stdin: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -59,14 +61,16 @@
         line arguments.
 
         Args:
           code: The code to execute in the sandbox.
 
           language: The interpreter to use when executing code.
 
+          allow_http_hosts: List of allowed hosts for HTTP requests
+
           args: List of command line arguments to pass to the script.
 
           env: Set of key-value pairs to add to the script's execution environment.
 
           stdin: Input to pass to the script via `stdin`.
 
           extra_headers: Send extra headers
@@ -79,41 +83,43 @@
         """
         return self._post(
             "/v1/execute",
             body=maybe_transform(
                 {
                     "code": code,
                     "language": language,
+                    "allow_http_hosts": allow_http_hosts,
                     "args": args,
                     "env": env,
                     "stdin": stdin,
                 },
                 command_exec_params.CommandExecParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=CommandExecResponse,
         )
 
 
-class AsyncCommand(AsyncAPIResource):
+class AsyncCommandResource(AsyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> AsyncCommandWithRawResponse:
-        return AsyncCommandWithRawResponse(self)
+    def with_raw_response(self) -> AsyncCommandResourceWithRawResponse:
+        return AsyncCommandResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> AsyncCommandWithStreamingResponse:
-        return AsyncCommandWithStreamingResponse(self)
+    def with_streaming_response(self) -> AsyncCommandResourceWithStreamingResponse:
+        return AsyncCommandResourceWithStreamingResponse(self)
 
     async def exec(
         self,
         *,
         code: str,
         language: Literal["PYTHON", "JAVASCRIPT", "TYPESCRIPT", "RUBY", "PHP"],
+        allow_http_hosts: List[str] | NotGiven = NOT_GIVEN,
         args: List[str] | NotGiven = NOT_GIVEN,
         env: Dict[str, str] | NotGiven = NOT_GIVEN,
         stdin: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -127,14 +133,16 @@
         line arguments.
 
         Args:
           code: The code to execute in the sandbox.
 
           language: The interpreter to use when executing code.
 
+          allow_http_hosts: List of allowed hosts for HTTP requests
+
           args: List of command line arguments to pass to the script.
 
           env: Set of key-value pairs to add to the script's execution environment.
 
           stdin: Input to pass to the script via `stdin`.
 
           extra_headers: Send extra headers
@@ -147,54 +155,55 @@
         """
         return await self._post(
             "/v1/execute",
             body=await async_maybe_transform(
                 {
                     "code": code,
                     "language": language,
+                    "allow_http_hosts": allow_http_hosts,
                     "args": args,
                     "env": env,
                     "stdin": stdin,
                 },
                 command_exec_params.CommandExecParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=CommandExecResponse,
         )
 
 
-class CommandWithRawResponse:
-    def __init__(self, command: Command) -> None:
+class CommandResourceWithRawResponse:
+    def __init__(self, command: CommandResource) -> None:
         self._command = command
 
         self.exec = to_raw_response_wrapper(
             command.exec,
         )
 
 
-class AsyncCommandWithRawResponse:
-    def __init__(self, command: AsyncCommand) -> None:
+class AsyncCommandResourceWithRawResponse:
+    def __init__(self, command: AsyncCommandResource) -> None:
         self._command = command
 
         self.exec = async_to_raw_response_wrapper(
             command.exec,
         )
 
 
-class CommandWithStreamingResponse:
-    def __init__(self, command: Command) -> None:
+class CommandResourceWithStreamingResponse:
+    def __init__(self, command: CommandResource) -> None:
         self._command = command
 
         self.exec = to_streamed_response_wrapper(
             command.exec,
         )
 
 
-class AsyncCommandWithStreamingResponse:
-    def __init__(self, command: AsyncCommand) -> None:
+class AsyncCommandResourceWithStreamingResponse:
+    def __init__(self, command: AsyncCommandResource) -> None:
         self._command = command
 
         self.exec = async_to_streamed_response_wrapper(
             command.exec,
         )
```

### Comparing `rizaio-0.1.0a6/src/rizaio/types/command_exec_params.py` & `rizaio-0.1.0a7/src/rizaio/types/command_exec_params.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 class CommandExecParams(TypedDict, total=False):
     code: Required[str]
     """The code to execute in the sandbox."""
 
     language: Required[Literal["PYTHON", "JAVASCRIPT", "TYPESCRIPT", "RUBY", "PHP"]]
     """The interpreter to use when executing code."""
 
+    allow_http_hosts: List[str]
+    """List of allowed hosts for HTTP requests"""
+
     args: List[str]
     """List of command line arguments to pass to the script."""
 
     env: Dict[str, str]
     """Set of key-value pairs to add to the script's execution environment."""
 
     stdin: str
```

### Comparing `rizaio-0.1.0a6/src/rizaio/types/command_exec_response.py` & `rizaio-0.1.0a7/src/rizaio/types/command_exec_response.py`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/LICENSE` & `rizaio-0.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `rizaio-0.1.0a6/pyproject.toml` & `rizaio-0.1.0a7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rizaio"
-version = "0.1.0-alpha.6"
+version = "0.1.0-alpha.7"
 description = "The official Python library for the riza API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Riza", email = "hello@riza.io" },
 ]
 dependencies = [
@@ -64,15 +64,15 @@
 [tool.rye.scripts]
 format = { chain = [
   "format:ruff",
   "format:docs",
   "fix:ruff",
 ]}
 "format:black" = "black ."
-"format:docs" = "python bin/ruffen-docs.py README.md api.md"
+"format:docs" = "python scripts/utils/ruffen-docs.py README.md api.md"
 "format:ruff" = "ruff format"
 "format:isort" = "isort ."
 
 "lint" = { chain = [
   "check:ruff",
   "typecheck",
 ]}
@@ -187,9 +187,10 @@
 length-sort-straight = true
 combine-as-imports = true
 extra-standard-library = ["typing_extensions"]
 known-first-party = ["rizaio", "tests"]
 
 [tool.ruff.per-file-ignores]
 "bin/**.py" = ["T201", "T203"]
+"scripts/**.py" = ["T201", "T203"]
 "tests/**.py" = ["T201", "T203"]
 "examples/**.py" = ["T201", "T203"]
```

### Comparing `rizaio-0.1.0a6/PKG-INFO` & `rizaio-0.1.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rizaio
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: The official Python library for the riza API
 Project-URL: Homepage, https://github.com/riza-io/riza-api-python
 Project-URL: Repository, https://github.com/riza-io/riza-api-python
 Author-email: Riza <hello@riza.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -199,15 +199,15 @@
 
 # More granular control:
 client = Riza(
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
 )
 
 # Override per-request:
-client.with_options(timeout=5 * 1000).command.exec(
+client.with_options(timeout=5.0).command.exec(
     code='print("Hello world!")',
     language="PYTHON",
 )
 ```
 
 On timeout, an `APITimeoutError` is thrown.
 
@@ -276,15 +276,15 @@
         print(line)
 ```
 
 The context manager is required so that the response will reliably be closed.
 
 ### Making custom/undocumented requests
 
-This library is typed for convenient access the documented API.
+This library is typed for convenient access to the documented API.
 
 If you need to access undocumented endpoints, params, or response properties, the library can still be used.
 
 #### Undocumented endpoints
 
 To make requests to undocumented endpoints, you can make requests using `client.get`, `client.post`, and other
 http verbs. Options on the client will be respected (such as retries) will be respected when making this
```

