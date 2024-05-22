# Comparing `tmp/crossfire-1.0.2.tar.gz` & `tmp/crossfire-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossfire-1.0.2.tar", max compression
+gzip compressed data, was "crossfire-1.1.0.tar", max compression
```

## Comparing `crossfire-1.0.2.tar` & `crossfire-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     5885 2023-12-13 21:16:48.244674 crossfire-1.0.2/README.md
--rw-r--r--   0        0        0      942 2023-12-22 12:54:27.314203 crossfire-1.0.2/crossfire/__init__.py
--rw-r--r--   0        0        0     5585 2023-12-13 21:16:48.248675 crossfire-1.0.2/crossfire/clients/__init__.py
--rw-r--r--   0        0        0     4642 2023-12-22 12:54:27.314203 crossfire-1.0.2/crossfire/clients/occurrences.py
--rw-r--r--   0        0        0      789 2023-12-13 21:16:48.248675 crossfire-1.0.2/crossfire/errors.py
--rw-r--r--   0        0        0     1188 2023-12-05 20:17:50.928648 crossfire-1.0.2/crossfire/logger.py
--rw-r--r--   0        0        0     2479 2023-12-31 00:49:51.427702 crossfire-1.0.2/crossfire/parser.py
--rw-r--r--   0        0        0     1201 2024-01-01 19:53:15.537818 crossfire-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     7027 1970-01-01 00:00:00.000000 crossfire-1.0.2/setup.py
--rw-r--r--   0        0        0     7039 1970-01-01 00:00:00.000000 crossfire-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     9276 2024-05-21 19:09:32.904791 crossfire-1.1.0/README.md
+-rw-r--r--   0        0        0      977 2024-05-21 19:09:32.904791 crossfire-1.1.0/crossfire/__init__.py
+-rw-r--r--   0        0        0     5722 2024-05-21 19:09:32.904791 crossfire-1.1.0/crossfire/clients/__init__.py
+-rw-r--r--   0        0        0     7459 2024-05-21 19:09:32.904791 crossfire-1.1.0/crossfire/clients/occurrences.py
+-rw-r--r--   0        0        0      976 2024-02-19 21:54:42.562284 crossfire-1.1.0/crossfire/errors.py
+-rw-r--r--   0        0        0     1188 2023-12-05 20:17:50.928648 crossfire-1.1.0/crossfire/logger.py
+-rw-r--r--   0        0        0     2479 2023-12-31 00:49:51.427702 crossfire-1.1.0/crossfire/parser.py
+-rw-r--r--   0        0        0     1225 2024-05-22 12:22:40.546454 crossfire-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    10567 1970-01-01 00:00:00.000000 crossfire-1.1.0/setup.py
+-rw-r--r--   0        0        0    10475 1970-01-01 00:00:00.000000 crossfire-1.1.0/PKG-INFO
```

### Comparing `crossfire-1.0.2/crossfire/__init__.py` & `crossfire-1.1.0/crossfire/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,17 +25,19 @@
     id_state,
     id_cities=None,
     type_occurrence="all",
     initial_date=None,
     final_date=None,
     max_parallel_requests=None,
     format=None,
+    flat=False,
 ):
     return client().occurrences(
         id_state,
         id_cities=id_cities,
         type_occurrence=type_occurrence,
         initial_date=initial_date,
         final_date=final_date,
         max_parallel_requests=max_parallel_requests,
         format=format,
+        flat=flat,
     )
```

### Comparing `crossfire-1.0.2/crossfire/clients/__init__.py` & `crossfire-1.1.0/crossfire/clients/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from asyncio import get_event_loop
 from datetime import datetime, timedelta
 from urllib.parse import urlencode
 
 import httpx
 from decouple import UndefinedValueError, config
+from nest_asyncio import apply
 
 from crossfire.clients.occurrences import Occurrences
 from crossfire.errors import CrossfireError, RetryAfterError
 from crossfire.parser import parse_response
 
 
 class CredentialsNotFoundError(CrossfireError):
