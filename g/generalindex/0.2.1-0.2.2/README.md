# Comparing `tmp/generalindex-0.2.1.tar.gz` & `tmp/generalindex-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generalindex-0.2.1.tar", last modified: Mon Jan 29 09:32:11 2024, max compression
+gzip compressed data, was "generalindex-0.2.2.tar", last modified: Wed May 22 11:00:24 2024, max compression
```

## Comparing `generalindex-0.2.1.tar` & `generalindex-0.2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:32:11.032278 generalindex-0.2.1/
--rw-rw-rw-   0 root         (0) root         (0)     1055 2024-01-29 09:31:55.000000 generalindex-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    17276 2024-01-29 09:32:11.032278 generalindex-0.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    16675 2024-01-29 09:31:55.000000 generalindex-0.2.1/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:32:11.024278 generalindex-0.2.1/generalindex/
--rw-rw-rw-   0 root         (0) root         (0)     1324 2024-01-29 09:31:55.000000 generalindex-0.2.1/generalindex/Authenticator.py
--rw-rw-rw-   0 root         (0) root         (0)     9789 2024-01-29 09:31:55.000000 generalindex-0.2.1/generalindex/DatalakeHandler.py
--rw-rw-rw-   0 root         (0) root         (0)     7396 2024-01-29 09:31:55.000000 generalindex-0.2.1/generalindex/GxApi.py
--rw-rw-rw-   0 root         (0) root         (0)     7126 2024-01-29 09:31:55.000000 generalindex-0.2.1/generalindex/HTTPCaller.py
--rw-rw-rw-   0 root         (0) root         (0)     2154 2024-01-29 09:31:55.000000 generalindex-0.2.1/generalindex/StatusHandler.py
--rw-rw-rw-   0 root         (0) root         (0)     8962 2024-01-29 09:31:55.000000 generalindex-0.2.1/generalindex/TaskHandler.py
--rw-rw-rw-   0 root         (0) root         (0)    28639 2024-01-29 09:31:55.000000 generalindex-0.2.1/generalindex/Timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)      271 2024-01-29 09:31:55.000000 generalindex-0.2.1/generalindex/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       96 2024-01-29 09:31:55.000000 generalindex-0.2.1/generalindex/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      551 2024-01-29 09:31:55.000000 generalindex-0.2.1/generalindex/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1779 2024-01-29 09:31:55.000000 generalindex-0.2.1/generalindex/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:32:11.032278 generalindex-0.2.1/generalindex.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17276 2024-01-29 09:32:10.000000 generalindex-0.2.1/generalindex.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      616 2024-01-29 09:32:10.000000 generalindex-0.2.1/generalindex.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-01-29 09:32:10.000000 generalindex-0.2.1/generalindex.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-01-29 09:32:10.000000 generalindex-0.2.1/generalindex.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       13 2024-01-29 09:32:10.000000 generalindex-0.2.1/generalindex.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-01-29 09:32:11.032278 generalindex-0.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1205 2024-01-29 09:31:57.000000 generalindex-0.2.1/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 09:32:11.032278 generalindex-0.2.1/test/
--rw-rw-rw-   0 root         (0) root         (0)     1631 2024-01-29 09:31:55.000000 generalindex-0.2.1/test/test_datalakehandler.py
--rw-rw-rw-   0 root         (0) root         (0)     8088 2024-01-29 09:31:55.000000 generalindex-0.2.1/test/test_gxapi.py
--rw-rw-rw-   0 root         (0) root         (0)     7987 2024-01-29 09:31:55.000000 generalindex-0.2.1/test/test_httpcaller.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2024-01-29 09:31:55.000000 generalindex-0.2.1/test/test_timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)     1716 2024-01-29 09:31:55.000000 generalindex-0.2.1/test/test_utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 11:00:24.567203 generalindex-0.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1055 2024-05-22 11:00:11.000000 generalindex-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    17501 2024-05-22 11:00:24.567203 generalindex-0.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    16900 2024-05-22 11:00:11.000000 generalindex-0.2.2/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 11:00:24.563203 generalindex-0.2.2/generalindex/
+-rw-rw-rw-   0 root         (0) root         (0)     1324 2024-05-22 11:00:11.000000 generalindex-0.2.2/generalindex/Authenticator.py
+-rw-rw-rw-   0 root         (0) root         (0)     9789 2024-05-22 11:00:11.000000 generalindex-0.2.2/generalindex/DatalakeHandler.py
+-rw-rw-rw-   0 root         (0) root         (0)     7696 2024-05-22 11:00:11.000000 generalindex-0.2.2/generalindex/GxApi.py
+-rw-rw-rw-   0 root         (0) root         (0)     7126 2024-05-22 11:00:11.000000 generalindex-0.2.2/generalindex/HTTPCaller.py
+-rw-rw-rw-   0 root         (0) root         (0)     2154 2024-05-22 11:00:11.000000 generalindex-0.2.2/generalindex/StatusHandler.py
+-rw-rw-rw-   0 root         (0) root         (0)     8962 2024-05-22 11:00:11.000000 generalindex-0.2.2/generalindex/TaskHandler.py
+-rw-rw-rw-   0 root         (0) root         (0)    28639 2024-05-22 11:00:11.000000 generalindex-0.2.2/generalindex/Timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)      271 2024-05-22 11:00:11.000000 generalindex-0.2.2/generalindex/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       96 2024-05-22 11:00:11.000000 generalindex-0.2.2/generalindex/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      551 2024-05-22 11:00:11.000000 generalindex-0.2.2/generalindex/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1779 2024-05-22 11:00:11.000000 generalindex-0.2.2/generalindex/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 11:00:24.567203 generalindex-0.2.2/generalindex.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17501 2024-05-22 11:00:24.000000 generalindex-0.2.2/generalindex.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      616 2024-05-22 11:00:24.000000 generalindex-0.2.2/generalindex.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-22 11:00:24.000000 generalindex-0.2.2/generalindex.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-05-22 11:00:24.000000 generalindex-0.2.2/generalindex.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       13 2024-05-22 11:00:24.000000 generalindex-0.2.2/generalindex.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-22 11:00:24.567203 generalindex-0.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1205 2024-05-22 11:00:13.000000 generalindex-0.2.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 11:00:24.567203 generalindex-0.2.2/test/
+-rw-rw-rw-   0 root         (0) root         (0)     1631 2024-05-22 11:00:11.000000 generalindex-0.2.2/test/test_datalakehandler.py
+-rw-rw-rw-   0 root         (0) root         (0)     8088 2024-05-22 11:00:11.000000 generalindex-0.2.2/test/test_gxapi.py
+-rw-rw-rw-   0 root         (0) root         (0)     7987 2024-05-22 11:00:11.000000 generalindex-0.2.2/test/test_httpcaller.py
+-rw-rw-rw-   0 root         (0) root         (0)      752 2024-05-22 11:00:11.000000 generalindex-0.2.2/test/test_timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1716 2024-05-22 11:00:11.000000 generalindex-0.2.2/test/test_utils.py
```

### Comparing `generalindex-0.2.1/LICENSE` & `generalindex-0.2.2/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2021 NorthGravity
+Copyright (c) 2024 GeneralIndex
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `generalindex-0.2.1/PKG-INFO` & `generalindex-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generalindex
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python SDK for the General Index platform
 Home-page: https://www.general-index.com/
 Author: General Index
 Author-email: info@general-index.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -108,36 +108,37 @@
   - ISO date ex. 2022-11-21T00:00:00
 - delta: Delta will filter timeseries by insertion date instead of the actual timestamp of data (default false)
 - metadata: to either return it in the response or not (default false) Accepted values: true, false, only
 - metadata_fields: Filter by metadata field e.g. {"metadata.tradinghub":"NWE"} 
 - order: Order of results by date (default desc)
 - timezone: Timezone as string used for the timestamps in the Date column. Format: Continent/City, for example Europe/London (default UTC)
 - fields: Filter by value field e.g. {"FactsheetVersion":"1"}
+- headers: Additional headers, which will be sent with request for symbols e.g. {"Example-Header":"Example_header_value"}
 
 The following code shows an example of how to query the index:
 
  ```python
 import pandas as pd
 
 import generalindex as gx
 
 # Instantiate GxApi 
 api = gx.GxApi()
 
 # retrieve all available data for specified code
 # and save as query.csv in test/
