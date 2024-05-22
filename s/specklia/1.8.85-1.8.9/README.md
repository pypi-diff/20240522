# Comparing `tmp/specklia-1.8.85.tar.gz` & `tmp/specklia-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specklia-1.8.85.tar", last modified: Tue May 21 02:45:48 2024, max compression
+gzip compressed data, was "specklia-1.8.9.tar", last modified: Wed Feb 28 15:11:11 2024, max compression
```

## Comparing `specklia-1.8.85.tar` & `specklia-1.8.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 02:45:48.451437 specklia-1.8.85/
--rw-r--r--   0 root         (0) root         (0)     1061 2024-05-21 01:22:50.000000 specklia-1.8.85/LICENCE
--rw-r--r--   0 root         (0) root         (0)     2898 2024-05-21 02:45:48.451437 specklia-1.8.85/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1611 2024-05-21 01:22:50.000000 specklia-1.8.85/README.md
--rw-r--r--   0 root         (0) root         (0)      484 2024-05-21 02:45:48.451437 specklia-1.8.85/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2366 2024-05-21 01:22:50.000000 specklia-1.8.85/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 02:45:48.447437 specklia-1.8.85/specklia/
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-21 01:22:50.000000 specklia-1.8.85/specklia/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14714 2024-05-21 01:22:50.000000 specklia-1.8.85/specklia/_websocket_helpers.py
--rw-r--r--   0 root         (0) root         (0)    40528 2024-05-21 01:22:50.000000 specklia-1.8.85/specklia/client.py
--rw-r--r--   0 root         (0) root         (0)     4074 2024-05-21 01:22:50.000000 specklia-1.8.85/specklia/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 02:45:48.451437 specklia-1.8.85/specklia.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2898 2024-05-21 02:45:48.000000 specklia-1.8.85/specklia.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      365 2024-05-21 02:45:48.000000 specklia-1.8.85/specklia.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 02:45:48.000000 specklia-1.8.85/specklia.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2024-05-21 02:45:48.000000 specklia-1.8.85/specklia.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-21 02:45:48.000000 specklia-1.8.85/specklia.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 02:45:48.447437 specklia-1.8.85/tests/
--rw-r--r--   0 root         (0) root         (0)    14689 2024-05-21 01:22:50.000000 specklia-1.8.85/tests/test_client.py
--rw-r--r--   0 root         (0) root         (0)     2654 2024-05-21 01:22:50.000000 specklia-1.8.85/tests/test_utilities.py
--rw-r--r--   0 root         (0) root         (0)    11623 2024-05-21 01:22:50.000000 specklia-1.8.85/tests/test_websocket_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 15:11:11.329601 specklia-1.8.9/
+-rw-r--r--   0 root         (0) root         (0)     1061 2024-02-27 11:34:21.000000 specklia-1.8.9/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     2897 2024-02-28 15:11:11.329601 specklia-1.8.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1611 2024-02-27 11:34:21.000000 specklia-1.8.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      484 2024-02-28 15:11:11.333601 specklia-1.8.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2366 2024-02-27 11:34:21.000000 specklia-1.8.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 15:11:11.325601 specklia-1.8.9/specklia/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-02-27 11:34:21.000000 specklia-1.8.9/specklia/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14715 2024-02-27 11:34:21.000000 specklia-1.8.9/specklia/_websocket_helpers.py
+-rw-r--r--   0 root         (0) root         (0)    39737 2024-02-27 11:34:21.000000 specklia-1.8.9/specklia/client.py
+-rw-r--r--   0 root         (0) root         (0)     3790 2024-02-27 11:34:21.000000 specklia-1.8.9/specklia/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 15:11:11.329601 specklia-1.8.9/specklia.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2897 2024-02-28 15:11:11.000000 specklia-1.8.9/specklia.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      365 2024-02-28 15:11:11.000000 specklia-1.8.9/specklia.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-28 15:11:11.000000 specklia-1.8.9/specklia.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2024-02-28 15:11:11.000000 specklia-1.8.9/specklia.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-02-28 15:11:11.000000 specklia-1.8.9/specklia.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 15:11:11.329601 specklia-1.8.9/tests/
+-rw-r--r--   0 root         (0) root         (0)    14649 2024-02-27 11:34:21.000000 specklia-1.8.9/tests/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2024-02-27 11:34:21.000000 specklia-1.8.9/tests/test_utilities.py
+-rw-r--r--   0 root         (0) root         (0)    11629 2024-02-27 11:34:21.000000 specklia-1.8.9/tests/test_websocket_helpers.py
```

### Comparing `specklia-1.8.85/LICENCE` & `specklia-1.8.9/LICENCE`

 * *Files identical despite different names*

### Comparing `specklia-1.8.85/PKG-INFO` & `specklia-1.8.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.8.85
+Version: 1.8.9
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/
 Author: Earthwave Ltd
 Author-email: support@earthwave.co.uk
 License: MIT
 Project-URL: Homepage, https://specklia.earthwave.co.uk/
 Project-URL: Changelog, https://specklia.earthwave.co.uk/generated_docs/change_log.html