@@ -109,36 +110,39 @@
         id_state,
         id_cities=None,
         type_occurrence="all",
         initial_date=None,
         final_date=None,
         max_parallel_requests=None,
         format=None,
+        flat=False,
     ):
         occurrences = Occurrences(
             self,
             id_state,
             id_cities=id_cities,
             type_occurrence=type_occurrence,
             initial_date=initial_date,
             final_date=final_date,
             max_parallel_requests=max_parallel_requests
             or self.max_parallel_requests,
             format=format,
+            flat=flat,
         )
         return await occurrences()
 
 
 class Client(AsyncClient):
     def __init__(self, email=None, password=None, max_parallel_requests=None):
         super().__init__(
             email=email,
             password=password,
             max_parallel_requests=max_parallel_requests,
         )
+        apply()
 
     def states(self, format=None):
         loop = get_event_loop()
         states, _ = loop.run_until_complete(super().states(format=format))
         return states
 
     def cities(self, city_id=None, city_name=None, state_id=None, format=None):
@@ -158,21 +162,23 @@
         id_state,
         id_cities=None,
         type_occurrence="all",
         initial_date=None,
         final_date=None,
         max_parallel_requests=None,
         format=None,
+        flat=False,
     ):
         loop = get_event_loop()
         occurrences = loop.run_until_complete(
             super().occurrences(
                 id_state=id_state,
                 id_cities=id_cities,
                 type_occurrence=type_occurrence,
                 initial_date=initial_date,
                 final_date=final_date,
                 max_parallel_requests=max_parallel_requests,
                 format=format,
+                flat=flat,
             )
         )
         return occurrences
```

### Comparing `crossfire-1.0.2/crossfire/errors.py` & `crossfire-1.1.0/crossfire/errors.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,7 +21,13 @@
         super().__init__(message)
 
 
 class DateFormatError(CrossfireError):
     def __init__(self, date):
         message = f"Date `{date}` does not match format YYYYMMDD, YYYY-MM-DD, or YYYY/MM/DD"
         super().__init__(message)
+
+
+class NestedColumnError(CrossfireError):
+    def __init__(self, nested_columns):
+        message = f"Invalid `nested_columns` value: {nested_columns}"
+        super().__init__(message)
```

### Comparing `crossfire-1.0.2/crossfire/logger.py` & `crossfire-1.1.0/crossfire/logger.py`

 * *Files identical despite different names*

### Comparing `crossfire-1.0.2/crossfire/parser.py` & `crossfire-1.1.0/crossfire/parser.py`

 * *Files identical despite different names*

### Comparing `crossfire-1.0.2/pyproject.toml` & `crossfire-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crossfire"
-version = "1.0.2"
+version = "1.1.0"
 description = "crossfire: Download spatial data sets from crossfire project"
 authors = ["Felipe Barros <felipe.b4rros@gmail.com>"]
 readme = "README.md"
 homepage = "https://fogocruzado.org.br/"
 repository = "https://github.com/felipesbarros/crossfire"
 classifiers = [
     "Intended Audience :: Science/Research",
@@ -16,14 +16,15 @@
 ]
 exclude =  ["env-example"]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.13"
 geopandas = { version = "^0.13.2", optional = true }
 httpx = "^0.25.0"
+nest-asyncio = "^1.6.0"
 pandas = { version = "^2.1.1", optional = true }
 python-decouple = "^3.5"
 tqdm = "^4.66.1"
 
 [tool.poetry.extras]
 df = ["pandas"]
 geodf = ["geopandas", "pandas"]
```

### Comparing `crossfire-1.0.2/PKG-INFO` & `crossfire-1.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossfire
-Version: 1.0.2
+Version: 1.1.0
 Summary: crossfire: Download spatial data sets from crossfire project
 Home-page: https://fogocruzado.org.br/
 Author: Felipe Barros
 Author-email: felipe.b4rros@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Provides-Extra: df
 Provides-Extra: geodf
 Requires-Dist: geopandas (>=0.13.2,<0.14.0) ; extra == "geodf"
 Requires-Dist: httpx (>=0.25.0,<0.26.0)