-api.index(code=['GX0000001'], start_from='all')\
+api.index(code=['GX0000001'], start_from='all', headers={"Example-Header":"Example_header_value"})\
     .file(file_name='test/query.csv', output_type='csv')
 
 # The retrieved data can be read as a pandas dataframe
 df = pd.read_csv("test/query.csv")
 
 # retrieve all available data for specified code
 # and stream to memory as BytesIO object
-data = api.index(code=['GX0000001'], start_from='all')\
+data = api.index(code=['GX0000001'], start_from='all' , headers={"Example-Header":"Example_header_value"})\
     .csv()
 
 # read as pandas dataframe
 df = pd.read_csv(data)
 ```
 ### How to read data from Index in JSON format?
```

### Comparing `generalindex-0.2.1/README.md` & `generalindex-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -89,36 +89,37 @@
   - ISO date ex. 2022-11-21T00:00:00
 - delta: Delta will filter timeseries by insertion date instead of the actual timestamp of data (default false)
 - metadata: to either return it in the response or not (default false) Accepted values: true, false, only
 - metadata_fields: Filter by metadata field e.g. {"metadata.tradinghub":"NWE"} 
 - order: Order of results by date (default desc)
 - timezone: Timezone as string used for the timestamps in the Date column. Format: Continent/City, for example Europe/London (default UTC)
 - fields: Filter by value field e.g. {"FactsheetVersion":"1"}