```

### Comparing `specklia-1.8.85/README.md` & `specklia-1.8.9/README.md`

 * *Files identical despite different names*

### Comparing `specklia-1.8.85/setup.py` & `specklia-1.8.9/setup.py`

 * *Files identical despite different names*

### Comparing `specklia-1.8.85/specklia/_websocket_helpers.py` & `specklia-1.8.9/specklia/_websocket_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
 def _extract_objects_to_serialise(data: object, object_dict: List[SerialisationData] = None) \
         -> Tuple[object, List[SerialisationData]]:
     """
     Iterate through an object, replacing complex objects with a placeholder string.
 
     This recursively traverses the object if it contains dictionaries or lists/iterables.
     When an object to be serialised is found, we explicitly:
-       - Replace it with a magic string: SERIALISED_SUBSTITUTION_PREFIX{X} where X is an increasing numeric index.
+       - Replace it with a magic string: SERIALISED_SUBSTITUTION_PREFIX{X} where X is an increasing numermic index.
        - Store the extracted object in a list, where X (above) is its place in this list. We use the
          SerialisationData type to keep both the object and the serialisation information.
 
     Parameters
     ----------
     data : object
         Input data object. Can be a single dataframe or primitive or a dictionary-like structure.
```

### Comparing `specklia-1.8.85/specklia/client.py` & `specklia-1.8.9/specklia/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,59 +260,51 @@
         NotImplementedError
             This route is not yet implemented.
         """
         _log.error('this method is not yet implemented.')
         raise NotImplementedError()
 
     def add_points_to_dataset(
-            self: Specklia, dataset_id: str, new_points: List[Dict[str, Union[Dict, gpd.GeoDataFrame]]]) -> None:
+            self: Specklia, dataset_id: str, new_points: gpd.GeoDataFrame, source_description: Dict) -> None:
         """
         Add new data to a dataset.
 
-        All of the columns present in the dataset must feature in the data to be added. Note that in addition to the
-        custom columns specified on the creation of the dataset (and retrievable via client.list_datasets()), you must
-        provide two additional mandatory columns: 'timestamp' and 'geometry'.
-
         You must have READ_WRITE or ADMIN permissions within the group that owns the dataset in order to do this.
 
         Note that Ingests are temporarily restricted to those that have READ_WRITE permissions
         within the all_users group (i.e. Specklia is read-only to the general public).
         This restriction will be lifted once we have per-user billing in place for Specklia.
 
-        Note that this can only be called up to 30,000 times per day for OLAP datasets - if you need to load more
-        individual data files than this, ensure that you use this method on groups of files
-        rather than individual files.
-
         Parameters
         ----------
         dataset_id : str
             The UUID of the dataset to add data to.
-        new_points : List[Dict[str, Union[Dict, gpd.GeoDataFrame]]]
-            A list of dictionaries with the keys 'source' and 'gdf'. Within each dictionary, the value for 'source'
-            is a dictionary describing the source of the data.
-            The value for 'gdf' is a GeoDataFrame containing the points to add to the dataset.
-            The GeoDataFrame must contain at minimum the columns 'geometry' and 'timestamp'.
+        new_points : gpd.GeoDataFrame
+            A GeoDataFrame containing the points to add to the dataset.
+            Must contain at minimum the columns 'geometry' and 'timestamp'.
             The timestamp column must contain POSIX timestamps.
-            The 'geometry' column must contain Points following the (lon, lat) convention.
-            The GeoDataFrame must have its CRS specified as EPSG 4326.
+            Must have its CRS specified as EPSG 4326.
+        source_description : Dict
+            A dictionary describing the source of the data.
 
         Raises
         ------
         RuntimeError
             If the ingest failed for some reason.
         """
         ws = simple_websocket.Client(
             self.server_url.replace("http://", "ws://") + "/ingest",
             headers={"Authorization": "Bearer " + self.auth_token})
 
         # Authorise the connection and then send the requestion dictionary.
         ws.send(bytes(self.auth_token, encoding="utf-8"))
         _websocket_helpers.send_object_to_websocket(ws, {
             'dataset_id': dataset_id,
-            'new_points': new_points})
+            'gdf': new_points,
+            'source': source_description})
 
         response = _websocket_helpers.receive_object_from_websocket(ws, self._data_streaming_timeout_s)
         if response['status'] == HTTPStatus.OK:
             _log.info('Added new data to specklia dataset ID %s.', dataset_id)
         else:
             _log.error('Failed to interact with Specklia server, error was %s', str(response))
             raise RuntimeError(str(response))