+Requires-Dist: nest-asyncio (>=1.6.0,<2.0.0)
 Requires-Dist: pandas (>=2.1.1,<3.0.0) ; extra == "df" or extra == "geodf"
 Requires-Dist: python-decouple (>=3.5,<4.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Project-URL: Repository, https://github.com/felipesbarros/crossfire
 Description-Content-Type: text/markdown
 
 <div style="text-align: center">
@@ -105,20 +106,20 @@
 
 ```python
 cities(format='df')
 ```
 
 #### `Cities` parameters
 
-| Name | Required | Description | Type | Default value | Example |
-|---|---|---|---|---|---|
-| `state_id` | ❌ | ID of the state | string | `None` | `'b112ffbe-17b3-4ad0-8f2a-2038745d1d14'` |
-| `city_id` | ❌ | ID of the city | string | `None` | `'88959ad9-b2f5-4a33-a8ec-ceff5a572ca5'` |
-| `city_name` | ❌ | Name of the city | string | `None` | `'Rio de Janeiro'` |
-| `format` | ❌ | Format of the result | string | `'dict'` | `'dict'`, `'df'` or `'geodf'` |
+| Name        | Required | Description          | Type   | Default value | Example                                  |
+|-------------|----------|----------------------|--------|---------------|------------------------------------------|
+| `state_id`  | ❌        | ID of the state      | string | `None`        | `'b112ffbe-17b3-4ad0-8f2a-2038745d1d14'` |
+| `city_id`   | ❌        | ID of the city       | string | `None`        | `'88959ad9-b2f5-4a33-a8ec-ceff5a572ca5'` |
+| `city_name` | ❌        | Name of the city     | string | `None`        | `'Rio de Janeiro'`                       |
+| `format`    | ❌        | Format of the result | string | `'dict'`      | `'dict'`, `'df'` or `'geodf'`            |
 
 
 ### Listing occurrences
 
 To get shooting occurrences from Fogo Cruzado dataset it is necessary to specify a state id in `id_state` parameter:
 
 ```python
@@ -138,25 +139,51 @@
 
 ```python
 occurrences('813ca36b-91e3-4a18-b408-60b27a1942ef', format='geodf')
 ```
 
 #### `Occurrences` parameters
 
-| Name | Required | Description | Type | Default value | Example                                                                                                                        |
-|---|---|---|---|---|--------------------------------------------------------------------------------------------------------------------------------|
-| `id_state` | ✅ | ID of the state | string | `None` | `'b112ffbe-17b3-4ad0-8f2a-2038745d1d14'`                                                                                       |
-| `id_cities` | ❌ | ID of the city | string or list of strings | `None` | `'88959ad9-b2f5-4a33-a8ec-ceff5a572ca5'` or `['88959ad9-b2f5-4a33-a8ec-ceff5a572ca5', '9d7b569c-ec84-4908-96ab-3706ec3bfc57']` |
-| `type_occurrence` | ❌ | Type of occurrence | string | `'all'` | `'all'`, `'withVictim'` or `'withoutVictim'`                                                                                   |
-| `initial_date` | ❌ | Initial date of the occurrences | string, `date` or `datetime` | `None` | `'2020-01-01'`, `'2020/01/01'`, `'20200101'`, `datetime.datetime(2023, 1, 1)` or `datetime.date(2023, 1, 1)`                   | 
-| `final_date` | ❌ | Final date of the occurrences | string, `date` or `datetime` | `None` | `'2020-01-01'`, `'2020/01/01'`, `'20200101'`, `datetime.datetime(2023, 1, 1)` or `datetime.date(2023, 1, 1)`                   |
-| `max_parallel_requests` | ❌ | Maximum number of parallel requests to the API | int | `16` | `32`                                                                                                                           |
-| `format` | ❌ | Format of the result | string | `'dict'` | `'dict'`, `'df'` or `'geodf'`                                                                                                  |
+| Name                    | Required | Description                                    | Type                         | Default value | Example                                                                                                                        |
+|-------------------------|----------|------------------------------------------------|------------------------------|---------------|--------------------------------------------------------------------------------------------------------------------------------|
+| `id_state`              | ✅        | ID of the state                                | string                       | `None`        | `'b112ffbe-17b3-4ad0-8f2a-2038745d1d14'`                                                                                       |
+| `id_cities`             | ❌        | ID of the city                                 | string or list of strings    | `None`        | `'88959ad9-b2f5-4a33-a8ec-ceff5a572ca5'` or `['88959ad9-b2f5-4a33-a8ec-ceff5a572ca5', '9d7b569c-ec84-4908-96ab-3706ec3bfc57']` |
+| `type_occurrence`       | ❌        | Type of occurrence                             | string                       | `'all'`       | `'all'`, `'withVictim'` or `'withoutVictim'`                                                                                   |
+| `initial_date`          | ❌        | Initial date of the occurrences                | string, `date` or `datetime` | `None`        | `'2020-01-01'`, `'2020/01/01'`, `'20200101'`, `datetime.datetime(2023, 1, 1)` or `datetime.date(2023, 1, 1)`                   | 
+| `final_date`            | ❌        | Final date of the occurrences                  | string, `date` or `datetime` | `None`        | `'2020-01-01'`, `'2020/01/01'`, `'20200101'`, `datetime.datetime(2023, 1, 1)` or `datetime.date(2023, 1, 1)`                   |
+| `max_parallel_requests` | ❌        | Maximum number of parallel requests to the API | int                          | `16`          | `32`                                                                                                                           |
+| `format`                | ❌        | Format of the result                           | string                       | `'dict'`      | `'dict'`, `'df'` or `'geodf'`                                                                                                  |
+| `flat`                  | ❌        | Return nested columns as separate columns      | bool                         | `False`       | `True` or `False`                                                                                                              |
 
 
+##### About `flat` parameter
+
+Occurrence data often contains nested information in several columns. By setting the parameter `flat=True`, you can simplify the analysis by separating nested data into individual columns. This feature is particularly useful for columns such as `contextInfo`, `state`, `region`, `city`, `neighborhood`, and `locality`.
+
+For example, to access detailed information about the context of occurrences, such as identifying the main reason, you would typically need to access the `contextInfo` column and then look for the mainReason key. With the `flat=True` parameter, this nested information is automatically split into separate columns, making the data easier to work with.
+
+When `flat=True` is set, the function returns occurrences with the flattened columns. Each new column retains the original column name as a prefix and the nested key as a suffix. For instance, the `contextInfo` column will be split into the following columns: `contextInfo_mainReason`, `contextInfo_complementaryReasons`, `contextInfo_clippings`, `contextInfo_massacre`, and `contextInfo_policeUnit`.
+
+
+###### Example
+
+```python
+from crossfire import occurrences
+from crossfire.clients.occurrences import flatten
+
+occs = occurrences('813ca36b-91e3-4a18-b408-60b27a1942ef')
+occs[0].keys()
+# dict_keys(['id', 'documentNumber', 'address', 'state', 'region', 'city', 'neighborhood', 'subNeighborhood', 'locality', 'latitude', 'longitude', 'date', 'policeAction', 'agentPresence', 'relatedRecord', 'contextInfo', 'transports', 'victims', 'animalVictims'])
+flattened_occs = occurrences('813ca36b-91e3-4a18-b408-60b27a1942ef', flat=True)
+occs[0].keys()
+# dict_keys(['id', 'documentNumber', 'address', 'state', 'region', 'city', 'neighborhood', 'subNeighborhood', 'locality', 'latitude', 'longitude', 'date', 'policeAction', 'agentPresence', 'relatedRecord', 'transports', 'victims', 'animalVictims', 'contextInfo', 'contextInfo_mainReason', 'contextInfo_complementaryReasons', 'contextInfo_clippings', 'contextInfo_massacre', 'contextInfo_policeUnit'])
+```
+
+By using the `flat=True parameter`, you ensure that all nested data is expanded into individual columns, simplifying data analysis and making it more straightforward to access specific details within your occurrence data.
+
 ### Custom client
 
 If not using the environment variables for authentication, it is recommended to use a custom client:
 
 ```python
 from crossfire import Client
```