+- headers: Additional headers, which will be sent with request for symbols e.g. {"Example-Header":"Example_header_value"}
 
 The following code shows an example of how to query the index:
 
  ```python
 import pandas as pd
 
 import generalindex as gx
 
 # Instantiate GxApi 
 api = gx.GxApi()
 
 # retrieve all available data for specified code
 # and save as query.csv in test/
-api.index(code=['GX0000001'], start_from='all')\
+api.index(code=['GX0000001'], start_from='all', headers={"Example-Header":"Example_header_value"})\
     .file(file_name='test/query.csv', output_type='csv')
 
 # The retrieved data can be read as a pandas dataframe
 df = pd.read_csv("test/query.csv")
 
 # retrieve all available data for specified code
 # and stream to memory as BytesIO object
-data = api.index(code=['GX0000001'], start_from='all')\
+data = api.index(code=['GX0000001'], start_from='all' , headers={"Example-Header":"Example_header_value"})\
     .csv()
 
 # read as pandas dataframe
 df = pd.read_csv(data)
 ```
 ### How to read data from Index in JSON format?
```

### Comparing `generalindex-0.2.1/generalindex/Authenticator.py` & `generalindex-0.2.2/generalindex/Authenticator.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.1/generalindex/DatalakeHandler.py` & `generalindex-0.2.2/generalindex/DatalakeHandler.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.1/generalindex/GxApi.py` & `generalindex-0.2.2/generalindex/GxApi.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,21 +18,30 @@
         '''
         Returns a list of the symbols available on a given group or symbols within search
         '''
         query_url = PathFormatter().get_symbol_queried_path(start=start_from, _size=size, group_name=group_name,
                                                             search_for=search)
         return json.load(_ApiRequest(path=query_url).json())
 
-    def index(self, code: list = None, period: list = None, period_type: list = None,
-              time_ref: list = None, group: str = None, module: list = None,
+    def index(self,
+              code: list = None,
+              period: list = None,
+              period_type: list = None,
+              time_ref: list = None,
+              group: str = None,
+              module: list = None,
               start_from: str = None,
-              to: str = None, delta: bool = None,
+              to: str = None,
+              delta: bool = None,
               metadata: MetadataVals = None,
-              metadata_fields: dict = None, order: OrderVals = None, timezone: str = None,
-              fields: dict = None):
+              metadata_fields: dict = None,
+              order: OrderVals = None,
+              timezone: str = None,
+              fields: dict = None,
+              headers: dict = None):
         """
         The method retrieves the data from Gx Api based on provided parameters.
 
         :param code: Symbol code (default '*' )
         :param period: Symbol period (default '*' ).
         :param period_type: Symbol periodType (default '*' )
         :param time_ref: Symbol timeRef (default '*' )
@@ -58,23 +67,24 @@
         :param delta: Delta will filter timeseries by insertion date instead of the actual timestamp of data (default false)
         :param metadata: Metadata (default false) Accepted values: true, false, only
         :param metadata_fields: Filter by metadata field e.g. {"metadata.tradinghub":"NWE"}
         :param order: Order of results by date (default desc)
         :param timezone: Timezone as string used for the timestamps in the Date column.
         Continent/City, for example Europe/London (default UTC)
         :param fields: Filter by value field e.g. {"FactsheetVersion":"1"}
+        :param headers: Additional headers, which will be sent with request for symbols e.g. {"Example-Header":"Example_header_value"}
 
         :return: _ApiRequest
         """
         sig, method_locals = inspect.signature(self.index), locals()
         query_params_dict = {self._to_camel_case(param.name): self._concatenate(method_locals[param.name]) for param in
                              sig.parameters.values() if
                              (method_locals[param.name] is not None)}
         query_params_dict = self._create_query_params(query_params_dict)