@@ -663,15 +655,15 @@
                 datasets_df[column] = gpd.GeoSeries(
                     datasets_df[column].apply(lambda x: shape(x) if x is not None else None), crs=4326)
 
         return datasets_df.convert_dtypes()  # convert the rest of the dtypes to pandas' best guest
 
     def create_dataset(
             self: Specklia, dataset_name: str, description: str,
-            columns: Optional[List[Dict[str, str]]] = None, storage_technology: str = 'OLAP') -> str:
+            columns: Optional(List[Dict[str, str]]) = None, storage_technology: str = 'OLAP') -> str:
         """
         Create a dataset.
 
         Specklia datasets contain point cloud data.
         When you create the dataset, you must specify the fields within the data.
 
         After you have created the dataset, you'll probably want to add data to it using
@@ -686,26 +678,26 @@
         ---------
         dataset_name : str
             The name the user provides for the dataset.
             Must contain alphanumeric characters, spaces, underscores and hyphens only.
         description : str
             A description of the dataset.
             Must contain alphanumeric characters, spaces, underscores and hyphens only.
-        columns : Optional[List[Dict[str, str]]],
+        columns : Optional(List[Dict[str, str]])),
             A list where each item is an additional column the user wishes to add to the dataset,
             beyond the mandatory EPSG4326 latitude, longitude and POSIX timestamp.
             A list of columns should follow the format::
 
                 [{'name': 'elevation', 'type': 'float', 'description': 'elevation', 'unit': 'metres'},
                 {'name': 'remarks', 'type': 'str', 'description': 'per-row remarks', 'unit': 'NA'}]
 
             Where valid values for 'type' are 'string', 'float', 'int', and 'polygon' and the other three fields are
             strings, which must contain alphanumeric characters, spaces, underscores and hyphens only.
 
-            When using 'type': 'polygon', the column must be a GeoPandas GeoSeries containing shapely Polygon objects
+            When using 'type': 'polygon', the column must be a goeseries.GeoSeries containing shapely Polygon objects
             in EPSG4326 using the Point(lon, lat) convention.
 
             Please do not create explicit EPSG4326 columns (e.g. 'lat', 'lon') or POSIX timestamp columns
             as these are unnecessary repetitions of Specklia default columns.
         storage_technology : str
             Determines the storage technology used for the dataset, by default 'OLAP'.
             This cannot be changed after the dataset is created.
```

### Comparing `specklia-1.8.85/specklia/utilities.py` & `specklia-1.8.9/specklia/utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,23 +47,21 @@
         crs = xy_proj4
     else:
         # we use the geometry within the GeoDataFrame.
         x_col = gdf.geometry.x
         y_col = gdf.geometry.y
         crs = gdf.geometry.crs
 
-    # TODO: The below lines will only work if there's at least one pair of adjacent pixels in X
-    # and at least one pair of adjacent pixels in Y. We'll reload Specklia's raster data at a later
-    # date to explicitly store the x and y resolutions to mitigate this, but it's a low priority problem.
-    dx = np.min(np.diff(np.sort(x_col.unique())))
-    dy = np.min(np.diff(np.sort(y_col.unique())))
+    unique_x_points = np.sort(x_col.unique())
+    unique_y_points = np.sort(y_col.unique())
+    dx = unique_x_points[1] - unique_x_points[0]
+    dy = unique_y_points[1] - unique_y_points[0]
 
     # generate all of the points we want to end up with in the output raster
-    # we need to offset both these axes by one in order to use np.searchsorted() in a manner that matches
-    # how the EOLIS Gridded products were loaded into Specklia.
+    # we need to offset both these axes by one in order to use np.searchsorted() correctly below.
     desired_x_axis = np.arange(bounds['min_x'], bounds['max_x'], dx) + dx
     desired_y_axis = np.arange(bounds['min_y'], bounds['max_y'], dy) + dy
 
     # create the output raster, but fill it with NaN
     gridded_data = np.full((len(desired_y_axis), len(desired_x_axis)), np.NaN)
 
     # set the valid points within it
```

### Comparing `specklia-1.8.85/specklia.egg-info/PKG-INFO` & `specklia-1.8.9/specklia.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.8.85
+Version: 1.8.9
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/
 Author: Earthwave Ltd
 Author-email: support@earthwave.co.uk
 License: MIT
 Project-URL: Homepage, https://specklia.earthwave.co.uk/
 Project-URL: Changelog, https://specklia.earthwave.co.uk/generated_docs/change_log.html
```

### Comparing `specklia-1.8.85/tests/test_client.py` & `specklia-1.8.9/tests/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,23 +21,23 @@
     'max_timestamp': datetime(2000, 1, 2),
     'columns_to_return': ['croissant'],
     'additional_filters': [
         {'column': 'cheese', 'operator': '<', 'threshold': 6.57},
         {'column': 'wine', 'operator': '>=', 'threshold': -23}]}
 
 
-@pytest.fixture
+@pytest.fixture()
 def example_geodataframe() -> gpd.GeoDataFrame:
     return gpd.GeoDataFrame({
         'geometry': gpd.points_from_xy([1, 2, 3, 4, 5], [0, 1, 2, 3, 4]),
         'timestamp': [2, 3, 4, 5, 6]},
         crs="EPSG:4326")
 
 
-@pytest.fixture
+@pytest.fixture()
 def example_datasets_dataframe() -> pd.DataFrame:
     return pd.DataFrame([{'columns': {'description': 'hobbit height in cm',
                                       'max_value': '150',
                                       'min_value': '0',
                                       'name': 'height',
                                       'type': 'int',
                                       'unit': 'centimetres'},
@@ -53,21 +53,21 @@
                           'owning_group_id': 'pippin',
                           'owning_group_name': 'merry',
                           'size_rows': 4,
                           'size_uncompressed_bytes': 726
                           }])
 
 
-@pytest.fixture
+@pytest.fixture()
 def example_usage_report() -> List[Dict]:
     return [{'total_billable_bytes_processed': 10, 'total_increase_in_bytes_stored': 20,
              'user_id': 'example_user', 'year': 2023, 'month': 11}]
 
 
-@pytest.fixture
+@pytest.fixture()
 def test_client():
     with patch.object(Specklia, '_fetch_user_id'):
         return Specklia(auth_token='fake_token', url='https://localhost')
 
 
 def test_create_client(test_client: Specklia):
     assert test_client is not None
@@ -92,21 +92,19 @@
 def test_add_points_to_dataset(test_client: Specklia, example_geodataframe: gpd.GeoDataFrame):
     with (patch('specklia.client.simple_websocket') as mock_simple_websocket,
             patch('specklia.client._websocket_helpers') as mock_websocket_helpers):
         mock_client = MagicMock(name="mock_client")
         mock_simple_websocket.Client.return_value = mock_client
         mock_websocket_helpers.receive_object_from_websocket.return_value = {'status': HTTPStatus.OK}
         test_client.add_points_to_dataset(
-            dataset_id='dummy_dataset',
-            new_points=[{'source': {'reference': 'cheese'}, 'gdf': example_geodataframe}])
+            dataset_id='dummy_dataset', new_points=example_geodataframe, source_description={'reference': 'cheese'})
 
         mock_websocket_helpers.send_object_to_websocket.assert_called_with(
             mock_client, {
-                'dataset_id': 'dummy_dataset',
-                'new_points': [{'source': {'reference': 'cheese'}, 'gdf': example_geodataframe}]})
+                'dataset_id': 'dummy_dataset', 'gdf': example_geodataframe, 'source': {'reference': 'cheese'}})
 
 
 def test_query_dataset(test_client: Specklia):
     with (patch('specklia.client.simple_websocket') as mock_simple_websocket,
             patch('specklia.client._websocket_helpers') as mock_websocket_helpers):
         mock_client = MagicMock(name="mock_client")
         mock_simple_websocket.Client.return_value = mock_client
```

### Comparing `specklia-1.8.85/tests/test_utilities.py` & `specklia-1.8.9/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `specklia-1.8.85/tests/test_websocket_helpers.py` & `specklia-1.8.9/tests/test_websocket_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,25 +27,25 @@
 import requests
 from shapely import Point
 import simple_websocket
 
 from specklia import _websocket_helpers as websocket_helpers
 
 
-@pytest.fixture
+@pytest.fixture()
 def example_dataframe() -> pd.DataFrame:
     np.random.seed(2501)
     return pd.DataFrame({
         'lat': np.random.rand(5000),
         'lon': np.random.rand(5000),
         'timestamp': np.random.randint(1000, 2000, 5000)
     })
 
 
-@pytest.fixture
+@pytest.fixture()
 def test_netcdf_filepath(test_inputs_path: str) -> str:
     return os.path.join(test_inputs_path, 'netcdf', 'test_swath_c_oib_unc_479889082.nc')
 
 
 def start_api_in_separate_process(flask_app: Flask, api_config: Dict, block_until_api_exits: bool = False) -> Process:
     """Start the API in a separate process.
 
@@ -118,15 +118,15 @@
 def crash_while_handling_websocket_message():
     print('crash_while_handling_websocket_message triggered')
     ws = simple_websocket.Server(request.environ)
     websocket_helpers.receive_object_from_websocket(ws)
     sleep(100)  # simulate a crash in a separate service
 
 
-@pytest.fixture
+@pytest.fixture()
 def _bent_pipe_server() -> None:
     # create the "bent pipe" - a server that just returns what it receives
     app = Flask('websocket_bent_pipe')
     app.add_url_rule('/endpoint/<nb_messages>', None, handle_websocket_message, websocket=True)
     app.add_url_rule('/broken_endpoint', None, crash_while_handling_websocket_message, websocket=True)
     api_process = start_api_in_separate_process(
         flask_app=app, api_config={'test_host_name': '127.0.0.1', 'test_port': 9066})
```