-        return _ApiRequest(path='/index', query_params=query_params_dict)
+        return _ApiRequest(path='/index', query_params=query_params_dict, headers=headers)
 
     def catalogue(self, code: list = None, no_module: bool = None, module: str = None,
                   fields: dict = None, limit_fields: list = None):
         """
         The method retrieves the data from Gx Api based on provided parameters.
 
         :param code: Symbol code (default '*' )
```

### Comparing `generalindex-0.2.1/generalindex/HTTPCaller.py` & `generalindex-0.2.2/generalindex/HTTPCaller.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.1/generalindex/StatusHandler.py` & `generalindex-0.2.2/generalindex/StatusHandler.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.1/generalindex/TaskHandler.py` & `generalindex-0.2.2/generalindex/TaskHandler.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.1/generalindex/Timeseries.py` & `generalindex-0.2.2/generalindex/Timeseries.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.1/generalindex/exceptions.py` & `generalindex-0.2.2/generalindex/exceptions.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.1/generalindex/utils.py` & `generalindex-0.2.2/generalindex/utils.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.1/generalindex.egg-info/PKG-INFO` & `generalindex-0.2.2/generalindex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generalindex
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python SDK for the General Index platform
 Home-page: https://www.general-index.com/
 Author: General Index
 Author-email: info@general-index.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -108,36 +108,37 @@
   - ISO date ex. 2022-11-21T00:00:00
 - delta: Delta will filter timeseries by insertion date instead of the actual timestamp of data (default false)
 - metadata: to either return it in the response or not (default false) Accepted values: true, false, only
 - metadata_fields: Filter by metadata field e.g. {"metadata.tradinghub":"NWE"} 
 - order: Order of results by date (default desc)
 - timezone: Timezone as string used for the timestamps in the Date column. Format: Continent/City, for example Europe/London (default UTC)
 - fields: Filter by value field e.g. {"FactsheetVersion":"1"}
+- headers: Additional headers, which will be sent with request for symbols e.g. {"Example-Header":"Example_header_value"}
 
 The following code shows an example of how to query the index:
 
  ```python
 import pandas as pd
 
 import generalindex as gx
 
 # Instantiate GxApi 
 api = gx.GxApi()
 
 # retrieve all available data for specified code
 # and save as query.csv in test/
-api.index(code=['GX0000001'], start_from='all')\
+api.index(code=['GX0000001'], start_from='all', headers={"Example-Header":"Example_header_value"})\
     .file(file_name='test/query.csv', output_type='csv')
 
 # The retrieved data can be read as a pandas dataframe
 df = pd.read_csv("test/query.csv")
 
 # retrieve all available data for specified code
 # and stream to memory as BytesIO object
-data = api.index(code=['GX0000001'], start_from='all')\
+data = api.index(code=['GX0000001'], start_from='all' , headers={"Example-Header":"Example_header_value"})\
     .csv()
 
 # read as pandas dataframe
 df = pd.read_csv(data)
 ```
 ### How to read data from Index in JSON format?
```

### Comparing `generalindex-0.2.1/generalindex.egg-info/SOURCES.txt` & `generalindex-0.2.2/generalindex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.1/setup.py` & `generalindex-0.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open('requirements.txt') as fin:
     requirements = fin.read()
 
 setuptools.setup(
     name="generalindex",
-    version="0.2.1",
+    version="0.2.2",
     author="General Index",
     author_email="info@general-index.com",
     description="Python SDK for the General Index platform",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.general-index.com/",
     packages=setuptools.find_packages(exclude=["test"]),
```

### Comparing `generalindex-0.2.1/test/test_datalakehandler.py` & `generalindex-0.2.2/test/test_datalakehandler.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.1/test/test_gxapi.py` & `generalindex-0.2.2/test/test_gxapi.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.1/test/test_httpcaller.py` & `generalindex-0.2.2/test/test_httpcaller.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.1/test/test_timeseries.py` & `generalindex-0.2.2/test/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.2.1/test/test_utils.py` & `generalindex-0.2.2/test/test_utils.py`

 * *Files identical despite different names*

